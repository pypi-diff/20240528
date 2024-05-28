# Comparing `tmp/fdk_rdf_parser-2.7.2.tar.gz` & `tmp/fdk_rdf_parser-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk_rdf_parser-2.7.2.tar", max compression
+gzip compressed data, was "fdk_rdf_parser-2.7.3.tar", max compression
```

## Comparing `fdk_rdf_parser-2.7.2.tar` & `fdk_rdf_parser-2.7.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0    11357 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/LICENSE
--rw-r--r--   0        0        0     1248 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/pyproject.toml
--rw-r--r--   0        0        0      473 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/__init__.py
--rw-r--r--   0        0        0     1587 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/__init__.py
--rw-r--r--   0        0        0      270 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/address.py
--rw-r--r--   0        0        0      342 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/agent.py
--rw-r--r--   0        0        0      766 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/business_event.py
--rw-r--r--   0        0        0      336 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/catalog.py
--rw-r--r--   0        0        0      610 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/channel.py
--rw-r--r--   0        0        0     2879 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/concept.py
--rw-r--r--   0        0        0      189 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/conforms_to.py
--rw-r--r--   0        0        0      750 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/contactpoint.py
--rw-r--r--   0        0        0      436 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/cost.py
--rw-r--r--   0        0        0     2449 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/cpsvno_service.py
--rw-r--r--   0        0        0      356 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/data_distribution_service.py
--rw-r--r--   0        0        0     1668 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dataservice.py
--rw-r--r--   0        0        0     8657 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dataset.py
--rw-r--r--   0        0        0     1143 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dcat_resource.py
--rw-r--r--   0        0        0      274 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dct_standard.py
--rw-r--r--   0        0        0      924 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/distribution.py
--rw-r--r--   0        0        0      777 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/event.py
--rw-r--r--   0        0        0      758 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/evidence.py
--rw-r--r--   0        0        0      355 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/exceptions.py
--rw-r--r--   0        0        0      349 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/format.py
--rw-r--r--   0        0        0      174 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/harvest_meta_data.py
--rw-r--r--   0        0        0     3478 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/info_model.py
--rw-r--r--   0        0        0      331 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/legal_resource.py
--rw-r--r--   0        0        0      758 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/life_event.py
--rw-r--r--   0        0        0      402 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/media_type.py
--rw-r--r--   0        0        0     1910 2024-05-22 14:09:14.485404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/model_element.py
--rw-r--r--   0        0        0     1147 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/model_property.py
--rw-r--r--   0        0        0      430 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/organization.py
--rw-r--r--   0        0        0      466 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/output.py
--rw-r--r--   0        0        0      376 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/participation.py
--rw-r--r--   0        0        0     1888 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/public_service.py
--rw-r--r--   0        0        0      326 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/publisher.py
--rw-r--r--   0        0        0      206 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/qualified_attribution.py
--rw-r--r--   0        0        0      202 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/quality_annotation.py
--rw-r--r--   0        0        0      227 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/reference_data_code.py
--rw-r--r--   0        0        0      277 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/references.py
--rw-r--r--   0        0        0      412 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/requirement.py
--rw-r--r--   0        0        0      424 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/rule.py
--rw-r--r--   0        0        0      317 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/skos_concept.py
--rw-r--r--   0        0        0      271 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/subject.py
--rw-r--r--   0        0        0      191 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/temporal.py
--rw-r--r--   0        0        0      610 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/theme.py
--rw-r--r--   0        0        0      506 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/types.py
--rw-r--r--   0        0        0     8796 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/fdk_rdf_parser.py
--rw-r--r--   0        0        0     1349 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/__init__.py
--rw-r--r--   0        0        0     1070 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/address.py
--rw-r--r--   0        0        0     2175 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/agent.py
--rw-r--r--   0        0        0     1153 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/catalog.py
--rw-r--r--   0        0        0     1739 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/channel.py
--rw-r--r--   0        0        0    15020 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/concept.py
--rw-r--r--   0        0        0      992 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/conforms_to.py
--rw-r--r--   0        0        0     3172 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/contactpoint.py
--rw-r--r--   0        0        0     1336 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/cost.py
--rw-r--r--   0        0        0     6030 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
--rw-r--r--   0        0        0     1555 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
--rw-r--r--   0        0        0     1671 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dataservice.py
--rw-r--r--   0        0        0     9262 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dataset.py
--rw-r--r--   0        0        0     2928 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dcat_resource.py
--rw-r--r--   0        0        0      979 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dct_standard.py
--rw-r--r--   0        0        0     2051 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/distribution.py
--rw-r--r--   0        0        0     3093 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/event.py
--rw-r--r--   0        0        0     2018 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/evidence.py
--rw-r--r--   0        0        0     1116 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/format.py
--rw-r--r--   0        0        0      422 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
--rw-r--r--   0        0        0     6492 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/info_model.py
--rw-r--r--   0        0        0     1047 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/legal_resource.py
--rw-r--r--   0        0        0     3338 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/media_type.py
--rw-r--r--   0        0        0     4432 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/model_element.py
--rw-r--r--   0        0        0     3439 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/model_property.py
--rw-r--r--   0        0        0     2623 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/organization.py
--rw-r--r--   0        0        0     1247 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/output.py
--rw-r--r--   0        0        0      816 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/participation.py
--rw-r--r--   0        0        0     2155 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/publisher.py
--rw-r--r--   0        0        0      911 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
--rw-r--r--   0        0        0     1451 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/quality_annotation.py
--rw-r--r--   0        0        0     5858 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/reference_data_code.py
--rw-r--r--   0        0        0     1610 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/references.py
--rw-r--r--   0        0        0     1170 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/requirement.py
--rw-r--r--   0        0        0     1251 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/rule.py
--rw-r--r--   0        0        0     1605 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/skos_concept.py
--rw-r--r--   0        0        0     1049 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/spatial.py
--rw-r--r--   0        0        0      965 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/subject.py
--rw-r--r--   0        0        0     2540 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/temporal.py
--rw-r--r--   0        0        0     2891 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/theme.py
--rw-r--r--   0        0        0      831 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/__init__.py
--rw-r--r--   0        0        0     3518 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/ns.py
--rw-r--r--   0        0        0     4675 2024-05-22 14:09:14.489404 fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/utils.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/LICENSE
+-rw-r--r--   0        0        0     1248 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0      473 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/__init__.py
+-rw-r--r--   0        0        0     1587 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/address.py
+-rw-r--r--   0        0        0      342 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/agent.py
+-rw-r--r--   0        0        0      766 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/business_event.py
+-rw-r--r--   0        0        0      336 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/catalog.py
+-rw-r--r--   0        0        0      610 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/channel.py
+-rw-r--r--   0        0        0     2879 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/concept.py
+-rw-r--r--   0        0        0      189 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/conforms_to.py
+-rw-r--r--   0        0        0      750 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/contactpoint.py
+-rw-r--r--   0        0        0      436 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/cost.py
+-rw-r--r--   0        0        0     2449 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/cpsvno_service.py
+-rw-r--r--   0        0        0      356 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/data_distribution_service.py
+-rw-r--r--   0        0        0     1668 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/dataservice.py
+-rw-r--r--   0        0        0     8657 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/dataset.py
+-rw-r--r--   0        0        0     1143 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/dcat_resource.py
+-rw-r--r--   0        0        0      274 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/dct_standard.py
+-rw-r--r--   0        0        0      924 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/distribution.py
+-rw-r--r--   0        0        0      777 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/event.py
+-rw-r--r--   0        0        0      758 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/evidence.py
+-rw-r--r--   0        0        0      355 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/exceptions.py
+-rw-r--r--   0        0        0      349 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/format.py
+-rw-r--r--   0        0        0      174 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/harvest_meta_data.py
+-rw-r--r--   0        0        0     3478 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/info_model.py
+-rw-r--r--   0        0        0      331 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/legal_resource.py
+-rw-r--r--   0        0        0      758 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/life_event.py
+-rw-r--r--   0        0        0      402 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/media_type.py
+-rw-r--r--   0        0        0     1910 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/model_element.py
+-rw-r--r--   0        0        0     1147 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/model_property.py
+-rw-r--r--   0        0        0      430 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/organization.py
+-rw-r--r--   0        0        0      466 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/output.py
+-rw-r--r--   0        0        0      376 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/participation.py
+-rw-r--r--   0        0        0     1888 2024-05-28 12:31:02.794363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/public_service.py
+-rw-r--r--   0        0        0      326 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/publisher.py
+-rw-r--r--   0        0        0      206 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/qualified_attribution.py
+-rw-r--r--   0        0        0      202 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/quality_annotation.py
+-rw-r--r--   0        0        0      227 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/reference_data_code.py
+-rw-r--r--   0        0        0      277 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/references.py
+-rw-r--r--   0        0        0      412 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/requirement.py
+-rw-r--r--   0        0        0      424 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/rule.py
+-rw-r--r--   0        0        0      317 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/skos_concept.py
+-rw-r--r--   0        0        0      271 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/subject.py
+-rw-r--r--   0        0        0      191 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/temporal.py
+-rw-r--r--   0        0        0      610 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/theme.py
+-rw-r--r--   0        0        0      506 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/types.py
+-rw-r--r--   0        0        0     8796 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/fdk_rdf_parser.py
+-rw-r--r--   0        0        0     1349 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/address.py
+-rw-r--r--   0        0        0     2175 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/agent.py
+-rw-r--r--   0        0        0     1153 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/catalog.py
+-rw-r--r--   0        0        0     1739 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/channel.py
+-rw-r--r--   0        0        0    17208 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/concept.py
+-rw-r--r--   0        0        0      992 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/conforms_to.py
+-rw-r--r--   0        0        0     3172 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/contactpoint.py
+-rw-r--r--   0        0        0     1336 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/cost.py
+-rw-r--r--   0        0        0     6030 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
+-rw-r--r--   0        0        0     1555 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
+-rw-r--r--   0        0        0     1671 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/dataservice.py
+-rw-r--r--   0        0        0     9262 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/dataset.py
+-rw-r--r--   0        0        0     2928 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/dcat_resource.py
+-rw-r--r--   0        0        0      979 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/dct_standard.py
+-rw-r--r--   0        0        0     2051 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/distribution.py
+-rw-r--r--   0        0        0     3093 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/event.py
+-rw-r--r--   0        0        0     2018 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/evidence.py
+-rw-r--r--   0        0        0     1116 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/format.py
+-rw-r--r--   0        0        0      422 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
+-rw-r--r--   0        0        0     6492 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/info_model.py
+-rw-r--r--   0        0        0     1047 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/legal_resource.py
+-rw-r--r--   0        0        0     3338 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/media_type.py
+-rw-r--r--   0        0        0     4432 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/model_element.py
+-rw-r--r--   0        0        0     3439 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/model_property.py
+-rw-r--r--   0        0        0     2623 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/organization.py
+-rw-r--r--   0        0        0     1247 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/output.py
+-rw-r--r--   0        0        0      816 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/participation.py
+-rw-r--r--   0        0        0     2155 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/publisher.py
+-rw-r--r--   0        0        0      911 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
+-rw-r--r--   0        0        0     1451 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/quality_annotation.py
+-rw-r--r--   0        0        0     5858 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/reference_data_code.py
+-rw-r--r--   0        0        0     1610 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/references.py
+-rw-r--r--   0        0        0     1170 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/requirement.py
+-rw-r--r--   0        0        0     1251 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/rule.py
+-rw-r--r--   0        0        0     1605 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/skos_concept.py
+-rw-r--r--   0        0        0     1049 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/spatial.py
+-rw-r--r--   0        0        0      965 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/subject.py
+-rw-r--r--   0        0        0     3259 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/temporal.py
+-rw-r--r--   0        0        0     2891 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/theme.py
+-rw-r--r--   0        0        0      831 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/rdf_utils/__init__.py
+-rw-r--r--   0        0        0     3518 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/rdf_utils/ns.py
+-rw-r--r--   0        0        0     4675 2024-05-28 12:31:02.798363 fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/rdf_utils/utils.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.7.3/PKG-INFO
```

### Comparing `fdk_rdf_parser-2.7.2/LICENSE` & `fdk_rdf_parser-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/pyproject.toml` & `fdk_rdf_parser-2.7.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "fdk-rdf-parser"
-version = "2.7.2"
+version = "2.7.3"
 description = ""
 authors = ["NilsOveTen <nils.ove.tendenes@digdir.no>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 rdflib = "^7.0.0"
 isodate = "^0.6.1"
-requests = "^2.31.0"
+requests = "^2.32.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^8.2.0"
-coverage = {extras = ["toml"], version = "^7.5.0"}
+pytest = "^8.2.1"
+coverage = {extras = ["toml"], version = "^7.5.2"}
 pytest-cov = "^5.0.0"
 black = "^24.4.2"
 flake8 = "^7.0.0"
 flake8-bandit = "^4.1.1"
 flake8-black = "^0.3.6"
 flake8-bugbear = "^24.4.26"
 flake8-import-order = "^0.18.2"
-pep8-naming = "^0.13.3"
-safety = "^3.1.0"
+pep8-naming = "^0.14.1"
+safety = "^3.2.0"
 pytest-mock = "^3.14.0"
 codecov = "^2.1.13"
-flake8-annotations = "^3.0.1"
+flake8-annotations = "^3.1.1"
 mypy = "^1.10.0"
 nox = "^2024.4.15"
 nox-poetry = "^1.0.3"
 
 [tool.coverage.paths]
 source = ["src"]
```

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/__init__.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/business_event.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/business_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/channel.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/concept.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/contactpoint.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/cpsvno_service.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dataservice.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dataset.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/dcat_resource.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/distribution.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/event.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/evidence.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/info_model.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/life_event.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/life_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/model_element.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/model_property.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/public_service.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/public_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/classes/theme.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/classes/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/fdk_rdf_parser.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/fdk_rdf_parser.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/__init__.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/address.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/address.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/agent.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/agent.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/catalog.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/catalog.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/channel.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/concept.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/concept.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 from rdflib.namespace import (
     DCTERMS,
     FOAF,
     RDFS,
     SKOS,
 )
 
-from fdk_rdf_parser.classes import (
-    Concept,
-    Temporal,
-)
+from fdk_rdf_parser.classes import Concept
 from fdk_rdf_parser.classes.concept import (
     AssociativeRelation,
     Collection,
     Definition,
     GenericRelation,
     PartitiveRelation,
     Subject,
@@ -46,15 +43,15 @@
     value_set,
     value_translations,
     xkos_uri_v_2,
 )
 from .contactpoint import extract_contact_points
 from .harvest_meta_data import extract_meta_data
 from .publisher import extract_publisher
-from .temporal import extract_temporal
+from .temporal import extract_temporal_skos
 
 
 def parse_text_and_uri(graph: Graph, subject: URIRef) -> TextAndURI:
     return TextAndURI(
         text=value_translations(graph, subject, RDFS.label),
         uri=object_value(graph, subject, RDFS.seeAlso),
     )
@@ -256,68 +253,115 @@
 def parse_associative_relation(
     graph: Graph, associative_relation_ref: URIRef
 ) -> AssociativeRelation:
     return AssociativeRelation(
         description=value_translations(
             graph, associative_relation_ref, skosno_uri("relationRole")
         ),
-        related=object_value(graph, associative_relation_ref, SKOS.related),
+        related=object_value(
+            graph, associative_relation_ref, skosno_uri("hasToConcept")
+        ),
     )
 
 
 def extract_associative_relations(
     graph: Graph, concept_uri: URIRef
 ) -> Optional[List[AssociativeRelation]]:
     associative_relations = []
-    for associative_relation_ref in graph.objects(
-        concept_uri, skosno_uri("assosiativRelasjon")
-    ):
-        if has_value_on_predicate(
-            graph, associative_relation_ref, skosno_uri("relationRole")
+
+    if has_value_on_predicate(graph, concept_uri, skosno_uri("isFromConceptIn")):
+        for associative_relation_ref in graph.objects(
+            concept_uri, skosno_uri("isFromConceptIn")
         ):
             associative_relations.append(
                 parse_associative_relation(graph, associative_relation_ref)
             )
-        else:
+    else:
+        for associative_relation_ref in graph.objects(
+            concept_uri, skosno_uri("assosiativRelasjon")
+        ):
             associative_relations.append(
                 parse_associative_relation_deprecated(graph, associative_relation_ref)
             )
     return associative_relations if len(associative_relations) > 0 else None
 
 
 def parse_partitive_relation(
     graph: Graph, partitive_relation_ref: URIRef
 ) -> PartitiveRelation:
     return PartitiveRelation(
         description=value_translations(
             graph, partitive_relation_ref, DCTERMS.description
         ),
+        hasPart=object_value(
+            graph, partitive_relation_ref, skosno_uri("hasPartitiveConcept")
+        ),
+        isPartOf=object_value(
+            graph, partitive_relation_ref, skosno_uri("hasComprehensiveConcept")
+        ),
+    )
+
+
+def parse_partitive_relation_deprecated(
+    graph: Graph, partitive_relation_ref: URIRef
+) -> PartitiveRelation:
+    return PartitiveRelation(
+        description=value_translations(
+            graph, partitive_relation_ref, DCTERMS.description
+        ),
         hasPart=object_value(graph, partitive_relation_ref, DCTERMS.hasPart),
         isPartOf=object_value(graph, partitive_relation_ref, DCTERMS.isPartOf),
     )
 
 
 def extract_partitive_relations(
     graph: Graph, concept_uri: URIRef
 ) -> Optional[List[PartitiveRelation]]:
     partitive_relations = []
-    for partitive_relation_ref in graph.objects(
-        concept_uri, skosno_uri("partitivRelasjon")
+    if has_value_on_predicate(
+        graph, concept_uri, skosno_uri("hasPartitiveConceptRelation")
     ):
-        partitive_relations.append(
-            parse_partitive_relation(graph, partitive_relation_ref)
-        )
+        for partitive_relation_ref in graph.objects(
+            concept_uri, skosno_uri("hasPartitiveConceptRelation")
+        ):
+            partitive_relations.append(
+                parse_partitive_relation(graph, partitive_relation_ref)
+            )
+    else:
+        for partitive_relation_ref in graph.objects(
+            concept_uri, skosno_uri("partitivRelasjon")
+        ):
+            partitive_relations.append(
+                parse_partitive_relation_deprecated(graph, partitive_relation_ref)
+            )
+
     return partitive_relations if len(partitive_relations) > 0 else None
 
 
 def parse_generic_relation(
     graph: Graph, generic_relation_ref: URIRef
 ) -> GenericRelation:
     return GenericRelation(
         divisioncriterion=value_translations(
+            graph, generic_relation_ref, DCTERMS.description
+        ),
+        generalizes=object_value(
+            graph, generic_relation_ref, skosno_uri("hasSpecificConcept")
+        ),
+        specializes=object_value(
+            graph, generic_relation_ref, skosno_uri("hasGenericConcept")
+        ),
+    )
+
+
+def parse_generic_relation_deprecated(
+    graph: Graph, generic_relation_ref: URIRef
+) -> GenericRelation:
+    return GenericRelation(
+        divisioncriterion=value_translations(
             graph, generic_relation_ref, skosno_uri("inndelingskriterium")
         ),
         generalizes=object_value(
             graph, generic_relation_ref, xkos_uri_v_2("generalizes")
         ),
         specializes=object_value(
             graph, generic_relation_ref, xkos_uri_v_2("specializes")
@@ -325,34 +369,56 @@
     )
 
 
 def extract_generic_relations(
     graph: Graph, concept_uri: URIRef
 ) -> Optional[List[GenericRelation]]:
     generic_relations = []
-    for generic_relation_ref in graph.objects(
-        concept_uri, skosno_uri("generiskRelasjon")
+
+    if has_value_on_predicate(
+        graph, concept_uri, skosno_uri("hasGenericConceptRelation")
     ):
-        generic_relations.append(parse_generic_relation(graph, generic_relation_ref))
+        for generic_relation_ref in graph.objects(
+            concept_uri, skosno_uri("hasGenericConceptRelation")
+        ):
+            generic_relations.append(
+                parse_generic_relation(graph, generic_relation_ref)
+            )
+    else:
+        for generic_relation_ref in graph.objects(
+            concept_uri, skosno_uri("generiskRelasjon")
+        ):
+            generic_relations.append(
+                parse_generic_relation_deprecated(graph, generic_relation_ref)
+            )
     return generic_relations if len(generic_relations) > 0 else None
 
 
+def extract_collection_label(
+    graph: Graph, collection_uri: URIRef
+) -> Optional[Dict[str, str]]:
+    if has_literal_value_on_predicate(graph, collection_uri, DCTERMS.title):
+        return value_translations(graph, collection_uri, DCTERMS.title)
+    else:
+        return value_translations(graph, collection_uri, RDFS.label)
+
+
 def parse_collection(graph: Graph, concept_record_uri: URIRef) -> Optional[Collection]:
     collection_record_uri = graph.value(concept_record_uri, DCTERMS.isPartOf)
 
     if collection_record_uri and is_type(
         dcat_uri("CatalogRecord"), graph, collection_record_uri
     ):
         collection_uri = graph.value(collection_record_uri, FOAF.primaryTopic)
 
         if collection_uri and is_type(SKOS.Collection, graph, collection_uri):
             return Collection(
                 id=object_value(graph, collection_record_uri, DCTERMS.identifier),
                 publisher=extract_publisher(graph, collection_uri),
-                label=value_translations(graph, collection_uri, RDFS.label),
+                label=extract_collection_label(graph, collection_uri),
                 uri=collection_uri.toPython(),
                 description=value_translations(
                     graph, collection_uri, DCTERMS.description
                 ),
             )
     return None
 
@@ -376,16 +442,16 @@
 
     return labels if len(labels) > 0 else None
 
 
 def _parse_concept(
     graph: Graph, fdk_record_uri: URIRef, concept_uri: URIRef
 ) -> Concept:
-    concept_temporal_list = extract_temporal(graph, concept_uri)
-    concept_temporal = concept_temporal_list[0] if concept_temporal_list else Temporal()
+
+    concept_temporal = extract_temporal_skos(graph, concept_uri)
     contact_points = extract_contact_points(graph, concept_uri)
 
     pref_label_list = extract_labels(
         graph, concept_uri, SKOS.prefLabel, skosxl_uri("prefLabel")
     )
     definition_list = extract_definitions(graph, concept_uri)
```

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/conforms_to.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/conforms_to.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/contactpoint.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/cost.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/cost.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/cpsvno_service.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/data_distribution_service.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/data_distribution_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dataservice.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dataset.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dcat_resource.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/dct_standard.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/dct_standard.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/distribution.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/event.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/evidence.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/format.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/format.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/info_model.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/legal_resource.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/legal_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/media_type.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/media_type.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/model_element.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/model_property.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/organization.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/organization.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/output.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/output.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/participation.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/participation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/publisher.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/publisher.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/qualified_attribution.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/qualified_attribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/quality_annotation.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/quality_annotation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/reference_data_code.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/reference_data_code.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/references.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/references.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/requirement.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/requirement.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/rule.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/rule.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/skos_concept.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/skos_concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/spatial.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/spatial.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/subject.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/subject.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/temporal.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/temporal.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 )
 from rdflib.namespace import DCTERMS
 
 from fdk_rdf_parser.classes import Temporal
 from fdk_rdf_parser.rdf_utils import (
     date_value,
     dcat_uri,
+    euvoc_uri,
     owl_time_uri,
     resource_list,
     schema_uri,
 )
 
 
 def extract_temporal(graph: Graph, subject: URIRef) -> Optional[List[Temporal]]:
@@ -55,14 +56,32 @@
         values.append(
             Temporal(uri=temporal_uri, startDate=start_value, endDate=end_value)
         )
 
     return values if len(values) > 0 else None
 
 
+def extract_temporal_skos(graph: Graph, subject: URIRef) -> Temporal:
+    temporal = Temporal()
+
+    start_value = date_value(graph, subject, euvoc_uri("startDate"))
+    end_value = date_value(graph, subject, euvoc_uri("endDate"))
+
+    deprecated_resource = graph.value(subject, DCTERMS.temporal)
+    if start_value or end_value:
+        temporal = Temporal(startDate=start_value, endDate=end_value)
+    elif deprecated_resource is not None:
+        start_value = date_value(graph, deprecated_resource, schema_uri("startDate"))
+        end_value = date_value(graph, deprecated_resource, schema_uri("endDate"))
+
+        temporal = Temporal(startDate=start_value, endDate=end_value)
+
+    return temporal
+
+
 def extract_owl_time_instant(graph: Graph, subject: Any) -> Optional[str]:
     owl_date = date_value(graph, subject, owl_time_uri("inXSDDateTime"))
     owl_date = (
         date_value(graph, subject, owl_time_uri("inXSDDateTimeStamp"))
         if owl_date is None
         else owl_date
     )
```

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/parse_functions/theme.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/parse_functions/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/__init__.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/rdf_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/ns.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/rdf_utils/ns.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/src/fdk_rdf_parser/rdf_utils/utils.py` & `fdk_rdf_parser-2.7.3/src/fdk_rdf_parser/rdf_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.7.2/PKG-INFO` & `fdk_rdf_parser-2.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fdk-rdf-parser
-Version: 2.7.2
+Version: 2.7.3
 Summary: 
 Author: NilsOveTen
 Author-email: nils.ove.tendenes@digdir.no
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
```

