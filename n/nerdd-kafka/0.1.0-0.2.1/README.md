# Comparing `tmp/nerdd-kafka-0.1.0.tar.gz` & `tmp/nerdd_kafka-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdd-kafka-0.1.0.tar", last modified: Mon Dec 11 13:01:56 2023, max compression
+gzip compressed data, was "nerdd_kafka-0.2.1.tar", last modified: Tue May 28 12:19:18 2024, max compression
```

## Comparing `nerdd-kafka-0.1.0.tar` & `nerdd_kafka-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-12-11 13:01:56.990883 nerdd-kafka-0.1.0/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1085 2023-12-10 20:08:42.000000 nerdd-kafka-0.1.0/LICENSE
--rw-r--r--   0 hirte     (1000) hirte     (1000)     1999 2023-12-11 13:01:56.990883 nerdd-kafka-0.1.0/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1092 2023-12-11 12:56:04.000000 nerdd-kafka-0.1.0/README.md
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-12-11 13:01:56.990883 nerdd-kafka-0.1.0/nerdd_kafka/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       28 2023-12-10 20:10:18.000000 nerdd-kafka-0.1.0/nerdd_kafka/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2141 2023-12-10 23:23:33.000000 nerdd-kafka-0.1.0/nerdd_kafka/__main__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     7798 2023-12-11 12:06:45.000000 nerdd-kafka-0.1.0/nerdd_kafka/kafka_server.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-12-11 13:01:56.990883 nerdd-kafka-0.1.0/nerdd_kafka/serialization/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      182 2023-10-18 13:09:43.000000 nerdd-kafka-0.1.0/nerdd_kafka/serialization/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      221 2023-10-18 13:50:03.000000 nerdd-kafka-0.1.0/nerdd_kafka/serialization/json_encoder.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1088 2023-10-18 12:24:03.000000 nerdd-kafka-0.1.0/nerdd_kafka/serialization/mol_serializer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      264 2023-10-18 12:27:30.000000 nerdd-kafka-0.1.0/nerdd_kafka/serialization/registry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      332 2023-10-18 12:30:38.000000 nerdd-kafka-0.1.0/nerdd_kafka/serialization/serializer.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-12-11 13:01:56.990883 nerdd-kafka-0.1.0/nerdd_kafka.egg-info/
--rw-r--r--   0 hirte     (1000) hirte     (1000)     1999 2023-12-11 13:01:56.000000 nerdd-kafka-0.1.0/nerdd_kafka.egg-info/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      685 2023-12-11 13:01:56.000000 nerdd-kafka-0.1.0/nerdd_kafka.egg-info/SOURCES.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-12-11 13:01:56.000000 nerdd-kafka-0.1.0/nerdd_kafka.egg-info/dependency_links.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       63 2023-12-11 13:01:56.000000 nerdd-kafka-0.1.0/nerdd_kafka.egg-info/entry_points.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      226 2023-12-11 13:01:56.000000 nerdd-kafka-0.1.0/nerdd_kafka.egg-info/requires.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       12 2023-12-11 13:01:56.000000 nerdd-kafka-0.1.0/nerdd_kafka.egg-info/top_level.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-12-11 13:01:56.990883 nerdd-kafka-0.1.0/setup.cfg
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1477 2023-12-11 13:01:41.000000 nerdd-kafka-0.1.0/setup.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-12-11 13:01:56.990883 nerdd-kafka-0.1.0/tests/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1408 2023-11-27 12:54:21.000000 nerdd-kafka-0.1.0/tests/test_backup.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2317 2023-11-17 11:11:05.000000 nerdd-kafka-0.1.0/tests/test_kafka_server_atom_property_predictor.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      981 2023-11-17 11:11:31.000000 nerdd-kafka-0.1.0/tests/test_kafka_server_initialization.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      430 2023-11-17 11:11:38.000000 nerdd-kafka-0.1.0/tests/test_kafka_server_molecule_property_predictor.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 12:19:18.706179 nerdd_kafka-0.2.1/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1085 2023-12-10 20:08:42.000000 nerdd_kafka-0.2.1/LICENSE
+-rw-r--r--   0 hirte     (1000) hirte     (1000)     2192 2024-05-28 12:19:18.706179 nerdd_kafka-0.2.1/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1092 2023-12-11 12:56:04.000000 nerdd_kafka-0.2.1/README.md
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 12:19:18.706179 nerdd_kafka-0.2.1/nerdd_kafka/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       28 2023-12-10 20:10:18.000000 nerdd_kafka-0.2.1/nerdd_kafka/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1788 2024-05-28 10:02:53.000000 nerdd_kafka-0.2.1/nerdd_kafka/__main__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)    10574 2024-05-28 12:01:48.000000 nerdd_kafka-0.2.1/nerdd_kafka/kafka_server.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 12:19:18.706179 nerdd_kafka-0.2.1/nerdd_kafka/serialization/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      182 2024-03-27 12:42:24.000000 nerdd_kafka-0.2.1/nerdd_kafka/serialization/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      235 2024-03-27 12:43:54.000000 nerdd_kafka-0.2.1/nerdd_kafka/serialization/json_encoder.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2232 2024-01-27 19:55:15.000000 nerdd_kafka-0.2.1/nerdd_kafka/serialization/mol_serializer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      264 2023-10-18 12:27:30.000000 nerdd_kafka-0.2.1/nerdd_kafka/serialization/registry.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      332 2023-10-18 12:30:38.000000 nerdd_kafka-0.2.1/nerdd_kafka/serialization/serializer.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 12:19:18.706179 nerdd_kafka-0.2.1/nerdd_kafka.egg-info/
+-rw-r--r--   0 hirte     (1000) hirte     (1000)     2192 2024-05-28 12:19:18.000000 nerdd_kafka-0.2.1/nerdd_kafka.egg-info/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      800 2024-05-28 12:19:18.000000 nerdd_kafka-0.2.1/nerdd_kafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2024-05-28 12:19:18.000000 nerdd_kafka-0.2.1/nerdd_kafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       63 2024-05-28 12:19:18.000000 nerdd_kafka-0.2.1/nerdd_kafka.egg-info/entry_points.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      297 2024-05-28 12:19:18.000000 nerdd_kafka-0.2.1/nerdd_kafka.egg-info/requires.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       18 2024-05-28 12:19:18.000000 nerdd_kafka-0.2.1/nerdd_kafka.egg-info/top_level.txt
+-rw-r--r--   0 hirte     (1000) hirte     (1000)       38 2024-05-28 12:19:18.706179 nerdd_kafka-0.2.1/setup.cfg
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1632 2024-05-27 14:37:26.000000 nerdd_kafka-0.2.1/setup.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 12:19:18.706179 nerdd_kafka-0.2.1/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        0 2024-03-24 11:23:22.000000 nerdd_kafka-0.2.1/tests/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      281 2024-05-28 12:09:19.000000 nerdd_kafka-0.2.1/tests/conftest.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 12:19:18.706179 nerdd_kafka-0.2.1/tests/steps/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       76 2024-05-28 12:08:52.000000 nerdd_kafka-0.2.1/tests/steps/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     4311 2024-05-28 12:02:25.000000 nerdd_kafka-0.2.1/tests/steps/mocked_kafka.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1499 2024-03-24 11:54:16.000000 nerdd_kafka-0.2.1/tests/steps/molecules.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1519 2024-05-28 11:54:17.000000 nerdd_kafka-0.2.1/tests/steps/records.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2317 2023-11-17 11:11:05.000000 nerdd_kafka-0.2.1/tests/test_kafka_server_atom_property_predictor.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      981 2024-05-28 10:57:40.000000 nerdd_kafka-0.2.1/tests/test_kafka_server_initialization.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      395 2024-05-28 10:52:48.000000 nerdd_kafka-0.2.1/tests/test_kafka_server_molecule_property_predictor.py
```

### Comparing `nerdd-kafka-0.1.0/LICENSE` & `nerdd_kafka-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nerdd-kafka-0.1.0/PKG-INFO` & `nerdd_kafka-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: nerdd-kafka
-Version: 0.1.0
+Version: 0.2.1
 Summary: Run a NERDD module as a Kafka service
-Home-page: https://gitlab.phaidra.org/comp3d/nerdd-kafka
+Home-page: https://github.com/molinfo-vienna/nerdd-kafka
 Maintainer: Steffen Hirte
 Maintainer-email: steffen.hirte@univie.ac.at
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdkit>=2022.3.3
 Requires-Dist: kafka-python==2.0.2
+Requires-Dist: nerdd-module>=0.2.0
 Requires-Dist: pandas>=1.2.1
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: filetype~=1.2.0
 Requires-Dist: rich-click>=1.7.1
 Requires-Dist: stringcase~=1.2.0
+Requires-Dist: numpy
+Requires-Dist: simplejson>=3
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-bdd; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-watch; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: hypothesis-rdkit; extra == "test"
+Provides-Extra: docs
+Requires-Dist: mkdocs; extra == "docs"
+Requires-Dist: mkdocs-material; extra == "docs"
 
 # NERDD Kafka
 
 Run a [NERDD module](https://github.com/molinfo-vienna/nerdd-module) as a Kafka 
 service that consumes input molecules and produces prediction tuples.
```

### Comparing `nerdd-kafka-0.1.0/README.md` & `nerdd_kafka-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nerdd-kafka-0.1.0/nerdd_kafka/__main__.py` & `nerdd_kafka-0.2.1/nerdd_kafka/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from importlib import import_module
 
 import rich_click as click
-from stringcase import spinalcase
 
-from .kafka_server import run_server
+from .kafka_server import KafkaServer
 
 logger = logging.getLogger(__name__)
 
 
 @click.command(context_settings={"show_default": True})
 @click.argument(
     "model-name",
@@ -18,70 +17,53 @@
 )
 @click.option(
     "--batch-size",
     default=100,
     help="The batch size that are efficiently processable by this model.",
 )
 @click.option(
-    "--job-type",
-    default=None,
-    help=(
-        "The job type this module accepts. If not specified, it will be inferred "
-        "from the model name."
-    ),
-)
-@click.option(
-    "--input-topic",
-    default=None,
-    help="The Kafka topic this server will obtain its tasks from.",
-)
-@click.option(
     "--log-level",
-    default="warning",
+    default="info",
     type=click.Choice(
         ["debug", "info", "warning", "error", "critical"], case_sensitive=False
     ),
     help="The logging level.",
 )
 def main(
     model_name: str,
     broker_url: str,
-    job_type: str,
-    input_topic: str,
     batch_size: int,
     log_level: str,
 ):
     logging.basicConfig(level=log_level.upper())
 
-    # model name
     package_name, class_name = model_name.rsplit(".", 1)
 
-    # job type
-    if job_type is None:
-        if class_name.endswith("Model"):
-            # remove the "Model" suffix and convert to spinal case
-            # e.g. SkinDoctorModel -> skin-doctor
-            job_type = spinalcase(class_name[: -len("Model")])
-        else:
-            job_type = spinalcase(class_name)
-
-    # input topic
-    if input_topic is None:
-        input_topic = f"{job_type}-inputs"
-
     package = import_module(package_name)
     Model = getattr(package, class_name)
     model = Model()
 
+    config = model.get_config().get_dict()
+    name = config.get("name", class_name)
+
+    # create job_type identifier from name by
+    # * converting to lowercase and
+    # * removing all characters except dash and alphanumeric characters
+    job_type = name.lower()
+    job_type = "".join([c for c in job_type if str.isalnum(c) or c == "-"])
+
+    # input topic is the job type with "-inputs" appended
+    input_topic = f"{job_type}-inputs"
+
     logger.info(
-        f"Running server using model {model_name} on {job_type} with input "
+        f"Running server using model {model_name} with job type {job_type} and input "
         f"topic {input_topic}. Using a batch size of {batch_size}. Connecting to "
         f"broker {broker_url}."
     )
 
-    run_server(
+    KafkaServer().start(
         model,
         job_type,
         broker_url,
         input_topic,
         batch_size=batch_size,
     )
```

### Comparing `nerdd-kafka-0.1.0/nerdd_kafka/kafka_server.py` & `nerdd_kafka-0.2.1/nerdd_kafka/kafka_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,214 +1,266 @@
-import json
 import logging
 from collections import defaultdict
+from threading import Event
 
+import simplejson as json
 from nerdd_module.abstract_model import AbstractModel
 from rdkit.Chem import MolToSmiles
 
 from .serialization import ComplexJsonEncoder
 
 logger = logging.getLogger(__name__)
 
-__all__ = ["run_server"]
+__all__ = ["KafkaServer"]
 
 
-def run_server(
-    model: AbstractModel,
-    job_type: str,
-    broker: str,
-    input_topic: str,
-    batch_size: int = 100,
-):
-    # we want to be able to mock KafkaConsumer and KafkaProducer in tests
-    # --> only import them here
-    from kafka import KafkaConsumer, KafkaProducer
-
-    logger.info("Start Kafka Consumer")
-    consumer = KafkaConsumer(
-        input_topic,
-        bootstrap_servers=[broker],
-        api_version=(3, 3, 1),
-        auto_offset_reset="earliest",
-        group_id=f"{job_type}-consumer-group",
-        enable_auto_commit=False,
-        max_poll_records=batch_size,
-    )
-
-    producer = KafkaProducer(
-        bootstrap_servers=[broker],
-        api_version=(3, 3, 1),
-        max_request_size=10 * 1024 * 1024,  # 10 MB
-    )
-
-    #
-    # send the initialization message
-    #
-    config = model.get_config()
-
-    config_dict = config.get_dict()
-
-    assert "name" in config_dict, "name is missing in config"
-
-    init_message = {
-        "type": "init",
-        "name": config_dict["name"],
-        "config": config_dict,
-    }
-
-    producer.send("modules", json.dumps(init_message).encode("utf-8")).get()
-
-    #
-    # identify the type of this module
-    #
-    module_type = config.get_module_type()
-
-    #
-    # check which columns of the predictions should be included in messages
-    # specifically, atom or derivative properties are sent in separate messages
-    #
-    default_molecule_columns = [
-        "job_id",
-        "job_type",
-        "mol_id",
-        "input_mol",
-        "input",
-        "input_type",
-        "name",
-        "input_smiles",
-        "preprocessed_smiles",
-        "errors",
-    ]
-
-    default_atom_columns = ["job_id", "job_type", "mol_id", "atom_id"]
-
-    default_derivative_columns = ["job_id", "job_type", "mol_id", "derivative_id"]
-
-    molecular_property_columns = (
-        default_molecule_columns + config.molecular_property_columns()
-    )
-    atom_property_columns = default_atom_columns + config.atom_property_columns()
-    derivative_property_columns = (
-        default_derivative_columns + config.derivative_property_columns()
-    )
-
-    #
-    # receive and process messages
-    #
-    while True:
-        # we use polling (instead of iterating through the consumer messages) to
-        # be able to process batches of messages at once (ML models love batches)
-        messages = consumer.poll(timeout_ms=1000)
-
-        if messages:
-            logger.info(f"Received {len(messages)} messages")
-
-            # A model can only process batches with the same model parameters (e.g.
-            # CYPstrate needs a constant prediction_mode for all molecules in a batch).
-            # --> partition messages into buckets by job-id and input-type
-            try:
-                job_messages = defaultdict(list)
-                for _, message_list in messages.items():
-                    for message in message_list:
-                        message_obj = json.loads(message.value)
-                        job_id = message_obj["job_id"]
-                        input_type = message_obj["input_type"]
-                        key = f"{job_id}-{input_type}"
-                        job_messages[key].append(message_obj)
-            except Exception as e:
-                logger.error("Error partitioning messages", exc_info=e)
-                continue
-
-            for _, message_list in job_messages.items():
+class KafkaServer:
+    def __init__(self):
+        self._stopped = Event()
+
+    def stop(self):
+        self._stopped.set()
+
+    def start(
+        self,
+        model: AbstractModel,
+        job_type: str,
+        broker: str,
+        input_topic: str,
+        batch_size: int = 100,
+    ):
+        self._stopped.clear()
+        # we want to be able to mock KafkaConsumer and KafkaProducer in tests
+        # --> only import them here
+        from kafka import KafkaConsumer, KafkaProducer
+
+        logger.info("Start Kafka Consumer")
+        consumer = KafkaConsumer(
+            input_topic,
+            bootstrap_servers=[broker],
+            api_version=(3, 3, 1),
+            auto_offset_reset="earliest",
+            group_id=f"{job_type}-consumer-group",
+            enable_auto_commit=False,
+            max_poll_records=batch_size,
+        )
+
+        producer = KafkaProducer(
+            bootstrap_servers=[broker],
+            api_version=(3, 3, 1),
+            max_request_size=10 * 1024 * 1024,  # 10 MB
+        )
+
+        #
+        # send the initialization message
+        #
+        config = model.get_config()
+
+        config_dict = config.get_dict()
+
+        assert "name" in config_dict, "name is missing in config"
+
+        init_message = {
+            "type": "init",
+            "name": config_dict["name"],
+            "config": config_dict,
+        }
+
+        producer.send("modules", json.dumps(init_message).encode("utf-8")).get()
+
+        #
+        # identify the type of this module
+        #
+        module_type = config.get_module_type()
+
+        #
+        # check which columns of the predictions should be included in messages
+        # specifically, atom or derivative properties are sent in separate messages
+        #
+        default_molecule_columns = [
+            "job_id",
+            "job_type",
+            "mol_id",
+            "input_mol",
+            "input",
+            "input_type",
+            "name",
+            "source",
+            "input_smiles",
+            "preprocessed_smiles",
+            "errors",
+        ]
+
+        default_atom_columns = ["job_id", "job_type", "mol_id", "atom_id"]
+
+        default_derivative_columns = ["job_id", "job_type", "mol_id", "derivative_id"]
+
+        molecular_property_columns = (
+            default_molecule_columns + config.molecular_property_columns()
+        )
+        atom_property_columns = default_atom_columns + config.atom_property_columns()
+        derivative_property_columns = (
+            default_derivative_columns + config.derivative_property_columns()
+        )
+
+        #
+        # receive and process messages
+        #
+        while not self._stopped.is_set():
+            # we use polling (instead of iterating through the consumer messages) to
+            # be able to process batches of messages at once (ML models love batches)
+            messages = consumer.poll(timeout_ms=1000)
+
+            if messages:
+                logger.info(f"Received {len(messages)} messages")
+
+                # A model can only process batches with the same model parameters (e.g.
+                # CYPstrate needs a constant prediction_mode for all molecules in a batch).
+                # --> partition messages into buckets by job-id and input-type
                 try:
-                    first_message = message_list[0]
-                    assert "job_id" in first_message, "job_id is missing"
-                    assert "job_type" in first_message, "job_type is missing"
-                    assert "input_type" in first_message, "input_type is missing"
-                    assert (
-                        first_message["job_type"] == job_type
-                    ), f"job_type is not {job_type}"
-
-                    job_id = first_message["job_id"]
-                    input_type = first_message["input_type"]
-                    params = first_message["params"]
-
-                    logger.info(
-                        f"Processing part of job {job_id} with a batch size of "
-                        f"{len(message_list)} molecules"
-                    )
-
-                    logger.info(f"Predicting molecules given as {input_type}")
-                    results = model.predict(
-                        [message["raw_input"] for message in message_list],
-                        input_type=input_type,
-                        **params,
-                    )
-
-                    logger.info(f"Produced results: {len(results)}")
-
-                    results["job_id"] = job_id
-                    results["job_type"] = job_type
-
-                    # map mol_id (ranging from 0 to n) to the original mol_id provided
-                    # in the field mol_id of each message in message_list
-                    results["mol_id"] = [
-                        message_list[mol_id]["mol_id"] for mol_id in results["mol_id"]
-                    ]
-
-                    def _to_smiles(mol):
-                        if mol is None:
-                            return None
-                        else:
-                            return MolToSmiles(mol)
-
-                    results["input_smiles"] = results.input_mol.map(_to_smiles)
-                    results["preprocessed_smiles"] = results.preprocessed_mol.map(
-                        _to_smiles
-                    )
-
-                    #
-                    # send results to output topic
-                    #
-
-                    # send molecule properties
-                    results_molecule = (
-                        results[molecular_property_columns]
-                        .drop_duplicates(subset="mol_id")
-                        .to_dict("records")
-                    )
-                    for entry in results_molecule:
-                        producer.send(
-                            "results",
-                            json.dumps(entry, cls=ComplexJsonEncoder).encode("utf-8"),
-                        ).get()
-
-                    # optionally send atom properties
-                    if module_type == "atom_property_predictor":
-                        results_atom = results[results.atom_id.notnull()][
-                            atom_property_columns
-                        ].to_dict("records")
-                        for entry in results_atom:
-                            producer.send(
-                                "results",
-                                json.dumps(entry, cls=ComplexJsonEncoder).encode(
-                                    "utf-8"
-                                ),
-                            ).get()
+                    job_messages = defaultdict(list)
+                    for _, message_list in messages.items():
+                        for message in message_list:
+                            message_obj = json.loads(message.value)
+                            job_id = message_obj["job_id"]
+                            input_type = message_obj["input_type"]
+                            key = f"{job_id}-{input_type}"
+                            job_messages[key].append(message_obj)
+                except Exception as e:
+                    logger.error("Error partitioning messages", exc_info=e)
+                    continue
 
-                    # optionally send derivative properties
-                    if module_type == "derivative_property_predictor":
-                        results_derivative = results[results.derivative_id.notnull()][
-                            derivative_property_columns
-                        ].to_dict("records")
-                        for entry in results_derivative:
+                for _, message_list in job_messages.items():
+                    try:
+                        first_message = message_list[0]
+                        assert "job_id" in first_message, "job_id is missing"
+                        assert "job_type" in first_message, "job_type is missing"
+                        assert "input_type" in first_message, "input_type is missing"
+                        assert (
+                            first_message["job_type"] == job_type
+                        ), f"job_type is not {job_type}"
+
+                        job_id = first_message["job_id"]
+                        input_type = first_message["input_type"]
+                        params = first_message["params"]
+
+                        logger.info(
+                            f"Processing part of job {job_id} with a batch size of "
+                            f"{len(message_list)} molecules"
+                        )
+
+                        logger.info(f"Predicting molecules given as {input_type}")
+
+                        # TODO: solve differently
+                        def _create_entry(message):
+                            from nerdd_module.input import MoleculeEntry
+                            from rdkit.Chem import (
+                                MolFromInchi,
+                                MolFromMolBlock,
+                                MolFromSmiles,
+                            )
+
+                            input_type = message["input_type"].lower()
+                            raw_input = message["raw_input"]
+                            try:
+                                if input_type == "smiles":
+                                    mol = MolFromSmiles(raw_input)
+                                elif input_type == "inchi":
+                                    mol = MolFromInchi(raw_input)
+                                elif input_type == "mol_block":
+                                    mol = MolFromMolBlock(raw_input)
+                                else:
+                                    mol = None
+                            except:
+                                mol = None
+
+                            return MoleculeEntry(
+                                raw_input=raw_input,
+                                input_type=message["input_type"],
+                                source=message["source"],
+                                mol=mol,
+                                errors=message["errors"],
+                            )
+
+                        entries = [_create_entry(message) for message in message_list]
+                        results = model._predict_entries(
+                            entries,
+                            **params,
+                        )
+
+                        logger.info(f"Produced results: {len(results)}")
+
+                        results["job_id"] = job_id
+                        results["job_type"] = job_type
+
+                        # map mol_id (ranging from 0 to n) to the original mol_id provided
+                        # in the field mol_id of each message in message_list
+                        results["mol_id"] = [
+                            message_list[mol_id]["mol_id"]
+                            for mol_id in results["mol_id"]
+                        ]
+
+                        def _to_smiles(mol):
+                            if mol is None:
+                                return None
+                            else:
+                                return MolToSmiles(mol)
+
+                        results["input_smiles"] = results.input_mol.map(_to_smiles)
+                        results["preprocessed_smiles"] = results.preprocessed_mol.map(
+                            _to_smiles
+                        )
+
+                        #
+                        # send results to output topic
+                        #
+
+                        # send molecule properties
+                        results_molecule = (
+                            results[molecular_property_columns]
+                            .drop_duplicates(subset="mol_id")
+                            .to_dict("records")
+                        )
+                        for entry in results_molecule:
                             producer.send(
                                 "results",
-                                json.dumps(entry, cls=ComplexJsonEncoder).encode(
-                                    "utf-8"
-                                ),
+                                json.dumps(
+                                    entry, cls=ComplexJsonEncoder, ignore_nan=True
+                                ).encode("utf-8"),
                             ).get()
-                except Exception as e:
-                    logger.error(f"Error processing input: {message_list}", exc_info=e)
 
-            # commit the message offsets we have processed
-            consumer.commit()
+                        # optionally send atom properties
+                        if module_type == "atom_property_predictor":
+                            results_atom = results[results.atom_id.notnull()][
+                                atom_property_columns
+                            ].to_dict("records")
+                            for entry in results_atom:
+                                producer.send(
+                                    "results",
+                                    json.dumps(
+                                        entry,
+                                        cls=ComplexJsonEncoder,
+                                        ignore_nan=True,
+                                    ).encode("utf-8"),
+                                ).get()
+
+                        # optionally send derivative properties
+                        if module_type == "derivative_property_predictor":
+                            results_derivative = results[
+                                results.derivative_id.notnull()
+                            ][derivative_property_columns].to_dict("records")
+                            for entry in results_derivative:
+                                producer.send(
+                                    "results",
+                                    json.dumps(
+                                        entry,
+                                        cls=ComplexJsonEncoder,
+                                        ignore_nan=True,
+                                    ).encode("utf-8"),
+                                ).get()
+                    except Exception as e:
+                        logger.error(
+                            f"Error processing input: {message_list}", exc_info=e
+                        )
+
+                # commit the message offsets we have processed
+                consumer.commit()
```

### Comparing `nerdd-kafka-0.1.0/nerdd_kafka.egg-info/PKG-INFO` & `nerdd_kafka-0.2.1/nerdd_kafka.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: nerdd-kafka
-Version: 0.1.0
+Version: 0.2.1
 Summary: Run a NERDD module as a Kafka service
-Home-page: https://gitlab.phaidra.org/comp3d/nerdd-kafka
+Home-page: https://github.com/molinfo-vienna/nerdd-kafka
 Maintainer: Steffen Hirte
 Maintainer-email: steffen.hirte@univie.ac.at
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdkit>=2022.3.3
 Requires-Dist: kafka-python==2.0.2
+Requires-Dist: nerdd-module>=0.2.0
 Requires-Dist: pandas>=1.2.1
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: filetype~=1.2.0
 Requires-Dist: rich-click>=1.7.1
 Requires-Dist: stringcase~=1.2.0
+Requires-Dist: numpy
+Requires-Dist: simplejson>=3
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-bdd; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-watch; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: hypothesis-rdkit; extra == "test"
+Provides-Extra: docs
+Requires-Dist: mkdocs; extra == "docs"
+Requires-Dist: mkdocs-material; extra == "docs"
 
 # NERDD Kafka
 
 Run a [NERDD module](https://github.com/molinfo-vienna/nerdd-module) as a Kafka 
 service that consumes input molecules and produces prediction tuples.
```

### Comparing `nerdd-kafka-0.1.0/nerdd_kafka.egg-info/SOURCES.txt` & `nerdd_kafka-0.2.1/nerdd_kafka.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,16 @@
 nerdd_kafka.egg-info/requires.txt
 nerdd_kafka.egg-info/top_level.txt
 nerdd_kafka/serialization/__init__.py
 nerdd_kafka/serialization/json_encoder.py
 nerdd_kafka/serialization/mol_serializer.py
 nerdd_kafka/serialization/registry.py
 nerdd_kafka/serialization/serializer.py
-tests/test_backup.py
+tests/__init__.py
+tests/conftest.py
 tests/test_kafka_server_atom_property_predictor.py
 tests/test_kafka_server_initialization.py
-tests/test_kafka_server_molecule_property_predictor.py
+tests/test_kafka_server_molecule_property_predictor.py
+tests/steps/__init__.py
+tests/steps/mocked_kafka.py
+tests/steps/molecules.py
+tests/steps/records.py
```

### Comparing `nerdd-kafka-0.1.0/setup.py` & `nerdd_kafka-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,43 +12,50 @@
     pass
 
 # rdkit 2022.3.3 is the oldest (reasonable) version
 rdkit_requirement = ["rdkit>=2022.3.3"] if not rdkit_installed else []
 
 setup(
     name="nerdd-kafka",
-    version="0.1.0",
+    version="0.2.1",
     maintainer="Steffen Hirte",
     maintainer_email="steffen.hirte@univie.ac.at",
     packages=find_packages(),
-    url="https://gitlab.phaidra.org/comp3d/nerdd-kafka",
+    url="https://github.com/molinfo-vienna/nerdd-kafka",
     description="Run a NERDD module as a Kafka service",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=rdkit_requirement
     + [
         "kafka-python==2.0.2",
+        "nerdd-module>=0.2.0",
         "pandas>=1.2.1",
         "pyyaml~=6.0",
         "filetype~=1.2.0",
         "rich-click>=1.7.1",
         "stringcase~=1.2.0",
+        "numpy",
+        "simplejson>=3",
     ],
     extras_require={
         "dev": [],
         "test": [
             "pytest",
             "pytest-cov",
             "pytest-asyncio",
             "pytest-bdd",
             "pytest-mock",
             "pytest-watch",
             "hypothesis",
             "hypothesis-rdkit",
         ],
+        "docs": [
+            "mkdocs",
+            "mkdocs-material",
+        ],
     },
     entry_points={
         "console_scripts": [
             "run_nerdd_server = nerdd_kafka.__main__:main",
         ],
     },
 )
```

### Comparing `nerdd-kafka-0.1.0/tests/test_backup.py` & `nerdd_kafka-0.2.1/tests/steps/records.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,54 @@
-@then("the image column should contain svg images")
-def check_image_column(subset):
-    if len(subset) > 0:
-        # check that all images start and end with svg tags
-        assert subset.image.str.strip().str.startswith("<svg version='1.1'").all()
-        assert subset.image.str.strip().str.endswith("</svg>").all()
+import numpy as np
+from pytest_bdd import given, parsers
+from rdkit.Chem import MolToInchi, MolToMolBlock, MolToSmiles
 
 
-@then("the image column should contain svg images")
-def check_image_column(subset):
-    # check that all images start and end with svg tags
-    if len(subset) > 0:
-        assert subset.image.str.strip().str.startswith("<svg version='1.1'").all()
-        assert subset.image.str.strip().str.endswith("</svg>").all()
+@given(
+    parsers.parse('the records of the molecules in "{input_type}" format'),
+    target_fixture="records",
+)
+def records(molecules, input_type, multiplier):
+    def _record(i, mol):
+        # convert to representation
+        if input_type == "smiles":
+            converter = MolToSmiles
+        elif input_type == "mol_block":
+            converter = MolToMolBlock
+        elif input_type == "inchi":
+            converter = MolToInchi
+        else:
+            raise ValueError(f"Unknown input_type: {input_type}")
+
+        if mol is None:
+            representation = None
+        else:
+            representation = converter(mol)
+
+        return {
+            "job_id": "abc",
+            "job_type": "dummy",
+            "mol_id": i,
+            "input_type": input_type,
+            "raw_input": representation,
+            "source": ("test.file"),
+            "errors": [],
+            "params": {"multiplier": multiplier},
+        }
+
+    return [_record(i, mol) for i, mol in enumerate(molecules)]
 
 
 @given(
-    parsers.parse(
-        "the molecules as {input_type} partitioned in {num_partitions:d} batch(es)"
-    ),
+    parsers.parse("the records partitioned in {num_partitions:d} batch(es)"),
     target_fixture="input_batches",
 )
-def input_batches(representations, input_type, multiplier, num_partitions):
+def input_batches(records, num_partitions):
     split_indices = np.random.choice(
-        len(representations), size=num_partitions - 1, replace=True
+        len(records), size=num_partitions - 1, replace=True
     )
     split_indices = sorted(split_indices)
 
     return np.split(
-        [
-            {
-                "job_id": "abc",
-                "job_type": "dummy",
-                "mol_id": i,
-                "input_type": input_type,
-                "raw_input": mol,
-                "params": {"multiplier": multiplier},
-            }
-            for i, mol in enumerate(representations)
-        ],
+        records,
         split_indices,
     )
```

### Comparing `nerdd-kafka-0.1.0/tests/test_kafka_server_atom_property_predictor.py` & `nerdd_kafka-0.2.1/tests/test_kafka_server_atom_property_predictor.py`

 * *Files identical despite different names*

### Comparing `nerdd-kafka-0.1.0/tests/test_kafka_server_initialization.py` & `nerdd_kafka-0.2.1/tests/test_kafka_server_initialization.py`

 * *Files identical despite different names*

