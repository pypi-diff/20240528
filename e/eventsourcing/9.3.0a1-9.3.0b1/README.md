# Comparing `tmp/eventsourcing-9.3.0a1.tar.gz` & `tmp/eventsourcing-9.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventsourcing-9.3.0a1.tar", max compression
+gzip compressed data, was "eventsourcing-9.3.0b1.tar", max compression
```

## Comparing `eventsourcing-9.3.0a1.tar` & `eventsourcing-9.3.0b1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0     1512 2023-10-14 15:08:00.736877 eventsourcing-9.3.0a1/LICENSE
--rw-r--r--   0        0        0     8175 2023-10-14 15:08:00.737655 eventsourcing-9.3.0a1/README.md
--rw-r--r--   0        0        0       26 2024-01-21 08:06:33.073701 eventsourcing-9.3.0a1/eventsourcing/__init__.py
--rw-r--r--   0        0        0    36109 2024-02-07 14:52:49.762818 eventsourcing-9.3.0a1/eventsourcing/application.py
--rw-r--r--   0        0        0     3200 2024-01-22 10:29:20.695472 eventsourcing-9.3.0a1/eventsourcing/cipher.py
--rw-r--r--   0        0        0      421 2024-01-21 08:06:33.076171 eventsourcing-9.3.0a1/eventsourcing/compressor.py
--rw-r--r--   0        0        0     1412 2024-01-22 10:29:19.038585 eventsourcing-9.3.0a1/eventsourcing/dispatch.py
--rw-r--r--   0        0        0    57442 2024-02-07 14:53:47.034468 eventsourcing-9.3.0a1/eventsourcing/domain.py
--rw-r--r--   0        0        0        0 2021-10-08 09:03:42.583990 eventsourcing-9.3.0a1/eventsourcing/examples/__init__.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.010096 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate1/__init__.py
--rw-r--r--   0        0        0      766 2024-01-22 11:48:56.743973 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate1/application.py
--rw-r--r--   0        0        0      369 2024-01-22 11:48:56.744344 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate1/domainmodel.py
--rw-r--r--   0        0        0     1214 2024-01-21 08:06:33.078319 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate1/test_application.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.010835 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate2/__init__.py
--rw-r--r--   0        0        0      766 2024-01-22 11:48:56.745078 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate2/application.py
--rw-r--r--   0        0        0      484 2024-01-22 11:48:56.745366 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate2/domainmodel.py
--rw-r--r--   0        0        0     1214 2024-01-21 08:06:33.079244 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate2/test_application.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.011384 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate3/__init__.py
--rw-r--r--   0        0        0      780 2024-01-22 11:48:56.745926 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate3/application.py
--rw-r--r--   0        0        0     1013 2024-01-22 11:48:56.796648 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate3/domainmodel.py
--rw-r--r--   0        0        0     1214 2024-01-21 08:06:33.079690 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate3/test_application.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.011880 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate4/__init__.py
--rw-r--r--   0        0        0      825 2024-01-22 11:48:56.747118 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate4/application.py
--rw-r--r--   0        0        0     3601 2024-01-22 11:48:56.797003 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate4/domainmodel.py
--rw-r--r--   0        0        0     1306 2024-01-21 08:06:33.081330 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate4/test_application.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.012537 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate5/__init__.py
--rw-r--r--   0        0        0      842 2024-01-22 11:48:56.797333 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate5/application.py
--rw-r--r--   0        0        0     3637 2024-01-22 11:48:56.797656 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate5/domainmodel.py
--rw-r--r--   0        0        0     1306 2024-01-21 08:06:33.083631 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate5/test_application.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.013238 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6/__init__.py
--rw-r--r--   0        0        0      870 2024-01-22 11:48:56.749232 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6/application.py
--rw-r--r--   0        0        0     2876 2024-01-22 11:48:56.798003 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6/domainmodel.py
--rw-r--r--   0        0        0     1312 2024-01-21 08:06:33.084631 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6/test_application.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.013238 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6a/__init__.py
--rw-r--r--   0        0        0     1247 2024-02-07 14:53:47.472028 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6a/application.py
--rw-r--r--   0        0        0     3627 2024-02-07 15:29:28.031218 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6a/domainmodel.py
--rw-r--r--   0        0        0     1673 2024-02-07 14:55:52.609471 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6a/test_application.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.014003 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/__init__.py
--rw-r--r--   0        0        0     1395 2024-01-22 11:48:56.750419 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/application.py
--rw-r--r--   0        0        0     3261 2024-01-22 11:48:56.798355 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/domainmodel.py
--rw-r--r--   0        0        0     1874 2024-01-22 11:48:56.798675 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/persistence.py
--rw-r--r--   0        0        0     1366 2024-01-22 10:29:19.047196 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/test_application.py
--rw-r--r--   0        0        0     1634 2024-01-22 10:29:19.049488 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/test_compression_and_encryption.py
--rw-r--r--   0        0        0     2190 2024-01-22 11:48:56.799051 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/test_snapshotting_intervals.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.014003 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/__init__.py
--rw-r--r--   0        0        0     1748 2024-02-07 14:53:47.589167 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/application.py
--rw-r--r--   0        0        0     4016 2024-02-07 15:29:37.193222 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/domainmodel.py
--rw-r--r--   0        0        0     1741 2024-02-07 14:55:24.719559 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/test_application.py
--rw-r--r--   0        0        0     1636 2024-02-07 14:41:27.654454 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/test_compression_and_encryption.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.015249 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/__init__.py
--rw-r--r--   0        0        0     1357 2024-03-28 18:21:09.300220 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/application.py
--rw-r--r--   0        0        0     1276 2024-01-22 11:48:56.753304 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/domainmodel.py
--rw-r--r--   0        0        0     1874 2024-01-22 11:48:56.799412 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/persistence.py
--rw-r--r--   0        0        0     1268 2024-01-22 10:29:19.052955 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/test_application.py
--rw-r--r--   0        0        0     1509 2024-01-22 10:29:19.054150 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/test_compression_and_encryption.py
--rw-r--r--   0        0        0     1261 2024-01-22 11:48:56.799858 eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/test_snapshotting_intervals.py
--rw-r--r--   0        0        0        0 2021-10-08 09:03:42.584262 eventsourcing-9.3.0a1/eventsourcing/examples/bankaccounts/__init__.py
--rw-r--r--   0        0        0     2286 2024-01-22 10:29:20.704274 eventsourcing-9.3.0a1/eventsourcing/examples/bankaccounts/application.py
--rw-r--r--   0        0        0     1574 2024-01-21 08:06:33.089141 eventsourcing-9.3.0a1/eventsourcing/examples/bankaccounts/domainmodel.py
--rw-r--r--   0        0        0     5577 2024-01-21 08:06:33.089500 eventsourcing-9.3.0a1/eventsourcing/examples/bankaccounts/test.py
--rw-r--r--   0        0        0        0 2021-10-08 09:03:42.586411 eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/__init__.py
--rw-r--r--   0        0        0     3646 2024-01-22 11:48:56.800443 eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/application.py
--rw-r--r--   0        0        0     9638 2024-01-22 11:48:56.758544 eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/domainmodel.py
--rw-r--r--   0        0        0     4846 2024-01-22 11:48:56.801005 eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/interface.py
--rw-r--r--   0        0        0     9649 2024-01-21 08:06:33.091724 eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/test.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.017339 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/__init__.py
--rw-r--r--   0        0        0     3918 2024-01-22 11:48:56.759873 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/application.py
--rw-r--r--   0        0        0     1825 2024-01-22 10:29:19.058391 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/domainmodel.py
--rw-r--r--   0        0        0     6230 2024-01-22 10:29:19.058947 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/test.py
--rw-r--r--   0        0        0      745 2024-01-22 10:29:19.059398 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/utils.py
--rw-r--r--   0        0        0        0 2024-01-21 05:01:11.255037 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagementsystem/__init__.py
--rw-r--r--   0        0        0     1877 2024-03-28 20:26:46.150093 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagementsystem/application.py
--rw-r--r--   0        0        0      423 2024-01-21 23:58:53.728905 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagementsystem/postgres.py
--rw-r--r--   0        0        0      411 2024-01-21 23:58:53.729620 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagementsystem/sqlite.py
--rw-r--r--   0        0        0      444 2024-01-21 08:06:33.093493 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagementsystem/system.py
--rw-r--r--   0        0        0     7106 2024-01-22 11:48:56.761172 eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagementsystem/test_system.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.018121 eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/__init__.py
--rw-r--r--   0        0        0     1670 2024-01-22 11:48:56.802116 eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/application.py
--rw-r--r--   0        0        0      596 2024-01-22 11:48:56.802634 eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/persistence.py
--rw-r--r--   0        0        0     3831 2024-01-22 11:48:56.803255 eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/postgres.py
--rw-r--r--   0        0        0     4736 2024-01-22 11:48:56.804304 eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/sqlite.py
--rw-r--r--   0        0        0     3954 2024-01-22 11:48:56.763879 eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/test_application.py
--rw-r--r--   0        0        0     2312 2024-01-22 11:48:56.806173 eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/test_recorder.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.018996 eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/__init__.py
--rw-r--r--   0        0        0     1325 2024-01-22 11:48:56.807345 eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/application.py
--rw-r--r--   0        0        0      543 2024-01-22 10:29:20.709386 eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/persistence.py
--rw-r--r--   0        0        0     3857 2024-01-22 11:48:56.765009 eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/postgres.py
--rw-r--r--   0        0        0     3312 2024-01-22 11:48:56.765505 eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/sqlite.py
--rw-r--r--   0        0        0     3191 2024-01-22 11:48:56.766081 eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/test_searchabletimestamps.py
--rw-r--r--   0        0        0     4890 2024-01-22 11:48:56.807938 eventsourcing-9.3.0a1/eventsourcing/examples/test_invoice.py
--rw-r--r--   0        0        0     6682 2024-01-22 11:48:56.808455 eventsourcing-9.3.0a1/eventsourcing/examples/test_parking_lot.py
--rw-r--r--   0        0        0     4676 2024-03-28 20:26:46.257401 eventsourcing-9.3.0a1/eventsourcing/interface.py
--rw-r--r--   0        0        0    37672 2024-01-22 11:48:56.809678 eventsourcing-9.3.0a1/eventsourcing/persistence.py
--rw-r--r--   0        0        0     6547 2024-01-22 11:48:56.810266 eventsourcing-9.3.0a1/eventsourcing/popo.py
--rw-r--r--   0        0        0    29757 2024-03-28 20:19:45.581979 eventsourcing-9.3.0a1/eventsourcing/postgres.py
--rw-r--r--   0        0        0        0 2021-10-08 09:03:57.613590 eventsourcing-9.3.0a1/eventsourcing/py.typed
--rw-r--r--   0        0        0    18466 2024-01-22 11:48:56.811630 eventsourcing-9.3.0a1/eventsourcing/sqlite.py
--rw-r--r--   0        0        0    45298 2024-01-22 11:48:56.812428 eventsourcing-9.3.0a1/eventsourcing/system.py
--rw-r--r--   0        0        0        0 2021-10-08 09:03:42.596319 eventsourcing-9.3.0a1/eventsourcing/tests/__init__.py
--rw-r--r--   0        0        0    17586 2024-01-22 11:48:56.813100 eventsourcing-9.3.0a1/eventsourcing/tests/application.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.023033 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/__init__.py
--rw-r--r--   0        0        0     1956 2024-01-22 11:48:56.813721 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_application_with_automatic_snapshotting.py
--rw-r--r--   0        0        0      678 2022-04-28 12:08:57.023305 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_application_with_popo.py
--rw-r--r--   0        0        0     2431 2024-01-22 10:29:19.073249 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_application_with_postgres.py
--rw-r--r--   0        0        0     2059 2024-01-21 23:58:53.751746 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_application_with_sqlite.py
--rw-r--r--   0        0        0     3516 2022-04-28 12:08:57.023909 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_cache.py
--rw-r--r--   0        0        0     5438 2024-01-22 10:29:20.716602 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_event_sourced_log.py
--rw-r--r--   0        0        0     9194 2024-01-21 23:58:53.756001 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_notificationlog.py
--rw-r--r--   0        0        0     4298 2022-04-28 12:08:57.024438 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_notificationlogreader.py
--rw-r--r--   0        0        0     3744 2024-01-22 10:29:19.074691 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_processapplication.py
--rw-r--r--   0        0        0     3212 2024-01-22 10:29:19.075755 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_processingpolicy.py
--rw-r--r--   0        0        0    18873 2024-01-22 10:29:19.076416 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_repository.py
--rw-r--r--   0        0        0     2042 2022-04-28 12:08:57.025270 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_snapshotting.py
--rw-r--r--   0        0        0    14355 2024-01-22 10:29:19.077050 eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_upcasting.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.025633 eventsourcing-9.3.0a1/eventsourcing/tests/docs_tests/__init__.py
--rw-r--r--   0        0        0    10777 2024-01-22 10:29:19.077703 eventsourcing-9.3.0a1/eventsourcing/tests/docs_tests/test_docs.py
--rw-r--r--   0        0        0     3254 2024-01-22 10:29:19.078596 eventsourcing-9.3.0a1/eventsourcing/tests/domain.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.026202 eventsourcing-9.3.0a1/eventsourcing/tests/domain_tests/__init__.py
--rw-r--r--   0        0        0    37851 2024-01-22 10:29:19.079321 eventsourcing-9.3.0a1/eventsourcing/tests/domain_tests/test_aggregate.py
--rw-r--r--   0        0        0    50256 2024-01-22 10:29:20.717494 eventsourcing-9.3.0a1/eventsourcing/tests/domain_tests/test_aggregate_decorators.py
--rw-r--r--   0        0        0     2782 2024-01-22 10:29:19.080834 eventsourcing-9.3.0a1/eventsourcing/tests/domain_tests/test_domainevent.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.027156 eventsourcing-9.3.0a1/eventsourcing/tests/interface_tests/__init__.py
--rw-r--r--   0        0        0     9140 2024-03-28 20:26:46.473036 eventsourcing-9.3.0a1/eventsourcing/tests/interface_tests/test_remotenotificationlog.py
--rw-r--r--   0        0        0    45723 2024-01-22 11:48:56.815084 eventsourcing-9.3.0a1/eventsourcing/tests/persistence.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.027915 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/__init__.py
--rw-r--r--   0        0        0     2873 2022-04-28 12:08:57.028057 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_aes.py
--rw-r--r--   0        0        0    23641 2024-01-22 11:48:56.774665 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_connection_pool.py
--rw-r--r--   0        0        0     2261 2024-01-22 10:29:19.085478 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_eventstore.py
--rw-r--r--   0        0        0      730 2024-01-21 23:58:53.776667 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_infrastructure_factory.py
--rw-r--r--   0        0        0     3806 2024-01-21 23:58:53.777480 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_mapper.py
--rw-r--r--   0        0        0     2130 2024-01-21 23:58:53.777951 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_noninterleaving_notification_ids.py
--rw-r--r--   0        0        0     3366 2023-10-14 15:08:00.772836 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_popo.py
--rw-r--r--   0        0        0    40906 2024-03-28 19:56:57.846822 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_postgres.py
--rw-r--r--   0        0        0    11744 2024-01-22 10:29:20.718467 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_sqlite.py
--rw-r--r--   0        0        0     1251 2022-04-28 12:08:57.030988 eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_transcoder.py
--rw-r--r--   0        0        0     1364 2024-01-22 10:29:19.087031 eventsourcing-9.3.0a1/eventsourcing/tests/postgres_utils.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.031415 eventsourcing-9.3.0a1/eventsourcing/tests/system_tests/__init__.py
--rw-r--r--   0        0        0    31841 2024-03-28 20:26:46.792935 eventsourcing-9.3.0a1/eventsourcing/tests/system_tests/test_runner.py
--rw-r--r--   0        0        0     9552 2024-01-22 10:29:20.719393 eventsourcing-9.3.0a1/eventsourcing/tests/system_tests/test_system.py
--rw-r--r--   0        0        0        0 2022-04-28 12:08:57.032281 eventsourcing-9.3.0a1/eventsourcing/tests/utils_tests/__init__.py
--rw-r--r--   0        0        0     6486 2024-01-21 23:58:53.786521 eventsourcing-9.3.0a1/eventsourcing/tests/utils_tests/test_utils.py
--rw-r--r--   0        0        0     8247 2024-01-22 11:48:56.816547 eventsourcing-9.3.0a1/eventsourcing/utils.py
--rw-r--r--   0        0        0     6810 2024-03-28 20:50:07.176935 eventsourcing-9.3.0a1/pyproject.toml
--rw-r--r--   0        0        0     9891 1970-01-01 00:00:00.000000 eventsourcing-9.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-10-14 15:08:00.736877 eventsourcing-9.3.0b1/LICENSE
+-rw-r--r--   0        0        0     8175 2023-10-14 15:08:00.737655 eventsourcing-9.3.0b1/README.md
+-rw-r--r--   0        0        0       26 2024-01-21 08:06:33.073701 eventsourcing-9.3.0b1/eventsourcing/__init__.py
+-rw-r--r--   0        0        0    36109 2024-02-07 14:52:49.762818 eventsourcing-9.3.0b1/eventsourcing/application.py
+-rw-r--r--   0        0        0     3200 2024-01-22 10:29:20.695472 eventsourcing-9.3.0b1/eventsourcing/cipher.py
+-rw-r--r--   0        0        0      421 2024-01-21 08:06:33.076171 eventsourcing-9.3.0b1/eventsourcing/compressor.py
+-rw-r--r--   0        0        0     1412 2024-01-22 10:29:19.038585 eventsourcing-9.3.0b1/eventsourcing/dispatch.py
+-rw-r--r--   0        0        0    57264 2024-05-28 13:55:34.961881 eventsourcing-9.3.0b1/eventsourcing/domain.py
+-rw-r--r--   0        0        0        0 2021-10-08 09:03:42.583990 eventsourcing-9.3.0b1/eventsourcing/examples/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.010096 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate1/__init__.py
+-rw-r--r--   0        0        0      766 2024-01-22 11:48:56.743973 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate1/application.py
+-rw-r--r--   0        0        0      369 2024-01-22 11:48:56.744344 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate1/domainmodel.py
+-rw-r--r--   0        0        0     1214 2024-01-21 08:06:33.078319 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate1/test_application.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.010835 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate2/__init__.py
+-rw-r--r--   0        0        0      766 2024-01-22 11:48:56.745078 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate2/application.py
+-rw-r--r--   0        0        0      484 2024-01-22 11:48:56.745366 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate2/domainmodel.py
+-rw-r--r--   0        0        0     1214 2024-01-21 08:06:33.079244 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate2/test_application.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.011384 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate3/__init__.py
+-rw-r--r--   0        0        0      780 2024-01-22 11:48:56.745926 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate3/application.py
+-rw-r--r--   0        0        0     1013 2024-01-22 11:48:56.796648 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate3/domainmodel.py
+-rw-r--r--   0        0        0     1214 2024-01-21 08:06:33.079690 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate3/test_application.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.011880 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate4/__init__.py
+-rw-r--r--   0        0        0      825 2024-01-22 11:48:56.747118 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate4/application.py
+-rw-r--r--   0        0        0     3601 2024-01-22 11:48:56.797003 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate4/domainmodel.py
+-rw-r--r--   0        0        0     1306 2024-01-21 08:06:33.081330 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate4/test_application.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.012537 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate5/__init__.py
+-rw-r--r--   0        0        0      842 2024-01-22 11:48:56.797333 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate5/application.py
+-rw-r--r--   0        0        0     3637 2024-05-28 13:37:43.804489 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate5/domainmodel.py
+-rw-r--r--   0        0        0     1306 2024-01-21 08:06:33.083631 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate5/test_application.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.013238 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6/__init__.py
+-rw-r--r--   0        0        0      870 2024-01-22 11:48:56.749232 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6/application.py
+-rw-r--r--   0        0        0     2876 2024-05-28 13:55:36.227392 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6/domainmodel.py
+-rw-r--r--   0        0        0     1312 2024-01-21 08:06:33.084631 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6/test_application.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.013238 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6a/__init__.py
+-rw-r--r--   0        0        0     1247 2024-02-07 14:53:47.472028 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6a/application.py
+-rw-r--r--   0        0        0     3627 2024-05-28 13:55:36.227791 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6a/domainmodel.py
+-rw-r--r--   0        0        0     1673 2024-02-07 14:55:52.609471 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6a/test_application.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.014003 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/__init__.py
+-rw-r--r--   0        0        0     1395 2024-01-22 11:48:56.750419 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/application.py
+-rw-r--r--   0        0        0     3261 2024-01-22 11:48:56.798355 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/domainmodel.py
+-rw-r--r--   0        0        0     1874 2024-01-22 11:48:56.798675 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/persistence.py
+-rw-r--r--   0        0        0     1366 2024-01-22 10:29:19.047196 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/test_application.py
+-rw-r--r--   0        0        0     1634 2024-01-22 10:29:19.049488 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/test_compression_and_encryption.py
+-rw-r--r--   0        0        0     2190 2024-01-22 11:48:56.799051 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/test_snapshotting_intervals.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.014003 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/__init__.py
+-rw-r--r--   0        0        0     1748 2024-02-07 14:53:47.589167 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/application.py
+-rw-r--r--   0        0        0     4016 2024-02-07 15:29:37.193222 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/domainmodel.py
+-rw-r--r--   0        0        0     1741 2024-02-07 14:55:24.719559 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/test_application.py
+-rw-r--r--   0        0        0     1636 2024-02-07 14:41:27.654454 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/test_compression_and_encryption.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.015249 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/__init__.py
+-rw-r--r--   0        0        0     1357 2024-03-28 18:21:09.300220 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/application.py
+-rw-r--r--   0        0        0     1276 2024-01-22 11:48:56.753304 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/domainmodel.py
+-rw-r--r--   0        0        0     1874 2024-01-22 11:48:56.799412 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/persistence.py
+-rw-r--r--   0        0        0     1268 2024-01-22 10:29:19.052955 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/test_application.py
+-rw-r--r--   0        0        0     1509 2024-01-22 10:29:19.054150 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/test_compression_and_encryption.py
+-rw-r--r--   0        0        0     1261 2024-01-22 11:48:56.799858 eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/test_snapshotting_intervals.py
+-rw-r--r--   0        0        0        0 2021-10-08 09:03:42.584262 eventsourcing-9.3.0b1/eventsourcing/examples/bankaccounts/__init__.py
+-rw-r--r--   0        0        0     2286 2024-01-22 10:29:20.704274 eventsourcing-9.3.0b1/eventsourcing/examples/bankaccounts/application.py
+-rw-r--r--   0        0        0     1574 2024-01-21 08:06:33.089141 eventsourcing-9.3.0b1/eventsourcing/examples/bankaccounts/domainmodel.py
+-rw-r--r--   0        0        0     5577 2024-01-21 08:06:33.089500 eventsourcing-9.3.0b1/eventsourcing/examples/bankaccounts/test.py
+-rw-r--r--   0        0        0        0 2021-10-08 09:03:42.586411 eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/__init__.py
+-rw-r--r--   0        0        0     3646 2024-01-22 11:48:56.800443 eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/application.py
+-rw-r--r--   0        0        0     9638 2024-01-22 11:48:56.758544 eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/domainmodel.py
+-rw-r--r--   0        0        0     4846 2024-01-22 11:48:56.801005 eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/interface.py
+-rw-r--r--   0        0        0     9649 2024-01-21 08:06:33.091724 eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/test.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.017339 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/__init__.py
+-rw-r--r--   0        0        0     3918 2024-01-22 11:48:56.759873 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/application.py
+-rw-r--r--   0        0        0     1825 2024-01-22 10:29:19.058391 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/domainmodel.py
+-rw-r--r--   0        0        0     6230 2024-01-22 10:29:19.058947 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/test.py
+-rw-r--r--   0        0        0      745 2024-01-22 10:29:19.059398 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/utils.py
+-rw-r--r--   0        0        0        0 2024-01-21 05:01:11.255037 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagementsystem/__init__.py
+-rw-r--r--   0        0        0     1877 2024-05-28 13:55:36.228175 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagementsystem/application.py
+-rw-r--r--   0        0        0      423 2024-01-21 23:58:53.728905 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagementsystem/postgres.py
+-rw-r--r--   0        0        0      411 2024-01-21 23:58:53.729620 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagementsystem/sqlite.py
+-rw-r--r--   0        0        0      444 2024-01-21 08:06:33.093493 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagementsystem/system.py
+-rw-r--r--   0        0        0     7106 2024-01-22 11:48:56.761172 eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagementsystem/test_system.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.018121 eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/__init__.py
+-rw-r--r--   0        0        0     1670 2024-01-22 11:48:56.802116 eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/application.py
+-rw-r--r--   0        0        0      596 2024-01-22 11:48:56.802634 eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/persistence.py
+-rw-r--r--   0        0        0     3831 2024-01-22 11:48:56.803255 eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/postgres.py
+-rw-r--r--   0        0        0     4736 2024-01-22 11:48:56.804304 eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/sqlite.py
+-rw-r--r--   0        0        0     3954 2024-01-22 11:48:56.763879 eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/test_application.py
+-rw-r--r--   0        0        0     2312 2024-01-22 11:48:56.806173 eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/test_recorder.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.018996 eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/__init__.py
+-rw-r--r--   0        0        0     1325 2024-01-22 11:48:56.807345 eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/application.py
+-rw-r--r--   0        0        0      543 2024-01-22 10:29:20.709386 eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/persistence.py
+-rw-r--r--   0        0        0     3857 2024-01-22 11:48:56.765009 eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/postgres.py
+-rw-r--r--   0        0        0     3312 2024-01-22 11:48:56.765505 eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/sqlite.py
+-rw-r--r--   0        0        0     3191 2024-01-22 11:48:56.766081 eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/test_searchabletimestamps.py
+-rw-r--r--   0        0        0     4890 2024-01-22 11:48:56.807938 eventsourcing-9.3.0b1/eventsourcing/examples/test_invoice.py
+-rw-r--r--   0        0        0     6682 2024-01-22 11:48:56.808455 eventsourcing-9.3.0b1/eventsourcing/examples/test_parking_lot.py
+-rw-r--r--   0        0        0     4676 2024-05-28 13:55:36.228528 eventsourcing-9.3.0b1/eventsourcing/interface.py
+-rw-r--r--   0        0        0    37672 2024-01-22 11:48:56.809678 eventsourcing-9.3.0b1/eventsourcing/persistence.py
+-rw-r--r--   0        0        0     6547 2024-01-22 11:48:56.810266 eventsourcing-9.3.0b1/eventsourcing/popo.py
+-rw-r--r--   0        0        0    29757 2024-03-28 20:19:45.581979 eventsourcing-9.3.0b1/eventsourcing/postgres.py
+-rw-r--r--   0        0        0        0 2021-10-08 09:03:57.613590 eventsourcing-9.3.0b1/eventsourcing/py.typed
+-rw-r--r--   0        0        0    18466 2024-01-22 11:48:56.811630 eventsourcing-9.3.0b1/eventsourcing/sqlite.py
+-rw-r--r--   0        0        0    45298 2024-01-22 11:48:56.812428 eventsourcing-9.3.0b1/eventsourcing/system.py
+-rw-r--r--   0        0        0        0 2021-10-08 09:03:42.596319 eventsourcing-9.3.0b1/eventsourcing/tests/__init__.py
+-rw-r--r--   0        0        0    17586 2024-01-22 11:48:56.813100 eventsourcing-9.3.0b1/eventsourcing/tests/application.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.023033 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/__init__.py
+-rw-r--r--   0        0        0     1956 2024-01-22 11:48:56.813721 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_application_with_automatic_snapshotting.py
+-rw-r--r--   0        0        0      678 2022-04-28 12:08:57.023305 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_application_with_popo.py
+-rw-r--r--   0        0        0     2431 2024-01-22 10:29:19.073249 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_application_with_postgres.py
+-rw-r--r--   0        0        0     2059 2024-01-21 23:58:53.751746 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_application_with_sqlite.py
+-rw-r--r--   0        0        0     3516 2022-04-28 12:08:57.023909 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_cache.py
+-rw-r--r--   0        0        0     5438 2024-01-22 10:29:20.716602 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_event_sourced_log.py
+-rw-r--r--   0        0        0     9194 2024-01-21 23:58:53.756001 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_notificationlog.py
+-rw-r--r--   0        0        0     4298 2022-04-28 12:08:57.024438 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_notificationlogreader.py
+-rw-r--r--   0        0        0     3744 2024-01-22 10:29:19.074691 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_processapplication.py
+-rw-r--r--   0        0        0     3212 2024-01-22 10:29:19.075755 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_processingpolicy.py
+-rw-r--r--   0        0        0    18873 2024-05-27 16:05:29.820265 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_repository.py
+-rw-r--r--   0        0        0     2042 2022-04-28 12:08:57.025270 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_snapshotting.py
+-rw-r--r--   0        0        0    14355 2024-01-22 10:29:19.077050 eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_upcasting.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.025633 eventsourcing-9.3.0b1/eventsourcing/tests/docs_tests/__init__.py
+-rw-r--r--   0        0        0    10777 2024-01-22 10:29:19.077703 eventsourcing-9.3.0b1/eventsourcing/tests/docs_tests/test_docs.py
+-rw-r--r--   0        0        0     3254 2024-01-22 10:29:19.078596 eventsourcing-9.3.0b1/eventsourcing/tests/domain.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.026202 eventsourcing-9.3.0b1/eventsourcing/tests/domain_tests/__init__.py
+-rw-r--r--   0        0        0    38255 2024-05-28 13:30:24.560114 eventsourcing-9.3.0b1/eventsourcing/tests/domain_tests/test_aggregate.py
+-rw-r--r--   0        0        0    50256 2024-01-22 10:29:20.717494 eventsourcing-9.3.0b1/eventsourcing/tests/domain_tests/test_aggregate_decorators.py
+-rw-r--r--   0        0        0     2782 2024-01-22 10:29:19.080834 eventsourcing-9.3.0b1/eventsourcing/tests/domain_tests/test_domainevent.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.027156 eventsourcing-9.3.0b1/eventsourcing/tests/interface_tests/__init__.py
+-rw-r--r--   0        0        0     9140 2024-05-28 13:55:36.228950 eventsourcing-9.3.0b1/eventsourcing/tests/interface_tests/test_remotenotificationlog.py
+-rw-r--r--   0        0        0    45723 2024-01-22 11:48:56.815084 eventsourcing-9.3.0b1/eventsourcing/tests/persistence.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.027915 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/__init__.py
+-rw-r--r--   0        0        0     2873 2022-04-28 12:08:57.028057 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_aes.py
+-rw-r--r--   0        0        0    23641 2024-01-22 11:48:56.774665 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_connection_pool.py
+-rw-r--r--   0        0        0     2261 2024-01-22 10:29:19.085478 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_eventstore.py
+-rw-r--r--   0        0        0      730 2024-01-21 23:58:53.776667 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_infrastructure_factory.py
+-rw-r--r--   0        0        0     3806 2024-01-21 23:58:53.777480 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_mapper.py
+-rw-r--r--   0        0        0     2130 2024-01-21 23:58:53.777951 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_noninterleaving_notification_ids.py
+-rw-r--r--   0        0        0     3366 2023-10-14 15:08:00.772836 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_popo.py
+-rw-r--r--   0        0        0    40906 2024-03-28 19:56:57.846822 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_postgres.py
+-rw-r--r--   0        0        0    11744 2024-01-22 10:29:20.718467 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_sqlite.py
+-rw-r--r--   0        0        0     1251 2022-04-28 12:08:57.030988 eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_transcoder.py
+-rw-r--r--   0        0        0     1364 2024-01-22 10:29:19.087031 eventsourcing-9.3.0b1/eventsourcing/tests/postgres_utils.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.031415 eventsourcing-9.3.0b1/eventsourcing/tests/system_tests/__init__.py
+-rw-r--r--   0        0        0    31841 2024-05-28 13:55:36.229423 eventsourcing-9.3.0b1/eventsourcing/tests/system_tests/test_runner.py
+-rw-r--r--   0        0        0     9552 2024-01-22 10:29:20.719393 eventsourcing-9.3.0b1/eventsourcing/tests/system_tests/test_system.py
+-rw-r--r--   0        0        0        0 2022-04-28 12:08:57.032281 eventsourcing-9.3.0b1/eventsourcing/tests/utils_tests/__init__.py
+-rw-r--r--   0        0        0     6486 2024-01-21 23:58:53.786521 eventsourcing-9.3.0b1/eventsourcing/tests/utils_tests/test_utils.py
+-rw-r--r--   0        0        0     8247 2024-01-22 11:48:56.816547 eventsourcing-9.3.0b1/eventsourcing/utils.py
+-rw-r--r--   0        0        0     6884 2024-05-28 14:11:33.971059 eventsourcing-9.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0     9890 1970-01-01 00:00:00.000000 eventsourcing-9.3.0b1/PKG-INFO
```

### Comparing `eventsourcing-9.3.0a1/LICENSE` & `eventsourcing-9.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/README.md` & `eventsourcing-9.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/application.py` & `eventsourcing-9.3.0b1/eventsourcing/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/cipher.py` & `eventsourcing-9.3.0b1/eventsourcing/cipher.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/dispatch.py` & `eventsourcing-9.3.0b1/eventsourcing/dispatch.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/domain.py` & `eventsourcing-9.3.0b1/eventsourcing/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -937,85 +937,64 @@
         except KeyError:
             base_event_cls = cls._define_event_class(
                 base_event_name, (cls.Event,), None
             )
             setattr(cls, base_event_name, base_event_cls)
 
         # Make sure all events defined on aggregate subclass the base event class.
+        created_event_classes: Dict[str, Type[CanInitAggregate]] = {}
         for name, value in tuple(cls.__dict__.items()):
             if name == base_event_name:
                 # Don't subclass the base event class again.
                 continue
             if name.lower() == name:
                 # Don't subclass lowercase named attributes that have classes.
                 continue
             if (
                 isinstance(value, type)
                 and issubclass(value, AggregateEvent)
                 and not issubclass(value, base_event_cls)
             ):
                 sub_class = cls._define_event_class(name, (value, base_event_cls), None)
                 setattr(cls, name, sub_class)
-
-        # Identify or define the aggregate's "created" event class.
-        created_event_class: Type[CanInitAggregate] | None = None
-
-        # Has the "created" event class been indicated with '_created_event_class'.
-        if "_created_event_class" in cls.__dict__:
-            created_event_class = cls.__dict__["_created_event_class"]
-            if isinstance(created_event_class, type) and issubclass(
-                created_event_class, CanInitAggregate
-            ):
-                # We just subclassed the event classes, so reassign this.
-                created_event_class = getattr(cls, created_event_class.__name__)
-                assert created_event_class
-                cls._created_event_class = created_event_class
-            else:
-                msg = (
-                    f"{created_event_class} not subclass of {CanInitAggregate.__name__}"
-                )
-                raise TypeError(msg)
+        for name, value in tuple(cls.__dict__.items()):
+            if isinstance(value, type) and issubclass(value, CanInitAggregate):
+                created_event_classes[name] = value
 
         # Disallow using both '_created_event_class' and 'created_event_name'.
+        created_event_class: Type[CanInitAggregate] | None = cls.__dict__.get(
+            "_created_event_class"
+        )
         if created_event_class and created_event_name:
             msg = "Can't use both '_created_event_class' and 'created_event_name'"
             raise TypeError(msg)
 
+        # Identify or define the aggregate's "created" event class.
+
         # Is the init method decorated with a CommandMethodDecorator?
         if isinstance(cls.__dict__.get("__init__"), CommandMethodDecorator):
             init_decorator: CommandMethodDecorator = cls.__dict__["__init__"]
 
             # Set the original method on the class (un-decorate __init__).
             cls.__init__ = init_decorator.decorated_method  # type: ignore
 
-            # Disallow using both 'created_event_name' and '_created_event_class'.
+            # Disallow using both 'created_event_name' and decorator on __init__.
             if created_event_name:
                 msg = "Can't use both 'created_event_name' and decorator on __init__"
                 raise TypeError(msg)
+            # Disallow using both '_created_event_class' and decorator on __init__.
             if created_event_class:
                 msg = "Can't use both '_created_event_class' and decorator on __init__"
                 raise TypeError(msg)
 
-            # Does the decorator specify a "create" event class?
+            # Does the decorator specify a "created" event class?
             if init_decorator.given_event_cls:
-                created_event_class = getattr(
-                    cls, init_decorator.given_event_cls.__name__
+                created_event_class = cast(
+                    Type[CanInitAggregate], init_decorator.given_event_cls
                 )
-                if isinstance(created_event_class, type) and issubclass(
-                    created_event_class, CanInitAggregate
-                ):
-                    assert created_event_class
-                    cls._created_event_class = created_event_class
-                else:
-                    msg = (
-                        f"{created_event_class} not subclass of "
-                        f"{CanInitAggregate.__name__}"
-                    )
-                    raise TypeError(msg)
-
             # Does the decorator specify a "created" event name?
             elif init_decorator.event_cls_name:
                 created_event_name = init_decorator.event_cls_name
 
             # Disallow using decorator on __init__ without event spec.
             else:
                 msg = "Decorator on __init__ has neither event name nor class"
@@ -1024,73 +1003,93 @@
         # TODO: Write a test to cover this when "Created" class is explicitly defined.
         # Check if init mentions ID.
         for param_name in inspect.signature(cls.__init__).parameters:  # type: ignore
             if param_name == "id":
                 _init_mentions_id.add(cls)
                 break
 
-        # If no "created" event class has been specified, find or create one.
-        if created_event_class is None:
-            # Discover all the "created" event classes already defined.
-            created_event_classes: Dict[str, Type[AggregateCreated]] = {}
-            for name, value in tuple(cls.__dict__.items()):
-                if isinstance(value, type) and issubclass(value, AggregateCreated):
-                    created_event_classes[name] = value
-
-            # Is a "created" event class already defined that matches the name?
-            if created_event_name in created_event_classes:
-                cls._created_event_class = created_event_classes[created_event_name]
-
-            # If there is only one class defined, and we have no name, use it.
-            elif len(created_event_classes) == 1 and not created_event_name:
-                cls._created_event_class = next(iter(created_event_classes.values()))
-
-            # If there are no "created" event classes already defined, or a name is
-            # specified that hasn't matched, then define a "created" event class.
-            elif len(created_event_classes) == 0 or created_event_name:
-                # If no "created" event name has been specified, use default name.
-                if not created_event_name:
-                    # This is safe because len(created_event_classes) == 0.
-                    created_event_name = "Created"
+        if created_event_class:
+            # Check specified "created" event class can init aggregate.
+            if not issubclass(created_event_class, CanInitAggregate):
+                msg = (
+                    f"{created_event_class} not subclass of {CanInitAggregate.__name__}"
+                )
+                raise TypeError(msg)
+
+            for sub_class in created_event_classes.values():
+                if issubclass(sub_class, created_event_class):
+                    # We just subclassed the created event class, so reassign it.
+                    created_event_class = sub_class
+
+        # Is a "created" event class already defined that matches the name?
+        elif created_event_name and created_event_name in created_event_classes:
+            created_event_class = created_event_classes[created_event_name]
+
+        # If there is only one class defined, then use it.
+        elif len(created_event_classes) == 1 and not created_event_name:
+            created_event_class = next(iter(created_event_classes.values()))
+
+        # If there are no "created" event classes already defined, or a name is
+        # specified that hasn't matched, then define a "created" event class.
+        elif len(created_event_classes) == 0 or created_event_name:
+
+            # Decide the base classes for the new "created" event class.
+            if created_event_name and len(created_event_classes) == 1:
+                base_created_event_cls = next(iter(created_event_classes.values()))
+            else:
+                for base_cls in cls.__mro__:
+                    if base_cls is cls:
+                        continue
+                    base_created_event_cls = base_cls.__dict__.get(
+                        "_created_event_class",
+                        base_cls.__dict__.get("Created"),
+                    )
+                    if base_created_event_cls:
+                        break
+                else:  # pragma: no cover
+                    msg = "Can't decide base class for new 'created' event class"
+                    raise TypeError(msg)
+
+            if not created_event_name:
+                created_event_name = base_created_event_cls.__name__
 
-                # Disallow init method from having variable params if
-                # we are using it to define a "created" event class.
+            # Disallow init method from having variable params if
+            # we are using it to define a "created" event class.
+            try:
+                init_method = cls.__dict__["__init__"]
+            except KeyError:
+                init_method = None
+            else:
                 try:
-                    init_method = cls.__dict__["__init__"]
-                except KeyError:
-                    init_method = None
-                else:
-                    try:
-                        _check_no_variable_params(init_method)
-                    except TypeError:
-                        raise
-
-                # Define a "created" event class for this aggregate.
-                if issubclass(cls.Created, base_event_cls):
-                    # Don't subclass from base event class twice.
-                    bases: Tuple[Type[CanMutateAggregate], ...] = (cls.Created,)
-                else:
-                    bases = (cls.Created, base_event_cls)
-                event_cls = cls._define_event_class(
+                    _check_no_variable_params(init_method)
+                except TypeError:
+                    raise
+
+            # Define a "created" event class for this aggregate.
+            if issubclass(base_created_event_cls, base_event_cls):
+                # Don't subclass from base event class twice.
+                bases: Tuple[Type[CanMutateAggregate], ...] = (base_created_event_cls,)
+            else:
+                bases = (base_created_event_cls, base_event_cls)
+            created_event_class = cast(
+                Type[CanInitAggregate],
+                cls._define_event_class(
                     created_event_name,
                     bases,
                     init_method,
-                )
-
-                # Set the event class as an attribute of the aggregate class.
-                setattr(cls, created_event_name, event_cls)
-
-                # Remember which is the "created" event class.
-                cls._created_event_class = cast(Type[AggregateCreated], event_cls)
+                ),
+            )
+            # Set the event class as an attribute of the aggregate class.
+            setattr(cls, created_event_name, created_event_class)
 
+        if created_event_class:
+            cls._created_event_class = created_event_class
+        else:
             # Prepare to disallow ambiguity of choice between created event classes.
-            else:
-                aggregate_has_many_created_event_classes[cls] = list(
-                    created_event_classes
-                )
+            aggregate_has_many_created_event_classes[cls] = list(created_event_classes)
 
         # Prepare the subsequent event classes.
         for attr_name, attr_value in tuple(cls.__dict__.items()):
             event_decorator: CommandMethodDecorator | None = None
 
             if isinstance(attr_value, CommandMethodDecorator):
                 event_decorator = attr_value
```

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate1/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate1/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate1/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate1/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate2/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate2/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate2/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate2/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate3/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate3/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate3/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate3/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate3/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate3/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate4/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate4/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate4/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate4/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate4/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate4/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate5/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate5/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate5/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate5/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate5/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate5/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6a/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6a/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6a/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6a/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate6a/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate6a/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/persistence.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/persistence.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/test_compression_and_encryption.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/test_compression_and_encryption.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7/test_snapshotting_intervals.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7/test_snapshotting_intervals.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate7a/test_compression_and_encryption.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate7a/test_compression_and_encryption.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/persistence.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/persistence.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/test_compression_and_encryption.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/test_compression_and_encryption.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/aggregate8/test_snapshotting_intervals.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/aggregate8/test_snapshotting_intervals.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/bankaccounts/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/bankaccounts/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/bankaccounts/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/bankaccounts/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/bankaccounts/test.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/bankaccounts/test.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/interface.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/interface.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/cargoshipping/test.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/cargoshipping/test.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/domainmodel.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/domainmodel.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/test.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/test.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagement/utils.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagement/utils.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagementsystem/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagementsystem/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/contentmanagementsystem/test_system.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/contentmanagementsystem/test_system.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/persistence.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/persistence.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/postgres.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/postgres.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/sqlite.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/sqlite.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/test_application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/test_application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchablecontent/test_recorder.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchablecontent/test_recorder.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/application.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/persistence.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/persistence.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/postgres.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/postgres.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/sqlite.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/sqlite.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/searchabletimestamps/test_searchabletimestamps.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/searchabletimestamps/test_searchabletimestamps.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/test_invoice.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/test_invoice.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/examples/test_parking_lot.py` & `eventsourcing-9.3.0b1/eventsourcing/examples/test_parking_lot.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/interface.py` & `eventsourcing-9.3.0b1/eventsourcing/interface.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/persistence.py` & `eventsourcing-9.3.0b1/eventsourcing/persistence.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/popo.py` & `eventsourcing-9.3.0b1/eventsourcing/popo.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/postgres.py` & `eventsourcing-9.3.0b1/eventsourcing/postgres.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/sqlite.py` & `eventsourcing-9.3.0b1/eventsourcing/sqlite.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/system.py` & `eventsourcing-9.3.0b1/eventsourcing/system.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_application_with_automatic_snapshotting.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_application_with_automatic_snapshotting.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_application_with_popo.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_application_with_popo.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_application_with_postgres.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_application_with_postgres.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_application_with_sqlite.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_application_with_sqlite.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_cache.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_event_sourced_log.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_event_sourced_log.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_notificationlog.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_notificationlog.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_notificationlogreader.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_notificationlogreader.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_processapplication.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_processapplication.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_processingpolicy.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_processingpolicy.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_repository.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_snapshotting.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_snapshotting.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/application_tests/test_upcasting.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/application_tests/test_upcasting.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/docs_tests/test_docs.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/docs_tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/domain.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/domain.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/domain_tests/test_aggregate.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/domain_tests/test_aggregate.py`

 * *Files 1% similar despite different names*

```diff
@@ -726,14 +726,15 @@
 
             class Created(AggregateCreated):
                 name: str
 
         order = Order("name")
         pending = order.collect_events()
         self.assertEqual(type(pending[0]).__name__, "Started")
+        self.assertTrue(isinstance(pending[0], Order.Created))
 
     def test_raises_when_given_created_event_name_conflicts_with_created_event_class(
         self,
     ):
         with self.assertRaises(TypeError) as cm:
 
             class Order(Aggregate, created_event_name="Started"):
@@ -1094,14 +1095,27 @@
             MySubclass.Started.__qualname__,
         )
         self.assertTrue(
             MySubclass.Ended.__qualname__.endswith("MySubclass.Ended"),
             MySubclass.Ended.__qualname__,
         )
 
+        self.assertTrue(
+            MySubclass._created_event_class.__qualname__.endswith("MySubclass.Opened")
+        )
+
+        class MySubSubClass(MySubclass):
+            pass
+
+        self.assertTrue(
+            MySubSubClass._created_event_class.__qualname__.endswith(
+                "MySubSubClass.Opened"
+            )
+        )
+
 
 class TestBankAccount(TestCase):
     def test_subclass_bank_account(self):
         # Open an account.
         account: BankAccount = BankAccount.open(
             full_name="Alice",
             email_address="alice@example.com",
```

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/domain_tests/test_aggregate_decorators.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/domain_tests/test_aggregate_decorators.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/domain_tests/test_domainevent.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/domain_tests/test_domainevent.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/interface_tests/test_remotenotificationlog.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/interface_tests/test_remotenotificationlog.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_aes.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_aes.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_connection_pool.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_eventstore.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_eventstore.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_infrastructure_factory.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_infrastructure_factory.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_mapper.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_noninterleaving_notification_ids.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_noninterleaving_notification_ids.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_popo.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_popo.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_postgres.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_sqlite.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/persistence_tests/test_transcoder.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/persistence_tests/test_transcoder.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/postgres_utils.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/system_tests/test_runner.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/system_tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/system_tests/test_system.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/system_tests/test_system.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/tests/utils_tests/test_utils.py` & `eventsourcing-9.3.0b1/eventsourcing/tests/utils_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/eventsourcing/utils.py` & `eventsourcing-9.3.0b1/eventsourcing/utils.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.3.0a1/pyproject.toml` & `eventsourcing-9.3.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "eventsourcing"
-version = "9.3.0-alpha.1"
+version = "9.3.0-beta.1"
 
 description = "Event sourcing in Python"
 authors = [
     "John Bywater <john.bywater@appropriatesoftware.net>",
 ]
 license = "BSD 3-Clause"
 classifiers = [
-    "Development Status :: 3 - Alpha",
-#    "Development Status :: 4 - Beta",
+#    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
 #    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
@@ -178,28 +178,29 @@
 skip = ".eggs,.pip-cache,.poetry,venv,.venv,dist"
 profile = "black"
 sections = "FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 
 [tool.ruff]
 # Same as Black.
 line-length = 88
-indent-width = 4
+#indent-width = 4
 
 # Assume Python 3.8
 target-version = "py38"
 
 [tool.ruff.lint]
 # Todo: "D"
 #select = ["E", "F", "W", "I", "N", "UP"]
 select = [
     "ALL",
 #    "RUF012",
 ]
 ignore = [
     "UP006",  # [*] Use `type` instead of `Type` for type annotation / Use `tuple` instead of `Tuple` for type annotation / etc  <- ignore while supporting Python3.8
+    "A003",  # "Class attribute `id/type` is shadowing a Python builtin
     "ANN",
     "D",
     "PT",
     "ERA",
     "COM812",
     "T201",
     "FIX",
@@ -249,18 +250,18 @@
 line-ending = "auto"
 
 # Enable auto-formatting of code examples in docstrings. Markdown,
 # reStructuredText code/literal blocks and doctests are all supported.
 #
 # This is currently disabled by default, but it is planned for this
 # to be opt-out in the future.
-docstring-code-format = false
+#docstring-code-format = false
 
 # Set the line length limit used when formatting code snippets in
 # docstrings.
 #
 # This only has an effect when the `docstring-code-format` setting is
 # enabled.
-docstring-code-line-length = "dynamic"
+#docstring-code-line-length = "dynamic"
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `eventsourcing-9.3.0a1/PKG-INFO` & `eventsourcing-9.3.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: eventsourcing
-Version: 9.3.0a1
+Version: 9.3.0b1
 Summary: Event sourcing in Python
 Home-page: https://github.com/pyeventsourcing/eventsourcing
 License: BSD 3-Clause
 Keywords: event sourcing,event store,domain driven design,domain-driven design,ddd,cqrs,cqs
 Author: John Bywater
 Author-email: john.bywater@appropriatesoftware.net
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

