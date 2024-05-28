# Comparing `tmp/neo4j_runway-0.2.1.tar.gz` & `tmp/neo4j_runway-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j_runway-0.2.1.tar", max compression
+gzip compressed data, was "neo4j_runway-0.2.2.tar", max compression
```

## Comparing `neo4j_runway-0.2.1.tar` & `neo4j_runway-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11354 2024-05-01 12:35:47.639470 neo4j_runway-0.2.1/LICENSE
--rw-r--r--   0        0        0     4780 2024-05-22 14:20:25.800919 neo4j_runway-0.2.1/README.md
--rw-r--r--   0        0        0      216 2024-05-22 14:20:25.801566 neo4j_runway-0.2.1/neo4j_runway/__init__.py
--rw-r--r--   0        0        0       33 2024-04-29 23:04:42.985466 neo4j_runway-0.2.1/neo4j_runway/discovery/__init__.py
--rw-r--r--   0        0        0     4373 2024-05-21 12:37:17.143781 neo4j_runway-0.2.1/neo4j_runway/discovery/discovery.py
--rw-r--r--   0        0        0       79 2024-04-29 23:04:42.986387 neo4j_runway-0.2.1/neo4j_runway/ingestion/__init__.py
--rw-r--r--   0        0        0    15503 2024-05-21 12:37:17.144321 neo4j_runway-0.2.1/neo4j_runway/ingestion/generate_ingest.py
--rwxr-xr-x   0        0        0     4922 2024-05-21 12:37:17.144800 neo4j_runway-0.2.1/neo4j_runway/ingestion/pyingest.py
--rw-r--r--   0        0        0       21 2024-04-29 23:04:42.987658 neo4j_runway-0.2.1/neo4j_runway/llm/__init__.py
--rw-r--r--   0        0        0     4962 2024-05-21 12:37:17.145297 neo4j_runway-0.2.1/neo4j_runway/llm/llm.py
--rw-r--r--   0        0        0       38 2024-04-29 23:04:42.988650 neo4j_runway-0.2.1/neo4j_runway/modeler/__init__.py
--rw-r--r--   0        0        0    10072 2024-05-21 12:37:17.146484 neo4j_runway-0.2.1/neo4j_runway/modeler/modeler.py
--rw-r--r--   0        0        0      229 2024-05-02 11:43:53.434393 neo4j_runway-0.2.1/neo4j_runway/objects/__init__.py
--rw-r--r--   0        0        0     2990 2024-05-21 12:37:17.147283 neo4j_runway-0.2.1/neo4j_runway/objects/arrows.py
--rw-r--r--   0        0        0    11786 2024-05-21 12:37:17.147911 neo4j_runway-0.2.1/neo4j_runway/objects/data_model.py
--rw-r--r--   0        0        0     4828 2024-05-21 12:37:17.148608 neo4j_runway-0.2.1/neo4j_runway/objects/node.py
--rw-r--r--   0        0        0     2934 2024-05-21 12:37:17.149307 neo4j_runway-0.2.1/neo4j_runway/objects/property.py
--rw-r--r--   0        0        0     5438 2024-05-21 12:37:17.149779 neo4j_runway-0.2.1/neo4j_runway/objects/relationship.py
--rw-r--r--   0        0        0      904 2024-05-02 11:43:53.436909 neo4j_runway-0.2.1/neo4j_runway/objects/user_input.py
--rw-r--r--   0        0        0     2393 2024-05-21 12:37:17.150388 neo4j_runway-0.2.1/neo4j_runway/resources/prompts/prompts.py
--rw-r--r--   0        0        0      138 2024-04-29 23:04:43.003742 neo4j_runway-0.2.1/neo4j_runway/utils/__init__.py
--rw-r--r--   0        0        0     3429 2024-04-29 23:04:43.003938 neo4j_runway-0.2.1/neo4j_runway/utils/naming_conventions.py
--rw-r--r--   0        0        0      917 2024-05-01 12:25:23.223161 neo4j_runway-0.2.1/neo4j_runway/utils/test_connection.py
--rw-r--r--   0        0        0     1133 2024-05-22 14:20:36.546370 neo4j_runway-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 neo4j_runway-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-01 12:35:47.639470 neo4j_runway-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4780 2024-05-22 14:20:25.800919 neo4j_runway-0.2.2/README.md
+-rw-r--r--   0        0        0      216 2024-05-22 14:20:25.801566 neo4j_runway-0.2.2/neo4j_runway/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-29 23:04:42.985466 neo4j_runway-0.2.2/neo4j_runway/discovery/__init__.py
+-rw-r--r--   0        0        0     5891 2024-05-28 15:16:17.524804 neo4j_runway-0.2.2/neo4j_runway/discovery/discovery.py
+-rw-r--r--   0        0        0       79 2024-04-29 23:04:42.986387 neo4j_runway-0.2.2/neo4j_runway/ingestion/__init__.py
+-rw-r--r--   0        0        0    17760 2024-05-28 13:21:24.152689 neo4j_runway-0.2.2/neo4j_runway/ingestion/generate_ingest.py
+-rwxr-xr-x   0        0        0     5476 2024-05-28 13:21:24.153290 neo4j_runway-0.2.2/neo4j_runway/ingestion/pyingest.py
+-rw-r--r--   0        0        0       21 2024-04-29 23:04:42.987658 neo4j_runway-0.2.2/neo4j_runway/llm/__init__.py
+-rw-r--r--   0        0        0     5069 2024-05-28 13:21:24.153884 neo4j_runway-0.2.2/neo4j_runway/llm/llm.py
+-rw-r--r--   0        0        0       38 2024-04-29 23:04:42.988650 neo4j_runway-0.2.2/neo4j_runway/modeler/__init__.py
+-rw-r--r--   0        0        0    10267 2024-05-28 15:16:17.534087 neo4j_runway-0.2.2/neo4j_runway/modeler/modeler.py
+-rw-r--r--   0        0        0      229 2024-05-02 11:43:53.434393 neo4j_runway-0.2.2/neo4j_runway/objects/__init__.py
+-rw-r--r--   0        0        0     3092 2024-05-28 13:21:24.154903 neo4j_runway-0.2.2/neo4j_runway/objects/arrows.py
+-rw-r--r--   0        0        0    13751 2024-05-28 13:21:24.155423 neo4j_runway-0.2.2/neo4j_runway/objects/data_model.py
+-rw-r--r--   0        0        0     6379 2024-05-28 13:21:24.155856 neo4j_runway-0.2.2/neo4j_runway/objects/node.py
+-rw-r--r--   0        0        0     2934 2024-05-21 12:37:17.149307 neo4j_runway-0.2.2/neo4j_runway/objects/property.py
+-rw-r--r--   0        0        0     5438 2024-05-21 12:37:17.149779 neo4j_runway-0.2.2/neo4j_runway/objects/relationship.py
+-rw-r--r--   0        0        0     1383 2024-05-28 15:10:02.679473 neo4j_runway-0.2.2/neo4j_runway/objects/user_input.py
+-rw-r--r--   0        0        0     2393 2024-05-21 12:37:17.150388 neo4j_runway-0.2.2/neo4j_runway/resources/prompts/prompts.py
+-rw-r--r--   0        0        0      138 2024-04-29 23:04:43.003742 neo4j_runway-0.2.2/neo4j_runway/utils/__init__.py
+-rw-r--r--   0        0        0     3896 2024-05-28 13:21:24.158549 neo4j_runway-0.2.2/neo4j_runway/utils/naming_conventions.py
+-rw-r--r--   0        0        0     1258 2024-05-28 13:21:24.158958 neo4j_runway-0.2.2/neo4j_runway/utils/test_connection.py
+-rw-r--r--   0        0        0     1133 2024-05-28 18:03:06.458790 neo4j_runway-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 neo4j_runway-0.2.2/PKG-INFO
```

### Comparing `neo4j_runway-0.2.1/LICENSE` & `neo4j_runway-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.1/README.md` & `neo4j_runway-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.1/neo4j_runway/discovery/discovery.py` & `neo4j_runway-0.2.2/neo4j_runway/discovery/discovery.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,74 @@
+"""
+The Discovery module that handles summarization and discovery generation via an LLM.
+"""
+
 import io
 import os
 from typing import Dict, Union
+import warnings
 
 import pandas as pd
 
 from ..llm.llm import LLM
 from ..objects.user_input import UserInput
 
 
 class Discovery:
+    """
+    The Discovery module that handles summarization and discovery generation via an LLM.
+    """
 
     def __init__(
-        self, llm: LLM, user_input: Union[Dict[str, str], UserInput], data: pd.DataFrame
+        self,
+        data: pd.DataFrame,
+        user_input: Union[Dict[str, str], UserInput] = {},
+        llm: LLM = None,
+        pandas_only: bool = False,
     ) -> None:
+        """
+        The Discovery module that handles summarization and discovery generation via an LLM.
+
+        Parameters
+        ----------
+        llm : LLM, optional
+            The LLM instance used to generate data discovery. Only required if pandas_only = False.
+        user_input : Union[Dict[str, str], UserInput]
+            User provided descriptions of the data.
+            If a dictionary, then should contain the keys "general_description" and all desired columns., by default = {}
+        data : pd.DataFrame
+            The data in Pandas DataFrame format.
+        pandas_only : bool
+            Whether to only generate discovery using Pandas. Will not call the LLM service.
+        """
         if isinstance(user_input, UserInput):
             self.user_input = user_input.formatted_dict
         else:
             self.user_input = user_input
-            assert "general_description" in self.user_input.keys(), (
-                "user_input must include key:value pair {general_description: ...}. "
-                + f"Found keys {self.user_input.keys()}"
-            )
+            if "general_description" not in self.user_input.keys():
+                warnings.warn(
+                    "user_input should include key:value pair {general_description: ...} for best results. "
+                    + f"Found keys {self.user_input.keys()}"
+                )
         self.llm = llm
 
         self.columns_of_interest = list(self.user_input.keys())
-        self.columns_of_interest.remove("general_description")
+        if "general_description" in self.columns_of_interest:
+            self.columns_of_interest.remove("general_description")
 
-        self.data = data[self.columns_of_interest]
+        if self.columns_of_interest:
+            self.data = data[self.columns_of_interest]
+        else:
+            warnings.warn(
+                "No columns detected in user input. Defaulting to all columns."
+            )
+            self.columns_of_interest = data.columns
+            self.data = data
 
+        self.pandas_only = not self.llm or pandas_only
         self._discovery_ran = False
         self.discovery = ""
 
     def _generate_csv_summary(self) -> Dict[str, pd.DataFrame]:
         """
         Generate the data summaries.
         """
@@ -82,17 +119,20 @@
     def run(self) -> str:
         """
         Run discovery on the data.
         """
 
         self._generate_csv_summary()
 
-        response = self.llm.get_discovery_response(
-            formatted_prompt=self._generate_discovery_prompt()
-        )
+        if not self.pandas_only:
+            response = self.llm.get_discovery_response(
+                formatted_prompt=self._generate_discovery_prompt()
+            )
+        else:
+            response = ""
 
         self._discovery_ran = True
         self.discovery = response
 
         return response
 
     def to_txt(self, file_dir: str = "./", file_name: str = "discovery") -> None:
```

### Comparing `neo4j_runway-0.2.1/neo4j_runway/ingestion/generate_ingest.py` & `neo4j_runway-0.2.2/neo4j_runway/ingestion/generate_ingest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This file contains the code to generate ingestion code.
+"""
+
 import os
 from typing import Dict, List, Any, Union
 
 import yaml
 
 from ..objects.data_model import DataModel
 from ..objects import Node
@@ -35,26 +39,52 @@
 
 
 def lowercase_first_letter(str):
     return str[0].lower() + str[1:]
 
 
 class IngestionGenerator:
+    """
+    Class responsible for generating the ingestion code.
+    """
 
     def __init__(
         self,
         data_model: DataModel,
         csv_name: str = "",
         username: Union[str, None] = None,
         password: Union[str, None] = None,
         uri: Union[str, None] = None,
         database: Union[str, None] = None,
         csv_dir: str = "",
         file_output_dir: str = "",
     ):
+        """
+        Class responsible for generating the ingestion code.
+
+        Parameters
+        ----------
+        data_model : DataModel
+            The data model to base ingestion code on.
+        csv_name : str, optional
+            The CSV containing the data. If data is contained in multiple CSVs,
+            then this should be "" and CSVs noted in the data model, by default ""
+        username : Union[str, None], optional
+            The username used to connect to Neo4j, by default None
+        password : Union[str, None], optional
+            The password used to connect to Neo4j, by default None
+        uri : Union[str, None], optional
+            The uri of the Neo4j instance, by default None
+        database : Union[str, None], optional
+            The database within the Neo4j instance to load the data, by default None
+        csv_dir : str, optional
+            The location of the CSV file(s), by default ""
+        file_output_dir : str, optional
+            The location that generated files should be saved to, by default ""
+        """
 
         self.data_model: DataModel = data_model
         self.username: Union[str, None] = username
         self.password: Union[str, None] = password
         self.uri: Union[str, None] = uri
         self.database: Union[str, None] = database
         self.csv_name: str = csv_name
@@ -157,26 +187,38 @@
                 file_dict["chunk_size"] = batch_size
                 self._config_files_list.append(file_dict)
 
     def generate_pyingest_yaml_file(
         self, file_name: str = "pyingest_config", batch_size: int = 100
     ) -> None:
         """
-        Generate the PyIngest yaml file.
+        Generate the PyIngest YAML config file.
+
+        Parameters
+        ----------
+        file_name : str, optional
+            Name of the file, by default "pyingest_config"
+        batch_size : int, optional
+            The desired batch size, by default 100
         """
 
         if self.file_output_dir != "":
             os.makedirs(self.file_output_dir, exist_ok=True)
 
         with open(f"./{self.file_output_dir}{file_name}.yml", "w") as config_yaml:
             config_yaml.write(self.generate_pyingest_yaml_string(batch_size=batch_size))
 
     def generate_pyingest_yaml_string(self, batch_size: int = 100) -> str:
         """
         Generate the PyIngest yaml in string format.
+
+        Parameters
+        ----------
+        batch_size : int, optional
+            The desired batch size, by default 100
         """
 
         self._generate_base_information(batch_size=batch_size)
 
         final_yaml = {}
         final_yaml["files"] = self._config_files_list
         config_dump = yaml.dump(final_yaml)
@@ -194,14 +236,19 @@
         to_return += config_dump
 
         return to_return
 
     def generate_constraints_cypher_file(self, file_name: str = "constraints") -> None:
         """
         Generate the Constraints cypher file.
+
+        Parameters
+        ----------
+        file_name : str, optional
+            Name of the file, by default "constraints"
         """
 
         if self.file_output_dir != "":
             os.makedirs(self.file_output_dir, exist_ok=True)
 
         with open(
             f"./{self.file_output_dir}{file_name}.cypher", "w"
@@ -224,14 +271,23 @@
         return to_return
 
     def generate_load_csv_file(
         self, file_name: str = "load_csv", batch_size: int = 100, method: str = "api"
     ) -> None:
         """
         Generate the load_csv cypher file.
+
+        Parameters
+        ----------
+        file_name : str, optional
+            Name of the file, by default "load_csv"
+        batch_size : int, optional
+            The desired batch size, by default 100
+        method : str, optional
+            The method that LOAD CSV will be run. Must be either "api" or "browser".
         """
 
         if self.file_output_dir != "":
             os.makedirs(self.file_output_dir, exist_ok=True)
 
         with open(f"./{self.file_output_dir}{file_name}.cypher", "w") as load_csv_file:
             load_csv_file.write(
@@ -239,14 +295,21 @@
             )
 
     def generate_load_csv_string(
         self, batch_size: int = 100, method: str = "api"
     ) -> str:
         """
         Generate the load_csv cypher in string format.
+
+        Parameters
+        ----------
+        batch_size : int, optional
+            The desired batch size, by default 100
+        method : str, optional
+            The method that LOAD CSV will be run. Must be either "api" or "browser".
         """
 
         self._generate_base_information(batch_size=batch_size, method=method)
 
         to_return = ""
 
         for constraint in self._constraints:
```

### Comparing `neo4j_runway-0.2.1/neo4j_runway/ingestion/pyingest.py` & `neo4j_runway-0.2.2/neo4j_runway/ingestion/pyingest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This is a modified PyIngest file for Neo4j Runway. It currently only supports Pandas DataFrame ingestion.
+This is a modified PyIngest file for Neo4j Runway. It currently only supports Pandas DataFrame and CSV ingestion.
 """
 
 import datetime
 from typing import Optional
 
 from neo4j import GraphDatabase
 import numpy as np
@@ -11,14 +11,17 @@
 import yaml
 
 
 config = dict()
 
 
 class LocalServer(object):
+    """
+    Handles data ingestion.
+    """
 
     def __init__(self):
         self._driver = GraphDatabase.driver(
             config["server_uri"], auth=(config["admin_user"], config["admin_pass"])
         )
         self.db_config = {}
         self.database = config["database"] if "database" in config else None
@@ -64,15 +67,15 @@
     def load_csv(self, file):
         with self._driver.session(**self.db_config) as session:
             params = self.get_params(file)
 
             with open(params["url"]) as openfile:
                 # Grab the header from the file and pass that to pandas.  This allow the header
                 # to be applied even if we are skipping lines of the file
-                header = str(openfile.readline()).strip().split(params['field_sep'])
+                header = str(openfile.readline()).strip().split(params["field_sep"])
 
                 # Pandas' read_csv method is highly optimized and fast :-)
                 row_chunks = pd.read_csv(
                     openfile,
                     dtype=str,
                     sep=params["field_sep"],
                     on_bad_lines="skip",
@@ -117,14 +120,26 @@
 
 def load_config(configuration):
     global config
     config = yaml.safe_load(configuration)
 
 
 def PyIngest(yaml_string: str, dataframe: Optional[pd.DataFrame] = None) -> None:
+    """
+    Function to ingest data according to a configuration YAML string.
+    This is a modified lite version of the original PyIngest.
+
+    Parameters
+    ----------
+    yaml_string : str
+        a string representation of the YAML file that is generated by the IngestionGenerator class.
+    dataframe : Optional[pd.DataFrame], optional
+        The data to ingest in Pandas DataFrame format.
+        If None, then will search for CSVs according to the urls in YAML config, by default None
+    """
     load_config(yaml_string)
     server = LocalServer()
     server.pre_ingest()
     file_list = config["files"]
     for file in file_list:
         if dataframe is not None:
             server.load_dataframe(file, dataframe=dataframe)
```

### Comparing `neo4j_runway-0.2.1/neo4j_runway/llm/llm.py` & `neo4j_runway-0.2.2/neo4j_runway/llm/llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This file contains the LLM module that interfaces with an OpenAI LLM via the Instructor library.
+"""
+
 import os
 from typing import List, Union
 
 
 from openai import OpenAI
 
 import instructor
@@ -25,14 +29,15 @@
     "gpt-3.5-turbo-0125",
 ]
 
 
 class LLM:
     """
     Interface for interacting with different LLMs.
+
     Attributes
     ----------
     model: str
         The OpenAI LLM to use.
     open_ai_key: Union[str, None] = None
         Your OpenAI API key if it is not declared in an environment variable.
     """
```

### Comparing `neo4j_runway-0.2.1/neo4j_runway/modeler/modeler.py` & `neo4j_runway-0.2.2/neo4j_runway/modeler/modeler.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,87 +7,85 @@
 from ..llm import LLM
 from ..objects import DataModel, UserInput
 from ..resources.prompts.prompts import model_generation_rules, model_format
 
 
 class GraphDataModeler:
     """
-    Attributes
-    ----------
-    llm : LLM
-        The LLM used to generate data models.
-    discovery : Union[str, Discovery] = ""
-        Either a string containing the LLM generated discovery or a Discovery object that has been ran.
-        If a Discovery object is provided then the remaining discovery attributes don't need to be provided.
-    user_input : Dict[str, UserInput] = {}
-        Either a dictionary with keys general_description and column names with descriptions or a UserInput object.
-        Not required.
-    general_data_description : str = ""
-        A general data description provided by Discovery. Not required.
-    numeric_data_description : str = ""
-        A numeric data description provided by Discovery. Not required.
-    categorical_data_description : str = ""
-        A categorical data description provided by Discovery. Not required.
-    feature_descriptions : str = ""
-        Feature descriptions provided by Discovery. Not required.
+    This class is responsible for generating a graph data model via communication with an LLM.
+    It handles prompt generation, model generation history as well as access to the generated data models.
     """
 
     def __init__(
         self,
         llm: LLM,
         discovery: Union[str, Discovery] = "",
         user_input: Union[Dict[str, str], UserInput] = {},
         general_data_description: str = "",
         numeric_data_description: str = "",
         categorical_data_description: str = "",
         feature_descriptions: str = "",
+        allowed_columns: List[str] = [],
     ) -> None:
         """
         Takes an LLM instance and Discovery information.
         Either a Discovery object can be provided, or each field can be provided individually.
+
+        Parameters
+        ----------
+        llm : LLM
+            The LLM used to generate data models.
+        discovery : Union[str, Discovery], optional
+            Either a string containing the LLM generated discovery or a Discovery object that has been ran.
+            If a Discovery object is provided then the remaining discovery attributes don't need to be provided, by default ""
+        user_input : Dict[str, UserInput], optional
+            Either a dictionary with keys general_description and column names with descriptions or a UserInput object, by default {}
+        general_data_description : str, optional
+            A general data description provided by Discovery, by default ""
+        numeric_data_description : str, optional
+            A numeric data description provided by Discovery, by default ""
+        categorical_data_description : str, optional
+            A categorical data description provided by Discovery, by default ""
+        feature_descriptions : str, optional
+            Feature descriptions provided by Discovery, by default ""
+        allowed_columns : List[str], optional
+            The columns that may be used in the data model. The argument should only be used in no columns are specified in
+            the discovery or user_input arguments., by default []
         """
 
         self.llm = llm
 
         if isinstance(discovery, Discovery):
             self.user_input = discovery.user_input
 
-            assert "general_description" in self.user_input.keys(), (
-                "user_input must include key:value pair {general_description: ...}. "
-                + f"Found keys {self.user_input.keys()}"
-            )
-
             self.columns_of_interest = discovery.columns_of_interest
 
             self.discovery = discovery.discovery
             self.general_info = discovery.df_info
             self.description_numeric = discovery.numeric_data_description
             self.description_categorical = discovery.categorical_data_description
             self.feature_descriptions = discovery.feature_descriptions
 
         else:
 
             if isinstance(user_input, UserInput):
                 self.user_input = user_input.formatted_dict
+
             else:
                 self.user_input = user_input
-                assert "general_description" in self.user_input.keys(), (
-                    "user_input must include key:value pair {general_description: ...}. "
+
+            if "general_description" not in self.user_input.keys():
+                warnings.warn(
+                    "user_input should include key:value pair {general_description: ...} for best results. "
                     + f"Found keys {self.user_input.keys()}"
                 )
 
-            # self.user_input = user_input
-
-            # assert "general_description" in self.user_input.keys(), (
-            #     "user_input must include key:value pair {general_description: ...}. "
-            #     + f"Found keys {self.user_input.keys()}"
-            # )
-
-            self.columns_of_interest = list(self.user_input.keys())
-            self.columns_of_interest.remove("general_description")
+            self.columns_of_interest = allowed_columns or list(self.user_input.keys())
+            if "general_description" in self.columns_of_interest:
+                self.columns_of_interest.remove("general_description")
 
             self.discovery = discovery
             self.general_info = general_data_description
             self.description_numeric = numeric_data_description
             self.description_categorical = categorical_data_description
             self.feature_descriptions = feature_descriptions
 
@@ -256,25 +254,25 @@
         """
         Iterate on the previous data model the number times indicated.
         """
 
         assert self._initial_model_created, "No data model present to iterate on."
 
         def iterate() -> DataModel:
-            for i in range(0, iterations):
+            for _ in range(0, iterations):
                 response = self.llm.get_data_model_response(
                     formatted_prompt=self._generate_data_model_iteration_prompt(
                         user_corrections=user_corrections,
                         use_yaml_data_model=use_yaml_data_model,
                     ),
                     csv_columns=self.columns_of_interest,
                     use_yaml_data_model=use_yaml_data_model,
                 )
 
                 self.model_history.append(response)
                 self.model_iterations += 1
 
             return response
-        
+
         current_model = iterate()
-        
+
         return current_model
```

### Comparing `neo4j_runway-0.2.1/neo4j_runway/objects/arrows.py` & `neo4j_runway-0.2.2/neo4j_runway/objects/arrows.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This file contains the objects to construct a data model as it is represented in arrows.app.
+"""
+
 from typing import Dict, List, Any
 import warnings
 
 from pydantic import BaseModel, field_validator
 
 DEFAULT_STYLE = {
     "font-family": "Nunito Sans",
```

### Comparing `neo4j_runway-0.2.1/neo4j_runway/objects/data_model.py` & `neo4j_runway-0.2.2/neo4j_runway/objects/data_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This file contains the DataModel class which is the standard representation of a graph data model in Neo4j Runway.
+"""
+
 from ast import literal_eval
 from typing import List, Dict, Union, Self
 
 from graphviz import Digraph
 from pydantic import BaseModel
 import yaml
 
@@ -14,80 +18,111 @@
     fix_property,
     fix_relationship_type,
 )
 
 
 class DataModel(BaseModel):
     """
-    Graph Data Model representation.
-
-    Attributes
-    ----------
-    nodes : List<Node>
-        A list of the nodes in the data model.
-    relationships : List<Relationship>
-        A list of the relationships in the data model.
-    use_neo4j_naming_conventions : bool
-        Whether to convert labels, relationships and properties to Neo4j naming conventions.
+    The standard Graph Data Model representation in Neo4j Runway.
     """
 
     nodes: List[Node]
     relationships: List[Relationship]
 
     def __init__(
         self,
         nodes: List[Node],
         relationships: List[Relationship],
         use_neo4j_naming_conventions: bool = True,
     ) -> None:
+        """
+        The standard Graph Data Model representation in Neo4j Runway.
+
+        Attributes
+        ----------
+        nodes : List[Node]
+            A list of the nodes in the data model.
+        relationships : List[Relationship]
+            A list of the relationships in the data model.
+        use_neo4j_naming_conventions : bool, optional
+            Whether to convert labels, relationships and properties to Neo4j naming conventions, by default True
+        """
         super().__init__(
             nodes=nodes, relationships=relationships, use_neo4j_naming_conventions=True
         )
 
         # default apply Neo4j naming conventions.
         if use_neo4j_naming_conventions:
             self.apply_neo4j_naming_conventions()
 
     @property
     def node_labels(self) -> List[str]:
         """
-        Return a list of the node labels.
+        Returns a list of node labels.
+
+        Returns
+        -------
+        List[str]
+            A list of node labels.
         """
 
         return [n.label for n in self.nodes]
 
     @property
     def relationship_types(self) -> List[str]:
         """
-        Return a list of the relationship types.
+        Returns a list of relationship types.
+
+        Returns
+        -------
+        List[str]
+            A list of relationship types.
         """
 
         return [r.type for r in self.relationships]
 
     @property
     def node_dict(self) -> Dict[str, Node]:
         """
-        Returns a dictionary of {<node label>: <Node>}
+        Returns a dictionary of node label to Node.
+
+        Returns
+        -------
+        Dict[str, Node]
+            A dictionary with node label keys and Node values.
         """
 
         return {node.label: node for node in self.nodes}
 
     @property
-    def relationship_dict(self) -> Dict[str, Node]:
+    def relationship_dict(self) -> Dict[str, Relationship]:
         """
-        Returns a dictionary of {<relationship type>: <Relationship>}
+        Returns a dictionary of relationship type to Relationships.
+
+        Returns
+        -------
+        Dict[str, Relationship]
+            A dictionary with relationship type keys and Relationship values.
         """
 
         return {r.type: r for r in self.relationships}
 
     def validate_model(self, csv_columns: List[str]) -> None:
         """
-        Validate the model.
-        """
+        Perform additional validation on the data model.
 
+        Parameters
+        ----------
+        csv_columns : List[str]
+            The CSV columns that are allowed in the data model.
+
+        Returns
+        -------
+        None
+        """
         errors = []
         for node in self.nodes:
             errors += node.validate_properties(csv_columns=csv_columns)
 
         for rel in self.relationships:
             errors += rel.validate_properties(csv_columns=csv_columns)
 
@@ -165,15 +200,20 @@
                     f"The property csv_mapping {prop} is used for {labels_or_types} in the data model. Each of these must use a different csv column as a property csv_mapping instead. Find alternative property csv_mappings from the column options or remove."
                 )
 
         return errors
 
     def visualize(self) -> Digraph:
         """
-        Visualize the data model.
+        Visualize the data model using Graphviz. Requires that Graphviz is installed.
+
+        Returns
+        -------
+        Digraph
+            A visual representation of the data model.
         """
 
         dot = Digraph(comment="Data Model")
 
         for node in self.nodes:
             dot.node(name=node.label, label=self._generate_node_text(node=node))
 
@@ -227,14 +267,18 @@
             )
 
         return result
 
     def apply_neo4j_naming_conventions(self) -> None:
         """
         Apply Neo4j naming conventions to all labels, relationships and properties in the data model.
+
+        Returns
+        -------
+        None
         """
 
         # fix node labels and properties
         for node in self.nodes:
             node.label = fix_node_label(node.label)
             for prop in node.properties:
                 prop.name = fix_property(prop.name)
@@ -271,14 +315,26 @@
         return yaml_string
 
     def to_arrows(
         self, file_name: str = "data-model", write_file: bool = True
     ) -> ArrowsDataModel:
         """
         Output the data model to arrows compatible JSON file.
+
+        Parameters
+        ----------
+        file_name : str, optional
+            The file name, by default "data-model"
+        write_file : bool, optional
+            Whether to write a file, by default True
+
+        Returns
+        -------
+        ArrowsDataModel
+            A representation of the data model in arrows.app format.
         """
 
         NODE_SPACING: int = 200
         y_current = 0
         arrows_nodes = []
         for idx, n in enumerate(self.nodes):
             if (idx + 1) % 5 == 0:
@@ -298,14 +354,24 @@
 
         return arrows_data_model
 
     @classmethod
     def from_arrows(cls, file_path: str) -> Self:
         """
         Construct a DataModel from an arrows data model JSON file.
+
+        Parameters
+        ----------
+        file_path : str
+            The location and name of the arrows.app JSON file to import.
+
+        Returns
+        -------
+        Self
+            An instance of a DataModel.
         """
 
         with open(f"{file_path}", "r") as f:
             content = literal_eval(f.read())
             node_id_label_map = {n["id"]: n["labels"][0] for n in content["nodes"]}
             return cls(
                 nodes=[
@@ -335,11 +401,21 @@
                     )
                     for r in content["relationships"]
                 ],
             )
 
     def to_solutions_workbench(self, file_name: str = "data-model") -> Dict[str, any]:
         """
-        Output the data model to Solutions Workbench compatible JSON file.
+        NOT IMPLEMENTED | Output the data model to Solutions Workbench compatible JSON file.
+
+        Parameters
+        ----------
+        file_path : str
+            The location and name of the Solutions Workbench JSON file to import.
+
+        Returns
+        -------
+        Self
+            An instance of a DataModel.
         """
 
         pass
```

### Comparing `neo4j_runway-0.2.1/neo4j_runway/objects/property.py` & `neo4j_runway-0.2.2/neo4j_runway/objects/property.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.1/neo4j_runway/objects/relationship.py` & `neo4j_runway-0.2.2/neo4j_runway/objects/relationship.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.1/neo4j_runway/objects/user_input.py` & `neo4j_runway-0.2.2/neo4j_runway/objects/user_input.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 from typing import Dict
+import warnings
 from pydantic import BaseModel, Field, field_validator
 
 
 class UserInput(BaseModel):
+    """
+    A container for user provided information about the data.
+
+    Attributes
+    ----------
+
+    general_description : str, optional
+        A general description of the CSV data, by default = ""
+    column_descriptions : Dict[str, str]
+        A mapping of the desired CSV columns to their descriptions.
+        The keys of this argument will determine which CSV columns are
+        evaluated in discovery and used to generate a data model.
+    """
 
     general_description: str = Field(
         default="", description="A general description of the CSV data."
     )
     column_descriptions: Dict[str, str] = Field(
         description="A mapping of the desired csv columns to their descriptions."
     )
 
     @field_validator("column_descriptions")
     def validate_column_description(cls, v) -> Dict[str, str]:
         if v == {}:
-            raise ValueError("Empty column_descriptions dictionary not allowed.")
+            warnings.warn("Empty column_descriptions dictionary is not recommended.")
         return v
 
     @property
     def formatted_dict(self) -> Dict[str, str]:
         """
         Dictionary representation of the user input to be used in Discovery.
         """
```

### Comparing `neo4j_runway-0.2.1/neo4j_runway/resources/prompts/prompts.py` & `neo4j_runway-0.2.2/neo4j_runway/resources/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.1/neo4j_runway/utils/naming_conventions.py` & `neo4j_runway-0.2.2/neo4j_runway/utils/naming_conventions.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 
 def fix_node_label(label: str) -> str:
     """
     Apply Neo4j naming convention PascalCase to a node label.
     """
 
     if is_mixed_case(label):
-        parts = re.findall("[A-Z_][^A-Z_]*", label[0].upper() + label[1:])
-        return "".join([x.capitalize() for x in parts if x != "_"])
+        parts = re.findall("[A-Z_ ][^A-Z_ ]*", label[0].upper() + label[1:])
+        return "".join([x.capitalize().strip() for x in parts if x != "_"])
 
     elif is_pascal_case(label):
-        return label
+        return remove_spaces(label)
 
     elif is_camel_case(label):
-        return label[0].upper() + label[1:]
+        return label[0].upper() + remove_spaces(label[1:])
 
     elif is_snake_case(label):
-        parts = label.split("_")
+        parts = remove_spaces(label).split("_")
         return "".join([x.capitalize() for x in parts])
 
     else:
-        return label
+        return "".join([x.capitalize().strip() for x in label.split(" ")])
 
 
 def fix_relationship_type(type: str) -> str:
     """
     Apply Neo4j naming convention SCREAMING_SNAKE_CASE to a relationship type.
     """
 
@@ -42,22 +42,23 @@
         parts = re.findall("[A-Z][^A-Z]*", type)
         return "_".join(x.upper() for x in parts)
 
     elif is_camel_case(type):
         parts = re.findall("[A-Z][^A-Z]*", type[0].upper() + type[1:])
         return "_".join(x.upper() for x in parts)
     else:
-        return type.upper()
+        return type.upper().replace(" ", "_")
 
 
 def fix_property(property_name: str) -> str:
     """
     Apply Neo4j naming convention camelCase to a property name.
     """
-
+    # treat property with spaces as snakecase property
+    property_name = property_name.replace(" ", "_")
     if is_mixed_case(property_name):
         parts = re.findall(
             "[A-Z_][^A-Z_]*", property_name[0].upper() + property_name[1:]
         )
         pascal = "".join([x.lower().capitalize() for x in parts if x != "_"])
         return pascal[0].lower() + pascal[1:]
 
@@ -67,52 +68,54 @@
     elif is_pascal_case(property_name):
         return property_name[0].lower() + property_name[1:]
 
     elif is_snake_case(property_name):
         parts = property_name.split("_")
         pascal = "".join([x.capitalize() for x in parts])
         return pascal[0].lower() + pascal[1:]
+    else:
+        return property_name
 
 
 def is_camel_case(input: str) -> bool:
     """
     Determine if input is camel case.
     """
 
     assert len(input) > 0, "No input provided!"
 
     # first letter capital
     if ord(input[0]) >= 65 and ord(input[0]) <= 90:
         return False
 
-    return not "_" in input
+    return not "_" in input and not " " in input
 
 
 def is_pascal_case(input: str) -> bool:
     """
     Determine if input is Pascal case.
     """
 
     assert len(input) > 0, "No input provided!"
 
     # first letter not capital
     if ord(input[0]) < 65 or ord(input[0]) > 90:
         return False
 
-    return not "_" in input
+    return not "_" in input and not " " in input
 
 
 def is_snake_case(input: str) -> bool:
     """
     Determine if input is snake case.
     """
 
     assert len(input) > 0, "No input provided!"
 
-    return "_" in input or input.isupper()
+    return ("_" in input or input.isupper()) and not " " in input
 
 
 def is_mixed_case(input: str) -> bool:
     """
     Determine if input is mix of camel, pascal or snake case.
     """
 
@@ -132,7 +135,14 @@
             camel_or_pascal = True
             break
 
     if "_" in input or input.isupper():
         snake = True
 
     return camel_or_pascal and snake
+
+
+def remove_spaces(text: str) -> str:
+    """
+    Remove the spaces from a text string.
+    """
+    return text.replace(" ", "")
```

### Comparing `neo4j_runway-0.2.1/pyproject.toml` & `neo4j_runway-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neo4j-runway"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Python library that contains tools for data discovery, data model generation and ingestion for the Neo4j graph database."
 authors = ["Alex Gilmore", "Jason Booth", "Dan Bukowski"]
 license = "MIT"
 readme = "README.md"
 keywords = ["graph", "neo4j", "data model"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `neo4j_runway-0.2.1/PKG-INFO` & `neo4j_runway-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j-runway
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python library that contains tools for data discovery, data model generation and ingestion for the Neo4j graph database.
 License: MIT
 Keywords: graph,neo4j,data model
 Author: Alex Gilmore
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

