# Comparing `tmp/nucliadb-4.0.1.post548-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.1.post550-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,464 +1,470 @@
-Zip file size: 765784 bytes, number of entries: 462
--rw-r--r--  2.0 unx     1135 b- defN 24-May-27 10:54 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-27 10:54 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-27 10:54 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-27 10:54 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-27 10:54 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-27 10:54 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-27 10:54 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-27 10:54 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-27 10:54 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-27 10:54 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-27 10:54 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-27 10:54 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-27 10:54 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-27 10:54 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-27 10:54 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-27 10:54 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-27 10:54 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-27 10:54 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-27 10:54 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-27 10:54 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-27 10:54 nucliadb/health.py
--rw-r--r--  2.0 unx    11639 b- defN 24-May-27 10:54 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-27 10:54 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-27 10:54 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-27 10:54 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5175 b- defN 24-May-27 10:54 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5080 b- defN 24-May-27 10:54 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-27 10:54 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-27 10:54 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-27 10:54 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22091 b- defN 24-May-27 10:54 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-27 10:54 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20209 b- defN 24-May-27 10:54 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-27 10:54 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-27 10:54 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-27 10:54 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12512 b- defN 24-May-27 10:54 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-27 10:54 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-27 10:54 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-27 10:54 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-27 10:54 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-May-27 10:54 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-27 10:54 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-27 10:54 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-27 10:54 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-27 10:54 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-27 10:54 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1906 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     2651 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/atomic.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx    12177 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1548 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/synonyms.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-27 10:54 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-27 10:54 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-27 10:54 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-27 10:54 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-27 10:54 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-27 10:54 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-27 10:54 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-27 10:54 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-27 10:54 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-27 10:54 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-27 10:54 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-27 10:54 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-27 10:54 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-27 10:54 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-27 10:54 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-27 10:54 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-27 10:54 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-27 10:54 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-27 10:54 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-27 10:54 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-27 10:54 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-27 10:54 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-27 10:54 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-27 10:54 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-27 10:54 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19904 b- defN 24-May-27 10:54 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-27 10:54 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-27 10:54 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-27 10:54 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3945 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-27 10:54 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    17461 b- defN 24-May-27 10:54 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-27 10:54 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-27 10:54 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-27 10:54 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     4840 b- defN 24-May-27 10:54 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-27 10:54 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-27 10:54 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-27 10:54 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4212 b- defN 24-May-27 10:54 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-27 10:54 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28311 b- defN 24-May-27 10:54 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-27 10:54 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-27 10:54 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    15621 b- defN 24-May-27 10:54 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-27 10:54 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    58955 b- defN 24-May-27 10:54 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     2685 b- defN 24-May-27 10:54 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27042 b- defN 24-May-27 10:54 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-May-27 10:54 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-27 10:54 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-27 10:54 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    30462 b- defN 24-May-27 10:54 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-27 10:54 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-27 10:54 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-27 10:54 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     3836 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-27 10:54 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-27 10:54 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-27 10:54 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-27 10:54 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-27 10:54 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-27 10:54 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-27 10:54 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-27 10:54 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-27 10:54 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-27 10:54 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-27 10:54 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-27 10:54 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-27 10:54 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-27 10:54 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-27 10:54 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-27 10:54 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-27 10:54 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-27 10:54 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-27 10:54 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-27 10:54 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-27 10:54 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-27 10:54 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13951 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12115 b- defN 24-May-27 10:54 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7979 b- defN 24-May-27 10:54 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-27 10:54 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-27 10:54 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-27 10:54 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-27 10:54 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-27 10:54 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-27 10:54 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-27 10:54 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-27 10:54 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-27 10:54 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-27 10:54 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-27 10:54 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-27 10:54 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-27 10:54 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-27 10:54 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-27 10:54 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-May-27 10:54 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9493 b- defN 24-May-27 10:54 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-27 10:54 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-27 10:54 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-27 10:54 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-27 10:54 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-27 10:54 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-27 10:54 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-27 10:54 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-27 10:54 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-27 10:54 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-27 10:54 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-27 10:54 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-27 10:54 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-27 10:54 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-27 10:54 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-27 10:54 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-27 10:54 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-27 10:54 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-27 10:54 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-27 10:54 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-27 10:54 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-27 10:54 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-27 10:54 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-27 10:54 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31093 b- defN 24-May-27 10:54 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-27 10:54 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-27 10:54 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-27 10:54 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-27 10:54 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-27 10:54 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-27 10:54 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-27 10:54 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-27 10:54 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-27 10:54 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-27 10:54 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-27 10:54 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-27 10:54 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-27 10:54 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-27 10:54 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-27 10:54 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-27 10:54 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-27 10:54 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-27 10:54 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-27 10:54 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5636 b- defN 24-May-27 10:54 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-27 10:54 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-27 10:54 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-27 10:54 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-27 10:54 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-27 10:54 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-27 10:54 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-27 10:54 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-27 10:54 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-27 10:54 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-27 10:54 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-May-27 10:54 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-27 10:54 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-27 10:54 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-27 10:54 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-27 10:54 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-27 10:54 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-27 10:54 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-27 10:54 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-27 10:54 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-27 10:54 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-27 10:54 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-27 10:54 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-27 10:54 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-27 10:54 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-27 10:54 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-27 10:54 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-27 10:54 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-27 10:54 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-27 10:54 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-27 10:54 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-27 10:54 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-27 10:54 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-27 10:54 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-27 10:54 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-27 10:54 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-27 10:54 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-27 10:54 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-27 10:54 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-27 10:54 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-27 10:54 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-27 10:54 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-27 10:54 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-27 10:54 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-27 10:54 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-27 10:54 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-27 10:54 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-27 10:54 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-27 10:54 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-27 10:54 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-27 10:54 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-27 10:54 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-27 10:54 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-27 10:54 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-27 10:54 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-27 10:54 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-27 10:54 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-27 10:54 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-27 10:54 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-27 10:54 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-27 10:54 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-27 10:54 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-27 10:54 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-27 10:54 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-27 10:54 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-27 10:54 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-27 10:54 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-27 10:54 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-27 10:54 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-27 10:54 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-27 10:54 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-27 10:54 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-27 10:54 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-27 10:54 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-27 10:54 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-27 10:54 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-27 10:54 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-27 10:54 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-27 10:54 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-27 10:54 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-27 10:54 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-27 10:54 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-27 10:54 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-27 10:54 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-27 10:54 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-27 10:54 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-27 10:54 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-27 10:54 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-27 10:54 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-27 10:54 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-27 10:54 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-27 10:54 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-27 10:54 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-27 10:54 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-27 10:54 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-27 10:54 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-27 10:54 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-27 10:54 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-27 10:54 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-27 10:54 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-27 10:54 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-27 10:54 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-27 10:54 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-27 10:54 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-27 10:54 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-27 10:54 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-27 10:54 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6421 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18628 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10216 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30985 b- defN 24-May-27 10:54 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-27 10:54 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-27 10:54 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-27 10:54 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-27 10:54 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16740 b- defN 24-May-27 10:54 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-27 10:54 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-27 10:54 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-27 10:54 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-27 10:54 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-27 10:54 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-27 10:54 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-27 10:54 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4400 b- defN 24-May-27 10:54 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16857 b- defN 24-May-27 10:54 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-27 10:54 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-27 10:54 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-27 10:54 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-27 10:54 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-27 10:54 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-27 10:54 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-27 10:54 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-27 10:54 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-27 10:54 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-27 10:54 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-27 10:54 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-27 10:54 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4423 b- defN 24-May-27 10:55 nucliadb-4.0.1.post548.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-27 10:55 nucliadb-4.0.1.post548.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-27 10:55 nucliadb-4.0.1.post548.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-27 10:55 nucliadb-4.0.1.post548.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-27 10:55 nucliadb-4.0.1.post548.dist-info/zip-safe
--rw-rw-r--  2.0 unx    43366 b- defN 24-May-27 10:55 nucliadb-4.0.1.post548.dist-info/RECORD
-462 files, 2261348 bytes uncompressed, 696426 bytes compressed:  69.2%
+Zip file size: 766377 bytes, number of entries: 468
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-28 09:29 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-28 09:29 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-28 09:29 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-28 09:29 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-28 09:29 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-28 09:29 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-28 09:29 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-28 09:29 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-28 09:29 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-28 09:29 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-28 09:29 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-28 09:29 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-28 09:29 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-28 09:29 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-28 09:29 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-28 09:29 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-28 09:29 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-28 09:29 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-28 09:29 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-28 09:29 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-28 09:29 nucliadb/health.py
+-rw-r--r--  2.0 unx    11639 b- defN 24-May-28 09:29 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-28 09:29 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-28 09:29 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:29 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-May-28 09:29 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5080 b- defN 24-May-28 09:29 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-28 09:29 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-28 09:29 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-28 09:29 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22091 b- defN 24-May-28 09:29 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-28 09:29 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20209 b- defN 24-May-28 09:29 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-May-28 09:29 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-28 09:29 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-28 09:29 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12512 b- defN 24-May-28 09:29 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-28 09:29 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-28 09:29 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-28 09:29 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-28 09:29 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-May-28 09:29 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-28 09:29 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-28 09:29 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-28 09:29 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-28 09:29 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-28 09:29 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1906 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     2651 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/atomic.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx    12177 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-28 09:29 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-28 09:29 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-28 09:29 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-28 09:29 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-28 09:29 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-28 09:29 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-28 09:29 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-28 09:29 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-28 09:29 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-28 09:29 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-28 09:29 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-28 09:29 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-May-28 09:29 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-28 09:29 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-28 09:29 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-28 09:29 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-28 09:29 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-28 09:29 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-28 09:29 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-28 09:29 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-28 09:29 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-28 09:29 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-28 09:29 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-28 09:29 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-28 09:29 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19904 b- defN 24-May-28 09:29 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:29 nucliadb/ingest/py.typed
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-28 09:29 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-May-28 09:29 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-28 09:29 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3945 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-28 09:29 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    17461 b- defN 24-May-28 09:29 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-28 09:29 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-28 09:29 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-28 09:29 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     4840 b- defN 24-May-28 09:29 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-28 09:29 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-28 09:29 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-28 09:29 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-May-28 09:29 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-28 09:29 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28311 b- defN 24-May-28 09:29 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-28 09:29 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-28 09:29 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    15621 b- defN 24-May-28 09:29 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-28 09:29 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    58955 b- defN 24-May-28 09:29 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-May-28 09:29 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27042 b- defN 24-May-28 09:29 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-May-28 09:29 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-28 09:29 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-28 09:29 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    30462 b- defN 24-May-28 09:29 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-28 09:29 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-28 09:29 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-28 09:29 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     3836 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-28 09:29 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-28 09:29 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-28 09:29 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-28 09:29 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-28 09:29 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-28 09:29 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-28 09:29 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-28 09:29 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-28 09:29 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-28 09:29 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-May-28 09:29 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-28 09:29 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-28 09:29 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-28 09:29 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-28 09:29 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-28 09:29 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-28 09:29 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-28 09:29 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-28 09:29 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:29 nucliadb/reader/py.typed
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-28 09:29 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-28 09:29 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-28 09:29 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13951 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-May-28 09:29 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-May-28 09:29 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-28 09:29 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-28 09:29 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-28 09:29 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-28 09:29 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-28 09:29 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-28 09:29 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-28 09:29 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-28 09:29 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-28 09:29 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-28 09:29 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-28 09:29 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:29 nucliadb/search/py.typed
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-28 09:29 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-28 09:29 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-28 09:29 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-28 09:29 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-28 09:29 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9493 b- defN 24-May-28 09:29 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-28 09:29 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-28 09:29 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-28 09:29 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-28 09:29 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-28 09:29 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-May-28 09:29 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-28 09:29 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-28 09:29 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-28 09:29 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-28 09:29 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-28 09:29 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-28 09:29 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-28 09:29 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-28 09:29 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-28 09:29 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-28 09:29 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-28 09:29 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-28 09:29 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-28 09:29 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-28 09:29 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-28 09:29 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-28 09:29 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-28 09:29 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-May-28 09:29 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-28 09:29 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-28 09:29 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-28 09:29 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-28 09:29 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-28 09:29 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-28 09:29 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-28 09:29 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-28 09:29 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-28 09:29 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-28 09:29 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-28 09:29 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-28 09:29 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-28 09:29 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-28 09:29 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-28 09:29 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-May-28 09:29 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-28 09:29 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-28 09:29 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-May-28 09:29 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:29 nucliadb/standalone/py.typed
+-rw-r--r--  2.0 unx     5636 b- defN 24-May-28 09:29 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-28 09:29 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-28 09:29 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-28 09:29 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-28 09:29 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-28 09:29 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-28 09:29 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-28 09:29 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-28 09:29 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-28 09:29 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-28 09:29 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-May-28 09:29 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-28 09:29 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-28 09:29 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-28 09:29 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-28 09:29 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-28 09:29 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-28 09:29 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-28 09:29 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-28 09:29 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-28 09:29 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-28 09:29 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-28 09:29 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-28 09:29 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-28 09:29 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-28 09:29 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-28 09:29 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-28 09:29 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-28 09:29 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-28 09:29 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-28 09:29 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-28 09:29 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-28 09:29 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-28 09:29 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-28 09:29 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-28 09:29 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-28 09:29 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-28 09:29 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-28 09:29 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-28 09:29 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-28 09:29 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-28 09:29 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-28 09:29 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-28 09:29 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-28 09:29 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-28 09:29 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-28 09:29 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-28 09:29 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-28 09:29 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-28 09:29 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-28 09:29 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-28 09:29 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-28 09:29 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-28 09:29 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-28 09:29 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-28 09:29 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-28 09:29 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-28 09:29 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:29 nucliadb/train/py.typed
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-28 09:29 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-28 09:29 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-28 09:29 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-28 09:29 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-28 09:29 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-28 09:29 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-28 09:29 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-28 09:29 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-28 09:29 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-28 09:29 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-28 09:29 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-28 09:29 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-28 09:29 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-28 09:29 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-28 09:29 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-28 09:29 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-28 09:29 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-28 09:29 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-28 09:29 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-28 09:29 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-28 09:29 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-28 09:29 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-28 09:29 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-28 09:29 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-28 09:29 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-28 09:29 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-28 09:29 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2201 b- defN 24-May-28 09:29 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-28 09:29 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-28 09:29 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-28 09:29 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-28 09:29 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-28 09:29 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-28 09:29 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-28 09:29 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-28 09:29 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-28 09:29 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-28 09:29 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-28 09:29 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-28 09:29 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-28 09:29 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19483 b- defN 24-May-28 09:29 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-28 09:29 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-28 09:29 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-28 09:29 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:29 nucliadb/writer/py.typed
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-28 09:29 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-28 09:29 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-28 09:29 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-28 09:29 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6421 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18628 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10216 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30985 b- defN 24-May-28 09:29 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-28 09:29 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-28 09:29 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-28 09:29 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-28 09:29 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16740 b- defN 24-May-28 09:29 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-28 09:29 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-28 09:29 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-28 09:29 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-28 09:29 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-28 09:29 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-28 09:29 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-28 09:29 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4400 b- defN 24-May-28 09:29 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16857 b- defN 24-May-28 09:29 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-28 09:29 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-28 09:29 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-28 09:29 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-28 09:29 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-28 09:29 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-28 09:29 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-28 09:29 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-28 09:29 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-28 09:29 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-28 09:29 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-28 09:29 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-28 09:29 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4474 b- defN 24-May-28 09:30 nucliadb-4.0.1.post550.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 09:30 nucliadb-4.0.1.post550.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-28 09:30 nucliadb-4.0.1.post550.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-28 09:30 nucliadb-4.0.1.post550.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-28 09:30 nucliadb-4.0.1.post550.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    43837 b- defN 24-May-28 09:30 nucliadb-4.0.1.post550.dist-info/RECORD
+468 files, 2261438 bytes uncompressed, 696269 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -267,14 +267,17 @@
 
 Filename: nucliadb/ingest/partitions.py
 Comment: 
 
 Filename: nucliadb/ingest/processing.py
 Comment: 
 
+Filename: nucliadb/ingest/py.typed
+Comment: 
+
 Filename: nucliadb/ingest/serialize.py
 Comment: 
 
 Filename: nucliadb/ingest/settings.py
 Comment: 
 
 Filename: nucliadb/ingest/utils.py
@@ -531,14 +534,17 @@
 
 Filename: nucliadb/reader/lifecycle.py
 Comment: 
 
 Filename: nucliadb/reader/openapi.py
 Comment: 
 
+Filename: nucliadb/reader/py.typed
+Comment: 
+
 Filename: nucliadb/reader/run.py
 Comment: 
 
 Filename: nucliadb/reader/api/__init__.py
 Comment: 
 
 Filename: nucliadb/reader/api/models.py
@@ -609,14 +615,17 @@
 
 Filename: nucliadb/search/openapi.py
 Comment: 
 
 Filename: nucliadb/search/predict.py
 Comment: 
 
+Filename: nucliadb/search/py.typed
+Comment: 
+
 Filename: nucliadb/search/run.py
 Comment: 
 
 Filename: nucliadb/search/settings.py
 Comment: 
 
 Filename: nucliadb/search/utilities.py
@@ -852,14 +861,17 @@
 
 Filename: nucliadb/standalone/migrations.py
 Comment: 
 
 Filename: nucliadb/standalone/purge.py
 Comment: 
 
+Filename: nucliadb/standalone/py.typed
+Comment: 
+
 Filename: nucliadb/standalone/run.py
 Comment: 
 
 Filename: nucliadb/standalone/settings.py
 Comment: 
 
 Filename: nucliadb/standalone/versions.py
@@ -1095,14 +1107,17 @@
 
 Filename: nucliadb/train/models.py
 Comment: 
 
 Filename: nucliadb/train/nodes.py
 Comment: 
 
+Filename: nucliadb/train/py.typed
+Comment: 
+
 Filename: nucliadb/train/run.py
 Comment: 
 
 Filename: nucliadb/train/servicer.py
 Comment: 
 
 Filename: nucliadb/train/settings.py
@@ -1239,14 +1254,17 @@
 
 Filename: nucliadb/writer/lifecycle.py
 Comment: 
 
 Filename: nucliadb/writer/openapi.py
 Comment: 
 
+Filename: nucliadb/writer/py.typed
+Comment: 
+
 Filename: nucliadb/writer/run.py
 Comment: 
 
 Filename: nucliadb/writer/settings.py
 Comment: 
 
 Filename: nucliadb/writer/utilities.py
@@ -1362,26 +1380,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.1.post548.dist-info/METADATA
+Filename: nucliadb-4.0.1.post550.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.1.post548.dist-info/WHEEL
+Filename: nucliadb-4.0.1.post550.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.1.post548.dist-info/entry_points.txt
+Filename: nucliadb-4.0.1.post550.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.1.post548.dist-info/top_level.txt
+Filename: nucliadb-4.0.1.post550.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.1.post548.dist-info/zip-safe
+Filename: nucliadb-4.0.1.post550.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.1.post548.dist-info/RECORD
+Filename: nucliadb-4.0.1.post550.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/train/tests/test_get_info.py

```diff
@@ -13,29 +13,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-import sys
-
 import pytest
 from aioresponses import aioresponses
 from nucliadb_protos.train_pb2 import GetInfoRequest, TrainInfo
 from nucliadb_protos.train_pb2_grpc import TrainStub
 
-VERSION = sys.version_info
-PY_GEQ_3_11 = VERSION.major > 3 or VERSION.major == 3 and VERSION.minor >= 11
-
 
 @pytest.mark.asyncio
-@pytest.mark.skipif(
-    PY_GEQ_3_11, reason="aioresponses not compatible with python 3.11 yet"
-)
 async def test_get_info(
     train_client: TrainStub, knowledgebox_ingest: str, test_pagination_resources
 ) -> None:
     req = GetInfoRequest()
     req.kb.uuid = knowledgebox_ingest
 
     with aioresponses() as m:
```

## nucliadb/train/tests/test_get_ontology_count.py

```diff
@@ -13,29 +13,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
-import sys
-
 import pytest
 from aioresponses import aioresponses
 from nucliadb_protos.train_pb2 import GetLabelsetsCountRequest, LabelsetsCount
 from nucliadb_protos.train_pb2_grpc import TrainStub
 
-VERSION = sys.version_info
-PY_GEQ_3_11 = VERSION.major > 3 or VERSION.major == 3 and VERSION.minor >= 11
-
 
 @pytest.mark.asyncio
-@pytest.mark.skipif(
-    PY_GEQ_3_11, reason="aioresponses not compatible with python 3.11 yet"
-)
 async def test_get_ontology_count(
     train_client: TrainStub, knowledgebox_ingest: str, test_pagination_resources
 ) -> None:
     req = GetLabelsetsCountRequest()
     req.kb.uuid = knowledgebox_ingest
 
     with aioresponses() as m:
```

## Comparing `nucliadb-4.0.1.post548.dist-info/METADATA` & `nucliadb-4.0.1.post550.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.1.post548
+Version: 4.0.1.post550
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -14,21 +14,22 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=4.0.1.post548
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.1.post548
-Requires-Dist: nucliadb-protos >=4.0.1.post548
-Requires-Dist: nucliadb-models >=4.0.1.post548
+Requires-Dist: nucliadb-telemetry[all] >=4.0.1.post550
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.1.post550
+Requires-Dist: nucliadb-protos >=4.0.1.post550
+Requires-Dist: nucliadb-models >=4.0.1.post550
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.1.post548.dist-info/entry_points.txt` & `nucliadb-4.0.1.post550.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.1.post548.dist-info/RECORD` & `nucliadb-4.0.1.post550.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 nucliadb/export_import/tasks.py,sha256=HptUd322AmFDrlXqXcHLD3UYzaeHA54PevbvWxhqZjo,2571
 nucliadb/export_import/utils.py,sha256=cNbbMy7JTyXXyNcS-SCGb-2hEW407igvYChXoo3mwr8,19401
 nucliadb/ingest/__init__.py,sha256=fsw3C38VP50km3R-nHL775LNGPpJ4JxqXJ2Ib1f5SqE,1011
 nucliadb/ingest/app.py,sha256=g51GuMZ9oLuIn8YZ7EKglVlLmu114VSmWzqMCbKtXRE,7277
 nucliadb/ingest/cache.py,sha256=w7jMMzamOmQ7gwXna6Dqm6isRNBVv6l5BTBlTxaYWjE,1005
 nucliadb/ingest/partitions.py,sha256=xhonCO-gqNO-8TlitjcmchVrxCLi-99SyOWvX4va1lE,2484
 nucliadb/ingest/processing.py,sha256=5UWQ8H_rBgDEmRYsiAI5CC9JPA_StMxhzRU8QKSs4bs,19904
+nucliadb/ingest/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/ingest/serialize.py,sha256=DM18fONnptJbUqSFQZl4kg33Q8S4GpJUqK432rzSHYU,20277
 nucliadb/ingest/settings.py,sha256=VrOfSSwadDb2LRl0rwlJl5DSiDILj03KSD-n0Jh4yaE,3207
 nucliadb/ingest/utils.py,sha256=dyFEv9V38OlkrQdM8_Xgii3YmbsRqNUoZeYApe39kx0,2314
 nucliadb/ingest/consumer/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/consumer/auditing.py,sha256=P6a7HgEJVE5WBJuyL7Q2avuqLqQ5QE3VaxoifS3YT3k,6918
 nucliadb/ingest/consumer/consumer.py,sha256=bJgVt1G7RchZrHX-5ykG2uHfGNY_HEjsLE2ZsgAv8HA,12174
 nucliadb/ingest/consumer/materializer.py,sha256=Zoe7DEks14nRvXFSLiBMzF6yKMq1v2TABNtOo0PsT1Q,3945
@@ -173,14 +174,15 @@
 nucliadb/models/responses.py,sha256=qnuOoc7TrVSUnpikfTwHLKez47_DE4mSFzpxrwtqijA,1599
 nucliadb/purge/__init__.py,sha256=IHnoGcbASPUQ74ewbPtHiOnUbRXfB92-aDH4sUYALTQ,6041
 nucliadb/purge/orphan_shards.py,sha256=tGFlF7-RLDHv2XPc5J_1lgBvBCM5UjUtUNUmpodGqBc,9364
 nucliadb/reader/__init__.py,sha256=TxsAOWhRnz9l8DuFy-Qfv0I5HrzrysaxtAzogg6FQB8,1328
 nucliadb/reader/app.py,sha256=dyvTCnVwXD3gVsk09tUB63N6hL-fS9q_S-AsI3zpFkk,3709
 nucliadb/reader/lifecycle.py,sha256=45NGAjNyi01Emi14Eh5GYBScS5N7yJbs2r1R2P-usSg,1366
 nucliadb/reader/openapi.py,sha256=ZwXYXZPYpxQL68HyWI310YnmMKJMzBUtYe-r9OSbN8I,1031
+nucliadb/reader/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/reader/run.py,sha256=AR-iCnON3YVXgI5-KEgg99G4KAPN1BKXDg7nr4dgoDA,1447
 nucliadb/reader/api/__init__.py,sha256=c-UD29C0FVzQDGEvslebDCKtvnyEcAbiDd-3Q_QgGN4,872
 nucliadb/reader/api/models.py,sha256=dBDxZf_LnZFzKIKB_Oaj1B2pccAhrwviJn8KAhxJzwY,2458
 nucliadb/reader/api/v1/__init__.py,sha256=81AhxhYJcni8K_a5apWfL8Dnj4Mf_EznIsFse7jN-gQ,1110
 nucliadb/reader/api/v1/download.py,sha256=ZO_KjjF9qM4K_xcEW7c1S0ZnieGkhv3Yu2E4kSU9F_s,12392
 nucliadb/reader/api/v1/export_import.py,sha256=nBYEwFnKUJYsiXUlbfKIL_jI9Ec5UVZE-2fCbK1rfQk,6459
 nucliadb/reader/api/v1/knowledgebox.py,sha256=Pd71iqTVRgx5u_Gb2LegDTQ3gGTKbVLsAvgcZne5_lM,3641
@@ -199,14 +201,15 @@
 nucliadb/reader/tests/test_reader_resource.py,sha256=A7XzHngspJxPqxzyMZ2Zg2Kp8SuDTi78Fo2rG1roLyo,10586
 nucliadb/reader/tests/test_reader_resource_field.py,sha256=YQ-U2mEGhs_rPGxcWPZmWLSEoCxBo3AVDtLZCtZrGb8,6535
 nucliadb/search/__init__.py,sha256=fwzdF6p7p9uDCtE38gTUxrRVIdbEDVQTAXWUMVKgSBM,1535
 nucliadb/search/app.py,sha256=azMj8BiaFr03pYQKcWSr2YqjB0FopJDeVKE2wwuj6pU,4905
 nucliadb/search/lifecycle.py,sha256=s6If2a78dcv4_71d-Q_uA6b9TaJCQOASUhqa2HcxfIw,1956
 nucliadb/search/openapi.py,sha256=t3Wo_4baTrfPftg2BHsyLWNZ1MYn7ZRdW7ht-wFOgRs,1016
 nucliadb/search/predict.py,sha256=F-EuRp00Q2wb5Ut1srXeomoY_JW_y-LEB0aKPU8Cf-Y,20665
+nucliadb/search/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/search/run.py,sha256=aFb-CXRi_C8YMpP_ivNj8KW1BYhADj88y8K9Lr_nUPI,1402
 nucliadb/search/settings.py,sha256=Nm4BkdNNdYfU1wGvvWMvlazRSlRGoae99GEdm48-bXI,1193
 nucliadb/search/utilities.py,sha256=9SsRDw0rJVXVoLBfF7rBb6q080h-thZc7u8uRcTiBeY,1037
 nucliadb/search/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/api/v1/__init__.py,sha256=FR4pbt1XyWQAS3TAiAhvOQb0kWSsZpmzL87JJMcAoMc,1298
 nucliadb/search/api/v1/ask.py,sha256=JRHdcMnOOSfB6nWY2TnVes0FXriumbT30_wI1IbfCyE,3534
 nucliadb/search/api/v1/chat.py,sha256=UsSgWBNRrBqf--gDnKvcbE3Qcx184QOwbAeGHnXL4s4,9493
@@ -280,14 +283,15 @@
 nucliadb/standalone/app.py,sha256=AVojB5tQE3K2I9hPxHgd06At2ofyclJti4JS1g5_Y5c,5763
 nucliadb/standalone/auth.py,sha256=bglXXYH7F3TWR5d8qrJq0VgVYb63mQCJJU4vQy8hMdQ,7800
 nucliadb/standalone/config.py,sha256=Np6pIpOY7Yi5gLf73yLcdxSaMwZtJwWVlPzcEcCR4m8,5313
 nucliadb/standalone/introspect.py,sha256=KJ91JYGaxMJ62lNe6Ji9NFfyEyks6lVJcGTmqfPjtp0,6986
 nucliadb/standalone/lifecycle.py,sha256=6cCkiXwom7LppzKoG_vRuW5Ubw_YsLuVChHlCqnhts8,2488
 nucliadb/standalone/migrations.py,sha256=wmdxORbqIzs7Zo4240sssVjFt3csCWRyTntJVbVvKec,1980
 nucliadb/standalone/purge.py,sha256=FzyO3P3wIcBrvg3Apknim_jcol3Ku2Zi_YTHdaELwxU,1322
+nucliadb/standalone/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/standalone/run.py,sha256=N-ADOERD_tSlMWGNkGupYgZc6dgudpxDoCbGhz_zxNg,5636
 nucliadb/standalone/settings.py,sha256=LmjaLrhpbPpEaCb64gUNSMSb1aOJJHBu2qpiYYm6hmw,5822
 nucliadb/standalone/versions.py,sha256=uA_jIpdu4gPM04kPx6C8xNL9d-uaItlMjCxXNzQ_1_k,3132
 nucliadb/standalone/static/favicon.ico,sha256=96pKGp6Sx457JkTfjy1dtApMhkitixfU6invCUGAYOU,2285
 nucliadb/standalone/static/index.html,sha256=PEZfuEQFYnYACAL1ceN8xC0im8lBrUx838RkE8tbvgA,3833
 nucliadb/standalone/static/logo.svg,sha256=-wQqSvPGTdlKjUP6pHE6kiq005pgYjDzp9nPl0X71Mk,2639
 nucliadb/standalone/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -361,14 +365,15 @@
 nucliadb/tests/utils/broker_messages/helpers.py,sha256=RGJ2YZ34ZU7ENsCUPVpFDkNEpxv9v45FYIvPVePML7o,1196
 nucliadb/train/__init__.py,sha256=qdZ6DeuwED8iIl32NVyDYWTy544FyHCZUQnQGnms604,1325
 nucliadb/train/app.py,sha256=3AucXVUiDFueskmw85nO22fu9YjRyZIU1yhGlh0jVOE,3530
 nucliadb/train/generator.py,sha256=zmoffpYvc6u3gk6cPXKcKPf0KKpMibu6xWnwDs143bQ,3800
 nucliadb/train/lifecycle.py,sha256=ZLqCl_IjFimon9pl3OJyF2UM4Jky_xsHuqilnrJj1as,1698
 nucliadb/train/models.py,sha256=BmgmMjDsu_1Ih5JDAqo6whhume90q0ASJcDP9dkMQm8,1198
 nucliadb/train/nodes.py,sha256=IIO0ub7yn47pAooVGpTBvk_bxdF0Rn9G21ZnbwR_bww,5706
+nucliadb/train/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/train/run.py,sha256=evz6CKVfJOzkbHMoaYz2mTMlKjJnNOb1O8zBBWMpeBw,1400
 nucliadb/train/servicer.py,sha256=b889xt0XiTOVpAPjK0AElJW3gJ7aV-55TQFbxdQe0MI,5926
 nucliadb/train/settings.py,sha256=eXe87TjqtGTa-bCKRPDIWdyb7qsaUW3VbLXV-zGBQZk,1415
 nucliadb/train/types.py,sha256=M3olA6vBosVs7L5QpzlxiFhuF3_vQhSkdlgClQzXjaQ,1496
 nucliadb/train/upload.py,sha256=Sz8KDXqFMD8reFw-8mb11il7Ab4onKcH0MPsZ1AbYUk,3265
 nucliadb/train/uploader.py,sha256=JEdZ6ozdFuKC_DmimljKnnH0gz2Nu-HxMFzjLa3gmkg,6420
 nucliadb/train/utils.py,sha256=Xoz7LjSWRfFNSHyZF-eK9DmWf9sgjyJXdYPppc3BE_c,3179
@@ -389,17 +394,17 @@
 nucliadb/train/generators/token_classifier.py,sha256=G7pE49c63P7bQJGSnTxz_GlMYhlfebO-pjz32l8WeB4,10446
 nucliadb/train/generators/utils.py,sha256=I-P_KV4HdILOpaPK3cdKP0iT2QzBfSNvuMdewyiIqpg,3877
 nucliadb/train/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/train/tests/conftest.py,sha256=8FfoA1iXscmNtHRXWDEGhMxLLqfjx3JUX3xrTaYXIAE,1125
 nucliadb/train/tests/fixtures.py,sha256=GBb19QpemIp8FL1_zLYiCtCYin0MRtHDJ8Tn1HMmVdU,11053
 nucliadb/train/tests/test_field_classification.py,sha256=rFhJKVJsPGLFTKMKuHMA9vWwtLrHixlC3DNg66Zx3vM,4598
 nucliadb/train/tests/test_get_entities.py,sha256=ndcEemTcITB70X_GxSIkUiAoNOnpTamfyPaXVtXmgKQ,2729
-nucliadb/train/tests/test_get_info.py,sha256=YG6y7MYbSPwUQW_n-137wxayIxlPZplkK71F2SR_nOQ,1876
+nucliadb/train/tests/test_get_info.py,sha256=uWKFC8uDXsmdzUp0xgNpEEuf5Ge9dNPE5CSfdZSDz_o,1660
 nucliadb/train/tests/test_get_ontology.py,sha256=Xjr-eIYQLzNkqFU3nwANmDi4fwY09VymdikC3ibgM8A,1382
-nucliadb/train/tests/test_get_ontology_count.py,sha256=K6XXI-4QNacOW2HioMTdC1YOMUTeHXb_aTvgGLTF9ck,2417
+nucliadb/train/tests/test_get_ontology_count.py,sha256=hyarvQOw5PyeYVJ7Z6v4I1Yagi0PwrEiIs615tsM4Z8,2201
 nucliadb/train/tests/test_image_classification.py,sha256=wegtn1V8ZS4HAkiQzOiQ-xs_W42DxG2xvB1NAofY7nQ,7669
 nucliadb/train/tests/test_list_fields.py,sha256=V6YS2ao09AiheI6GKaC9GVLUG_ypf-WrvId_mRdBJB8,1416
 nucliadb/train/tests/test_list_paragraphs.py,sha256=fvDh-vvgTj-XonTS8t9CDq0eDGgNl8iWw3E9OBmGK7c,2944
 nucliadb/train/tests/test_list_resources.py,sha256=QkrsRzRHAWHyJHEtSsrr0xOtrALtiUasSvoPHcjHsCc,1423
 nucliadb/train/tests/test_list_sentences.py,sha256=__4bq6Jmig-wr2LJQHjRZ8QxywNgc4EbDDtzeN0Gt7k,2947
 nucliadb/train/tests/test_paragraph_classification.py,sha256=_d2z8hxGBcdszBc4vIg-WyEnBR_QJQjhcVGyvsHBcuc,4645
 nucliadb/train/tests/test_paragraph_streaming.py,sha256=CMwGEDBQ3iwf7pldZfOBphFSYCvTLKPd1dDHgoHtslQ,4320
@@ -409,14 +414,15 @@
 nucliadb/train/tests/utils.py,sha256=J5UZoCz4Ss5b6SmZuyC7jJQlomQE8mDQ8E2OdYEV-gA,3324
 nucliadb/writer/__init__.py,sha256=HkfMuQR3CbbPU3g-A85Ibt8iwSTTADhLc0-pi3F3hvk,1328
 nucliadb/writer/app.py,sha256=Q55CmGR85wG5pjf_Ro-73QVWc7_wMpIt69xJSZ0kjCQ,4268
 nucliadb/writer/back_pressure.py,sha256=0aM0VRVpaBXArtFPekC8iCnIATwroQkFcYmN3OERgVA,19483
 nucliadb/writer/exceptions.py,sha256=2dMvuoF68v3BZuyzaBEsbG6gusQqwLFcn47qm1zNdTc,972
 nucliadb/writer/lifecycle.py,sha256=gF9it0w98uBGCwzjs72e8mGi6H-qv_XAa2GGNBTOEDY,1953
 nucliadb/writer/openapi.py,sha256=thqCO1ht_RJgOkXs-aIsv8aXJrU5z8wo2n05l2_LqMs,1032
+nucliadb/writer/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/writer/run.py,sha256=euVZ_rtHDXs-O1kB-Pt1Id8eft9CYVpWH3zJzEoEqls,1448
 nucliadb/writer/settings.py,sha256=EGY6ZKg-BTKD0xPRIam7EN_FxAQEU_eb5ywNCQOQEg0,3103
 nucliadb/writer/utilities.py,sha256=AZ5qEny1Xm0IDsFtH13oJa2usvJZK8f0FdgF1LrnLCw,1036
 nucliadb/writer/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/api/constants.py,sha256=b63uWvu7_bwg51R6EL5DaJwoT550Ih4GhVXzvEYLQNQ,1429
 nucliadb/writer/api/v1/__init__.py,sha256=FVn7N9VJ6bsEoy4TRnkclr4Umd5hECiwPXVqRnJ8BME,1095
 nucliadb/writer/api/v1/export_import.py,sha256=9Gqxq1EAPOXCX80F2G7s0UVkvMV1Kgwo66o5sHn2KGY,6421
@@ -450,13 +456,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.1.post548.dist-info/METADATA,sha256=sv6UaaSHLgmh8-dinga_jMF4TTYyvcU1KEcnHJolRJo,4423
-nucliadb-4.0.1.post548.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.1.post548.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.1.post548.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.1.post548.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.1.post548.dist-info/RECORD,,
+nucliadb-4.0.1.post550.dist-info/METADATA,sha256=U36tLcJVoZc5DR0y6r9T4wscGg9zOpJVx1wsRbZwmuI,4474
+nucliadb-4.0.1.post550.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.1.post550.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.1.post550.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.1.post550.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.1.post550.dist-info/RECORD,,
```

