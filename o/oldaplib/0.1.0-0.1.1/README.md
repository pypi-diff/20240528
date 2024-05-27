# Comparing `tmp/oldaplib-0.1.0.tar.gz` & `tmp/oldaplib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldaplib-0.1.0.tar", max compression
+gzip compressed data, was "oldaplib-0.1.1.tar", max compression
```

## Comparing `oldaplib-0.1.0.tar` & `oldaplib-0.1.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0     1406 2024-05-17 21:15:50.741523 oldaplib-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.860798 oldaplib-0.1.0/oldaplib/__init__.py
--rw-r--r--   0        0        0     9892 2024-05-24 22:11:53.229656 oldaplib-0.1.0/oldaplib/ontologies/admin.trig
--rw-r--r--   0        0        0    31964 2024-05-24 20:29:28.376369 oldaplib-0.1.0/oldaplib/ontologies/oldap.shacl.trig
--rw-r--r--   0        0        0    31147 2024-05-24 20:29:28.379250 oldaplib-0.1.0/oldaplib/ontologies/oldap.ttl
--rw-r--r--   0        0        0    17976 2024-05-17 12:28:38.672082 oldaplib-0.1.0/oldaplib/src/ObjectFactory.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.862923 oldaplib-0.1.0/oldaplib/src/__init__.py
--rw-r--r--   0        0        0    19932 2024-05-26 21:39:24.866447 oldaplib-0.1.0/oldaplib/src/connection.py
--rw-r--r--   0        0        0    14065 2024-05-17 16:27:00.108249 oldaplib-0.1.0/oldaplib/src/datamodel.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.863726 oldaplib-0.1.0/oldaplib/src/dtypes/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-17 12:28:38.584913 oldaplib-0.1.0/oldaplib/src/dtypes/bnode.py
--rw-r--r--   0        0        0     4917 2024-05-17 12:28:38.714172 oldaplib-0.1.0/oldaplib/src/dtypes/languagein.py
--rw-r--r--   0        0        0     1067 2024-05-17 12:28:38.356660 oldaplib-0.1.0/oldaplib/src/dtypes/namespaceiri.py
--rw-r--r--   0        0        0     4088 2024-05-17 12:28:38.589960 oldaplib-0.1.0/oldaplib/src/dtypes/rdfset.py
--rw-r--r--   0        0        0     1900 2024-05-17 12:28:38.505893 oldaplib-0.1.0/oldaplib/src/dtypes/xsdset.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.865443 oldaplib-0.1.0/oldaplib/src/enums/__init__.py
--rw-r--r--   0        0        0      828 2024-05-17 12:28:38.730926 oldaplib-0.1.0/oldaplib/src/enums/action.py
--rw-r--r--   0        0        0     4623 2024-05-17 12:28:38.372733 oldaplib-0.1.0/oldaplib/src/enums/language.py
--rw-r--r--   0        0        0     2466 2024-05-17 16:17:14.367204 oldaplib-0.1.0/oldaplib/src/enums/permissions.py
--rw-r--r--   0        0        0      348 2024-05-24 21:27:46.468388 oldaplib-0.1.0/oldaplib/src/enums/permissionsetattr.py
--rw-r--r--   0        0        0     2069 2024-05-16 21:38:25.885179 oldaplib-0.1.0/oldaplib/src/enums/propertyclassattr.py
--rw-r--r--   0        0        0      245 2024-05-24 20:29:28.380276 oldaplib-0.1.0/oldaplib/src/enums/resourceclassattr.py
--rw-r--r--   0        0        0      636 2024-05-16 20:58:19.867251 oldaplib-0.1.0/oldaplib/src/enums/sparql_result_format.py
--rw-r--r--   0        0        0      922 2024-05-17 16:16:02.047994 oldaplib-0.1.0/oldaplib/src/enums/userdataclassattr.py
--rw-r--r--   0        0        0     6133 2024-05-16 20:58:19.867821 oldaplib-0.1.0/oldaplib/src/enums/xsd_datatypes.py
--rw-r--r--   0        0        0      406 2024-05-25 22:49:56.860916 oldaplib-0.1.0/oldaplib/src/globalconfig.py
--rw-r--r--   0        0        0     2054 2024-05-18 20:31:39.060235 oldaplib-0.1.0/oldaplib/src/helpers/Notify.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.868316 oldaplib-0.1.0/oldaplib/src/helpers/__init__.py
--rw-r--r--   0        0        0    13645 2024-05-26 21:25:16.747717 oldaplib-0.1.0/oldaplib/src/helpers/context.py
--rw-r--r--   0        0        0    30931 2024-05-17 12:28:38.368045 oldaplib-0.1.0/oldaplib/src/helpers/langstring.py
--rw-r--r--   0        0        0     2031 2024-05-24 20:29:28.381026 oldaplib-0.1.0/oldaplib/src/helpers/observable_dict.py
--rw-r--r--   0        0        0     5525 2024-05-18 20:48:09.073657 oldaplib-0.1.0/oldaplib/src/helpers/observable_set.py
--rw-r--r--   0        0        0     1265 2024-05-16 21:17:59.026464 oldaplib-0.1.0/oldaplib/src/helpers/oldaperror.py
--rw-r--r--   0        0        0     1141 2024-05-17 12:28:38.168566 oldaplib-0.1.0/oldaplib/src/helpers/propertyclass_singleton.py
--rw-r--r--   0        0        0    10146 2024-05-19 22:50:03.808918 oldaplib-0.1.0/oldaplib/src/helpers/query_processor.py
--rw-r--r--   0        0        0     3218 2024-05-17 12:28:38.445610 oldaplib-0.1.0/oldaplib/src/helpers/semantic_version.py
--rw-r--r--   0        0        0     4086 2024-05-16 20:58:19.870752 oldaplib-0.1.0/oldaplib/src/helpers/serializer.py
--rw-r--r--   0        0        0      332 2024-05-25 22:49:56.844500 oldaplib-0.1.0/oldaplib/src/helpers/singletonmeta.py
--rw-r--r--   0        0        0    12609 2024-05-19 20:59:15.236199 oldaplib-0.1.0/oldaplib/src/helpers/tools.py
--rw-r--r--   0        0        0     2430 2024-05-17 12:28:38.306954 oldaplib-0.1.0/oldaplib/src/iconnection.py
--rw-r--r--   0        0        0     7590 2024-05-22 21:47:27.190971 oldaplib-0.1.0/oldaplib/src/in_project.py
--rw-r--r--   0        0        0     3036 2024-05-17 12:28:38.146377 oldaplib-0.1.0/oldaplib/src/model.py
--rw-r--r--   0        0        0    21622 2024-05-17 16:12:17.599380 oldaplib-0.1.0/oldaplib/src/oldaplist.py
--rw-r--r--   0        0        0     2372 2024-05-17 16:10:49.541460 oldaplib-0.1.0/oldaplib/src/oldaplistnode.py
--rw-r--r--   0        0        0    22727 2024-05-26 22:05:19.415113 oldaplib-0.1.0/oldaplib/src/permissionset.py
--rw-r--r--   0        0        0    33436 2024-05-25 20:24:23.509178 oldaplib-0.1.0/oldaplib/src/project.py
--rw-r--r--   0        0        0    58711 2024-05-20 20:46:37.094562 oldaplib-0.1.0/oldaplib/src/propertyclass.py
--rw-r--r--   0        0        0    54918 2024-05-24 20:29:28.381983 oldaplib-0.1.0/oldaplib/src/resourceclass.py
--rw-r--r--   0        0        0    26641 2024-05-17 16:07:43.693473 oldaplib-0.1.0/oldaplib/src/user.py
--rw-r--r--   0        0        0    30434 2024-05-17 16:06:07.068855 oldaplib-0.1.0/oldaplib/src/user_dataclass.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.874593 oldaplib-0.1.0/oldaplib/src/xsd/__init__.py
--rw-r--r--   0        0        0     7896 2024-05-17 12:28:38.536038 oldaplib-0.1.0/oldaplib/src/xsd/floatingpoint.py
--rw-r--r--   0        0        0     4821 2024-05-26 22:05:53.954324 oldaplib-0.1.0/oldaplib/src/xsd/iri.py
--rw-r--r--   0        0        0     1499 2024-05-16 20:58:19.875428 oldaplib-0.1.0/oldaplib/src/xsd/xsd.py
--rw-r--r--   0        0        0     5523 2024-05-25 22:00:25.651776 oldaplib-0.1.0/oldaplib/src/xsd/xsd_anyuri.py
--rw-r--r--   0        0        0     3543 2024-05-17 12:28:38.710082 oldaplib-0.1.0/oldaplib/src/xsd/xsd_base64binary.py
--rw-r--r--   0        0        0     2648 2024-05-20 20:22:47.068509 oldaplib-0.1.0/oldaplib/src/xsd/xsd_boolean.py
--rw-r--r--   0        0        0      979 2024-05-17 12:28:38.314066 oldaplib-0.1.0/oldaplib/src/xsd/xsd_byte.py
--rw-r--r--   0        0        0     7043 2024-05-17 12:28:38.281355 oldaplib-0.1.0/oldaplib/src/xsd/xsd_date.py
--rw-r--r--   0        0        0     3972 2024-05-17 12:28:38.567099 oldaplib-0.1.0/oldaplib/src/xsd/xsd_datetime.py
--rw-r--r--   0        0        0     3904 2024-05-17 12:28:38.599870 oldaplib-0.1.0/oldaplib/src/xsd/xsd_datetimestamp.py
--rw-r--r--   0        0        0     1376 2024-05-17 12:28:38.696167 oldaplib-0.1.0/oldaplib/src/xsd/xsd_decimal.py
--rw-r--r--   0        0        0     1422 2024-05-17 12:28:38.618206 oldaplib-0.1.0/oldaplib/src/xsd/xsd_double.py
--rw-r--r--   0        0        0     3319 2024-05-17 12:28:38.203063 oldaplib-0.1.0/oldaplib/src/xsd/xsd_duration.py
--rw-r--r--   0        0        0     1242 2024-05-17 12:28:38.746441 oldaplib-0.1.0/oldaplib/src/xsd/xsd_float.py
--rw-r--r--   0        0        0     3517 2024-05-17 12:28:38.705599 oldaplib-0.1.0/oldaplib/src/xsd/xsd_gday.py
--rw-r--r--   0        0        0     3628 2024-05-17 12:28:38.677544 oldaplib-0.1.0/oldaplib/src/xsd/xsd_gmonth.py
--rw-r--r--   0        0        0     3840 2024-05-17 12:28:38.519315 oldaplib-0.1.0/oldaplib/src/xsd/xsd_gmonthday.py
--rw-r--r--   0        0        0     3780 2024-05-17 12:28:38.723526 oldaplib-0.1.0/oldaplib/src/xsd/xsd_gyear.py
--rw-r--r--   0        0        0     4186 2024-05-17 12:28:38.657789 oldaplib-0.1.0/oldaplib/src/xsd/xsd_gyearmonth.py
--rw-r--r--   0        0        0     3073 2024-05-17 12:28:38.595486 oldaplib-0.1.0/oldaplib/src/xsd/xsd_hexbinary.py
--rw-r--r--   0        0        0      617 2024-05-17 12:28:38.552712 oldaplib-0.1.0/oldaplib/src/xsd/xsd_id.py
--rw-r--r--   0        0        0      647 2024-05-17 12:28:38.562362 oldaplib-0.1.0/oldaplib/src/xsd/xsd_idref.py
--rw-r--r--   0        0        0     1123 2024-05-17 12:28:38.236235 oldaplib-0.1.0/oldaplib/src/xsd/xsd_int.py
--rw-r--r--   0        0        0     5727 2024-05-17 12:28:38.644946 oldaplib-0.1.0/oldaplib/src/xsd/xsd_integer.py
--rw-r--r--   0        0        0     3504 2024-05-17 12:28:38.346404 oldaplib-0.1.0/oldaplib/src/xsd/xsd_language.py
--rw-r--r--   0        0        0     1179 2024-05-17 12:28:38.423635 oldaplib-0.1.0/oldaplib/src/xsd/xsd_long.py
--rw-r--r--   0        0        0     3436 2024-05-17 12:28:38.741813 oldaplib-0.1.0/oldaplib/src/xsd/xsd_name.py
--rw-r--r--   0        0        0     5067 2024-05-25 20:39:47.835986 oldaplib-0.1.0/oldaplib/src/xsd/xsd_ncname.py
--rw-r--r--   0        0        0      999 2024-05-17 12:28:38.701096 oldaplib-0.1.0/oldaplib/src/xsd/xsd_negativeinteger.py
--rw-r--r--   0        0        0     3298 2024-05-17 12:28:38.181051 oldaplib-0.1.0/oldaplib/src/xsd/xsd_nmtoken.py
--rw-r--r--   0        0        0     1043 2024-05-17 12:28:38.351243 oldaplib-0.1.0/oldaplib/src/xsd/xsd_nonnegativeinteger.py
--rw-r--r--   0        0        0      964 2024-05-17 12:28:38.499113 oldaplib-0.1.0/oldaplib/src/xsd/xsd_nonpositiveinteger.py
--rw-r--r--   0        0        0     3967 2024-05-17 12:28:38.435583 oldaplib-0.1.0/oldaplib/src/xsd/xsd_normalizedstring.py
--rw-r--r--   0        0        0      945 2024-05-17 12:28:38.528978 oldaplib-0.1.0/oldaplib/src/xsd/xsd_positiveinteger.py
--rw-r--r--   0        0        0     6750 2024-05-17 12:28:38.271692 oldaplib-0.1.0/oldaplib/src/xsd/xsd_qname.py
--rw-r--r--   0        0        0      989 2024-05-17 12:28:38.240593 oldaplib-0.1.0/oldaplib/src/xsd/xsd_short.py
--rw-r--r--   0        0        0     9512 2024-05-17 12:28:38.513898 oldaplib-0.1.0/oldaplib/src/xsd/xsd_string.py
--rw-r--r--   0        0        0     3670 2024-05-17 12:28:38.458232 oldaplib-0.1.0/oldaplib/src/xsd/xsd_time.py
--rw-r--r--   0        0        0     3546 2024-05-17 12:28:38.302060 oldaplib-0.1.0/oldaplib/src/xsd/xsd_token.py
--rw-r--r--   0        0        0     1027 2024-05-17 12:28:38.682094 oldaplib-0.1.0/oldaplib/src/xsd/xsd_unsignedbyte.py
--rw-r--r--   0        0        0     1040 2024-05-17 12:28:38.576156 oldaplib-0.1.0/oldaplib/src/xsd/xsd_unsignedint.py
--rw-r--r--   0        0        0     1007 2024-05-17 12:28:38.524210 oldaplib-0.1.0/oldaplib/src/xsd/xsd_unsignedlong.py
--rw-r--r--   0        0        0     1012 2024-05-17 12:28:38.572122 oldaplib-0.1.0/oldaplib/src/xsd/xsd_unsignedshort.py
--rw-r--r--   0        0        0        0 2024-05-16 20:58:19.898288 oldaplib-0.1.0/oldaplib/test/__init__.py
--rw-r--r--   0        0        0    14309 2024-05-24 20:29:28.389690 oldaplib-0.1.0/oldaplib/test/gaga.trig
--rw-r--r--   0        0        0     1759 2024-05-18 22:18:06.660501 oldaplib-0.1.0/oldaplib/test/propclass_test.trig
--rw-r--r--   0        0        0    13591 2024-05-26 21:44:40.793610 oldaplib-0.1.0/oldaplib/test/test_connection.py
--rw-r--r--   0        0        0     4777 2024-05-25 22:24:17.528153 oldaplib-0.1.0/oldaplib/test/test_context.py
--rw-r--r--   0        0        0    21746 2024-05-24 20:29:28.392421 oldaplib-0.1.0/oldaplib/test/test_datamodel.py
--rw-r--r--   0        0        0     8221 2024-05-17 12:33:33.047906 oldaplib-0.1.0/oldaplib/test/test_dtypes.py
--rw-r--r--   0        0        0     7774 2024-05-17 16:39:06.614379 oldaplib-0.1.0/oldaplib/test/test_in_project.py
--rw-r--r--   0        0        0    11628 2024-05-17 12:28:38.294685 oldaplib-0.1.0/oldaplib/test/test_langstring.py
--rw-r--r--   0        0        0     8826 2024-05-17 12:28:38.474410 oldaplib-0.1.0/oldaplib/test/test_language_in.py
--rw-r--r--   0        0        0     3645 2024-05-17 16:00:20.113780 oldaplib-0.1.0/oldaplib/test/test_objectfactory.py
--rw-r--r--   0        0        0     6249 2024-05-17 12:28:38.736345 oldaplib-0.1.0/oldaplib/test/test_observable_set.py
--rw-r--r--   0        0        0     7288 2024-05-17 16:40:34.925874 oldaplib-0.1.0/oldaplib/test/test_oldaplist.py
--rw-r--r--   0        0        0    13292 2024-05-26 22:06:20.088817 oldaplib-0.1.0/oldaplib/test/test_permissionset.py
--rw-r--r--   0        0        0    16905 2024-05-17 12:49:24.206742 oldaplib-0.1.0/oldaplib/test/test_project.py
--rw-r--r--   0        0        0    28492 2024-05-17 12:33:32.999538 oldaplib-0.1.0/oldaplib/test/test_propertyclass.py
--rw-r--r--   0        0        0    42274 2024-05-24 20:29:28.394589 oldaplib-0.1.0/oldaplib/test/test_resourceclass.py
--rw-r--r--   0        0        0     3392 2024-05-17 12:28:38.215443 oldaplib-0.1.0/oldaplib/test/test_semantic_version.py
--rw-r--r--   0        0        0    40179 2024-05-25 22:37:42.478850 oldaplib-0.1.0/oldaplib/test/test_user.py
--rw-r--r--   0        0        0    64182 2024-05-17 12:33:33.043637 oldaplib-0.1.0/oldaplib/test/test_xsd_datatypes.py
--rw-r--r--   0        0        0    12312 2024-05-20 22:29:47.421485 oldaplib-0.1.0/oldaplib/testdata/connection_test.trig
--rw-r--r--   0        0        0     1382 2024-05-16 21:56:28.046244 oldaplib-0.1.0/oldaplib/testdata/datamodel_test.trig
--rw-r--r--   0        0        0    14936 2024-05-24 20:29:28.395766 oldaplib-0.1.0/oldaplib/testdata/objectfactory_test.trig
--rw-r--r--   0        0        0      303 2024-05-16 21:56:27.962931 oldaplib-0.1.0/oldaplib/testit.http
--rw-r--r--   0        0        0      914 2024-05-26 22:13:42.936761 oldaplib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 oldaplib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1406 2024-05-23 11:56:31.253193 oldaplib-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 11:56:31.257752 oldaplib-0.1.1/oldaplib/__init__.py
+-rw-r--r--   0        0        0     9892 2024-05-27 09:21:13.277211 oldaplib-0.1.1/oldaplib/ontologies/admin.trig
+-rw-r--r--   0        0        0    31964 2024-05-24 14:39:31.486274 oldaplib-0.1.1/oldaplib/ontologies/oldap.shacl.trig
+-rw-r--r--   0        0        0    31147 2024-05-24 14:36:38.679988 oldaplib-0.1.1/oldaplib/ontologies/oldap.ttl
+-rw-r--r--   0        0        0    17976 2024-05-23 11:56:31.258169 oldaplib-0.1.1/oldaplib/src/ObjectFactory.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:56:31.258205 oldaplib-0.1.1/oldaplib/src/__init__.py
+-rw-r--r--   0        0        0    19932 2024-05-27 09:21:13.277500 oldaplib-0.1.1/oldaplib/src/connection.py
+-rw-r--r--   0        0        0    14065 2024-05-23 11:56:31.258398 oldaplib-0.1.1/oldaplib/src/datamodel.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:56:31.258472 oldaplib-0.1.1/oldaplib/src/dtypes/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-23 11:56:31.258540 oldaplib-0.1.1/oldaplib/src/dtypes/bnode.py
+-rw-r--r--   0        0        0     4917 2024-05-23 11:56:31.258606 oldaplib-0.1.1/oldaplib/src/dtypes/languagein.py
+-rw-r--r--   0        0        0     1067 2024-05-23 11:56:31.258662 oldaplib-0.1.1/oldaplib/src/dtypes/namespaceiri.py
+-rw-r--r--   0        0        0     4088 2024-05-23 11:56:31.258713 oldaplib-0.1.1/oldaplib/src/dtypes/rdfset.py
+-rw-r--r--   0        0        0     1900 2024-05-23 11:56:31.258767 oldaplib-0.1.1/oldaplib/src/dtypes/xsdset.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:56:31.258828 oldaplib-0.1.1/oldaplib/src/enums/__init__.py
+-rw-r--r--   0        0        0      828 2024-05-23 11:56:31.258965 oldaplib-0.1.1/oldaplib/src/enums/action.py
+-rw-r--r--   0        0        0     4623 2024-05-23 11:56:31.259076 oldaplib-0.1.1/oldaplib/src/enums/language.py
+-rw-r--r--   0        0        0     2466 2024-05-23 11:56:31.259179 oldaplib-0.1.1/oldaplib/src/enums/permissions.py
+-rw-r--r--   0        0        0      348 2024-05-27 09:21:13.277709 oldaplib-0.1.1/oldaplib/src/enums/permissionsetattr.py
+-rw-r--r--   0        0        0     2069 2024-05-23 11:56:31.259328 oldaplib-0.1.1/oldaplib/src/enums/propertyclassattr.py
+-rw-r--r--   0        0        0      245 2024-05-23 12:05:35.502734 oldaplib-0.1.1/oldaplib/src/enums/resourceclassattr.py
+-rw-r--r--   0        0        0      636 2024-05-23 11:56:31.259459 oldaplib-0.1.1/oldaplib/src/enums/sparql_result_format.py
+-rw-r--r--   0        0        0      922 2024-05-23 11:56:31.259516 oldaplib-0.1.1/oldaplib/src/enums/userdataclassattr.py
+-rw-r--r--   0        0        0     6133 2024-05-23 11:56:31.259591 oldaplib-0.1.1/oldaplib/src/enums/xsd_datatypes.py
+-rw-r--r--   0        0        0      406 2024-05-27 09:21:13.277893 oldaplib-0.1.1/oldaplib/src/globalconfig.py
+-rw-r--r--   0        0        0     2054 2024-05-23 11:56:31.259727 oldaplib-0.1.1/oldaplib/src/helpers/Notify.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:56:31.259754 oldaplib-0.1.1/oldaplib/src/helpers/__init__.py
+-rw-r--r--   0        0        0    13645 2024-05-27 09:21:13.278119 oldaplib-0.1.1/oldaplib/src/helpers/context.py
+-rw-r--r--   0        0        0    30931 2024-05-23 11:56:31.259917 oldaplib-0.1.1/oldaplib/src/helpers/langstring.py
+-rw-r--r--   0        0        0     2031 2024-05-23 13:56:27.295115 oldaplib-0.1.1/oldaplib/src/helpers/observable_dict.py
+-rw-r--r--   0        0        0     5525 2024-05-23 11:56:31.260057 oldaplib-0.1.1/oldaplib/src/helpers/observable_set.py
+-rw-r--r--   0        0        0     1265 2024-05-23 11:56:31.260107 oldaplib-0.1.1/oldaplib/src/helpers/oldaperror.py
+-rw-r--r--   0        0        0     1141 2024-05-23 11:56:31.260156 oldaplib-0.1.1/oldaplib/src/helpers/propertyclass_singleton.py
+-rw-r--r--   0        0        0    10146 2024-05-23 11:56:31.260221 oldaplib-0.1.1/oldaplib/src/helpers/query_processor.py
+-rw-r--r--   0        0        0     3218 2024-05-23 11:56:31.260272 oldaplib-0.1.1/oldaplib/src/helpers/semantic_version.py
+-rw-r--r--   0        0        0     4086 2024-05-23 11:56:31.260341 oldaplib-0.1.1/oldaplib/src/helpers/serializer.py
+-rw-r--r--   0        0        0      332 2024-05-27 09:21:13.278255 oldaplib-0.1.1/oldaplib/src/helpers/singletonmeta.py
+-rw-r--r--   0        0        0    12609 2024-05-23 11:56:31.260417 oldaplib-0.1.1/oldaplib/src/helpers/tools.py
+-rw-r--r--   0        0        0     2430 2024-05-23 11:56:31.260472 oldaplib-0.1.1/oldaplib/src/iconnection.py
+-rw-r--r--   0        0        0     7590 2024-05-23 11:56:31.260560 oldaplib-0.1.1/oldaplib/src/in_project.py
+-rw-r--r--   0        0        0     3036 2024-05-23 11:56:31.260619 oldaplib-0.1.1/oldaplib/src/model.py
+-rw-r--r--   0        0        0    21622 2024-05-23 11:56:31.260692 oldaplib-0.1.1/oldaplib/src/oldaplist.py
+-rw-r--r--   0        0        0     2372 2024-05-23 11:56:31.260765 oldaplib-0.1.1/oldaplib/src/oldaplistnode.py
+-rw-r--r--   0        0        0    26674 2024-05-27 10:00:42.847139 oldaplib-0.1.1/oldaplib/src/permissionset.py
+-rw-r--r--   0        0        0    33455 2024-05-27 09:38:24.231422 oldaplib-0.1.1/oldaplib/src/project.py
+-rw-r--r--   0        0        0    58711 2024-05-23 11:56:31.261172 oldaplib-0.1.1/oldaplib/src/propertyclass.py
+-rw-r--r--   0        0        0    54918 2024-05-24 14:34:53.000228 oldaplib-0.1.1/oldaplib/src/resourceclass.py
+-rw-r--r--   0        0        0    26641 2024-05-23 11:56:31.261476 oldaplib-0.1.1/oldaplib/src/user.py
+-rw-r--r--   0        0        0    30434 2024-05-23 11:56:31.261602 oldaplib-0.1.1/oldaplib/src/user_dataclass.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:56:31.261661 oldaplib-0.1.1/oldaplib/src/xsd/__init__.py
+-rw-r--r--   0        0        0     7896 2024-05-23 11:56:31.261736 oldaplib-0.1.1/oldaplib/src/xsd/floatingpoint.py
+-rw-r--r--   0        0        0     4821 2024-05-27 09:21:13.278986 oldaplib-0.1.1/oldaplib/src/xsd/iri.py
+-rw-r--r--   0        0        0     1499 2024-05-23 11:56:31.261866 oldaplib-0.1.1/oldaplib/src/xsd/xsd.py
+-rw-r--r--   0        0        0     5523 2024-05-23 11:56:31.261950 oldaplib-0.1.1/oldaplib/src/xsd/xsd_anyuri.py
+-rw-r--r--   0        0        0     3543 2024-05-23 11:56:31.262011 oldaplib-0.1.1/oldaplib/src/xsd/xsd_base64binary.py
+-rw-r--r--   0        0        0     2648 2024-05-23 11:56:31.262080 oldaplib-0.1.1/oldaplib/src/xsd/xsd_boolean.py
+-rw-r--r--   0        0        0      979 2024-05-23 11:56:31.262144 oldaplib-0.1.1/oldaplib/src/xsd/xsd_byte.py
+-rw-r--r--   0        0        0     7043 2024-05-23 11:56:31.262209 oldaplib-0.1.1/oldaplib/src/xsd/xsd_date.py
+-rw-r--r--   0        0        0     3972 2024-05-23 11:56:31.262273 oldaplib-0.1.1/oldaplib/src/xsd/xsd_datetime.py
+-rw-r--r--   0        0        0     3904 2024-05-23 11:56:31.262327 oldaplib-0.1.1/oldaplib/src/xsd/xsd_datetimestamp.py
+-rw-r--r--   0        0        0     1376 2024-05-23 11:56:31.262397 oldaplib-0.1.1/oldaplib/src/xsd/xsd_decimal.py
+-rw-r--r--   0        0        0     1422 2024-05-23 11:56:31.262464 oldaplib-0.1.1/oldaplib/src/xsd/xsd_double.py
+-rw-r--r--   0        0        0     3319 2024-05-23 11:56:31.262551 oldaplib-0.1.1/oldaplib/src/xsd/xsd_duration.py
+-rw-r--r--   0        0        0     1242 2024-05-23 11:56:31.262608 oldaplib-0.1.1/oldaplib/src/xsd/xsd_float.py
+-rw-r--r--   0        0        0     3517 2024-05-23 11:56:31.262699 oldaplib-0.1.1/oldaplib/src/xsd/xsd_gday.py
+-rw-r--r--   0        0        0     3628 2024-05-23 11:56:31.262764 oldaplib-0.1.1/oldaplib/src/xsd/xsd_gmonth.py
+-rw-r--r--   0        0        0     3840 2024-05-23 11:56:31.262812 oldaplib-0.1.1/oldaplib/src/xsd/xsd_gmonthday.py
+-rw-r--r--   0        0        0     3780 2024-05-23 11:56:31.262865 oldaplib-0.1.1/oldaplib/src/xsd/xsd_gyear.py
+-rw-r--r--   0        0        0     4186 2024-05-23 11:56:31.262917 oldaplib-0.1.1/oldaplib/src/xsd/xsd_gyearmonth.py
+-rw-r--r--   0        0        0     3073 2024-05-23 11:56:31.262961 oldaplib-0.1.1/oldaplib/src/xsd/xsd_hexbinary.py
+-rw-r--r--   0        0        0      617 2024-05-23 11:56:31.263024 oldaplib-0.1.1/oldaplib/src/xsd/xsd_id.py
+-rw-r--r--   0        0        0      647 2024-05-23 11:56:31.263071 oldaplib-0.1.1/oldaplib/src/xsd/xsd_idref.py
+-rw-r--r--   0        0        0     1123 2024-05-23 11:56:31.263135 oldaplib-0.1.1/oldaplib/src/xsd/xsd_int.py
+-rw-r--r--   0        0        0     5727 2024-05-23 11:56:31.263215 oldaplib-0.1.1/oldaplib/src/xsd/xsd_integer.py
+-rw-r--r--   0        0        0     3504 2024-05-23 11:56:31.263300 oldaplib-0.1.1/oldaplib/src/xsd/xsd_language.py
+-rw-r--r--   0        0        0     1179 2024-05-23 11:56:31.263349 oldaplib-0.1.1/oldaplib/src/xsd/xsd_long.py
+-rw-r--r--   0        0        0     3436 2024-05-23 11:56:31.263398 oldaplib-0.1.1/oldaplib/src/xsd/xsd_name.py
+-rw-r--r--   0        0        0     5067 2024-05-27 09:21:13.279188 oldaplib-0.1.1/oldaplib/src/xsd/xsd_ncname.py
+-rw-r--r--   0        0        0      999 2024-05-23 11:56:31.263547 oldaplib-0.1.1/oldaplib/src/xsd/xsd_negativeinteger.py
+-rw-r--r--   0        0        0     3298 2024-05-23 11:56:31.263655 oldaplib-0.1.1/oldaplib/src/xsd/xsd_nmtoken.py
+-rw-r--r--   0        0        0     1043 2024-05-23 11:56:31.263719 oldaplib-0.1.1/oldaplib/src/xsd/xsd_nonnegativeinteger.py
+-rw-r--r--   0        0        0      964 2024-05-23 11:56:31.263775 oldaplib-0.1.1/oldaplib/src/xsd/xsd_nonpositiveinteger.py
+-rw-r--r--   0        0        0     3967 2024-05-23 11:56:31.263836 oldaplib-0.1.1/oldaplib/src/xsd/xsd_normalizedstring.py
+-rw-r--r--   0        0        0      945 2024-05-23 11:56:31.263884 oldaplib-0.1.1/oldaplib/src/xsd/xsd_positiveinteger.py
+-rw-r--r--   0        0        0     6750 2024-05-23 11:56:31.263935 oldaplib-0.1.1/oldaplib/src/xsd/xsd_qname.py
+-rw-r--r--   0        0        0      989 2024-05-23 11:56:31.263979 oldaplib-0.1.1/oldaplib/src/xsd/xsd_short.py
+-rw-r--r--   0        0        0     9512 2024-05-23 11:56:31.264056 oldaplib-0.1.1/oldaplib/src/xsd/xsd_string.py
+-rw-r--r--   0        0        0     3670 2024-05-23 11:56:31.264116 oldaplib-0.1.1/oldaplib/src/xsd/xsd_time.py
+-rw-r--r--   0        0        0     3546 2024-05-23 11:56:31.264193 oldaplib-0.1.1/oldaplib/src/xsd/xsd_token.py
+-rw-r--r--   0        0        0     1027 2024-05-23 11:56:31.264245 oldaplib-0.1.1/oldaplib/src/xsd/xsd_unsignedbyte.py
+-rw-r--r--   0        0        0     1040 2024-05-23 11:56:31.264294 oldaplib-0.1.1/oldaplib/src/xsd/xsd_unsignedint.py
+-rw-r--r--   0        0        0     1007 2024-05-23 11:56:31.264350 oldaplib-0.1.1/oldaplib/src/xsd/xsd_unsignedlong.py
+-rw-r--r--   0        0        0     1012 2024-05-23 11:56:31.264403 oldaplib-0.1.1/oldaplib/src/xsd/xsd_unsignedshort.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:56:31.264460 oldaplib-0.1.1/oldaplib/test/__init__.py
+-rw-r--r--   0        0        0    14309 2024-05-24 14:40:43.315846 oldaplib-0.1.1/oldaplib/test/gaga.trig
+-rw-r--r--   0        0        0     1759 2024-05-23 11:56:31.264648 oldaplib-0.1.1/oldaplib/test/propclass_test.trig
+-rw-r--r--   0        0        0    13591 2024-05-27 09:21:13.279380 oldaplib-0.1.1/oldaplib/test/test_connection.py
+-rw-r--r--   0        0        0     4777 2024-05-27 09:21:13.279588 oldaplib-0.1.1/oldaplib/test/test_context.py
+-rw-r--r--   0        0        0    21746 2024-05-24 14:27:35.161430 oldaplib-0.1.1/oldaplib/test/test_datamodel.py
+-rw-r--r--   0        0        0     8221 2024-05-23 11:56:31.265040 oldaplib-0.1.1/oldaplib/test/test_dtypes.py
+-rw-r--r--   0        0        0     7774 2024-05-23 11:56:31.265129 oldaplib-0.1.1/oldaplib/test/test_in_project.py
+-rw-r--r--   0        0        0    11628 2024-05-23 11:56:31.265227 oldaplib-0.1.1/oldaplib/test/test_langstring.py
+-rw-r--r--   0        0        0     8826 2024-05-23 11:56:31.265313 oldaplib-0.1.1/oldaplib/test/test_language_in.py
+-rw-r--r--   0        0        0     3645 2024-05-23 11:56:31.265401 oldaplib-0.1.1/oldaplib/test/test_objectfactory.py
+-rw-r--r--   0        0        0     6249 2024-05-23 11:56:31.265480 oldaplib-0.1.1/oldaplib/test/test_observable_set.py
+-rw-r--r--   0        0        0     7288 2024-05-23 11:56:31.265575 oldaplib-0.1.1/oldaplib/test/test_oldaplist.py
+-rw-r--r--   0        0        0    14077 2024-05-27 09:46:09.360871 oldaplib-0.1.1/oldaplib/test/test_permissionset.py
+-rw-r--r--   0        0        0    17012 2024-05-27 09:41:09.937612 oldaplib-0.1.1/oldaplib/test/test_project.py
+-rw-r--r--   0        0        0    28492 2024-05-23 11:56:31.265836 oldaplib-0.1.1/oldaplib/test/test_propertyclass.py
+-rw-r--r--   0        0        0    42274 2024-05-24 15:06:32.867260 oldaplib-0.1.1/oldaplib/test/test_resourceclass.py
+-rw-r--r--   0        0        0     3392 2024-05-23 11:56:31.266067 oldaplib-0.1.1/oldaplib/test/test_semantic_version.py
+-rw-r--r--   0        0        0    40179 2024-05-27 09:21:13.280005 oldaplib-0.1.1/oldaplib/test/test_user.py
+-rw-r--r--   0        0        0    64182 2024-05-23 11:56:31.266246 oldaplib-0.1.1/oldaplib/test/test_xsd_datatypes.py
+-rw-r--r--   0        0        0    12312 2024-05-23 11:56:31.266363 oldaplib-0.1.1/oldaplib/testdata/connection_test.trig
+-rw-r--r--   0        0        0     1382 2024-05-23 11:56:31.266459 oldaplib-0.1.1/oldaplib/testdata/datamodel_test.trig
+-rw-r--r--   0        0        0    14936 2024-05-24 14:52:30.959752 oldaplib-0.1.1/oldaplib/testdata/objectfactory_test.trig
+-rw-r--r--   0        0        0      303 2024-05-23 11:56:31.266619 oldaplib-0.1.1/oldaplib/testit.http
+-rw-r--r--   0        0        0      914 2024-05-27 10:01:02.826592 oldaplib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 oldaplib-0.1.1/PKG-INFO
```

### Comparing `oldaplib-0.1.0/README.md` & `oldaplib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/ontologies/admin.trig` & `oldaplib-0.1.1/oldaplib/ontologies/admin.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/ontologies/oldap.shacl.trig` & `oldaplib-0.1.1/oldaplib/ontologies/oldap.shacl.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/ontologies/oldap.ttl` & `oldaplib-0.1.1/oldaplib/ontologies/oldap.ttl`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/ObjectFactory.py` & `oldaplib-0.1.1/oldaplib/src/ObjectFactory.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/connection.py` & `oldaplib-0.1.1/oldaplib/src/connection.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/datamodel.py` & `oldaplib-0.1.1/oldaplib/src/datamodel.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/dtypes/bnode.py` & `oldaplib-0.1.1/oldaplib/src/dtypes/bnode.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/dtypes/languagein.py` & `oldaplib-0.1.1/oldaplib/src/dtypes/languagein.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/dtypes/namespaceiri.py` & `oldaplib-0.1.1/oldaplib/src/dtypes/namespaceiri.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/dtypes/rdfset.py` & `oldaplib-0.1.1/oldaplib/src/dtypes/rdfset.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/dtypes/xsdset.py` & `oldaplib-0.1.1/oldaplib/src/dtypes/xsdset.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/enums/action.py` & `oldaplib-0.1.1/oldaplib/src/enums/action.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/enums/language.py` & `oldaplib-0.1.1/oldaplib/src/enums/language.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/enums/permissions.py` & `oldaplib-0.1.1/oldaplib/src/enums/permissions.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/enums/propertyclassattr.py` & `oldaplib-0.1.1/oldaplib/src/enums/propertyclassattr.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/enums/sparql_result_format.py` & `oldaplib-0.1.1/oldaplib/src/enums/sparql_result_format.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/enums/userdataclassattr.py` & `oldaplib-0.1.1/oldaplib/src/enums/userdataclassattr.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/enums/xsd_datatypes.py` & `oldaplib-0.1.1/oldaplib/src/enums/xsd_datatypes.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/Notify.py` & `oldaplib-0.1.1/oldaplib/src/helpers/Notify.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/context.py` & `oldaplib-0.1.1/oldaplib/src/helpers/context.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/langstring.py` & `oldaplib-0.1.1/oldaplib/src/helpers/langstring.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/observable_dict.py` & `oldaplib-0.1.1/oldaplib/src/helpers/observable_dict.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/observable_set.py` & `oldaplib-0.1.1/oldaplib/src/helpers/observable_set.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/oldaperror.py` & `oldaplib-0.1.1/oldaplib/src/helpers/oldaperror.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/propertyclass_singleton.py` & `oldaplib-0.1.1/oldaplib/src/helpers/propertyclass_singleton.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/query_processor.py` & `oldaplib-0.1.1/oldaplib/src/helpers/query_processor.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/semantic_version.py` & `oldaplib-0.1.1/oldaplib/src/helpers/semantic_version.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/serializer.py` & `oldaplib-0.1.1/oldaplib/src/helpers/serializer.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/helpers/tools.py` & `oldaplib-0.1.1/oldaplib/src/helpers/tools.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/iconnection.py` & `oldaplib-0.1.1/oldaplib/src/iconnection.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/in_project.py` & `oldaplib-0.1.1/oldaplib/src/in_project.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/model.py` & `oldaplib-0.1.1/oldaplib/src/model.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/oldaplist.py` & `oldaplib-0.1.1/oldaplib/src/oldaplist.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/oldaplistnode.py` & `oldaplib-0.1.1/oldaplib/src/oldaplistnode.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/permissionset.py` & `oldaplib-0.1.1/oldaplib/src/permissionset.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,52 +61,83 @@
                  created: Xsd_dateTime | datetime | str | None = None,
                  contributor: Iri | None = None,
                  modified: Xsd_dateTime | datetime | str | None = None,
                  id: Xsd_NCName | str,
                  label: LangString | str | None = None,
                  comment: LangString | str | None = None,
                  givesPermission: DataPermission,
-                 definedByProject: Iri):
+                 definedByProject: Iri | Xsd_NCName):
+        """
+        Constructor for a permission set.
+        :param con: Subclass of IConnection
+        :type con: IConnection
+        :param creator: Usually not being used (internal use only)
+        :type creator: Iri | None
+        :param created: Usually not being used (internal use only)
+        :type created: Xsd_dateTime | datetime | str | None
+        :param contributor: Usually not being used (internal use only)
+        :type contributor: Iri | None
+        :param modified: Usually not being used (internal use only)
+        :type modified: Xsd_dateTime | datetime | str | None
+        :param id: A unique identifier for the permission set (unique within the project as given be :definedByProject)
+        :type id: Xsd_NCName | str
+        :param label: A meaninful label for the permission set (several languages allowed)
+        :type label: LangString | str
+        :param comment: A meaningful comment for the permission set (several languages allowed)
+        :type comment: LangString | str
+        :param givesPermission: The permission that this permision set grants
+        :type givesPermission: DataPermission
+        :param definedByProject: The project that defines this permission set (either the IRI or the shortname)
+        :type definedByProject: Iri | Xsd_NCName
+        :raises OldapErrorNoFound: Given project does not exist
+        """
         super().__init__(con)
         self.__creator = Iri(creator) if creator else con.userIri
         self.__created = Xsd_dateTime(created) if created else None
         self.__contributor = Iri(contributor) if contributor else con.userIri
         self.__modified = Xsd_dateTime(modified) if modified else None
         self.__attributes = {}
 
         self.__attributes[PermissionSetAttr.ID] = Xsd_NCName(id)
         self.__attributes[PermissionSetAttr.LABEL] = LangString(label)
         self.__attributes[PermissionSetAttr.LABEL].set_notifier(self.notifier, PermissionSetAttr.LABEL)
         self.__attributes[PermissionSetAttr.COMMENT] = LangString(comment)
         self.__attributes[PermissionSetAttr.COMMENT].set_notifier(self.notifier, PermissionSetAttr.COMMENT)
         self.__attributes[PermissionSetAttr.GIVES_PERMISSION] = givesPermission
-        self.__attributes[PermissionSetAttr.DEFINED_BY_PROJECT] = Iri(definedByProject)
+        #
+        # get the project IRI
+        #
+        project = Project.read(self._con, definedByProject)
+        self.__attributes[PermissionSetAttr.DEFINED_BY_PROJECT] = project.projectIri
 
         if not self.__attributes[PermissionSetAttr.ID]:
             raise OldapErrorInconsistency(f'PermissionSet must have a unique ID, none given.')
         if not self.__attributes[PermissionSetAttr.LABEL]:
             raise OldapErrorInconsistency(f'PermissionSet must have at least one rdfs:label, none given.')
         if not self.__attributes[PermissionSetAttr.GIVES_PERMISSION]:
             raise OldapErrorInconsistency(f'PermissionSet must have at least one oldap:givesPermission, none given.')
         if not self.__attributes[PermissionSetAttr.DEFINED_BY_PROJECT]:
             raise OldapErrorInconsistency(f'PermissionSet must have at least one oldap:definedByProject, none given.')
 
         project = Project.read(self._con, self.__attributes[PermissionSetAttr.DEFINED_BY_PROJECT])
         self.__permset_iri = Iri.fromPrefixFragment(project.projectShortName, self.__attributes[PermissionSetAttr.ID], validate=False)
 
-
         for field in PermissionSetAttr:
             prefix, name = field.value.split(':')
             setattr(PermissionSet, name, property(
                 partial(self.__get_value, field=field),
                 partial(self.__set_value, field=field),
                 partial(self.__del_value, field=field)))
         self.__changeset = {}
 
     def check_for_permissions(self) -> (bool, str):
+        """
+        Internal method to check if a user may modify the permission set.
+        :return: a tuple with a boolean (True, False) and the error message (or "OK")
+        """
         #
         # First we check if the logged-in user ("actor") has the ADMIN_PERMISSION_SETS permission for
         # the given project!
         #
         actor = self._con.userdata
         sysperms = actor.inProject.get(Iri('oldap:SystemProject'))
         if sysperms and AdminPermission.ADMIN_OLDAP in sysperms:
@@ -218,14 +249,22 @@
         """
         Clear the changeset.
         :return: None
         """
         self.__changeset = {}
 
     def create(self, indent: int = 0, indent_inc: int = 4) -> None:
+        """
+        Create the given permission set in the triple store.
+        :param indent: indentation for SPARQL text
+        :type indent: int
+        :param indent_inc: indentation increment for the SPARQL text
+        :type indent_inc: int
+        :return: None
+        """
         if self._con is None:
             raise OldapError("Cannot create: no connection")
 
         result, message = self.check_for_permissions()
         if not result:
             raise OldapErrorNoPermission(message)
 
@@ -284,15 +323,28 @@
             raise
         self.__created = timestamp
         self.__creator = self._con.userIri
         self.__modified = timestamp
         self.__contributor = self._con.userIri
 
     @classmethod
-    def read(cls, con: IConnection, id: Xsd_NCName | str, definedByProject: Iri | str) -> Self:
+    def read(cls, con: IConnection, id: Xsd_NCName | str, definedByProject: Iri | Xsd_NCName | str) -> Self:
+        """
+        Reads a given permission set. The permission set is defined by its ID (which must be unique within
+        one project) and the project IRI.
+        :param con: A Connection object.
+        :type con: IConnection
+        :param id: The ID of the permission set.
+        :type id: Xsd_NCName | str
+        :param definedByProject: Iri or the shortname of the project
+        :type definedByProject: Iri | Xsd_NCName | str
+        :return: A PermissionSet instance
+        :rtype: OldapPermissionSet
+        :raises OldapErrorNot found: If the permission set cannot be found.
+        """
         id = Xsd_NCName(id)
         definedByProject = Iri(definedByProject)
 
         project = Project.read(con, definedByProject)
         permset_iri = Iri.fromPrefixFragment(project.projectShortName, id, validate=False)
         context = Context(name=con.context_name)
         sparql = context.sparql_context
@@ -355,15 +407,31 @@
                    definedByProject=Iri(definedByProject, validate=False))
 
     @staticmethod
     def search(con: IConnection, *,
                id: str | None = None,
                definedByProject: Iri | str | None = None,
                givesPermission: DataPermission | None = None,
-               label: Xsd_string | str | None = None) -> list[Iri]:
+               label: Xsd_string | str | None = None) -> list[Iri | Xsd_QName]:
+        """
+        Search for a permission set. At least one of the search criteria is required. Multiple search criteria are
+        combined using a logical AND.
+        :param con: A valid Connection object.
+        :type con: IConnection
+        :param id: Search for the given ID. The given string must be _contained_ in the ID (substring)
+        :type id: str | None
+        :param definedByProject: The project which is responsible for the permission set
+        :type definedByProject: str | None
+        :param givesPermission: The permission that the permission set should grant
+        :type givesPermission: str | None
+        :param label: The label string. The given string must be within at least one language label.
+        :type label: str | None
+        :return: A list or permission set Iri's (possibly as Xsd_QName
+        :rtype: list[Iri | Xsd_QName]
+        """
         if definedByProject:
             definedByProject = Iri(definedByProject)
         label = Xsd_string(label)
         context = Context(name=con.context_name)
         sparql = context.sparql_context
         if definedByProject:
             sparql += 'SELECT DISTINCT ?permsetIri ?namespaceIri ?projectShortName'
@@ -415,15 +483,25 @@
                 #context[r['projectShortName']] = r['namespaceIri']
                 psqname = r['permsetIri'].as_qname or context.iri2qname(str(r['permsetIri']), validate=False)
                 permissionSets.append(psqname or r['permsetIri'])
             else:
                 permissionSets.append(r['permsetIri'])
         return permissionSets
 
-    def update(self, indent: int = 0, indent_inc: int = 4):
+    def update(self, indent: int = 0, indent_inc: int = 4) -> None:
+        """
+        Update a changed permission set
+        :param indent: Internal use (indent of SPARQL text)
+        :type indent: int
+        :param indent_inc: Internal use (indent increment of SPARQL text)
+        :type indent_inc: int
+        :return: None
+        :rtype: None
+        :raises OldapErrorUpdateFailed: Update failed
+        """
         result, message = self.check_for_permissions()
         if not result:
             raise OldapErrorNoPermission(message)
         timestamp = Xsd_dateTime.now()
         context = Context(name=self._con.context_name)
         blank = ''
         sparql_list = []
@@ -480,14 +558,19 @@
         except OldapError:
             self._con.transaction_abort()
             raise
         self.__modified = timestamp
         self.__contributor = self._con.userIri  # TODO: move creator, created etc. to Model!
 
     def delete(self) -> None:
+        """
+        Delete the given permission set.
+        :return: None
+        :rtype: None
+        """
         result, message = self.check_for_permissions()
         if not result:
             raise OldapErrorNoPermission(message)
 
         context = Context(name=self._con.context_name)
         sparql = context.sparql_context
         sparql += f"""
```

### Comparing `oldaplib-0.1.0/oldaplib/src/project.py` & `oldaplib-0.1.1/oldaplib/src/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,16 +381,16 @@
 
     @classmethod
     def read(cls, con: IConnection, projectIri_SName: Iri | Xsd_NCName | str) -> Self:
         """
         Read the project from the triplestore and return an instance of the project
         :param con: A valid Connection object
         :type con: IConnection
-        :param projectIri: The IRI/QName of the project to be read
-        :type projectIri: Xsd_anyURI | Xsd_QName
+        :param projectIri_SName: The IRI or shortname of the project to be read
+        :type projectIri_SName: Iri | Xsd_NCName | str
         :return: Project instance
         :rtype: Project
         :raise: OldapErrorNotFound: project with given Iri not found
         :raise: OldapError: All other errors/problems
         """
         context = Context(name=con.context_name)
         query = context.sparql_context
```

### Comparing `oldaplib-0.1.0/oldaplib/src/propertyclass.py` & `oldaplib-0.1.1/oldaplib/src/propertyclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/resourceclass.py` & `oldaplib-0.1.1/oldaplib/src/resourceclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/user.py` & `oldaplib-0.1.1/oldaplib/src/user.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/user_dataclass.py` & `oldaplib-0.1.1/oldaplib/src/user_dataclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/floatingpoint.py` & `oldaplib-0.1.1/oldaplib/src/xsd/floatingpoint.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/iri.py` & `oldaplib-0.1.1/oldaplib/src/xsd/iri.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_anyuri.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_anyuri.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_base64binary.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_base64binary.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_boolean.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_boolean.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_byte.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_byte.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_date.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_date.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_datetime.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_datetime.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_datetimestamp.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_datetimestamp.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_decimal.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_decimal.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_double.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_double.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_duration.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_duration.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_float.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_float.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_gday.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_gday.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_gmonth.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_gmonth.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_gmonthday.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_gmonthday.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_gyear.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_gyear.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_gyearmonth.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_gyearmonth.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_hexbinary.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_hexbinary.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_id.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_id.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_idref.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_idref.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_int.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_int.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_integer.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_integer.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_language.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_language.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_long.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_long.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_name.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_name.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_ncname.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_ncname.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_negativeinteger.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_negativeinteger.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_nmtoken.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_nmtoken.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_nonnegativeinteger.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_nonnegativeinteger.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_nonpositiveinteger.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_nonpositiveinteger.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_normalizedstring.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_normalizedstring.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_positiveinteger.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_positiveinteger.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_qname.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_qname.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_short.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_short.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_string.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_string.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_time.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_time.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_token.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_token.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_unsignedbyte.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_unsignedbyte.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_unsignedint.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_unsignedint.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_unsignedlong.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_unsignedlong.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/src/xsd/xsd_unsignedshort.py` & `oldaplib-0.1.1/oldaplib/src/xsd/xsd_unsignedshort.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/gaga.trig` & `oldaplib-0.1.1/oldaplib/test/gaga.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/propclass_test.trig` & `oldaplib-0.1.1/oldaplib/test/propclass_test.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_connection.py` & `oldaplib-0.1.1/oldaplib/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_context.py` & `oldaplib-0.1.1/oldaplib/test/test_context.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_datamodel.py` & `oldaplib-0.1.1/oldaplib/test/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_dtypes.py` & `oldaplib-0.1.1/oldaplib/test/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_in_project.py` & `oldaplib-0.1.1/oldaplib/test/test_in_project.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_langstring.py` & `oldaplib-0.1.1/oldaplib/test/test_langstring.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_language_in.py` & `oldaplib-0.1.1/oldaplib/test/test_language_in.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_objectfactory.py` & `oldaplib-0.1.1/oldaplib/test/test_objectfactory.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_observable_set.py` & `oldaplib-0.1.1/oldaplib/test/test_observable_set.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_oldaplist.py` & `oldaplib-0.1.1/oldaplib/test/test_oldaplist.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_permissionset.py` & `oldaplib-0.1.1/oldaplib/test/test_permissionset.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         with self.assertRaises(OldapErrorInconsistency):
             ps = PermissionSet(con=self._connection,
                                id="test2_ps",
                                comment=LangString("Testing a PermissionSet@en", "Test eines PermissionSet@Perm@de"),
                                givesPermission=DataPermission.DATA_UPDATE,
                                definedByProject=Iri('oldap:SystemProject'))
 
+    def test_create_permissionset(self):
         ps = PermissionSet(con=self._connection,
                            id="test3_ps",
                            label=LangString("\";SELECT * { password ?p ?o . }@en", "test@Perm@de"),
                            comment=LangString("Testing a PermissionSet@en", "Test eines PermissionSet@Perm@de"),
                            givesPermission=DataPermission.DATA_UPDATE,
                            definedByProject=Iri('oldap:SystemProject'))
         ps.create()
@@ -93,14 +94,25 @@
         del ps
         ps = PermissionSet.read(self._connection, "test3_ps", Iri('oldap:SystemProject'))
         self.assertEqual(ps.givesPermission, DataPermission.DATA_UPDATE)
         self.assertEqual(ps.label, LangString("\";SELECT * { password ?p ?o . }@en", "test@Perm@de"))
         self.assertEqual(ps.comment, LangString("Testing a PermissionSet@en", "Test eines PermissionSet@Perm@de"))
         self.assertEqual(ps.definedByProject, Iri('oldap:SystemProject'))
 
+    def test_create_permset_with_shortname(self):
+        ps = PermissionSet(con=self._connection,
+                           id="test4_ps",
+                           label=LangString("test4@en", "test4@Perm@de"),
+                           comment=LangString("Testing a PermissionSet 4@en", "Test eines PermissionSet 4@Perm@de"),
+                           givesPermission=DataPermission.DATA_UPDATE,
+                           definedByProject='britnet')
+        ps.create()
+        ps = PermissionSet.read(self._connection, "test4_ps", Iri('http://www.salsah.org/version/2.0/SwissBritNet'))
+        self.assertEqual(ps.givesPermission, DataPermission.DATA_UPDATE)
+        self.assertEqual(ps.label, LangString("test4@en", "test4@Perm@de"))
 
     # @unittest.skip('Work in progress')
     def test_read_permission_A(self):
         ps = PermissionSet.read(self._connection, 'GenericView', 'oldap:SystemProject')
         self.assertEqual(ps.givesPermission, DataPermission.DATA_VIEW)  # add assertion here
         self.assertEqual(ps.label, LangString("GenericView@en", "GenericView@de", "GenericView@fr", "GenericView@it"))
         self.assertEqual(ps.definedByProject, Iri('oldap:SystemProject'))
```

### Comparing `oldaplib-0.1.0/oldaplib/test/test_project.py` & `oldaplib-0.1.1/oldaplib/test/test_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,17 @@
         self.assertEqual(NamespaceIRI("http://oldap.org/base#"), project.namespaceIri)
         self.assertEqual(LangString(["Project for system administration@en"]), project.comment)
         self.assertEqual(Xsd_date("2024-01-01"), project.projectStart)
 
         project = Project.read(con=self._connection, projectIri_SName='http://www.salsah.org/version/2.0/SwissBritNet')
         self.assertEqual(Xsd_NCName("britnet"), project.projectShortName)
 
-        project2 = Project.read(con=self._connection, projectIri_SName='hyha')
-        self.assertEqual(Xsd_NCName("hyha"), project2.projectShortName)
+        project2 = Project.read(con=self._connection, projectIri_SName='britnet')
+        self.assertEqual(Xsd_NCName("britnet"), project2.projectShortName)
+        self.assertEqual(Iri('http://www.salsah.org/version/2.0/SwissBritNet'), project2.projectIri)
 
     # @unittest.skip('Work in progress')
     def test_project_search(self):
         projects = Project.search(con=self._connection, label="HyperHamlet")
         self.assertEqual(["oldap:HyperHamlet"], projects)
 
     # @unittest.skip('Work in progress')
```

### Comparing `oldaplib-0.1.0/oldaplib/test/test_propertyclass.py` & `oldaplib-0.1.1/oldaplib/test/test_propertyclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_resourceclass.py` & `oldaplib-0.1.1/oldaplib/test/test_resourceclass.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_semantic_version.py` & `oldaplib-0.1.1/oldaplib/test/test_semantic_version.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_user.py` & `oldaplib-0.1.1/oldaplib/test/test_user.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/test/test_xsd_datatypes.py` & `oldaplib-0.1.1/oldaplib/test/test_xsd_datatypes.py`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/testdata/connection_test.trig` & `oldaplib-0.1.1/oldaplib/testdata/connection_test.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/testdata/datamodel_test.trig` & `oldaplib-0.1.1/oldaplib/testdata/datamodel_test.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/oldaplib/testdata/objectfactory_test.trig` & `oldaplib-0.1.1/oldaplib/testdata/objectfactory_test.trig`

 * *Files identical despite different names*

### Comparing `oldaplib-0.1.0/pyproject.toml` & `oldaplib-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oldaplib"
-version = "0.1.0"
+version = "0.1.1"
 description = "Open Media Access Server Library (Linked Open Data middleware/RESTApi)"
 authors = ["Lukas Rosenthaler <lukas.rosenthaler@unibas.ch>"]
 license = "GNU Affero General Public License version 3"
 readme = "README.md"
 
 [tool.mkdocs]
 plugins = ["mkdocs-material", "mkdocstrings"]
```

### Comparing `oldaplib-0.1.0/PKG-INFO` & `oldaplib-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oldaplib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Open Media Access Server Library (Linked Open Data middleware/RESTApi)
 License: GNU Affero General Public License version 3
 Author: Lukas Rosenthaler
 Author-email: lukas.rosenthaler@unibas.ch
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

