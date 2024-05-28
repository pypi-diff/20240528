# Comparing `tmp/cardscan_client-0.0.1.tar.gz` & `tmp/cardscan_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardscan_client-0.0.1.tar", max compression
+gzip compressed data, was "cardscan_client-0.1.0.tar", max compression
```

## Comparing `cardscan_client-0.0.1.tar` & `cardscan_client-0.1.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0     9583 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/README.md
--rw-r--r--   0        0        0     5385 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/__init__.py
--rw-r--r--   0        0        0      106 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/api/__init__.py
--rw-r--r--   0        0        0    88662 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/api/card_scan_api.py
--rw-r--r--   0        0        0    28347 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/api_client.py
--rw-r--r--   0        0        0      852 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/api_response.py
--rw-r--r--   0        0        0    14244 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/configuration.py
--rw-r--r--   0        0        0     5372 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/exceptions.py
--rw-r--r--   0        0        0     4774 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/__init__.py
--rw-r--r--   0        0        0     3536 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/address.py
--rw-r--r--   0        0        0     2254 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/api_error_response.py
--rw-r--r--   0        0        0     3977 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/card_api_response.py
--rw-r--r--   0        0        0     5636 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/card_api_response_details.py
--rw-r--r--   0        0        0     2663 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/card_api_response_images.py
--rw-r--r--   0        0        0     2007 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/card_api_response_images_back.py
--rw-r--r--   0        0        0     2016 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/card_api_response_images_front.py
--rw-r--r--   0        0        0      980 2024-05-22 01:36:13.039179 cardscan_client-0.0.1/cardscan_client/models/card_state.py
--rw-r--r--   0        0        0     3062 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/card_websocket_event.py
--rw-r--r--   0        0        0     1893 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/co_insurance.py
--rw-r--r--   0        0        0     1875 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/co_payment.py
--rw-r--r--   0        0        0     3840 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/coverage_summary.py
--rw-r--r--   0        0        0     2767 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/create_card_request.py
--rw-r--r--   0        0        0     2410 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/create_card_request_backside.py
--rw-r--r--   0        0        0     2394 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/create_eligibility_request.py
--rw-r--r--   0        0        0     2106 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/deductible.py
--rw-r--r--   0        0        0     2472 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/direct_upload200_response.py
--rw-r--r--   0        0        0     2076 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/direct_upload200_response_metadata.py
--rw-r--r--   0        0        0     5292 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/direct_upload_request.py
--rw-r--r--   0        0        0     5259 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/eligibility_api_response.py
--rw-r--r--   0        0        0     3270 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/eligibility_api_response_eligibility_request.py
--rw-r--r--   0        0        0     2354 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/eligibility_api_response_error.py
--rw-r--r--   0        0        0     2554 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/eligibility_info.py
--rw-r--r--   0        0        0      747 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/eligibility_state.py
--rw-r--r--   0        0        0     5934 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/eligibility_summarized_response.py
--rw-r--r--   0        0        0     3254 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/eligibility_websocket_event.py
--rw-r--r--   0        0        0     2722 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/generate_card_upload_url200_response.py
--rw-r--r--   0        0        0     2643 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/generate_card_upload_url_request.py
--rw-r--r--   0        0        0     2354 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/generate_magic_link200_response.py
--rw-r--r--   0        0        0     2314 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/get_access_token200_response.py
--rw-r--r--   0        0        0     2016 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/get_access_token500_response.py
--rw-r--r--   0        0        0     3072 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/list_eligibility200_response.py
--rw-r--r--   0        0        0     2008 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/match_score.py
--rw-r--r--   0        0        0     2056 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/oop.py
--rw-r--r--   0        0        0     2286 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/payer_details.py
--rw-r--r--   0        0        0     3039 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/plan_details.py
--rw-r--r--   0        0        0     2748 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/provider_dto.py
--rw-r--r--   0        0        0     2268 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/response_metadata.py
--rw-r--r--   0        0        0      764 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_capture_type.py
--rw-r--r--   0        0        0     6782 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata.py
--rw-r--r--   0        0        0     4266 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_camera_capabilities.py
--rw-r--r--   0        0        0     2197 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_camera_capabilities_aspect_ratio.py
--rw-r--r--   0        0        0     2050 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_capture_canvas.py
--rw-r--r--   0        0        0     2801 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_capture_score.py
--rw-r--r--   0        0        0     2181 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_capture_score_scores_inner.py
--rw-r--r--   0        0        0     2153 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_guides.py
--rw-r--r--   0        0        0     2066 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_video_background.py
--rw-r--r--   0        0        0     2784 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_video_track.py
--rw-r--r--   0        0        0     2027 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_metadata_window_inner.py
--rw-r--r--   0        0        0      702 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/scan_orientation.py
--rw-r--r--   0        0        0     2877 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/search_cards200_response.py
--rw-r--r--   0        0        0     2916 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/service.py
--rw-r--r--   0        0        0     3145 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/subscriber_details.py
--rw-r--r--   0        0        0     2847 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/subscriber_dto.py
--rw-r--r--   0        0        0     4811 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/upload_parameters.py
--rw-r--r--   0        0        0     2182 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/models/validate_magic_link200_response.py
--rw-r--r--   0        0        0        0 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/py.typed
--rw-r--r--   0        0        0    10063 2024-05-22 01:36:13.042512 cardscan_client-0.0.1/cardscan_client/rest.py
--rw-r--r--   0        0        0      808 2024-05-22 01:36:13.045845 cardscan_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    10587 1970-01-01 00:00:00.000000 cardscan_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7938 2024-05-28 01:47:59.250290 cardscan_client-0.1.0/README.md
+-rw-r--r--   0        0        0     5527 2024-05-28 01:48:31.203852 cardscan_client-0.1.0/cardscan_client/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-28 01:48:31.207185 cardscan_client-0.1.0/cardscan_client/api/__init__.py
+-rw-r--r--   0        0        0   101554 2024-05-28 01:48:31.187185 cardscan_client-0.1.0/cardscan_client/api/card_scan_api.py
+-rw-r--r--   0        0        0    29459 2024-05-28 01:48:31.210518 cardscan_client-0.1.0/cardscan_client/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-28 01:48:31.213852 cardscan_client-0.1.0/cardscan_client/api_response.py
+-rw-r--r--   0        0        0    14591 2024-05-28 01:48:31.203852 cardscan_client-0.1.0/cardscan_client/configuration.py
+-rw-r--r--   0        0        0     5372 2024-05-28 01:48:31.207185 cardscan_client-0.1.0/cardscan_client/exceptions.py
+-rw-r--r--   0        0        0     4916 2024-05-28 01:48:31.207185 cardscan_client-0.1.0/cardscan_client/models/__init__.py
+-rw-r--r--   0        0        0     3536 2024-05-28 01:48:30.990517 cardscan_client-0.1.0/cardscan_client/models/address.py
+-rw-r--r--   0        0        0     2254 2024-05-28 01:48:30.997184 cardscan_client-0.1.0/cardscan_client/models/api_error_response.py
+-rw-r--r--   0        0        0     3977 2024-05-28 01:48:31.003850 cardscan_client-0.1.0/cardscan_client/models/card_api_response.py
+-rw-r--r--   0        0        0     5636 2024-05-28 01:48:31.007184 cardscan_client-0.1.0/cardscan_client/models/card_api_response_details.py
+-rw-r--r--   0        0        0     2663 2024-05-28 01:48:31.013850 cardscan_client-0.1.0/cardscan_client/models/card_api_response_images.py
+-rw-r--r--   0        0        0     2007 2024-05-28 01:48:31.017184 cardscan_client-0.1.0/cardscan_client/models/card_api_response_images_back.py
+-rw-r--r--   0        0        0     2016 2024-05-28 01:48:31.020517 cardscan_client-0.1.0/cardscan_client/models/card_api_response_images_front.py
+-rw-r--r--   0        0        0      980 2024-05-28 01:48:31.020517 cardscan_client-0.1.0/cardscan_client/models/card_state.py
+-rw-r--r--   0        0        0     3062 2024-05-28 01:48:31.023850 cardscan_client-0.1.0/cardscan_client/models/card_websocket_event.py
+-rw-r--r--   0        0        0     1893 2024-05-28 01:48:31.027184 cardscan_client-0.1.0/cardscan_client/models/co_insurance.py
+-rw-r--r--   0        0        0     1875 2024-05-28 01:48:31.030517 cardscan_client-0.1.0/cardscan_client/models/co_payment.py
+-rw-r--r--   0        0        0     3840 2024-05-28 01:48:31.030517 cardscan_client-0.1.0/cardscan_client/models/coverage_summary.py
+-rw-r--r--   0        0        0     2767 2024-05-28 01:48:31.033851 cardscan_client-0.1.0/cardscan_client/models/create_card_request.py
+-rw-r--r--   0        0        0     2410 2024-05-28 01:48:31.037184 cardscan_client-0.1.0/cardscan_client/models/create_card_request_backside.py
+-rw-r--r--   0        0        0     2394 2024-05-28 01:48:31.040517 cardscan_client-0.1.0/cardscan_client/models/create_eligibility_request.py
+-rw-r--r--   0        0        0     2106 2024-05-28 01:48:31.040517 cardscan_client-0.1.0/cardscan_client/models/deductible.py
+-rw-r--r--   0        0        0     2472 2024-05-28 01:48:31.043851 cardscan_client-0.1.0/cardscan_client/models/direct_upload200_response.py
+-rw-r--r--   0        0        0     2076 2024-05-28 01:48:31.047184 cardscan_client-0.1.0/cardscan_client/models/direct_upload200_response_metadata.py
+-rw-r--r--   0        0        0     5292 2024-05-28 01:48:31.050517 cardscan_client-0.1.0/cardscan_client/models/direct_upload_request.py
+-rw-r--r--   0        0        0     5259 2024-05-28 01:48:31.053851 cardscan_client-0.1.0/cardscan_client/models/eligibility_api_response.py
+-rw-r--r--   0        0        0     3422 2024-05-28 01:48:31.057184 cardscan_client-0.1.0/cardscan_client/models/eligibility_api_response_eligibility_request.py
+-rw-r--r--   0        0        0     2754 2024-05-28 01:48:31.057184 cardscan_client-0.1.0/cardscan_client/models/eligibility_api_response_eligibility_request_subscriber.py
+-rw-r--r--   0        0        0     2354 2024-05-28 01:48:31.060517 cardscan_client-0.1.0/cardscan_client/models/eligibility_api_response_error.py
+-rw-r--r--   0        0        0     2554 2024-05-28 01:48:31.063851 cardscan_client-0.1.0/cardscan_client/models/eligibility_info.py
+-rw-r--r--   0        0        0      747 2024-05-28 01:48:31.063851 cardscan_client-0.1.0/cardscan_client/models/eligibility_state.py
+-rw-r--r--   0        0        0     5934 2024-05-28 01:48:31.067184 cardscan_client-0.1.0/cardscan_client/models/eligibility_summarized_response.py
+-rw-r--r--   0        0        0     3254 2024-05-28 01:48:31.070517 cardscan_client-0.1.0/cardscan_client/models/eligibility_websocket_event.py
+-rw-r--r--   0        0        0     2722 2024-05-28 01:48:31.070517 cardscan_client-0.1.0/cardscan_client/models/generate_card_upload_url200_response.py
+-rw-r--r--   0        0        0     2643 2024-05-28 01:48:31.073851 cardscan_client-0.1.0/cardscan_client/models/generate_card_upload_url_request.py
+-rw-r--r--   0        0        0     2354 2024-05-28 01:48:31.073851 cardscan_client-0.1.0/cardscan_client/models/generate_magic_link200_response.py
+-rw-r--r--   0        0        0     2314 2024-05-28 01:48:31.077184 cardscan_client-0.1.0/cardscan_client/models/get_access_token200_response.py
+-rw-r--r--   0        0        0     2016 2024-05-28 01:48:31.080517 cardscan_client-0.1.0/cardscan_client/models/get_access_token500_response.py
+-rw-r--r--   0        0        0     3072 2024-05-28 01:48:31.080517 cardscan_client-0.1.0/cardscan_client/models/list_eligibility200_response.py
+-rw-r--r--   0        0        0     2008 2024-05-28 01:48:31.083851 cardscan_client-0.1.0/cardscan_client/models/match_score.py
+-rw-r--r--   0        0        0     2056 2024-05-28 01:48:31.083851 cardscan_client-0.1.0/cardscan_client/models/oop.py
+-rw-r--r--   0        0        0     2286 2024-05-28 01:48:31.087184 cardscan_client-0.1.0/cardscan_client/models/payer_details.py
+-rw-r--r--   0        0        0     3039 2024-05-28 01:48:31.090518 cardscan_client-0.1.0/cardscan_client/models/plan_details.py
+-rw-r--r--   0        0        0     2748 2024-05-28 01:48:31.090518 cardscan_client-0.1.0/cardscan_client/models/provider_dto.py
+-rw-r--r--   0        0        0     2268 2024-05-28 01:48:31.093851 cardscan_client-0.1.0/cardscan_client/models/response_metadata.py
+-rw-r--r--   0        0        0      764 2024-05-28 01:48:31.093851 cardscan_client-0.1.0/cardscan_client/models/scan_capture_type.py
+-rw-r--r--   0        0        0     6782 2024-05-28 01:48:31.093851 cardscan_client-0.1.0/cardscan_client/models/scan_metadata.py
+-rw-r--r--   0        0        0     4266 2024-05-28 01:48:31.097184 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_camera_capabilities.py
+-rw-r--r--   0        0        0     2197 2024-05-28 01:48:31.097184 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_camera_capabilities_aspect_ratio.py
+-rw-r--r--   0        0        0     2050 2024-05-28 01:48:31.100518 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_capture_canvas.py
+-rw-r--r--   0        0        0     2801 2024-05-28 01:48:31.103851 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_capture_score.py
+-rw-r--r--   0        0        0     2181 2024-05-28 01:48:31.103851 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_capture_score_scores_inner.py
+-rw-r--r--   0        0        0     2153 2024-05-28 01:48:31.107184 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_guides.py
+-rw-r--r--   0        0        0     2066 2024-05-28 01:48:31.110518 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_video_background.py
+-rw-r--r--   0        0        0     2784 2024-05-28 01:48:31.110518 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_video_track.py
+-rw-r--r--   0        0        0     2027 2024-05-28 01:48:31.113851 cardscan_client-0.1.0/cardscan_client/models/scan_metadata_window_inner.py
+-rw-r--r--   0        0        0      702 2024-05-28 01:48:31.113851 cardscan_client-0.1.0/cardscan_client/models/scan_orientation.py
+-rw-r--r--   0        0        0     2877 2024-05-28 01:48:31.117184 cardscan_client-0.1.0/cardscan_client/models/search_cards200_response.py
+-rw-r--r--   0        0        0     2916 2024-05-28 01:48:31.120518 cardscan_client-0.1.0/cardscan_client/models/service.py
+-rw-r--r--   0        0        0     3145 2024-05-28 01:48:31.120518 cardscan_client-0.1.0/cardscan_client/models/subscriber_details.py
+-rw-r--r--   0        0        0     2847 2024-05-28 01:48:31.123851 cardscan_client-0.1.0/cardscan_client/models/subscriber_dto.py
+-rw-r--r--   0        0        0     4811 2024-05-28 01:48:31.123851 cardscan_client-0.1.0/cardscan_client/models/upload_parameters.py
+-rw-r--r--   0        0        0     2182 2024-05-28 01:48:31.127184 cardscan_client-0.1.0/cardscan_client/models/validate_magic_link200_response.py
+-rw-r--r--   0        0        0        0 2024-05-28 01:48:31.200518 cardscan_client-0.1.0/cardscan_client/py.typed
+-rw-r--r--   0        0        0    13824 2024-05-28 01:48:31.213852 cardscan_client-0.1.0/cardscan_client/rest.py
+-rw-r--r--   0        0        0      808 2024-05-28 01:58:39.048732 cardscan_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8942 1970-01-01 00:00:00.000000 cardscan_client-0.1.0/PKG-INFO
```

### Comparing `cardscan_client-0.0.1/README.md` & `cardscan_client-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: cardscan-client
+Version: 0.1.0
+Summary: Python CardScan API client
+Home-page: https://github.com/CardScan-ai/api-clients.git
+License: SEE LICENSE IN LICENSE.md
+Keywords: CardScan,CardScan client,CardScan API client
+Author: Team CardScan
+Author-email: dev@cardscan.ai
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aenum (>=3.1.11)
+Requires-Dist: aiohttp (>=3.8.4)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: python-dateutil (>=2.8.2)
+Requires-Dist: urllib3 (>=1.25.3)
+Requires-Dist: websockets (>=12.0)
+Project-URL: Repository, https://github.com/CardScan-ai/api-clients.git
+Description-Content-Type: text/markdown
+
 # cardscan-client
 
 The official python client for the CardScan API
 
 ## Requirements.
 
 Python 3.8+
@@ -12,97 +38,51 @@
 pip install cardscan-client
 ```
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
-````python
+```python
 from cardscan_client.api_client import ApiClient
 from cardscan_client.api.card_scan_api import CardScanApi
 from cardscan_client.configuration import Configuration
 from cardscan_client.exceptions import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://sandbox.cardscan.ai/v1
 # See configuration.py for a list of all supported configuration parameters.
-# configuration = Configuration(host="https://sandbox.cardscan.ai/v1")
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
 # Configure Bearer authorization: bearerAuth
 configuration = Configuration(
-    host=os.environ["HOST"],
-    api_key=os.environ["API_KEY"],
-)
-
-
-async def main():
-    # Enter a context with an instance of the API client
-    async with ApiClient(configuration) as api_client:
-        # Create an instance of the API class
-        api_instance = CardScanApi(api_client)
-
-        try:
-            # Creates a new card
-            api_response = await api_instance.get_access_token()
-
-            print("The response of GetAccessToken->get_access_token:\n")
-            pprint(api_response)
-        except ApiException as e:
-            print("Exception when calling GetAccessToken->get_access_token: %s\n" % e)
-
-
-if __name__ == "__main__":
-    import asyncio
-
-    asyncio.run(main())
-
-```python
-
-import time
-import cardscan_client
-from cardscan_client.rest import ApiException
-from pprint import pprint
-
-# Defining the host is optional and defaults to https://sandbox.cardscan.ai/v1
-# See configuration.py for a list of all supported configuration parameters.
-configuration = cardscan_client.Configuration(
-    host = "https://sandbox.cardscan.ai/v1"
+    api_key=os.environ['API_KEY'],
+    environment='sandbox'
 )
 
-# The client must configure the authentication and authorization parameters
-# in accordance with the API server security policy.
-# Examples for each auth method are provided below, use the example that
-# satisfies your auth use case.
-
-# Configure Bearer authorization: bearerAuth
-configuration = cardscan_client.Configuration(
-    access_token = os.environ["BEARER_TOKEN"]
-)
 
-
-# Enter a context with an instance of the API client
-async with cardscan_client.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = cardscan_client.CardScanApi(api_client)
-    create_card_request = cardscan_client.CreateCardRequest() # CreateCardRequest |  (optional)
+def main():
+    client = CardScanApi(api_client=ApiClient(configuration=configuration))
 
     try:
-        # Creates a new card
-        api_response = await api_instance.create_card(create_card_request=create_card_request)
-        print("The response of CardScanApi->create_card:\n")
+        api_response = client.full_scan(front_image_path="test/cards/front.jpg")
+
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling CardScanApi->create_card: %s\n" % e)
+        print("Exception when calling FullScan->full_scan: %s\n" % e)
 
-````
+
+if __name__ == "__main__":
+    main()
+
+```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://sandbox.cardscan.ai/v1*
 
 | Class         | Method                                                                       | HTTP request                                  | Description                |
 | ------------- | ---------------------------------------------------------------------------- | --------------------------------------------- | -------------------------- |
@@ -141,14 +121,15 @@
 - [CreateEligibilityRequest](docs/CreateEligibilityRequest.md)
 - [Deductible](docs/Deductible.md)
 - [DirectUpload200Response](docs/DirectUpload200Response.md)
 - [DirectUpload200ResponseMetadata](docs/DirectUpload200ResponseMetadata.md)
 - [DirectUploadRequest](docs/DirectUploadRequest.md)
 - [EligibilityApiResponse](docs/EligibilityApiResponse.md)
 - [EligibilityApiResponseEligibilityRequest](docs/EligibilityApiResponseEligibilityRequest.md)
+- [EligibilityApiResponseEligibilityRequestSubscriber](docs/EligibilityApiResponseEligibilityRequestSubscriber.md)
 - [EligibilityApiResponseError](docs/EligibilityApiResponseError.md)
 - [EligibilityInfo](docs/EligibilityInfo.md)
 - [EligibilityState](docs/EligibilityState.md)
 - [EligibilitySummarizedResponse](docs/EligibilitySummarizedResponse.md)
 - [EligibilityWebsocketEvent](docs/EligibilityWebsocketEvent.md)
 - [GenerateCardUploadUrl200Response](docs/GenerateCardUploadUrl200Response.md)
 - [GenerateCardUploadUrlRequest](docs/GenerateCardUploadUrlRequest.md)
@@ -177,19 +158,20 @@
 - [SearchCards200Response](docs/SearchCards200Response.md)
 - [Service](docs/Service.md)
 - [SubscriberDetails](docs/SubscriberDetails.md)
 - [SubscriberDto](docs/SubscriberDto.md)
 - [UploadParameters](docs/UploadParameters.md)
 - [ValidateMagicLink200Response](docs/ValidateMagicLink200Response.md)
 
-`<a id="documentation-for-authorization"></a>`
+<a id="documentation-for-authorization"></a>
 
 ## Documentation For Authorization
 
 Authentication schemes defined for the API:
-`<a id="bearerAuth"></a>`
+<a id="bearerAuth"></a>
 
 ### bearerAuth
 
 - **Type**: Bearer authentication
 
 ## Author
+
```

### Comparing `cardscan_client-0.0.1/cardscan_client/__init__.py` & `cardscan_client-0.1.0/cardscan_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from cardscan_client.models.create_eligibility_request import CreateEligibilityRequest
 from cardscan_client.models.deductible import Deductible
 from cardscan_client.models.direct_upload200_response import DirectUpload200Response
 from cardscan_client.models.direct_upload200_response_metadata import DirectUpload200ResponseMetadata
 from cardscan_client.models.direct_upload_request import DirectUploadRequest
 from cardscan_client.models.eligibility_api_response import EligibilityApiResponse
 from cardscan_client.models.eligibility_api_response_eligibility_request import EligibilityApiResponseEligibilityRequest
+from cardscan_client.models.eligibility_api_response_eligibility_request_subscriber import EligibilityApiResponseEligibilityRequestSubscriber
 from cardscan_client.models.eligibility_api_response_error import EligibilityApiResponseError
 from cardscan_client.models.eligibility_info import EligibilityInfo
 from cardscan_client.models.eligibility_state import EligibilityState
 from cardscan_client.models.eligibility_summarized_response import EligibilitySummarizedResponse
 from cardscan_client.models.eligibility_websocket_event import EligibilityWebsocketEvent
 from cardscan_client.models.generate_card_upload_url200_response import GenerateCardUploadUrl200Response
 from cardscan_client.models.generate_card_upload_url_request import GenerateCardUploadUrlRequest
```

### Comparing `cardscan_client-0.0.1/cardscan_client/api/card_scan_api.py` & `cardscan_client-0.1.0/cardscan_client/api/card_scan_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 import re  # noqa: F401
 import io
 import warnings
 
 from pydantic import validate_arguments, ValidationError
-from typing import overload, Optional, Union, Awaitable
 
 import asyncio
 import json
 import websockets
 
 from cardscan_client.models.card_websocket_event import CardWebsocketEvent
 from cardscan_client.models.eligibility_websocket_event import EligibilityWebsocketEvent
@@ -72,79 +71,96 @@
         token = (
             self.api_client.configuration.access_token
             or self.api_client.configuration.api_key
         )
 
         self.websocket_url = f"{self.api_client.configuration.websocket_url}?token={token}"
 
-    async def full_scan(
-        self, back_image_path: str, front_image_path: str
+    def full_scan(
+        self, front_image_path: str, back_image_path: Optional[str] = None
     ) -> CardWebsocketEvent:
         """
         Perform a full scan of a card, including both sides of a card.
         :param back_image_path: The path to the back image of the card.
         :param front_image_path: The path to the front image of the card.
         """
 
+        return asyncio.run(self._full_scan(front_image_path, back_image_path=back_image_path))
+
+    async def _full_scan(
+        self, front_image_path: str, back_image_path: Optional[str] = None
+    ) -> CardWebsocketEvent:
+        """
+        Perform a full scan of a card, including both sides of a card.
+        :param back_image_path: The path to the back image of the card. (optional)
+        :param front_image_path: The path to the front image of the card.
+        """
+
         if not self.websocket_url:
             raise ValueError("This method cannot be called without a websocket URL.")
 
-        response = await self.create_card(
-            CreateCardRequest(enable_livescan=False, enable_backside_scan=True)
+        response = self.create_card(
+            CreateCardRequest(enable_livescan=False, enable_backside_scan=(back_image_path is not None))
         )
 
         result = None
 
         async with websockets.connect(self.websocket_url) as ws:
             await ws.send(
                 json.dumps({"card_id": response.card_id, "action": "register"})
             )
 
-            front_upload_url_response = await self.generate_card_upload_url(
+            front_upload_url_response = self.generate_card_upload_url(
                 response.card_id,
                 3600,
                 GenerateCardUploadUrlRequest(orientation=ScanOrientation.FRONT),
             )
 
             upload_params = front_upload_url_response.upload_parameters.to_dict()
 
-            await self.api_client.call_api(
-                "",
+            self.api_client.call_api(
+                '',
                 "POST",
                 _host=front_upload_url_response.upload_url,
                 post_params=list(upload_params.items()),
                 files={"file": front_image_path},
                 header_params={"Content-Type": "multipart/form-data"},
                 response_types_map={}
             )
 
-
             front_side_rejection_states = [
                 CardState.FRONTSIDE_FAILED,
                 CardState.ERROR,
             ]
 
             async for message in ws:
                 event = json.loads(message)
 
                 if event["state"] in front_side_rejection_states:
                     raise Exception(
                             f"Front side failed: {event.get('error', {}).get('message', 'Unknown error')}"
                         )
 
+                if event['state'] == CardState.COMPLETED and event['type'] == 'card':
+                    result = CardWebsocketEvent.from_dict(event)
+                    break
+
                 if event["state"] == CardState.BACKSIDE_PROCESSING and event["type"] == "card":
                     break
 
-            back_upload_url_response = await self.generate_card_upload_url(
+            if back_image_path is None:
+                return result
+
+            back_upload_url_response = self.generate_card_upload_url(
                 response.card_id,
                 3600,
                 GenerateCardUploadUrlRequest(orientation=ScanOrientation.BACK),
             )
 
-            await self.api_client.call_api(
+            self.api_client.call_api(
                 '',
                 "POST",
                 _host=back_upload_url_response.upload_url,
                 post_params=list(back_upload_url_response.upload_parameters.to_dict().items()),
                 files={
                     "file": back_image_path,
                 },
@@ -169,21 +185,29 @@
                     result = CardWebsocketEvent.from_dict(event)
                     break
 
             await ws.close()
 
         return result
 
-    async def check_eligibility(
+    def check_eligibility(self, create_eligibility_request: CreateEligibilityRequest) -> EligibilityWebsocketEvent:
+        """
+        Check the eligibility of a card.
+        :param create_eligibility_request: The request object.
+        """
+
+        return asyncio.run(self._check_eligibility(create_eligibility_request))
+
+    async def _check_eligibility(
         self, create_eligibility_request: CreateEligibilityRequest
     ) -> EligibilityWebsocketEvent:
         if not self.websocket_url:
             raise ValueError("This method cannot be called without a websocket URL.")
 
-        response = await self.create_eligibility(create_eligibility_request)
+        response = self.create_eligibility(create_eligibility_request)
 
         result = None
 
         async with websockets.connect(self.websocket_url) as ws:
             await ws.send(
                 json.dumps({"card_id": response.card_id, "action": "register"})
             )
@@ -197,42 +221,56 @@
                 elif event["state"] == EligibilityState.ERROR:
                     raise Exception(f"Eligibility check failed: {event['error']}")
 
         return result
 
 
     @validate_arguments
-    async def create_card(self, create_card_request : Optional[CreateCardRequest] = None, **kwargs) -> CardApiResponse:  # noqa: E501
+    def create_card(self, create_card_request : Optional[CreateCardRequest] = None, **kwargs) -> CardApiResponse:  # noqa: E501
         """Creates a new card  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_card(create_card_request, async_req=True)
+        >>> result = thread.get()
 
         :param create_card_request:
         :type create_card_request: CreateCardRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: CardApiResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the create_card_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.create_card_with_http_info(create_card_request, **kwargs)  # noqa: E501
+        return self.create_card_with_http_info(create_card_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def create_card_with_http_info(self, create_card_request : Optional[CreateCardRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def create_card_with_http_info(self, create_card_request : Optional[CreateCardRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Creates a new card  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_card_with_http_info(create_card_request, async_req=True)
+        >>> result = thread.get()
 
         :param create_card_request:
         :type create_card_request: CreateCardRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -255,14 +293,15 @@
         _params = locals()
 
         _all_params = [
             'create_card_request'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -312,59 +351,74 @@
         _response_types_map = {
             '201': "CardApiResponse",
             '400': "ApiErrorResponse",
             '401': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/cards', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def create_eligibility(self, create_eligibility_request : Optional[CreateEligibilityRequest] = None, **kwargs) -> EligibilityApiResponse:  # noqa: E501
+    def create_eligibility(self, create_eligibility_request : Optional[CreateEligibilityRequest] = None, **kwargs) -> EligibilityApiResponse:  # noqa: E501
         """Create Eligibility Record  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_eligibility(create_eligibility_request, async_req=True)
+        >>> result = thread.get()
 
         :param create_eligibility_request:
         :type create_eligibility_request: CreateEligibilityRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: EligibilityApiResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the create_eligibility_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.create_eligibility_with_http_info(create_eligibility_request, **kwargs)  # noqa: E501
+        return self.create_eligibility_with_http_info(create_eligibility_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def create_eligibility_with_http_info(self, create_eligibility_request : Optional[CreateEligibilityRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def create_eligibility_with_http_info(self, create_eligibility_request : Optional[CreateEligibilityRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Create Eligibility Record  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_eligibility_with_http_info(create_eligibility_request, async_req=True)
+        >>> result = thread.get()
 
         :param create_eligibility_request:
         :type create_eligibility_request: CreateEligibilityRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -387,14 +441,15 @@
         _params = locals()
 
         _all_params = [
             'create_eligibility_request'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -445,59 +500,74 @@
             '201': "EligibilityApiResponse",
             '400': "ApiErrorResponse",
             '401': "ApiErrorResponse",
             '404': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/eligibility', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def delete_card_by_id(self, card_id : Annotated[StrictStr, Field(..., description="The ID of the card")], **kwargs) -> None:  # noqa: E501
+    def delete_card_by_id(self, card_id : Annotated[StrictStr, Field(..., description="The ID of the card")], **kwargs) -> None:  # noqa: E501
         """Delete Card  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_card_by_id(card_id, async_req=True)
+        >>> result = thread.get()
 
         :param card_id: The ID of the card (required)
         :type card_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the delete_card_by_id_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.delete_card_by_id_with_http_info(card_id, **kwargs)  # noqa: E501
+        return self.delete_card_by_id_with_http_info(card_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def delete_card_by_id_with_http_info(self, card_id : Annotated[StrictStr, Field(..., description="The ID of the card")], **kwargs) -> ApiResponse:  # noqa: E501
+    def delete_card_by_id_with_http_info(self, card_id : Annotated[StrictStr, Field(..., description="The ID of the card")], **kwargs) -> ApiResponse:  # noqa: E501
         """Delete Card  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_card_by_id_with_http_info(card_id, async_req=True)
+        >>> result = thread.get()
 
         :param card_id: The ID of the card (required)
         :type card_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -520,14 +590,15 @@
         _params = locals()
 
         _all_params = [
             'card_id'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -565,71 +636,86 @@
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {}
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/cards/{card_id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def direct_upload(self, orientation : ScanOrientation, capture_type : ScanCaptureType, card_id : StrictStr, direct_upload_request : Optional[DirectUploadRequest] = None, **kwargs) -> DirectUpload200Response:  # noqa: E501
+    def direct_upload(self, orientation : ScanOrientation, capture_type : ScanCaptureType, card_id : StrictStr, direct_upload_request : Optional[DirectUploadRequest] = None, **kwargs) -> DirectUpload200Response:  # noqa: E501
         """Direct Upload  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.direct_upload(orientation, capture_type, card_id, direct_upload_request, async_req=True)
+        >>> result = thread.get()
 
         :param orientation: (required)
         :type orientation: ScanOrientation
         :param capture_type: (required)
         :type capture_type: ScanCaptureType
         :param card_id: (required)
         :type card_id: str
         :param direct_upload_request:
         :type direct_upload_request: DirectUploadRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DirectUpload200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the direct_upload_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.direct_upload_with_http_info(orientation, capture_type, card_id, direct_upload_request, **kwargs)  # noqa: E501
+        return self.direct_upload_with_http_info(orientation, capture_type, card_id, direct_upload_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def direct_upload_with_http_info(self, orientation : ScanOrientation, capture_type : ScanCaptureType, card_id : StrictStr, direct_upload_request : Optional[DirectUploadRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def direct_upload_with_http_info(self, orientation : ScanOrientation, capture_type : ScanCaptureType, card_id : StrictStr, direct_upload_request : Optional[DirectUploadRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Direct Upload  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.direct_upload_with_http_info(orientation, capture_type, card_id, direct_upload_request, async_req=True)
+        >>> result = thread.get()
 
         :param orientation: (required)
         :type orientation: ScanOrientation
         :param capture_type: (required)
         :type capture_type: ScanCaptureType
         :param card_id: (required)
         :type card_id: str
         :param direct_upload_request:
         :type direct_upload_request: DirectUploadRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -655,14 +741,15 @@
             'orientation',
             'capture_type',
             'card_id',
             'direct_upload_request'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -723,67 +810,82 @@
             '400': "ApiErrorResponse",
             '401': "ApiErrorResponse",
             '403': "ApiErrorResponse",
             '404': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/cards/{card_id}/upload', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def generate_card_upload_url(self, card_id : StrictStr, expiration : Optional[conint(strict=True, le=3600, ge=100)] = None, generate_card_upload_url_request : Optional[GenerateCardUploadUrlRequest] = None, **kwargs) -> GenerateCardUploadUrl200Response:  # noqa: E501
+    def generate_card_upload_url(self, card_id : StrictStr, expiration : Optional[conint(strict=True, le=3600, ge=100)] = None, generate_card_upload_url_request : Optional[GenerateCardUploadUrlRequest] = None, **kwargs) -> GenerateCardUploadUrl200Response:  # noqa: E501
         """Card - Generate Upload URL  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.generate_card_upload_url(card_id, expiration, generate_card_upload_url_request, async_req=True)
+        >>> result = thread.get()
 
         :param card_id: (required)
         :type card_id: str
         :param expiration:
         :type expiration: int
         :param generate_card_upload_url_request:
         :type generate_card_upload_url_request: GenerateCardUploadUrlRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenerateCardUploadUrl200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the generate_card_upload_url_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.generate_card_upload_url_with_http_info(card_id, expiration, generate_card_upload_url_request, **kwargs)  # noqa: E501
+        return self.generate_card_upload_url_with_http_info(card_id, expiration, generate_card_upload_url_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def generate_card_upload_url_with_http_info(self, card_id : StrictStr, expiration : Optional[conint(strict=True, le=3600, ge=100)] = None, generate_card_upload_url_request : Optional[GenerateCardUploadUrlRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def generate_card_upload_url_with_http_info(self, card_id : StrictStr, expiration : Optional[conint(strict=True, le=3600, ge=100)] = None, generate_card_upload_url_request : Optional[GenerateCardUploadUrlRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Card - Generate Upload URL  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.generate_card_upload_url_with_http_info(card_id, expiration, generate_card_upload_url_request, async_req=True)
+        >>> result = thread.get()
 
         :param card_id: (required)
         :type card_id: str
         :param expiration:
         :type expiration: int
         :param generate_card_upload_url_request:
         :type generate_card_upload_url_request: GenerateCardUploadUrlRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -808,14 +910,15 @@
         _all_params = [
             'card_id',
             'expiration',
             'generate_card_upload_url_request'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -873,55 +976,70 @@
             '400': "ApiErrorResponse",
             '401': "ApiErrorResponse",
             '403': "ApiErrorResponse",
             '404': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/cards/{card_id}/generate-upload-url', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def generate_magic_link(self, **kwargs) -> GenerateMagicLink200Response:  # noqa: E501
+    def generate_magic_link(self, **kwargs) -> GenerateMagicLink200Response:  # noqa: E501
         """Generate Magic Link  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
 
+        >>> thread = api.generate_magic_link(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenerateMagicLink200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the generate_magic_link_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.generate_magic_link_with_http_info(**kwargs)  # noqa: E501
+        return self.generate_magic_link_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    async def generate_magic_link_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
+    def generate_magic_link_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
         """Generate Magic Link  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.generate_magic_link_with_http_info(async_req=True)
+        >>> result = thread.get()
 
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -943,14 +1061,15 @@
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -989,59 +1108,74 @@
 
         _response_types_map = {
             '200': "GenerateMagicLink200Response",
             '401': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/generate-magic-link', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def generate_upload_url(self, expiration : conint(strict=True, le=3600, ge=100), **kwargs) -> GenerateCardUploadUrl200Response:  # noqa: E501
+    def generate_upload_url(self, expiration : conint(strict=True, le=3600, ge=100), **kwargs) -> GenerateCardUploadUrl200Response:  # noqa: E501
         """Generate an upload URL  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.generate_upload_url(expiration, async_req=True)
+        >>> result = thread.get()
 
         :param expiration: (required)
         :type expiration: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenerateCardUploadUrl200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the generate_upload_url_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.generate_upload_url_with_http_info(expiration, **kwargs)  # noqa: E501
+        return self.generate_upload_url_with_http_info(expiration, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def generate_upload_url_with_http_info(self, expiration : conint(strict=True, le=3600, ge=100), **kwargs) -> ApiResponse:  # noqa: E501
+    def generate_upload_url_with_http_info(self, expiration : conint(strict=True, le=3600, ge=100), **kwargs) -> ApiResponse:  # noqa: E501
         """Generate an upload URL  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.generate_upload_url_with_http_info(expiration, async_req=True)
+        >>> result = thread.get()
 
         :param expiration: (required)
         :type expiration: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -1064,14 +1198,15 @@
         _params = locals()
 
         _all_params = [
             'expiration'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -1114,59 +1249,74 @@
         _response_types_map = {
             '200': "GenerateCardUploadUrl200Response",
             '400': "ApiErrorResponse",
             '401': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/generate-upload-url', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def get_access_token(self, user_id : Annotated[Optional[StrictStr], Field(description="The ID of the user")] = None, **kwargs) -> GetAccessToken200Response:  # noqa: E501
+    def get_access_token(self, user_id : Annotated[Optional[StrictStr], Field(description="The ID of the user")] = None, **kwargs) -> GetAccessToken200Response:  # noqa: E501
         """Access Token  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_access_token(user_id, async_req=True)
+        >>> result = thread.get()
 
         :param user_id: The ID of the user
         :type user_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GetAccessToken200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the get_access_token_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.get_access_token_with_http_info(user_id, **kwargs)  # noqa: E501
+        return self.get_access_token_with_http_info(user_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def get_access_token_with_http_info(self, user_id : Annotated[Optional[StrictStr], Field(description="The ID of the user")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_access_token_with_http_info(self, user_id : Annotated[Optional[StrictStr], Field(description="The ID of the user")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Access Token  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_access_token_with_http_info(user_id, async_req=True)
+        >>> result = thread.get()
 
         :param user_id: The ID of the user
         :type user_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -1189,14 +1339,15 @@
         _params = locals()
 
         _all_params = [
             'user_id'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -1238,59 +1389,74 @@
 
         _response_types_map = {
             '200': "GetAccessToken200Response",
             '401': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/access-token', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def get_card_by_id(self, card_id : Annotated[StrictStr, Field(..., description="The ID of the card")], **kwargs) -> CardApiResponse:  # noqa: E501
+    def get_card_by_id(self, card_id : Annotated[StrictStr, Field(..., description="The ID of the card")], **kwargs) -> CardApiResponse:  # noqa: E501
         """Get Card by ID  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_card_by_id(card_id, async_req=True)
+        >>> result = thread.get()
 
         :param card_id: The ID of the card (required)
         :type card_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: CardApiResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the get_card_by_id_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.get_card_by_id_with_http_info(card_id, **kwargs)  # noqa: E501
+        return self.get_card_by_id_with_http_info(card_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def get_card_by_id_with_http_info(self, card_id : Annotated[StrictStr, Field(..., description="The ID of the card")], **kwargs) -> ApiResponse:  # noqa: E501
+    def get_card_by_id_with_http_info(self, card_id : Annotated[StrictStr, Field(..., description="The ID of the card")], **kwargs) -> ApiResponse:  # noqa: E501
         """Get Card by ID  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_card_by_id_with_http_info(card_id, async_req=True)
+        >>> result = thread.get()
 
         :param card_id: The ID of the card (required)
         :type card_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -1313,14 +1479,15 @@
         _params = locals()
 
         _all_params = [
             'card_id'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -1364,59 +1531,74 @@
             '200': "CardApiResponse",
             '401': "ApiErrorResponse",
             '403': "ApiErrorResponse",
             '404': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/cards/{card_id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def get_eligibility_by_id(self, eligibility_id : StrictStr, **kwargs) -> EligibilityApiResponse:  # noqa: E501
+    def get_eligibility_by_id(self, eligibility_id : StrictStr, **kwargs) -> EligibilityApiResponse:  # noqa: E501
         """Get Eligibility  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_eligibility_by_id(eligibility_id, async_req=True)
+        >>> result = thread.get()
 
         :param eligibility_id: (required)
         :type eligibility_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: EligibilityApiResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the get_eligibility_by_id_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.get_eligibility_by_id_with_http_info(eligibility_id, **kwargs)  # noqa: E501
+        return self.get_eligibility_by_id_with_http_info(eligibility_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def get_eligibility_by_id_with_http_info(self, eligibility_id : StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_eligibility_by_id_with_http_info(self, eligibility_id : StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
         """Get Eligibility  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_eligibility_by_id_with_http_info(eligibility_id, async_req=True)
+        >>> result = thread.get()
 
         :param eligibility_id: (required)
         :type eligibility_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -1439,14 +1621,15 @@
         _params = locals()
 
         _all_params = [
             'eligibility_id'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -1490,59 +1673,74 @@
             '200': "EligibilityApiResponse",
             '400': "ApiErrorResponse",
             '401': "ApiErrorResponse",
             '404': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/eligibility/{eligibility_id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def get_scan_metadata(self, scan_id : StrictStr, **kwargs) -> None:  # noqa: E501
+    def get_scan_metadata(self, scan_id : StrictStr, **kwargs) -> None:  # noqa: E501
         """Get Scan Metadata  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_scan_metadata(scan_id, async_req=True)
+        >>> result = thread.get()
 
         :param scan_id: (required)
         :type scan_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the get_scan_metadata_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.get_scan_metadata_with_http_info(scan_id, **kwargs)  # noqa: E501
+        return self.get_scan_metadata_with_http_info(scan_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def get_scan_metadata_with_http_info(self, scan_id : StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_scan_metadata_with_http_info(self, scan_id : StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
         """Get Scan Metadata  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_scan_metadata_with_http_info(scan_id, async_req=True)
+        >>> result = thread.get()
 
         :param scan_id: (required)
         :type scan_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -1565,14 +1763,15 @@
         _params = locals()
 
         _all_params = [
             'scan_id'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -1610,63 +1809,78 @@
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {}
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/scans/{scan_id}/metadata', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def list_cards(self, limit : Optional[StrictInt] = None, cursor : Optional[StrictStr] = None, **kwargs) -> SearchCards200Response:  # noqa: E501
+    def list_cards(self, limit : Optional[StrictInt] = None, cursor : Optional[StrictStr] = None, **kwargs) -> SearchCards200Response:  # noqa: E501
         """List Cards  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_cards(limit, cursor, async_req=True)
+        >>> result = thread.get()
 
         :param limit:
         :type limit: int
         :param cursor:
         :type cursor: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: SearchCards200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the list_cards_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.list_cards_with_http_info(limit, cursor, **kwargs)  # noqa: E501
+        return self.list_cards_with_http_info(limit, cursor, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def list_cards_with_http_info(self, limit : Optional[StrictInt] = None, cursor : Optional[StrictStr] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def list_cards_with_http_info(self, limit : Optional[StrictInt] = None, cursor : Optional[StrictStr] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """List Cards  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_cards_with_http_info(limit, cursor, async_req=True)
+        >>> result = thread.get()
 
         :param limit:
         :type limit: int
         :param cursor:
         :type cursor: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -1690,14 +1904,15 @@
 
         _all_params = [
             'limit',
             'cursor'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -1742,55 +1957,70 @@
 
         _response_types_map = {
             '200': "SearchCards200Response",
             '401': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/cards', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def list_eligibility(self, **kwargs) -> ListEligibility200Response:  # noqa: E501
+    def list_eligibility(self, **kwargs) -> ListEligibility200Response:  # noqa: E501
         """List Eligibility  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_eligibility(async_req=True)
+        >>> result = thread.get()
 
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ListEligibility200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the list_eligibility_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.list_eligibility_with_http_info(**kwargs)  # noqa: E501
+        return self.list_eligibility_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    async def list_eligibility_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
+    def list_eligibility_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
         """List Eligibility  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
 
+        >>> thread = api.list_eligibility_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -1812,14 +2042,15 @@
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -1857,67 +2088,82 @@
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
             '200': "ListEligibility200Response",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/eligibility', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def search_cards(self, query : StrictStr, limit : Optional[StrictInt] = None, cursor : Optional[StrictStr] = None, **kwargs) -> SearchCards200Response:  # noqa: E501
+    def search_cards(self, query : StrictStr, limit : Optional[StrictInt] = None, cursor : Optional[StrictStr] = None, **kwargs) -> SearchCards200Response:  # noqa: E501
         """Search Cards (200) OK  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.search_cards(query, limit, cursor, async_req=True)
+        >>> result = thread.get()
 
         :param query: (required)
         :type query: str
         :param limit:
         :type limit: int
         :param cursor:
         :type cursor: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: SearchCards200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the search_cards_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.search_cards_with_http_info(query, limit, cursor, **kwargs)  # noqa: E501
+        return self.search_cards_with_http_info(query, limit, cursor, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def search_cards_with_http_info(self, query : StrictStr, limit : Optional[StrictInt] = None, cursor : Optional[StrictStr] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def search_cards_with_http_info(self, query : StrictStr, limit : Optional[StrictInt] = None, cursor : Optional[StrictStr] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Search Cards (200) OK  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.search_cards_with_http_info(query, limit, cursor, async_req=True)
+        >>> result = thread.get()
 
         :param query: (required)
         :type query: str
         :param limit:
         :type limit: int
         :param cursor:
         :type cursor: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -1942,14 +2188,15 @@
         _all_params = [
             'query',
             'limit',
             'cursor'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -1997,59 +2244,74 @@
 
         _response_types_map = {
             '200': "SearchCards200Response",
             '401': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/cards/search', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    async def validate_magic_link(self, token : StrictStr, **kwargs) -> ValidateMagicLink200Response:  # noqa: E501
+    def validate_magic_link(self, token : StrictStr, **kwargs) -> ValidateMagicLink200Response:  # noqa: E501
         """Validate Magic Link  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.validate_magic_link(token, async_req=True)
+        >>> result = thread.get()
 
         :param token: (required)
         :type token: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ValidateMagicLink200Response
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the validate_magic_link_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return await self.validate_magic_link_with_http_info(token, **kwargs)  # noqa: E501
+        return self.validate_magic_link_with_http_info(token, **kwargs)  # noqa: E501
 
     @validate_arguments
-    async def validate_magic_link_with_http_info(self, token : StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
+    def validate_magic_link_with_http_info(self, token : StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
         """Validate Magic Link  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.validate_magic_link_with_http_info(token, async_req=True)
+        >>> result = thread.get()
 
         :param token: (required)
         :type token: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
@@ -2072,14 +2334,15 @@
         _params = locals()
 
         _all_params = [
             'token'
         ]
         _all_params.extend(
             [
+                'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
                 '_headers'
             ]
@@ -2123,22 +2386,23 @@
             '200': "ValidateMagicLink200Response",
             '400': "ApiErrorResponse",
             '404': "ApiErrorResponse",
             '410': "ApiErrorResponse",
             '500': "GetAccessToken500Response",
         }
 
-        return await self.api_client.call_api(
+        return self.api_client.call_api(
             '/validate-magic-link', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `cardscan_client-0.0.1/cardscan_client/api_client.py` & `cardscan_client-0.1.0/cardscan_client/api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 import atexit
 import datetime
 from dateutil.parser import parse
 import json
 import mimetypes
+from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
 
 from cardscan_client.configuration import Configuration
@@ -40,14 +41,16 @@
 
     :param configuration: .Configuration object for this client
     :param header_name: a header to pass when making calls to the API.
     :param header_value: a header value to pass when making calls to
         the API.
     :param cookie: a cookie to include in the header when making calls
         to the API
+    :param pool_threads: The number of threads to use for async requests
+        to the API. More threads means more concurrent API requests.
     """
 
     PRIMITIVE_TYPES = (float, bool, bytes, str, int)
     NATIVE_TYPES_MAPPING = {
         'int': int,
         'long': int, # TODO remove as only py3 is supported?
         'float': float,
@@ -56,37 +59,53 @@
         'date': datetime.date,
         'datetime': datetime.datetime,
         'object': object,
     }
     _pool = None
 
     def __init__(self, configuration=None, header_name=None, header_value=None,
-                 cookie=None) -> None:
+                 cookie=None, pool_threads=1) -> None:
         # use default configuration if none is provided
         if configuration is None:
             configuration = Configuration.get_default()
         self.configuration = configuration
+        self.pool_threads = pool_threads
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         self.user_agent = 'OpenAPI-Generator/1.0.0/python'
         self.client_side_validation = configuration.client_side_validation
 
-    async def __aenter__(self):
+    def __enter__(self):
         return self
 
-    async def __aexit__(self, exc_type, exc_value, traceback):
-        await self.close()
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
 
-    async def close(self):
-        await self.rest_client.close()
+    def close(self):
+        if self._pool:
+            self._pool.close()
+            self._pool.join()
+            self._pool = None
+            if hasattr(atexit, 'unregister'):
+                atexit.unregister(self.close)
+
+    @property
+    def pool(self):
+        """Create thread pool on first request
+         avoids instantiating unused threadpool for blocking clients.
+        """
+        if self._pool is None:
+            atexit.register(self.close)
+            self._pool = ThreadPool(self.pool_threads)
+        return self._pool
 
     @property
     def user_agent(self):
         """User agent for this API client"""
         return self.default_headers['User-Agent']
 
     @user_agent.setter
@@ -119,15 +138,15 @@
 
         It stores default ApiClient.
 
         :param default: object of ApiClient.
         """
         cls._default = default
 
-    async def __call_api(
+    def __call_api(
             self, resource_path, method, path_params=None,
             query_params=None, header_params=None, body=None, post_params=None,
             files=None, response_types_map=None, auth_settings=None,
             _return_http_data_only=None, collection_formats=None,
             _preload_content=True, _request_timeout=None, _host=None,
             _request_auth=None):
 
@@ -185,15 +204,15 @@
             query_params = self.sanitize_for_serialization(query_params)
             url_query = self.parameters_to_url_query(query_params,
                                                      collection_formats)
             url += "?" + url_query
 
         try:
             # perform request and return response
-            response_data = await self.request(
+            response_data = self.request(
                 method, url,
                 query_params=query_params,
                 headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout)
         except ApiException as e:
@@ -334,36 +353,39 @@
         elif klass == datetime.date:
             return self.__deserialize_date(data)
         elif klass == datetime.datetime:
             return self.__deserialize_datetime(data)
         else:
             return self.__deserialize_model(data, klass)
 
-    async def call_api(self, resource_path, method,
+    def call_api(self, resource_path, method,
                  path_params=None, query_params=None, header_params=None,
                  body=None, post_params=None, files=None,
                  response_types_map=None, auth_settings=None,
-                 _return_http_data_only=None,
+                 async_req=None, _return_http_data_only=None,
                  collection_formats=None, _preload_content=True,
                  _request_timeout=None, _host=None, _request_auth=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
+        To make an async_req request, set the async_req parameter.
+
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
         :param query_params: Query parameters in the url.
         :param header_params: Header parameters to be
             placed in the request header.
         :param body: Request body.
         :param post_params dict: Request post form parameters,
             for `application/x-www-form-urlencoded`, `multipart/form-data`.
         :param auth_settings list: Auth Settings names for the request.
         :param response: Response data type.
         :param files dict: key -> filename, value -> filepath,
             for `multipart/form-data`.
+        :param async_req bool: execute request asynchronously
         :param _return_http_data_only: response data instead of ApiResponse
                                        object with status code, headers, etc
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :param collection_formats: dict of collection formats for path, query,
@@ -373,15 +395,19 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_token: dict, optional
         :return:
-            The response.
+            If async_req parameter is True,
+            the request will be called asynchronously.
+            The method will return the request thread.
+            If parameter async_req is False or missing,
+            then the method will return the response directly.
         """
         args = (
             resource_path,
             method,
             path_params,
             query_params,
             header_params,
@@ -393,64 +419,67 @@
             _return_http_data_only,
             collection_formats,
             _preload_content,
             _request_timeout,
             _host,
             _request_auth,
         )
-        return await self.__call_api(*args)
+        if not async_req:
+            return self.__call_api(*args)
+
+        return self.pool.apply_async(self.__call_api, args)
 
-    async def request(self, method, url, query_params=None, headers=None,
+    def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
                 _request_timeout=None):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
-            return await self.rest_client.get_request(url,
+            return self.rest_client.get_request(url,
                                         query_params=query_params,
                                         _preload_content=_preload_content,
                                         _request_timeout=_request_timeout,
                                         headers=headers)
         elif method == "HEAD":
-            return await self.rest_client.head_request(url,
+            return self.rest_client.head_request(url,
                                          query_params=query_params,
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
                                          headers=headers)
         elif method == "OPTIONS":
-            return await self.rest_client.options_request(url,
+            return self.rest_client.options_request(url,
                                             query_params=query_params,
                                             headers=headers,
                                             _preload_content=_preload_content,
                                             _request_timeout=_request_timeout)
         elif method == "POST":
-            return await self.rest_client.post_request(url,
+            return self.rest_client.post_request(url,
                                          query_params=query_params,
                                          headers=headers,
                                          post_params=post_params,
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
                                          body=body)
         elif method == "PUT":
-            return await self.rest_client.put_request(url,
+            return self.rest_client.put_request(url,
                                         query_params=query_params,
                                         headers=headers,
                                         post_params=post_params,
                                         _preload_content=_preload_content,
                                         _request_timeout=_request_timeout,
                                         body=body)
         elif method == "PATCH":
-            return await self.rest_client.patch_request(url,
+            return self.rest_client.patch_request(url,
                                           query_params=query_params,
                                           headers=headers,
                                           post_params=post_params,
                                           _preload_content=_preload_content,
                                           _request_timeout=_request_timeout,
                                           body=body)
         elif method == "DELETE":
-            return await self.rest_client.delete_request(url,
+            return self.rest_client.delete_request(url,
                                            query_params=query_params,
                                            headers=headers,
                                            _preload_content=_preload_content,
                                            _request_timeout=_request_timeout,
                                            body=body)
         else:
             raise ApiValueError(
```

### Comparing `cardscan_client-0.0.1/cardscan_client/api_response.py` & `cardscan_client-0.1.0/cardscan_client/api_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/configuration.py` & `cardscan_client-0.1.0/cardscan_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
 import logging
+import multiprocessing
 import sys
 import urllib3
 
 import http.client as httplib
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
@@ -65,16 +66,18 @@
                  ) -> None:
         """Constructor
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
+        prefix = 'api' if environment.startswith('prod') else 'sandbox'
+
         self.server_variables = server_variables or {
-            "prefix": environment,
+            "prefix": prefix,
             "version": "v1",
         }
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
 
         self._base_path = host if host is not None else self.get_host_from_settings(0)
@@ -138,17 +141,20 @@
         """Set this to True/False to enable/disable SSL hostname verification.
         """
         self.tls_server_name = None
         """SSL/TLS Server Name Indication (SNI)
            Set this to the SNI value expected by the server.
         """
 
-        self.connection_pool_maxsize = 100
-        """This value is passed to the aiohttp to limit simultaneous connections.
-           Default values is 100, None means no-limit.
+        self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
+        """urllib3 connection pool's maximum number of connections saved
+           per pool. urllib3 uses 1 connection as default value, but this is
+           not the best value when you are making a lot of possibly parallel
+           requests to the same host, which is often the case here.
+           cpu_count * 5 is used as default value to increase performance.
         """
 
         self.proxy = None
         """Proxy URL
         """
         self.proxy_headers = None
         """Proxy headers
@@ -170,15 +176,15 @@
         """datetime format
         """
 
         self.date_format = "%Y-%m-%d"
         """date format
         """
 
-        self.websocket_url = websocket_url or f"wss://{environment}-ws.cardscan.ai"
+        self.websocket_url = websocket_url or f"wss://{prefix}-ws.cardscan.ai"
         """websocket url
         """
 
         self.environment = environment
         """api environment to use
         """
```

### Comparing `cardscan_client-0.0.1/cardscan_client/exceptions.py` & `cardscan_client-0.1.0/cardscan_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/__init__.py` & `cardscan_client-0.1.0/cardscan_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from cardscan_client.models.create_eligibility_request import CreateEligibilityRequest
 from cardscan_client.models.deductible import Deductible
 from cardscan_client.models.direct_upload200_response import DirectUpload200Response
 from cardscan_client.models.direct_upload200_response_metadata import DirectUpload200ResponseMetadata
 from cardscan_client.models.direct_upload_request import DirectUploadRequest
 from cardscan_client.models.eligibility_api_response import EligibilityApiResponse
 from cardscan_client.models.eligibility_api_response_eligibility_request import EligibilityApiResponseEligibilityRequest
+from cardscan_client.models.eligibility_api_response_eligibility_request_subscriber import EligibilityApiResponseEligibilityRequestSubscriber
 from cardscan_client.models.eligibility_api_response_error import EligibilityApiResponseError
 from cardscan_client.models.eligibility_info import EligibilityInfo
 from cardscan_client.models.eligibility_state import EligibilityState
 from cardscan_client.models.eligibility_summarized_response import EligibilitySummarizedResponse
 from cardscan_client.models.eligibility_websocket_event import EligibilityWebsocketEvent
 from cardscan_client.models.generate_card_upload_url200_response import GenerateCardUploadUrl200Response
 from cardscan_client.models.generate_card_upload_url_request import GenerateCardUploadUrlRequest
```

### Comparing `cardscan_client-0.0.1/cardscan_client/models/address.py` & `cardscan_client-0.1.0/cardscan_client/models/address.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/api_error_response.py` & `cardscan_client-0.1.0/cardscan_client/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/card_api_response.py` & `cardscan_client-0.1.0/cardscan_client/models/card_api_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/card_api_response_details.py` & `cardscan_client-0.1.0/cardscan_client/models/card_api_response_details.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/card_api_response_images.py` & `cardscan_client-0.1.0/cardscan_client/models/card_api_response_images.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/card_api_response_images_back.py` & `cardscan_client-0.1.0/cardscan_client/models/card_api_response_images_back.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/card_api_response_images_front.py` & `cardscan_client-0.1.0/cardscan_client/models/card_api_response_images_front.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/card_state.py` & `cardscan_client-0.1.0/cardscan_client/models/card_state.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/card_websocket_event.py` & `cardscan_client-0.1.0/cardscan_client/models/card_websocket_event.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/co_insurance.py` & `cardscan_client-0.1.0/cardscan_client/models/co_insurance.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/co_payment.py` & `cardscan_client-0.1.0/cardscan_client/models/co_payment.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/coverage_summary.py` & `cardscan_client-0.1.0/cardscan_client/models/coverage_summary.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/create_card_request.py` & `cardscan_client-0.1.0/cardscan_client/models/create_card_request.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/create_card_request_backside.py` & `cardscan_client-0.1.0/cardscan_client/models/create_card_request_backside.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/create_eligibility_request.py` & `cardscan_client-0.1.0/cardscan_client/models/create_eligibility_request.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/deductible.py` & `cardscan_client-0.1.0/cardscan_client/models/deductible.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/direct_upload200_response.py` & `cardscan_client-0.1.0/cardscan_client/models/direct_upload200_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/direct_upload200_response_metadata.py` & `cardscan_client-0.1.0/cardscan_client/models/direct_upload200_response_metadata.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/direct_upload_request.py` & `cardscan_client-0.1.0/cardscan_client/models/direct_upload_request.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/eligibility_api_response.py` & `cardscan_client-0.1.0/cardscan_client/models/eligibility_api_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/eligibility_api_response_eligibility_request.py` & `cardscan_client-0.1.0/cardscan_client/models/eligibility_api_response_eligibility_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
+from cardscan_client.models.eligibility_api_response_eligibility_request_subscriber import EligibilityApiResponseEligibilityRequestSubscriber
 from cardscan_client.models.provider_dto import ProviderDto
-from cardscan_client.models.subscriber_dto import SubscriberDto
 
 class EligibilityApiResponseEligibilityRequest(BaseModel):
     """
     The eligibility request.  # noqa: E501
     """
     control_number: Optional[StrictStr] = Field(default=None, alias="controlNumber", description="The control number of the claim.")
     trading_partner_service_id: Optional[StrictStr] = Field(default=None, alias="tradingPartnerServiceId", description="The ID of the trading partner service.")
     provider: Optional[ProviderDto] = None
-    subscriber: Optional[SubscriberDto] = None
+    subscriber: Optional[EligibilityApiResponseEligibilityRequestSubscriber] = None
     __properties = ["controlNumber", "tradingPartnerServiceId", "provider", "subscriber"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -74,12 +74,12 @@
         if not isinstance(obj, dict):
             return EligibilityApiResponseEligibilityRequest.parse_obj(obj)
 
         _obj = EligibilityApiResponseEligibilityRequest.parse_obj({
             "control_number": obj.get("controlNumber"),
             "trading_partner_service_id": obj.get("tradingPartnerServiceId"),
             "provider": ProviderDto.from_dict(obj.get("provider")) if obj.get("provider") is not None else None,
-            "subscriber": SubscriberDto.from_dict(obj.get("subscriber")) if obj.get("subscriber") is not None else None
+            "subscriber": EligibilityApiResponseEligibilityRequestSubscriber.from_dict(obj.get("subscriber")) if obj.get("subscriber") is not None else None
         })
         return _obj
```

### Comparing `cardscan_client-0.0.1/cardscan_client/models/eligibility_api_response_error.py` & `cardscan_client-0.1.0/cardscan_client/models/eligibility_api_response_error.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/eligibility_info.py` & `cardscan_client-0.1.0/cardscan_client/models/eligibility_info.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/eligibility_state.py` & `cardscan_client-0.1.0/cardscan_client/models/eligibility_state.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/eligibility_summarized_response.py` & `cardscan_client-0.1.0/cardscan_client/models/eligibility_summarized_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/eligibility_websocket_event.py` & `cardscan_client-0.1.0/cardscan_client/models/eligibility_websocket_event.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/generate_card_upload_url200_response.py` & `cardscan_client-0.1.0/cardscan_client/models/generate_card_upload_url200_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/generate_card_upload_url_request.py` & `cardscan_client-0.1.0/cardscan_client/models/generate_card_upload_url_request.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/generate_magic_link200_response.py` & `cardscan_client-0.1.0/cardscan_client/models/generate_magic_link200_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/get_access_token200_response.py` & `cardscan_client-0.1.0/cardscan_client/models/get_access_token200_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/get_access_token500_response.py` & `cardscan_client-0.1.0/cardscan_client/models/get_access_token500_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/list_eligibility200_response.py` & `cardscan_client-0.1.0/cardscan_client/models/list_eligibility200_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/match_score.py` & `cardscan_client-0.1.0/cardscan_client/models/match_score.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/oop.py` & `cardscan_client-0.1.0/cardscan_client/models/oop.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/payer_details.py` & `cardscan_client-0.1.0/cardscan_client/models/payer_details.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/plan_details.py` & `cardscan_client-0.1.0/cardscan_client/models/plan_details.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/provider_dto.py` & `cardscan_client-0.1.0/cardscan_client/models/provider_dto.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/response_metadata.py` & `cardscan_client-0.1.0/cardscan_client/models/response_metadata.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_capture_type.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_capture_type.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_camera_capabilities.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_camera_capabilities.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_camera_capabilities_aspect_ratio.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_camera_capabilities_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_capture_canvas.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_capture_canvas.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_capture_score.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_capture_score.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_capture_score_scores_inner.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_capture_score_scores_inner.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_guides.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_guides.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_video_background.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_video_background.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_video_track.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_video_track.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_metadata_window_inner.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_metadata_window_inner.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/scan_orientation.py` & `cardscan_client-0.1.0/cardscan_client/models/scan_orientation.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/search_cards200_response.py` & `cardscan_client-0.1.0/cardscan_client/models/search_cards200_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/service.py` & `cardscan_client-0.1.0/cardscan_client/models/service.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/subscriber_details.py` & `cardscan_client-0.1.0/cardscan_client/models/subscriber_details.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/subscriber_dto.py` & `cardscan_client-0.1.0/cardscan_client/models/subscriber_dto.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/upload_parameters.py` & `cardscan_client-0.1.0/cardscan_client/models/upload_parameters.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/models/validate_magic_link200_response.py` & `cardscan_client-0.1.0/cardscan_client/models/validate_magic_link200_response.py`

 * *Files identical despite different names*

### Comparing `cardscan_client-0.0.1/cardscan_client/rest.py` & `cardscan_client-0.1.0/cardscan_client/rest.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,89 +14,139 @@
 
 import io
 import json
 import logging
 import re
 import ssl
 
-import aiohttp
 from urllib.parse import urlencode, quote_plus
+import urllib3
+
+from cardscan_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError, BadRequestException
 
-from cardscan_client.exceptions import ApiException, ApiValueError
 
 logger = logging.getLogger(__name__)
 
+SUPPORTED_SOCKS_PROXIES = {"socks5", "socks5h", "socks4", "socks4a"}
+
+
+def is_socks_proxy_url(url):
+    if url is None:
+        return False
+    split_section = url.split("://")
+    if len(split_section) < 2:
+        return False
+    else:
+        return split_section[0].lower() in SUPPORTED_SOCKS_PROXIES
+
 
 class RESTResponse(io.IOBase):
 
-    def __init__(self, resp, data) -> None:
-        self.aiohttp_response = resp
+    def __init__(self, resp) -> None:
+        self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
-        self.data = data
+        self.data = resp.data
 
     def getheaders(self):
-        """Returns a CIMultiDictProxy of the response headers."""
-        return self.aiohttp_response.headers
+        """Returns a dictionary of the response headers."""
+        return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
-        return self.aiohttp_response.headers.get(name, default)
+        return self.urllib3_response.headers.get(name, default)
 
 
 class RESTClientObject:
 
     def __init__(self, configuration, pools_size=4, maxsize=None) -> None:
+        # urllib3.PoolManager will pass all kw parameters to connectionpool
+        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
+        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
+        # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
+        # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
+
+        # cert_reqs
+        if configuration.verify_ssl:
+            cert_reqs = ssl.CERT_REQUIRED
+        else:
+            cert_reqs = ssl.CERT_NONE
+
+        addition_pool_args = {}
+        if configuration.assert_hostname is not None:
+            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
+
+        if configuration.retries is not None:
+            addition_pool_args['retries'] = configuration.retries
 
-        # maxsize is number of requests to host that are allowed in parallel
-        if maxsize is None:
-            maxsize = configuration.connection_pool_maxsize
+        if configuration.tls_server_name:
+            addition_pool_args['server_hostname'] = configuration.tls_server_name
 
-        ssl_context = ssl.create_default_context(cafile=configuration.ssl_ca_cert)
-        if configuration.cert_file:
-            ssl_context.load_cert_chain(
-                configuration.cert_file, keyfile=configuration.key_file
-            )
 
-        if not configuration.verify_ssl:
-            ssl_context.check_hostname = False
-            ssl_context.verify_mode = ssl.CERT_NONE
-
-        connector = aiohttp.TCPConnector(
-            limit=maxsize,
-            ssl=ssl_context
-        )
+        if configuration.socket_options is not None:
+            addition_pool_args['socket_options'] = configuration.socket_options
 
-        self.proxy = configuration.proxy
-        self.proxy_headers = configuration.proxy_headers
+        if maxsize is None:
+            if configuration.connection_pool_maxsize is not None:
+                maxsize = configuration.connection_pool_maxsize
+            else:
+                maxsize = 4
 
         # https pool manager
-        self.pool_manager = aiohttp.ClientSession(
-            connector=connector,
-            trust_env=True
-        )
-
-    async def close(self):
-        await self.pool_manager.close()
-
-    async def request(self, method, url, query_params=None, headers=None,
-                      body=None, post_params=None, _preload_content=True,
-                      _request_timeout=None):
-        """Execute request
+        if configuration.proxy:
+            if is_socks_proxy_url(configuration.proxy):
+                from urllib3.contrib.socks import SOCKSProxyManager
+                self.pool_manager = SOCKSProxyManager(
+                        cert_reqs=cert_reqs,
+                        ca_certs=configuration.ssl_ca_cert,
+                        cert_file=configuration.cert_file,
+                        key_file=configuration.key_file,
+                        proxy_url=configuration.proxy,
+                        headers=configuration.proxy_headers,
+                        **addition_pool_args
+                    )
+            else:
+                self.pool_manager = urllib3.ProxyManager(
+                    num_pools=pools_size,
+                    maxsize=maxsize,
+                    cert_reqs=cert_reqs,
+                    ca_certs=configuration.ssl_ca_cert,
+                    cert_file=configuration.cert_file,
+                    key_file=configuration.key_file,
+                    proxy_url=configuration.proxy,
+                    proxy_headers=configuration.proxy_headers,
+                    **addition_pool_args
+                )
+        else:
+            self.pool_manager = urllib3.PoolManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=configuration.ssl_ca_cert,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                **addition_pool_args
+            )
+
+    def request(self, method, url, query_params=None, headers=None,
+                body=None, post_params=None, _preload_content=True,
+                _request_timeout=None):
+        """Perform requests.
 
         :param method: http request method
         :param url: http request url
         :param query_params: query parameters in the url
         :param headers: http request headers
         :param body: request json body, for `application/json`
         :param post_params: request post parameters,
                             `application/x-www-form-urlencoded`
                             and `multipart/form-data`
-        :param _preload_content: this is a non-applicable field for
-                                 the AiohttpClient.
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         """
         method = method.upper()
         assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
@@ -108,144 +158,170 @@
             )
 
         post_params = post_params or {}
         headers = headers or {}
         # url already contains the URL query string
         # so reset query_params to empty dict
         query_params = {}
-        timeout = _request_timeout or 5 * 60
-
-        if 'Content-Type' not in headers:
-            headers['Content-Type'] = 'application/json'
 
-        args = {
-            "method": method,
-            "url": url,
-            "timeout": timeout,
-            "headers": headers
-        }
-
-        if self.proxy:
-            args["proxy"] = self.proxy
-        if self.proxy_headers:
-            args["proxy_headers"] = self.proxy_headers
-
-        if query_params:
-            args["url"] += '?' + urlencode(query_params)
-
-        # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
-        if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-            if re.search('json', headers['Content-Type'], re.IGNORECASE):
-                if body is not None:
-                    body = json.dumps(body)
-                args["data"] = body
-            elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
-                args["data"] = aiohttp.FormData(post_params)
-            elif headers['Content-Type'] == 'multipart/form-data':
-                # must del headers['Content-Type'], or the correct
-                # Content-Type which generated by aiohttp
-                del headers['Content-Type']
-                data = aiohttp.FormData()
-                for param in post_params:
-                    k, v = param
-                    if isinstance(v, tuple) and len(v) == 3:
-                        data.add_field(k,
-                                       value=v[1],
-                                       filename=v[0],
-                                       content_type=v[2])
-                    else:
-                        data.add_field(k, v)
-                args["data"] = data
-
-            # Pass a `bytes` parameter directly in the body to support
-            # other content types than Json when `body` argument is provided
-            # in serialized form
-            elif isinstance(body, bytes):
-                args["data"] = body
+        timeout = None
+        if _request_timeout:
+            if isinstance(_request_timeout, (int,float)):  # noqa: E501,F821
+                timeout = urllib3.Timeout(total=_request_timeout)
+            elif (isinstance(_request_timeout, tuple) and
+                  len(_request_timeout) == 2):
+                timeout = urllib3.Timeout(
+                    connect=_request_timeout[0], read=_request_timeout[1])
+
+        try:
+            # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
+            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
+
+                # no content type provided or payload is json
+                if not headers.get('Content-Type') or re.search('json', headers['Content-Type'], re.IGNORECASE):
+                    request_body = None
+                    if body is not None:
+                        request_body = json.dumps(body)
+                    r = self.pool_manager.request(
+                        method, url,
+                        body=request_body,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
+                    r = self.pool_manager.request(
+                        method, url,
+                        fields=post_params,
+                        encode_multipart=False,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                elif headers['Content-Type'] == 'multipart/form-data':
+                    # must del headers['Content-Type'], or the correct
+                    # Content-Type which generated by urllib3 will be
+                    # overwritten.
+                    del headers['Content-Type']
+                    r = self.pool_manager.request(
+                        method, url,
+                        fields=post_params,
+                        encode_multipart=True,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                # Pass a `string` parameter directly in the body to support
+                # other content types than Json when `body` argument is
+                # provided in serialized form
+                elif isinstance(body, str) or isinstance(body, bytes):
+                    request_body = body
+                    r = self.pool_manager.request(
+                        method, url,
+                        body=request_body,
+                        preload_content=_preload_content,
+                        timeout=timeout,
+                        headers=headers)
+                else:
+                    # Cannot generate the request from given parameters
+                    msg = """Cannot prepare a request message for provided
+                             arguments. Please check that your arguments match
+                             declared content type."""
+                    raise ApiException(status=0, reason=msg)
+            # For `GET`, `HEAD`
             else:
-                # Cannot generate the request from given parameters
-                msg = """Cannot prepare a request message for provided
-                         arguments. Please check that your arguments match
-                         declared content type."""
-                raise ApiException(status=0, reason=msg)
+                r = self.pool_manager.request(method, url,
+                                              fields={},
+                                              preload_content=_preload_content,
+                                              timeout=timeout,
+                                              headers=headers)
+        except urllib3.exceptions.SSLError as e:
+            msg = "{0}\n{1}".format(type(e).__name__, str(e))
+            raise ApiException(status=0, reason=msg)
 
-        r = await self.pool_manager.request(**args)
         if _preload_content:
-
-            data = await r.read()
-            r = RESTResponse(r, data)
+            r = RESTResponse(r)
 
             # log response body
             logger.debug("response body: %s", r.data)
 
-            if not 200 <= r.status <= 299:
-                raise ApiException(http_resp=r)
+        if not 200 <= r.status <= 299:
+            if r.status == 400:
+                raise BadRequestException(http_resp=r)
+
+            if r.status == 401:
+                raise UnauthorizedException(http_resp=r)
+
+            if r.status == 403:
+                raise ForbiddenException(http_resp=r)
+
+            if r.status == 404:
+                raise NotFoundException(http_resp=r)
+
+            if 500 <= r.status <= 599:
+                raise ServiceException(http_resp=r)
+
+            raise ApiException(http_resp=r)
 
         return r
 
-    async def get_request(self, url, headers=None, query_params=None,
-                  _preload_content=True, _request_timeout=None):
-        return (await self.request("GET", url,
-                                   headers=headers,
-                                   _preload_content=_preload_content,
-                                   _request_timeout=_request_timeout,
-                                   query_params=query_params))
-
-    async def head_request(self, url, headers=None, query_params=None,
-                   _preload_content=True, _request_timeout=None):
-        return (await self.request("HEAD", url,
-                                   headers=headers,
-                                   _preload_content=_preload_content,
-                                   _request_timeout=_request_timeout,
-                                   query_params=query_params))
-
-    async def options_request(self, url, headers=None, query_params=None,
-                      post_params=None, body=None, _preload_content=True,
-                      _request_timeout=None):
-        return (await self.request("OPTIONS", url,
-                                   headers=headers,
-                                   query_params=query_params,
-                                   post_params=post_params,
-                                   _preload_content=_preload_content,
-                                   _request_timeout=_request_timeout,
-                                   body=body))
-
-    async def delete_request(self, url, headers=None, query_params=None, body=None,
-                     _preload_content=True, _request_timeout=None):
-        return (await self.request("DELETE", url,
-                                   headers=headers,
-                                   query_params=query_params,
-                                   _preload_content=_preload_content,
-                                   _request_timeout=_request_timeout,
-                                   body=body))
-
-    async def post_request(self, url, headers=None, query_params=None,
-                   post_params=None, body=None, _preload_content=True,
-                   _request_timeout=None):
-        return (await self.request("POST", url,
-                                   headers=headers,
-                                   query_params=query_params,
-                                   post_params=post_params,
-                                   _preload_content=_preload_content,
-                                   _request_timeout=_request_timeout,
-                                   body=body))
-
-    async def put_request(self, url, headers=None, query_params=None, post_params=None,
-                  body=None, _preload_content=True, _request_timeout=None):
-        return (await self.request("PUT", url,
-                                   headers=headers,
-                                   query_params=query_params,
-                                   post_params=post_params,
-                                   _preload_content=_preload_content,
-                                   _request_timeout=_request_timeout,
-                                   body=body))
-
-    async def patch_request(self, url, headers=None, query_params=None,
-                    post_params=None, body=None, _preload_content=True,
-                    _request_timeout=None):
-        return (await self.request("PATCH", url,
-                                   headers=headers,
-                                   query_params=query_params,
-                                   post_params=post_params,
-                                   _preload_content=_preload_content,
-                                   _request_timeout=_request_timeout,
-                                   body=body))
+    def get_request(self, url, headers=None, query_params=None, _preload_content=True,
+            _request_timeout=None):
+        return self.request("GET", url,
+                            headers=headers,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
+
+    def head_request(self, url, headers=None, query_params=None, _preload_content=True,
+             _request_timeout=None):
+        return self.request("HEAD", url,
+                            headers=headers,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
+
+    def options_request(self, url, headers=None, query_params=None, post_params=None,
+                body=None, _preload_content=True, _request_timeout=None):
+        return self.request("OPTIONS", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def delete_request(self, url, headers=None, query_params=None, body=None,
+               _preload_content=True, _request_timeout=None):
+        return self.request("DELETE", url,
+                            headers=headers,
+                            query_params=query_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def post_request(self, url, headers=None, query_params=None, post_params=None,
+             body=None, _preload_content=True, _request_timeout=None):
+        return self.request("POST", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def put_request(self, url, headers=None, query_params=None, post_params=None,
+            body=None, _preload_content=True, _request_timeout=None):
+        return self.request("PUT", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
+
+    def patch_request(self, url, headers=None, query_params=None, post_params=None,
+              body=None, _preload_content=True, _request_timeout=None):
+        return self.request("PATCH", url,
+                            headers=headers,
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
```

### Comparing `cardscan_client-0.0.1/pyproject.toml` & `cardscan_client-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cardscan-client"
-version = "0.0.1"
+version = "0.1.0"
 description = "Python CardScan API client"
 authors = ["Team CardScan <dev@cardscan.ai>"]
 license = "SEE LICENSE IN LICENSE.md"
 readme = "README.md"
 repository = "https://github.com/CardScan-ai/api-clients.git"
 keywords = ["CardScan", "CardScan client", "CardScan API client"]
```

