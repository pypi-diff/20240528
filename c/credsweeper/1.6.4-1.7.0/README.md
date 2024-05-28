# Comparing `tmp/credsweeper-1.6.4.tar.gz` & `tmp/credsweeper-1.7.0.tar.gz`

## Comparing `credsweeper-1.6.4.tar` & `credsweeper-1.7.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/__init__.py
--rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/__main__.py
--rw-r--r--   0        0        0    18285 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/py.typed
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/__init__.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/constants.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/keyword_checklist.py
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/keyword_checklist.txt
--rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/morpheme_checklist.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/config/__init__.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/config/config.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/__init__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/candidate.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/candidate_key.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/credential_manager.py
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/line_data.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0        0        0    13907 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/deep_scanner.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/docx_scanner.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/eml_scanner.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/jks_scanner.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/pkcs12_scanner.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/zip_scanner.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/__init__.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/abstract_provider.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/content_provider.py
--rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/descriptor.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/files_provider.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/patches_provider.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/filter.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/line_git_binary_check.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_atlassian_token_check.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_base32_data_check.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_base64_data_check.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_base64_encoded_pem_check.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_base64_key_check.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_couple_keyword_check.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_entropy_base32_check.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_entropy_base36_check.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_entropy_base64_check.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_github_check.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_grafana_check.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_hex_number_check.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_ip_check.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_jfrog_token_check.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_json_web_token_check.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_length_check.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_method_check.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_not_part_encoded_check.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_number_check.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_pattern_length_check.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_split_keyword_check.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_token_base32_check.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_token_base36_check.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_token_base64_check.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_token_check.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/variable_not_allowed_pattern_check.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/group.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/token_pattern.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/weird_base36_token.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/weird_base64_token.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/logger/__init__.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/logger/logger.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/__init__.py
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/features.py
--rw-r--r--   0        0        0   868645 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/model_config.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/rules/__init__.py
--rw-r--r--   0        0        0    24774 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/rules/config.yaml
--rw-r--r--   0        0        0    10857 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/rules/rule.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/__init__.py
--rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scanner.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/secret/config.json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/secret/log.yaml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/utils/__init__.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/utils/entropy_validator.py
--rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/utils/pem_key_detector.py
--rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/utils/util.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/apply_validation.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/github_token_validation.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/validation.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 credsweeper-1.6.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 credsweeper-1.6.4/LICENSE
--rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 credsweeper-1.6.4/README.md
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 credsweeper-1.6.4/pyproject.toml
--rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 credsweeper-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/__init__.py
+-rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/__main__.py
+-rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/py.typed
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/__init__.py
+-rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/constants.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/morpheme_checklist.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/config/__init__.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/config/config.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/candidate.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/line_data.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0        0        0    13915 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/docx_scanner.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/eml_scanner.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/jks_scanner.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/pkcs12_scanner.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/zip_scanner.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/abstract_provider.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/descriptor.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/patches_provider.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/filter.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/line_git_binary_check.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_atlassian_token_check.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_base64_data_check.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_base64_encoded_pem_check.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_base64_key_check.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_entropy_base64_check.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_github_check.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_hex_number_check.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_ip_check.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_jfrog_token_check.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_length_check.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_method_check.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_not_part_encoded_check.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_number_check.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_token_base64_check.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_token_check.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/variable_not_allowed_pattern_check.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/group.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/weird_base64_token.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/logger/__init__.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/logger/logger.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/__init__.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/features.py
+-rw-r--r--   0        0        0  5036009 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0        0        0    11401 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/model_config.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/rules/__init__.py
+-rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/rules/config.yaml
+-rw-r--r--   0        0        0    10564 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/rules/rule.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/__init__.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scanner.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/secret/config.json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/secret/log.yaml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/utils/__init__.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/utils/entropy_validator.py
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/utils/pem_key_detector.py
+-rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/utils/util.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/apply_validation.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/validation.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 credsweeper-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 credsweeper-1.7.0/LICENSE
+-rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 credsweeper-1.7.0/README.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 credsweeper-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 credsweeper-1.7.0/PKG-INFO
```

### Comparing `credsweeper-1.6.4/credsweeper/__init__.py` & `credsweeper-1.7.0/credsweeper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
     '__version__'
 ]
 
-__version__ = "1.6.4"
+__version__ = "1.7.0"
```

### Comparing `credsweeper-1.6.4/credsweeper/__main__.py` & `credsweeper-1.7.0/credsweeper/__main__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/app.py` & `credsweeper-1.7.0/credsweeper/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import itertools
 import logging
 import multiprocessing
 import signal
 import sys
 from pathlib import Path
-from typing import Any, List, Optional, Union, Dict, Sequence
+from typing import Any, List, Optional, Union, Dict, Sequence, Tuple
 
 import pandas as pd
 
 # Directory of credsweeper sources MUST be placed before imports to avoid circular import error
 APP_PATH = Path(__file__).resolve().parent
 
 from credsweeper.common.constants import KeyValidationOption, Severity, ThresholdPreset
 from credsweeper.config import Config
-from credsweeper.credentials import Candidate, CredentialManager
+from credsweeper.credentials import Candidate, CredentialManager, CandidateKey
 from credsweeper.deep_scanner.deep_scanner import DeepScanner
 from credsweeper.file_handler.diff_content_provider import DiffContentProvider
 from credsweeper.file_handler.file_path_extractor import FilePathExtractor
 from credsweeper.file_handler.abstract_provider import AbstractProvider
 from credsweeper.file_handler.text_content_provider import TextContentProvider
 from credsweeper.scanner import Scanner
 from credsweeper.utils import Util
@@ -332,40 +332,41 @@
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def post_processing(self) -> None:
         """Machine learning validation for received credential candidates."""
         if self._use_ml_validation():
             logger.info(f"Grouping {len(self.credential_manager.candidates)} candidates")
-            new_cred_list = []
+            new_cred_list: List[Candidate] = []
             cred_groups = self.credential_manager.group_credentials()
-            ml_cred_groups = []
+            ml_cred_groups: List[Tuple[CandidateKey, List[Candidate]]] = []
             for group_key, group_candidates in cred_groups.items():
-                # Analyze with ML if all candidates in group require ML
+                # Analyze with ML if any candidate in group require ML
                 for candidate in group_candidates:
-                    if not candidate.use_ml:
+                    if candidate.use_ml:
+                        ml_cred_groups.append((group_key, group_candidates))
                         break
                 else:
-                    ml_cred_groups.append((group_key.value, group_candidates))
-                    continue
-                # If at least one of credentials in the group do not require ML - automatically report to user
-                for candidate in group_candidates:
-                    candidate.ml_validation = KeyValidationOption.NOT_AVAILABLE
-                new_cred_list += group_candidates
+                    # all candidates do not require ML
+                    new_cred_list.extend(group_candidates)
 
             # prevent extra ml_validator creation if ml_cred_groups is empty
             if ml_cred_groups:
                 logger.info(f"Run ML Validation for {len(ml_cred_groups)} groups")
                 is_cred, probability = self.ml_validator.validate_groups(ml_cred_groups, self.ml_batch_size)
                 for i, (_, group_candidates) in enumerate(ml_cred_groups):
-                    if is_cred[i]:
-                        for candidate in group_candidates:
-                            candidate.ml_validation = KeyValidationOption.VALIDATED_KEY
-                            candidate.ml_probability = probability[i]
-                        new_cred_list += group_candidates
+                    for candidate in group_candidates:
+                        if candidate.use_ml:
+                            if is_cred[i]:
+                                candidate.ml_validation = KeyValidationOption.VALIDATED_KEY
+                                candidate.ml_probability = probability[i]
+                                new_cred_list.append(candidate)
+                        else:
+                            candidate.ml_validation = KeyValidationOption.NOT_AVAILABLE
+                            new_cred_list.append(candidate)
             else:
                 logger.info("Skipping ML validation due not applicable")
 
             self.credential_manager.set_credentials(new_cred_list)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
```

### Comparing `credsweeper-1.6.4/credsweeper/common/constants.py` & `credsweeper-1.7.0/credsweeper/common/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 class KeywordPattern:
     """Pattern set of keyword types"""
     key_left = r"(?P<variable>(([`'\"]+[^:='\"`}<>\\/&?]*|[^:='\"`}<>\s()\\/&?]*)" \
                r"(?P<keyword>"
     # there will be inserted a keyword
     key_right = r")" \
                 r"[^:='\"`<>{?!&]*)[`'\"]*)"  # <variable>
+    # Authentication scheme ( oauth | basic | bearer | apikey ) precedes to credential
     separator = r"\s*\]?\s*" \
-                r"(?P<separator>:( [a-z]{3,9} )?=|:|=>|!=|===|==|=)" \
+                r"(?P<separator>:( [a-z]{3,9}[?]? )?="\
+                r"|:( oauth | basic | bearer | apikey | accesskey )?"\
+                r"|=>|!=|===|==|=)" \
                 r"((?!\s*ENC(\(|\[))(\s|\w)*\((\s|\w|=|\()*|\s*)"
     value = r"(?P<value_leftquote>((b|r|br|rb|u|f|rf|fr|\\)?[`'\"])+)?" \
             r"(?P<value>(?:\{[^}]{3,8000}\})|(?:<[^>]{3,8000}>)|" \
-            r"(?(value_leftquote)(?:\\[nrux0-7][0-9a-f]*|[^`'\"\\])|(?:\\n|\\r|\\?[^\s`'\"\\])){3,8000})" \
+            r"(?(value_leftquote)(?:\\[tnrux0-7][0-9a-f]*|[^`'\"\\])|(?:\\n|\\r|\\?[^\s`'\"\\])){3,8000})" \
             r"(?P<value_rightquote>(\\?[`'\"])+)?"
 
     @classmethod
     def get_keyword_pattern(cls, keyword: str) -> re.Pattern:
         """Returns compiled regex pattern"""
         expression = "".join([cls.key_left, keyword, cls.key_right, cls.separator, cls.value])
         return re.compile(expression, flags=re.IGNORECASE)
@@ -152,15 +155,19 @@
     ADDED = "added"
     DELETED = "deleted"
 
 
 MIN_VARIABLE_LENGTH = 1
 MIN_SEPARATOR_LENGTH = 1
 MIN_VALUE_LENGTH = 4
+# if the line is oversize - it will be scanned by chunks with overlapping
 MAX_LINE_LENGTH = 8000
+# the size for overlapping chunks must be less than MAX_LINE_LENGTH
+CHUNKS_OVERLAP_SIZE = 1000
+CHUNK_STEP_SIZE = MAX_LINE_LENGTH - CHUNKS_OVERLAP_SIZE
 """ values according https://docs.python.org/3/library/codecs.html """
 UTF_8 = "utf_8"
 UTF_16 = "utf_16"
 LATIN_1 = "latin_1"
 ASCII = "ascii"
 
 DEFAULT_ENCODING = UTF_8
```

### Comparing `credsweeper-1.6.4/credsweeper/common/keyword_checklist.py` & `credsweeper-1.7.0/credsweeper/common/keyword_checklist.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.7.0/credsweeper/common/keyword_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/common/morpheme_checklist.txt` & `credsweeper-1.7.0/credsweeper/common/morpheme_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/config/config.py` & `credsweeper-1.7.0/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.7.0/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/credentials/candidate.py` & `credsweeper-1.7.0/credsweeper/credentials/candidate.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.7.0/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/credentials/candidate_key.py` & `credsweeper-1.7.0/credsweeper/credentials/candidate_key.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,23 @@
 
     Candidates that detected same value on same string in a same file would have identical CandidateKey
     """
 
     def __init__(self, line_data: LineData):
         self.path: str = line_data.path
         self.line_num: int = line_data.line_num
-        self.value: str = line_data.value
-        self.key: Tuple[str, int, str] = (self.path, self.line_num, self.value)
+        self.value_start: int = line_data.value_start
+        self.value_end: int = line_data.value_end
+        self.key: Tuple[str, int, int, int] = (self.path, self.line_num, self.value_start, self.value_end)
+        self.__line = line_data.line
 
     def __hash__(self):
         return hash(self.key)
 
     def __eq__(self, other):
         return self.key == other.key
 
     def __ne__(self, other):
         return not (self == other)
+
+    def __repr__(self) -> str:
+        return f"{self.key}:{self.__line}"
```

### Comparing `credsweeper-1.6.4/credsweeper/credentials/credential_manager.py` & `credsweeper-1.7.0/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/credentials/line_data.py` & `credsweeper-1.7.0/credsweeper/credentials/line_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import contextlib
 import re
 from typing import Any, Dict, Optional, Tuple
 
+from credsweeper.common.constants import MAX_LINE_LENGTH
 from credsweeper.config import Config
 from credsweeper.utils import Util
 from credsweeper.utils.entropy_validator import EntropyValidator
 
 
 class LineData:
     """Object to treat and store scanned line related data.
@@ -23,14 +24,17 @@
         value: optional string variable, detected value in line
         variable: optional string variable, detected variable in line
 
     """
 
     comment_starts = ["//", "*", "#", "/*", "<!––", "%{", "%", "...", "(*", "--", "--[[", "#="]
     bash_param_split = re.compile("\\s+(\\-|\\||\\>|\\w+?\\>|\\&)")
+    # some symbols e.g. double quotes cannot be in URL string https://www.ietf.org/rfc/rfc1738.txt
+    # \ - was added for case of url in escaped string \u0026amp; - means escaped & in HTML
+    url_detect_regex = re.compile(r".*\w{3,33}://[\w;,/?:@&=+$%.!~*'()#\\-]+$")
 
     INITIAL_WRONG_POSITION = -3
     EXCEPTION_POSITION = -2
 
     def __init__(
             self,  #
             config: Config,  #
@@ -67,15 +71,15 @@
         self.value_rightquote: Optional[str] = None
 
         self.initialize(match_obj)
 
     def initialize(self, match_obj: Optional[re.Match] = None) -> None:
         """Apply regex to the candidate line and set internal fields based on match."""
         if not isinstance(match_obj, re.Match) and isinstance(self.pattern, re.Pattern):
-            match_obj = self.pattern.search(self.line)
+            match_obj = self.pattern.search(self.line, endpos=MAX_LINE_LENGTH)
         if match_obj is None:
             return
 
         def get_group_from_match_obj(_match_obj: re.Match, group: str) -> Any:
             with contextlib.suppress(Exception):
                 return _match_obj.group(group)
             return None
@@ -114,19 +118,20 @@
 
     def clean_url_parameters(self) -> None:
         """Clean url address from 'query parameters'.
 
         If line seem to be a URL - split by & character.
         Variable should be right most value after & or ? ([-1]). And value should be left most before & ([0])
         """
-        if "http://" in self.line or "https://" in self.line:
+        line_before_value = self.line[:self.value_start]
+        if self.url_detect_regex.match(line_before_value):
             if self.variable:
-                self.variable = self.variable.split('&')[-1].split('?')[-1]
+                self.variable = self.variable.split('&')[-1].split('?')[-1].split(';')[-1]
             if self.value:
-                self.value = self.value.split('&')[0]
+                self.value = self.value.split('&')[0].split(';')[0]
 
     def clean_bash_parameters(self) -> None:
         """Split variable and value by bash special characters, if line assumed to be CLI command."""
         if self.variable and self.variable.startswith("-") and self.value:
             value_spl = self.bash_param_split.split(self.value)
             # If variable name starts with `-` (usual case for args in CLI)
             #  and value can be split by bash special characters
```

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/byte_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/deep_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/deep_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return self.__config
 
     @property
     def scanner(self) -> Scanner:
         return self.__scanner
 
     @staticmethod
-    def get_deep_scanners(data: bytes, file_type: Optional[str] = None) -> List[Any]:
+    def get_deep_scanners(data: bytes, file_type: str) -> List[Any]:
         """Returns possibly scan methods for the data depends on content"""
         deep_scanners: List[Any] = []
         if Util.is_zip(data):
             deep_scanners.append(ZipScanner)
             # probably, there might be a docx, xlxs and so on.
             # It might be scanned with text representation in third-party libraries.
             deep_scanners.append(DocxScanner)
@@ -170,15 +170,15 @@
         if FilePathExtractor.is_find_by_ext_file(self.config, data_provider.file_type):
             # Skip scanning file and makes fake candidate due the extension is suspicious
             dummy_candidate = Candidate.get_dummy_candidate(self.config, data_provider.file_path,
                                                             data_provider.file_type, data_provider.info)
             candidates.append(dummy_candidate)
         else:
             # iterate for all possibly scanner methods
-            for scanner_classes in self.get_deep_scanners(data_provider.data):
+            for scanner_classes in self.get_deep_scanners(data_provider.data, data_provider.file_type):
                 new_candidates = scanner_classes.data_scan(self, data_provider, depth, recursive_limit_size)
                 augment_candidates(candidates, new_candidates)
 
         return candidates
 
     def structure_scan(
             self,  #
```

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/docx_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/docx_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/eml_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/eml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/gzip_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/html_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/jks_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/jks_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/lang_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/pkcs12_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/pkcs12_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/tar_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/xml_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/xml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.7.0/credsweeper/deep_scanner/zip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/__init__.py` & `credsweeper-1.7.0/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/abstract_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/abstract_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/analysis_target.py` & `credsweeper-1.7.0/credsweeper/file_handler/analysis_target.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/byte_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/content_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/content_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from abc import ABC, abstractmethod
 from functools import cached_property
 from typing import List, Optional, Generator
 
-from credsweeper.common.constants import MAX_LINE_LENGTH
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.file_handler.descriptor import Descriptor
 from credsweeper.utils import Util
 
 logger = logging.getLogger(__name__)
 
 
@@ -90,14 +89,9 @@
             line_nums = [1 + x for x in lines_range]
 
         for line_pos in lines_range:
             line = lines[line_pos]
             if min_len > len(line.strip()):
                 # Ignore target if stripped part is too short for all types
                 continue
-            line_len = len(line)
-            if MAX_LINE_LENGTH < line_len:
-                # Ignore target if it's too long
-                logger.warning(f"Skipped oversize({line_len}) line in {self.descriptor.path}:{line_nums[line_pos]}")
-                continue
             target = AnalysisTarget(line_pos, lines, line_nums, self.descriptor)
             yield target
```

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/data_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/diff_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.7.0/credsweeper/file_handler/file_path_extractor.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/files_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/files_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/patches_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/patches_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/string_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/struct_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/file_handler/text_content_provider.py` & `credsweeper-1.7.0/credsweeper/file_handler/text_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/__init__.py` & `credsweeper-1.7.0/credsweeper/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/filter.py` & `credsweeper-1.7.0/credsweeper/filters/filter.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/line_git_binary_check.py` & `credsweeper-1.7.0/credsweeper/filters/line_git_binary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.7.0/credsweeper/filters/line_specific_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.7.0/credsweeper/filters/separator_unusual_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_allowlist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_array_dictionary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_atlassian_token_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_atlassian_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_base32_data_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_base32_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_base64_data_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_base64_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_base64_encoded_pem_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_base64_encoded_pem_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_base64_key_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_base64_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_blocklist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_camel_case_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_couple_keyword_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_couple_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_entropy_base32_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_entropy_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_entropy_base36_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_entropy_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_entropy_base64_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_entropy_base64_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 
-from credsweeper.common.constants import Chars
+from credsweeper.common.constants import Chars, ENTROPY_LIMIT_BASE64
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
@@ -41,13 +41,18 @@
             y = 3.8
         elif 20 == x:
             y = 3.9
         elif 24 == x:
             y = 4.1
         elif 32 == x:
             y = 4.4
-        elif 12 <= x:
+        elif 12 <= x < 35:
             # logarithm base 2 - slow, but precise. Approximation does not exceed stdev
             y = 0.77 * math.log2(x) + 0.62
+        elif 35 <= x < 60:
+            y = ENTROPY_LIMIT_BASE64
+        elif 60 <= x:
+            # the entropy grows slowly after 60
+            y = 5.0
         else:
             y = 0
         return y
```

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_file_path_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_first_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_github_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_github_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_grafana_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_grafana_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_hex_number_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_hex_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_ip_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_ip_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_jfrog_token_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_jfrog_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_json_web_token_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_json_web_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_last_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_length_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_method_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_method_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_not_part_encoded_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_not_part_encoded_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_number_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_similarity_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_split_keyword_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_split_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_string_type_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_token_base32_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_token_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_token_base36_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_token_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_token_base64_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_token_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_token_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.7.0/credsweeper/filters/value_useless_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.7.0/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/group/__init__.py` & `credsweeper-1.7.0/credsweeper/filters/group/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/group/group.py` & `credsweeper-1.7.0/credsweeper/filters/group/group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/group/password_keyword.py` & `credsweeper-1.7.0/credsweeper/filters/group/password_keyword.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/group/token_pattern.py` & `credsweeper-1.7.0/credsweeper/filters/group/token_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.7.0/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/group/weird_base36_token.py` & `credsweeper-1.7.0/credsweeper/filters/group/weird_base36_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/filters/group/weird_base64_token.py` & `credsweeper-1.7.0/credsweeper/filters/group/weird_base64_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/logger/logger.py` & `credsweeper-1.7.0/credsweeper/logger/logger.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/ml_model/features.py` & `credsweeper-1.7.0/credsweeper/ml_model/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         return True
 
 
 class PossibleComment(Feature):
     r"""Feature is true if candidate line starts with #,\*,/\*? (Possible comment)."""
 
     def extract(self, candidate: Candidate) -> bool:
-        for i in ["#", "*", "/*"]:
+        for i in ["#", "*", "/*", "//"]:
             if candidate.line_data_list[0].line.startswith(i):
                 return True
         return False
 
 
 class IsSecretNumeric(Feature):
     """Feature is true if candidate value is a numerical value."""
@@ -256,21 +256,21 @@
     Parameters:
         extensions: extension labels
 
     """
 
     def __init__(self, extensions: List[str]) -> None:
         super().__init__()
-        self.extensions = extensions
+        self.label_binarizer = LabelBinarizer()
+        self.label_binarizer.fit(extensions)
 
     def __call__(self, candidates: List[Candidate]) -> csr_matrix:
-        enc = LabelBinarizer()
-        enc.fit(self.extensions)
         extensions = [candidate.line_data_list[0].file_type for candidate in candidates]
-        return enc.transform(extensions)
+        result = self.label_binarizer.transform(extensions)
+        return result
 
     def extract(self, candidate: Candidate) -> Any:
         raise NotImplementedError
 
 
 class RuleName(Feature):
     """Categorical feature that corresponds to rule name.
@@ -278,17 +278,17 @@
     Parameters:
         rule_names: rule name labels
 
     """
 
     def __init__(self, rule_names: List[str]) -> None:
         super().__init__()
-        self.rule_names = rule_names
+        self.label_binarizer = LabelBinarizer()
+        self.label_binarizer.fit(rule_names)
 
     def __call__(self, candidates: List[Candidate]) -> csr_matrix:
-        enc = LabelBinarizer()
-        enc.fit(self.rule_names)
         rule_names = [candidate.rule_name for candidate in candidates]
-        return enc.transform(rule_names)
+        result = self.label_binarizer.transform(rule_names)
+        return result
 
     def extract(self, candidate: Candidate) -> Any:
         raise NotImplementedError
```

### Comparing `credsweeper-1.6.4/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.7.0/credsweeper/ml_model/ml_validator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import logging
 import os
 import string
-from typing import List, Tuple, Union, Any
+from typing import List, Tuple, Union
 
 import numpy as np
 import onnxruntime as ort
 
 from credsweeper.common.constants import ThresholdPreset
-from credsweeper.credentials import Candidate
+from credsweeper.credentials import Candidate, CandidateKey
 from credsweeper.ml_model import features
 from credsweeper.utils import Util
 
 logger = logging.getLogger(__name__)
 
 
 class MlValidator:
     """ML validation class"""
+    HALF_LEN = 80  # limit of variable or value size
+    MAX_LEN = 2 * HALF_LEN  # for whole line limit
+    NON_ASCII = '\xFF'
+    CHAR_INDEX = {char: index for index, char in enumerate('\0' + string.printable + NON_ASCII)}
+    NUM_CLASSES = len(CHAR_INDEX)
 
     def __init__(self, threshold: Union[float, ThresholdPreset], azure: bool = False, cuda: bool = False) -> None:
         """Init
 
         Args:
             threshold: decision threshold
         """
@@ -28,68 +33,104 @@
         if azure:
             provider = "AzureExecutionProvider"
         elif cuda:
             provider = "CUDAExecutionProvider"
         else:
             provider = "CPUExecutionProvider"
         self.model_session = ort.InferenceSession(model_file_path, providers=[provider])
-        char_filtered = string.ascii_lowercase + string.digits + string.punctuation
-
-        self.char_to_index = {char: index + 1 for index, char in enumerate(char_filtered)}
-        self.char_to_index['NON_ASCII'] = len(self.char_to_index) + 1
 
         model_details = Util.json_load(os.path.join(dir_path, "model_config.json"))
         if isinstance(threshold, float):
             self.threshold = threshold
         elif isinstance(threshold, ThresholdPreset) and "thresholds" in model_details:
             self.threshold = model_details["thresholds"][threshold.value]
         else:
             self.threshold = 0.5
-        self.maxlen = int(model_details.get("max_len", 160))
+
         self.common_feature_list = []
         self.unique_feature_list = []
         logger.info("Init ML validator, model file path: %s", model_file_path)
         logger.debug("ML validator details: %s", model_details)
         for feature_definition in model_details["features"]:
             feature_class = feature_definition["type"]
             kwargs = feature_definition.get("kwargs", {})
             feature_constructor = getattr(features, feature_class, None)
             if feature_constructor is None:
                 raise ValueError(f'Error while parsing model details. Cannot create feature "{feature_class}"')
             try:
                 feature = feature_constructor(**kwargs)
             except TypeError:
-                raise TypeError(
-                    f'Error while parsing model details. Cannot create feature "{feature_class}" with kwargs "{kwargs}"'
-                )
+                raise TypeError(f'Error while parsing model details. Cannot create feature "{feature_class}"'
+                                f' with kwargs "{kwargs}"')
             if feature_definition["type"] in ["RuleName"]:
                 self.unique_feature_list.append(feature)
             else:
                 self.common_feature_list.append(feature)
 
-    def encode(self, line, char_to_index) -> np.ndarray:
-        """Encodes line to array"""
-        num_classes = len(char_to_index) + 1
-        result_array = np.zeros((self.maxlen, num_classes), dtype=np.float32)
-        line = line.strip().lower()[-self.maxlen:]
-        for i in range(self.maxlen):
-            if i < len(line):
-                c = line[i]
-                if c in char_to_index:
-                    result_array[i, char_to_index[c]] = 1
-                else:
-                    result_array[i, char_to_index["NON_ASCII"]] = 1
+    @staticmethod
+    def encode(text: str, limit: int) -> np.ndarray:
+        """Encodes prepared text to array"""
+        result_array = np.zeros(shape=(limit, MlValidator.NUM_CLASSES), dtype=np.float32)
+        if text is None:
+            return result_array
+        len_text = len(text)
+        if limit > len_text:
+            # fill empty part
+            text += '\0' * (limit - len_text)
+        for i, c in enumerate(text):
+            if c in MlValidator.CHAR_INDEX:
+                result_array[i, MlValidator.CHAR_INDEX[c]] = 1
             else:
-                result_array[i, 0] = 1
+                result_array[i, MlValidator.CHAR_INDEX[MlValidator.NON_ASCII]] = 1
         return result_array
 
-    def _call_model(self, line_input: np.ndarray, feature_input: np.ndarray) -> Any:
-        line_input = line_input.astype(np.float32)
-        feature_input = feature_input.astype(np.float32)
-        return self.model_session.run(None, {"line_input": line_input, "feature_input": feature_input})[0]
+    @staticmethod
+    def subtext(text: str, pos: int, hunk_size: int) -> str:
+        """cut text symmetrically for given position or use remained quota to be fitted in 2x hunk_size"""
+        left_quota = 0 if hunk_size <= pos else hunk_size - pos
+        right_remain = len(text) - pos
+        right_quota = 0 if hunk_size <= right_remain else right_remain - hunk_size
+        left_pos = pos - hunk_size
+        right_pos = pos + hunk_size
+        if left_quota:
+            left_pos += left_quota
+            right_pos += left_quota
+        if right_quota:
+            left_pos += right_quota
+            right_pos += right_quota
+        return text[left_pos:right_pos]
+
+    @staticmethod
+    def encode_line(text: str, position: int):
+        """Encodes line with balancing for position"""
+        offset = len(text) - len(text.lstrip())
+        pos = position - offset
+        stripped = text.strip()
+        if MlValidator.MAX_LEN < len(stripped):
+            stripped = MlValidator.subtext(stripped, pos, MlValidator.HALF_LEN)
+        return MlValidator.encode(stripped, MlValidator.MAX_LEN)
+
+    @staticmethod
+    def encode_value(text: str) -> np.ndarray:
+        """Encodes line with balancing for position"""
+        stripped = text.strip()
+        return MlValidator.encode(stripped[:MlValidator.HALF_LEN], MlValidator.HALF_LEN)
+
+    def _call_model(self, line_input: np.ndarray, variable_input: np.ndarray, value_input: np.ndarray,
+                    feature_input: np.ndarray) -> np.ndarray:
+        input_feed = {
+            "line_input": line_input.astype(np.float32),
+            "variable_input": variable_input.astype(np.float32),
+            "value_input": value_input.astype(np.float32),
+            "feature_input": feature_input.astype(np.float32),
+        }
+        result = self.model_session.run(output_names=None, input_feed=input_feed)
+        if result and isinstance(result[0], np.ndarray):
+            return result[0]
+        raise RuntimeError(f"Unexpected type {type(result[0])}")
 
     def extract_common_features(self, candidates: List[Candidate]) -> np.ndarray:
         """Extract features that are guaranteed to be the same for all candidates on the same line with same value."""
         feature_array = np.array([], dtype=np.float32)
         # Extract features from credential candidate
         default_candidate = candidates[0]
         for feature in self.common_feature_list:
@@ -112,66 +153,92 @@
             for feature in self.unique_feature_list:
                 new_feature = feature([candidate])[0]
                 if not isinstance(new_feature, np.ndarray):
                     new_feature = np.array([new_feature])
                 feature_array = feature_array | new_feature
         return feature_array
 
-    def validate(self, candidate: Candidate) -> Tuple[bool, float]:
-        """Validate single credential candidate."""
-        sample_as_batch = [(candidate.line_data_list[0].value, [candidate])]
-        is_cred_batch, probability_batch = self.validate_groups(sample_as_batch, 1)
-        return is_cred_batch[0], probability_batch[0]
-
-    def get_group_features(self, value: str, candidates: List[Candidate]) -> Tuple[np.ndarray, np.ndarray]:
+    def get_group_features(self, candidates: List[Candidate]) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
         """
         `np.newaxis` used to add new dimension if front, so input will be treated as a batch
         """
-        line_input = self.encode(value, self.char_to_index)[np.newaxis]
+        # all candidates are from the same line
+        default_candidate = candidates[0]
+        line_input = MlValidator.encode_line(default_candidate.line_data_list[0].line,
+                                             default_candidate.line_data_list[0].value_start)[np.newaxis]
+        variable = ""
+        value = ""
+        for candidate in candidates:
+            if not variable and candidate.line_data_list[0].variable:
+                variable = candidate.line_data_list[0].variable
+            if not value and candidate.line_data_list[0].value:
+                value = candidate.line_data_list[0].value
+            if variable and value:
+                break
+        variable_input = MlValidator.encode_value(variable)[np.newaxis]
+        value_input = MlValidator.encode_value(value)[np.newaxis]
+        feature_array = self.extract_features(candidates)
+        return line_input, variable_input, value_input, feature_array
 
+    def extract_features(self, candidates: List[Candidate]) -> np.ndarray:
+        """extracts common and unique features from list of candidates"""
         common_features = self.extract_common_features(candidates)
         unique_features = self.extract_unique_features(candidates)
-        feature_array = np.hstack([common_features, unique_features])
-        feature_array = np.array([feature_array])
-        return line_input, feature_array
+        feature_hstack = np.hstack([common_features, unique_features])
+        feature_array = np.array([feature_hstack])
+        return feature_array
 
-    def _batch_call_model(self, line_inputs, feature_array_list):
+    def _batch_call_model(self, line_input_list, variable_input_list, value_input_list, features_list) -> np.ndarray:
         """auxiliary method to invoke twice"""
-        line_inputs_stack = np.vstack(line_inputs)
-        feature_array_vstack = np.vstack(feature_array_list)
-        return self._call_model(line_inputs_stack, feature_array_vstack)[:, 0]
+        line_inputs_vstack = np.vstack(line_input_list)
+        variable_inputs_vstack = np.vstack(variable_input_list)
+        value_inputs_vstack = np.vstack(value_input_list)
+        feature_array_vstack = np.vstack(features_list)
+        result_call = self._call_model(line_inputs_vstack, variable_inputs_vstack, value_inputs_vstack,
+                                       feature_array_vstack)
+        result = result_call[:, 0]
+        return result
 
-    def validate_groups(self, group_list: List[Tuple[str, List[Candidate]]],
+    def validate_groups(self, group_list: List[Tuple[CandidateKey, List[Candidate]]],
                         batch_size: int) -> Tuple[np.ndarray, np.ndarray]:
         """Use ml model on list of candidate groups.
 
         Args:
             group_list: List of tuples (value, group)
             batch_size: ML model batch
 
         Return:
             Boolean numpy array with decision based on the threshold,
             and numpy array with probability predicted by the model
 
         """
         line_input_list = []
+        variable_input_list = []
+        value_input_list = []
         features_list = []
-        probability = np.zeros(len(group_list))
+        probability = np.zeros(len(group_list), dtype=np.float32)
         head = tail = 0
-        for (value, candidates) in group_list:
-            line_input, feature_array = self.get_group_features(value, candidates)
+        for group_key, candidates in group_list:
+            line_input, variable_input, value_input, feature_array = self.get_group_features(candidates)
             line_input_list.append(line_input)
+            variable_input_list.append(variable_input)
+            value_input_list.append(value_input)
             features_list.append(feature_array)
             tail += 1
             if 0 == tail % batch_size:
                 # use the approach to reduce memory consumption for huge candidates list
-                probability[head:tail] = self._batch_call_model(line_input_list, features_list)
+                probability[head:tail] = self._batch_call_model(line_input_list, variable_input_list, value_input_list,
+                                                                features_list)
                 head = tail
                 line_input_list.clear()
+                variable_input_list.clear()
+                value_input_list.clear()
                 features_list.clear()
         if head != tail:
-            probability[head:tail] = self._batch_call_model(line_input_list, features_list)
+            probability[head:tail] = self._batch_call_model(line_input_list, variable_input_list, value_input_list,
+                                                            features_list)
         is_cred = probability > self.threshold
         for i in range(len(is_cred)):
             logger.debug("ML decision: %s with prediction: %s for value: %s", is_cred[i], round(probability[i], 8),
                          group_list[i][0])
-        return is_cred, probability
+        # apply cast to float to avoid json export issue
+        return is_cred, probability.astype(float)
```

### Comparing `credsweeper-1.6.4/credsweeper/ml_model/model_config.json` & `credsweeper-1.7.0/credsweeper/ml_model/model_config.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6660056467748775%*

 * *Differences: {"'features'": "{37: {'kwargs': {'extensions': {insert: [(1, '.1'), (4, '.axaml'), (8, '.bazel'), "*

 * *               "(9, '.bundle'), (10, '.bzl'), (13, '.cf'), (14, '.cjs'), (15, '.cljc'), (16, "*

 * *               "'.cmd'), (18, '.coffee'), (22, '.creds'), (23, '.crt'), (25, '.csp'), (26, "*

 * *               "'.dist'), (27, '.doc'), (28, '.dockerfile'), (29, '.eex'), (31, '.erb'), (32, "*

 * *               "'.erl'), (37, '.gml'), (38, '.gni'), (44, '.haml'), (47, '.iml'), (50, '.j'), (53, "*

 * *               "'.jenkinsfi […]*

```diff
@@ -289,122 +289,173 @@
         {
             "type": "IsSecretNumeric"
         },
         {
             "kwargs": {
                 "extensions": [
                     "",
+                    ".1",
                     ".adoc",
                     ".asciidoc",
+                    ".axaml",
                     ".bash",
                     ".bat",
                     ".bats",
+                    ".bazel",
+                    ".bundle",
+                    ".bzl",
                     ".c",
                     ".cc",
-                    ".cfg",
+                    ".cf",
+                    ".cjs",
+                    ".cljc",
+                    ".cmd",
                     ".cnf",
+                    ".coffee",
                     ".conf",
                     ".config",
                     ".cpp",
+                    ".creds",
+                    ".crt",
                     ".cs",
-                    ".diff",
+                    ".csp",
+                    ".dist",
+                    ".doc",
+                    ".dockerfile",
+                    ".eex",
                     ".env",
+                    ".erb",
+                    ".erl",
                     ".ex",
                     ".example",
-                    ".ex",
-                    ".tf",
                     ".exs",
                     ".ext",
+                    ".gml",
+                    ".gni",
                     ".go",
                     ".golden",
                     ".gradle",
                     ".groovy",
                     ".h",
-                    ".hpp",
+                    ".haml",
                     ".hs",
                     ".html",
+                    ".iml",
                     ".in",
-                    ".inc",
                     ".ini",
+                    ".j",
                     ".j2",
                     ".java",
+                    ".jenkinsfile",
                     ".js",
                     ".json",
                     ".jsp",
+                    ".jsx",
+                    ".jwt",
                     ".kt",
+                    ".las",
+                    ".ldif",
+                    ".ldml",
+                    ".libsonnet",
+                    ".lock",
+                    ".log",
                     ".lua",
                     ".m",
-                    ".markdown",
                     ".markerb",
                     ".md",
+                    ".mjs",
+                    ".mk",
+                    ".ml",
+                    ".mlir",
+                    ".moo",
                     ".ndjson",
+                    ".nix",
+                    ".odd",
+                    ".patch",
                     ".php",
                     ".pl",
+                    ".pm",
+                    ".po",
                     ".pod",
                     ".postinst",
                     ".pp",
+                    ".ppk",
                     ".properties",
                     ".proto",
                     ".ps1",
                     ".pxd",
                     ".py",
+                    ".pyx",
                     ".r",
                     ".rb",
+                    ".rexx",
                     ".rnh",
+                    ".rrc",
                     ".rs",
                     ".rsp",
                     ".rst",
                     ".sample",
                     ".sbt",
                     ".scala",
-                    ".scss",
+                    ".secrets",
                     ".sh",
                     ".slim",
                     ".snap",
                     ".sql",
+                    ".storyboard",
+                    ".strings",
+                    ".swift",
                     ".t",
+                    ".tdf",
                     ".template",
+                    ".test",
                     ".tf",
                     ".tfstate",
+                    ".tfvars",
                     ".tl",
                     ".tmpl",
+                    ".token",
                     ".toml",
                     ".travis",
                     ".ts",
                     ".tsx",
                     ".txt",
                     ".vue",
+                    ".xaml",
+                    ".xib",
+                    ".xml",
                     ".yaml",
-                    ".yml"
+                    ".yml",
+                    ".zsh",
+                    ".zsh-theme"
                 ]
             },
             "type": "FileExtension"
         },
         {
             "kwargs": {
                 "rule_names": [
-                    "Token",
-                    "Secret",
-                    "Github Old Token",
                     "API",
-                    "Credential",
-                    "Password",
-                    "Key",
                     "Auth",
+                    "Certificate",
+                    "Credential",
+                    "Github Old Token",
                     "JSON Web Token",
-                    "URL Credentials",
+                    "Key",
                     "Nonce",
+                    "Password",
                     "Salt",
-                    "Certificate"
+                    "Secret",
+                    "Token",
+                    "URL Credentials"
                 ]
             },
             "type": "RuleName"
         }
     ],
-    "max_len": 160,
     "thresholds": {
         "high": 0.79791,
         "highest": 0.92996,
         "low": 0.35739,
         "lowest": 0.22917,
         "medium": 0.62204
     }
```

### Comparing `credsweeper-1.6.4/credsweeper/rules/rule.py` & `credsweeper-1.7.0/credsweeper/rules/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 
     # auxiliary fields
     FILTER_TYPE = "filter_type"
     USE_ML = "use_ml"
     REQUIRED_SUBSTRINGS = "required_substrings"
     REQUIRED_REGEX = "required_regex"
     VALIDATIONS = "validations"
-    DOC_AVAILABLE = "doc_available"  # True - by default
-    DOC_ONLY = "doc_only"  # False - by default
+    TARGET = "target"
 
     def __init__(self, config: Config, rule_dict: Dict) -> None:
         self.config = config
         self._assert_rule_mandatory_fields(rule_dict)
         # mandatory fields
         self.__rule_name = str(rule_dict[Rule.NAME])
         if severity := Severity.get(rule_dict[Rule.SEVERITY]):
@@ -76,16 +75,15 @@
         self.__required_substrings = set(i.strip().lower() for i in rule_dict.get(Rule.REQUIRED_SUBSTRINGS, []))
         self.__has_required_substrings = bool(self.__required_substrings)
         required_regex = rule_dict.get(Rule.REQUIRED_REGEX)
         if required_regex and not isinstance(required_regex, str):
             self._malformed_rule_error(rule_dict, Rule.REQUIRED_REGEX)
         self.__required_regex = re.compile(required_regex) if required_regex else None
         self.__min_line_len = int(rule_dict.get(Rule.MIN_LINE_LEN, MAX_LINE_LENGTH))
-        self.__doc_available: bool = rule_dict.get(Rule.DOC_AVAILABLE, True)
-        self.__doc_only: bool = rule_dict.get(Rule.DOC_ONLY, False)
+        self.__target: List[str] = rule_dict.get(Rule.TARGET, [])
 
     def _malformed_rule_error(self, rule_dict: Dict, field: str):
         raise ValueError(f"Malformed rule '{self.__rule_name}'."
                          f" field '{field}' has invalid value"
                          f" '{rule_dict.get(field)}'")
 
     @cached_property
@@ -246,15 +244,10 @@
 
     @cached_property
     def min_line_len(self) -> int:
         """min_line_len getter"""
         return self.__min_line_len
 
     @cached_property
-    def doc_available(self) -> bool:
-        """doc_available getter"""
-        return self.__doc_available
-
-    @cached_property
-    def doc_only(self) -> bool:
-        """doc_only getter"""
-        return self.__doc_only
+    def target(self) -> List[str]:
+        """target getter"""
+        return self.__target
```

### Comparing `credsweeper-1.6.4/credsweeper/scanner/scanner.py` & `credsweeper-1.7.0/credsweeper/scanner/scanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,19 +89,18 @@
             raise RuntimeError(f"Wrong rules '{rule_templates}' were read from '{rule_path}'")
 
     def _is_available(self, rule: Rule) -> bool:
         """separate the method to reduce complexity"""
         if rule.severity < self.config.severity:
             return False
         if self.config.doc:
-            # apply only available for doc scanning rules
-            if rule.doc_available or rule.doc_only:
+            if "doc" in rule.target:
                 return True
         else:
-            if rule.doc_only:
+            if "code" not in rule.target:
                 return False
             else:
                 return True
         return False
 
     def yield_rule_scanner(
             self,  #
@@ -136,15 +135,15 @@
             # Trim string from outer spaces to make future `x in str` checks faster
             target_line_stripped = target.line_strip
             target_line_stripped_len = target.line_strip_len
 
             # "cache" - YAPF and pycharm formatters ...
             matched_keyword = \
                 target_line_stripped_len >= self.min_keyword_len and (  #
-                        '=' in target_line_stripped or ':' in target_line_stripped)  #
+                    '=' in target_line_stripped or ':' in target_line_stripped)  #
             matched_pem_key = \
                 target_line_stripped_len >= self.min_pem_key_len \
                 and PEM_BEGIN_PATTERN in target_line_stripped and "PRIVATE" in target_line_stripped
             matched_pattern = target_line_stripped_len >= self.min_pattern_len
             matched_multi = target_line_stripped_len >= self.min_multi_len
 
             if not (matched_keyword or matched_pem_key or matched_pattern or matched_multi):
```

### Comparing `credsweeper-1.6.4/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.7.0/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from credsweeper.common.constants import MAX_LINE_LENGTH, RuleType
+from credsweeper.common.constants import RuleType
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.rules import Rule
 from credsweeper.scanner.scan_type import ScanType
 
 
@@ -76,17 +76,14 @@
 
         Return:
             Boolean. True if second part detected. False otherwise
 
         """
         new_target = AnalysisTarget(candi_line_pos, target.lines, target.line_nums, target.descriptor)
 
-        if MAX_LINE_LENGTH < new_target.line_len:
-            return False
-
         line_data_list = cls.get_line_data_list(config=config,
                                                 target=new_target,
                                                 pattern=rule.patterns[1],
                                                 filters=rule.filters)
 
         if not line_data_list:
             return False
```

### Comparing `credsweeper-1.6.4/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.7.0/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.7.0/credsweeper/scanner/scan_type/scan_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import re
 from abc import ABC, abstractmethod
-from typing import List
+from typing import List, Optional, Tuple, Dict
 
-from credsweeper.common.constants import RuleType
+from credsweeper.common.constants import RuleType, MAX_LINE_LENGTH, CHUNK_STEP_SIZE, CHUNKS_OVERLAP_SIZE
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate, LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.rules import Rule
 
 logger = logging.getLogger(__name__)
@@ -80,28 +80,55 @@
         Return:
             List of LineData objects if pattern a line and filters do not remove current line. Empty otherwise
 
         """
         line_data_list: List[LineData] = []
         # starting positions for continuously searching for overlapping pattern
         offsets = {0}
+        # case for oversize line
+        next_offset = CHUNK_STEP_SIZE
+        while target.line_len > next_offset + CHUNKS_OVERLAP_SIZE:
+            # the target is too long for single "finditer" - it will be scanned by chunks
+            if target.line_len < next_offset + MAX_LINE_LENGTH:
+                # best overlap for tail
+                offsets.add(target.line_len - MAX_LINE_LENGTH)
+                break
+            else:
+                # the chunk is not the last
+                offsets.add(next_offset)
+                next_offset += CHUNK_STEP_SIZE
+
+        # used to avoid duplicates for overlap cases only if line is oversize
+        purged_line_data: Optional[Dict[Tuple[int, int, int, int, int, int, int], LineData]] = {} if 1 < len(offsets) \
+            else None
+
         while offsets:
             offset = offsets.pop()
-            for _match in pattern.finditer(target.line, offset):
+            for _match in pattern.finditer(target.line, pos=offset, endpos=offset + MAX_LINE_LENGTH):
                 logger.debug("Valid line for pattern: %s in file: %s:%d in line: %s", pattern.pattern, target.file_path,
                              target.line_num, target.line)
                 line_data = LineData(config, target.line, target.line_pos, target.line_num, target.file_path,
                                      target.file_type, target.info, pattern, _match)
 
                 if config.use_filters and cls.filtering(config, target, line_data, filters):
                     if 0 < line_data.variable_end:
                         # may be next matched item will be not filtered - let search it after variable
                         offsets.add(line_data.variable_end)
                     continue
                 line_data_list.append(line_data)
+
+        if isinstance(purged_line_data, dict) and 1 < len(line_data_list):
+            # workaround for removing duplicates in case of oversize line only
+            for i in line_data_list:
+                ld_key = (i.line_num, i.value_start, i.value_end, i.separator_start, i.separator_end, i.variable_start,
+                          i.variable_end)
+                if ld_key not in purged_line_data:
+                    purged_line_data[ld_key] = i
+            line_data_list = [x for x in purged_line_data.values()]
+
         return line_data_list
 
     @classmethod
     def _get_candidates(cls, config: Config, rule: Rule, target: AnalysisTarget) -> List[Candidate]:
         """Returns Candidate objects list.
 
         Args:
```

### Comparing `credsweeper-1.6.4/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.7.0/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/secret/config.json` & `credsweeper-1.7.0/credsweeper/secret/config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999221910986615%*

 * *Differences: {"'exclude'": "{'extension': {insert: [(29, '.psd')]}}"}*

```diff
@@ -48,14 +48,15 @@
             ".mp4",
             ".npy",
             ".npz",
             ".ogg",
             ".pak",
             ".png",
             ".pptx",
+            ".psd",
             ".pyc",
             ".pyd",
             ".pyo",
             ".rar",
             ".realm",
             ".s7z",
             ".scss",
```

### Comparing `credsweeper-1.6.4/credsweeper/secret/log.yaml` & `credsweeper-1.7.0/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/utils/entropy_validator.py` & `credsweeper-1.7.0/credsweeper/utils/entropy_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/utils/pem_key_detector.py` & `credsweeper-1.7.0/credsweeper/utils/pem_key_detector.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/utils/util.py` & `credsweeper-1.7.0/credsweeper/utils/util.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/__init__.py` & `credsweeper-1.7.0/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/apply_validation.py` & `credsweeper-1.7.0/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/github_token_validation.py` & `credsweeper-1.7.0/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.7.0/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.7.0/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.7.0/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.7.0/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.7.0/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.7.0/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.7.0/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/credsweeper/validations/validation.py` & `credsweeper-1.7.0/credsweeper/validations/validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/.gitignore` & `credsweeper-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/LICENSE` & `credsweeper-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/README.md` & `credsweeper-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/pyproject.toml` & `credsweeper-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.4/PKG-INFO` & `credsweeper-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: credsweeper
-Version: 1.6.4
+Version: 1.7.0
 Summary: Credential Sweeper
 Project-URL: Homepage, https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 License: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

