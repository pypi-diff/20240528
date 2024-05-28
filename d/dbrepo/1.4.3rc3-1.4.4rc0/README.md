# Comparing `tmp/dbrepo-1.4.3rc3.tar.gz` & `tmp/dbrepo-1.4.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbrepo-1.4.3rc3.tar", last modified: Fri May  3 12:18:21 2024, max compression
+gzip compressed data, was "dbrepo-1.4.4rc0.tar", last modified: Tue May 28 09:32:03 2024, max compression
```

## Comparing `dbrepo-1.4.3rc3.tar` & `dbrepo-1.4.4rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/LICENSE
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)     4814 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/README.md
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.466653 dbrepo-1.4.3rc3/dbrepo/
--rw-r--r--   0 mweise    (1000) mweise    (1000)     2940 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/dbrepo/AmqpClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    75175 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/dbrepo/RestClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1609 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/dbrepo/UploadClient.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/dbrepo/__init__.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.466653 dbrepo-1.4.3rc3/dbrepo/api/
--rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/dbrepo/api/__init__.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    21236 2024-05-03 12:17:16.000000 dbrepo-1.4.3rc3/dbrepo/api/dto.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-04-19 11:42:17.000000 dbrepo-1.4.3rc3/dbrepo/api/encoder.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/dbrepo/api/exceptions.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/dbrepo.egg-info/
--rw-r--r--   0 mweise    (1000) mweise    (1000)    18899 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/PKG-INFO
--rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/SOURCES.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/dependency_links.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/requires.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-05-03 12:18:21.000000 dbrepo-1.4.3rc3/dbrepo.egg-info/top_level.txt
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1102 2024-05-03 12:18:17.000000 dbrepo-1.4.3rc3/pyproject.toml
--rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/setup.cfg
--rw-r--r--   0 mweise    (1000) mweise    (1000)      410 2024-05-03 12:18:17.000000 dbrepo-1.4.3rc3/setup.py
-drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-03 12:18:21.470653 dbrepo-1.4.3rc3/tests/
--rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_analyse.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_container.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_database.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11310 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_identifier.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_license.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14639 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_query.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)     1308 2024-04-12 20:45:40.000000 dbrepo-1.4.3rc3/tests/test_rest_client.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    29497 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_table.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_user.py
--rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.3rc3/tests/test_view.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-28 09:32:03.268117 dbrepo-1.4.4rc0/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11357 2024-04-12 20:45:40.000000 dbrepo-1.4.4rc0/LICENSE
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18895 2024-05-28 09:32:03.264117 dbrepo-1.4.4rc0/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     4805 2024-05-27 05:20:58.000000 dbrepo-1.4.4rc0/README.md
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-28 09:32:03.264117 dbrepo-1.4.4rc0/dbrepo/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     2819 2024-05-17 21:25:33.000000 dbrepo-1.4.4rc0/dbrepo/AmqpClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    82986 2024-05-28 09:29:44.000000 dbrepo-1.4.4rc0/dbrepo/RestClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1488 2024-05-17 21:25:33.000000 dbrepo-1.4.4rc0/dbrepo/UploadClient.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.4rc0/dbrepo/__init__.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-28 09:32:03.264117 dbrepo-1.4.4rc0/dbrepo/api/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        0 2024-04-12 20:45:40.000000 dbrepo-1.4.4rc0/dbrepo/api/__init__.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    21849 2024-05-27 15:29:41.000000 dbrepo-1.4.4rc0/dbrepo/api/dto.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      368 2024-05-17 21:25:33.000000 dbrepo-1.4.4rc0/dbrepo/api/encoder.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1265 2024-04-12 20:45:40.000000 dbrepo-1.4.4rc0/dbrepo/api/exceptions.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-28 09:32:03.264117 dbrepo-1.4.4rc0/dbrepo.egg-info/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    18895 2024-05-28 09:32:03.000000 dbrepo-1.4.4rc0/dbrepo.egg-info/PKG-INFO
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      582 2024-05-28 09:32:03.000000 dbrepo-1.4.4rc0/dbrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        1 2024-05-28 09:32:03.000000 dbrepo-1.4.4rc0/dbrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       42 2024-05-28 09:32:03.000000 dbrepo-1.4.4rc0/dbrepo.egg-info/requires.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)        7 2024-05-28 09:32:03.000000 dbrepo-1.4.4rc0/dbrepo.egg-info/top_level.txt
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1102 2024-05-28 09:31:42.000000 dbrepo-1.4.4rc0/pyproject.toml
+-rw-r--r--   0 mweise    (1000) mweise    (1000)       38 2024-05-28 09:32:03.268117 dbrepo-1.4.4rc0/setup.cfg
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      415 2024-05-28 09:31:43.000000 dbrepo-1.4.4rc0/setup.py
+drwxr-xr-x   0 mweise    (1000) mweise    (1000)        0 2024-05-28 09:32:03.264117 dbrepo-1.4.4rc0/tests/
+-rw-r--r--   0 mweise    (1000) mweise    (1000)      729 2024-04-13 22:35:52.000000 dbrepo-1.4.4rc0/tests/test_analyse.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     5565 2024-04-13 22:35:52.000000 dbrepo-1.4.4rc0/tests/test_container.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    26166 2024-04-13 22:35:52.000000 dbrepo-1.4.4rc0/tests/test_database.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11439 2024-05-17 21:25:33.000000 dbrepo-1.4.4rc0/tests/test_identifier.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1083 2024-04-13 22:35:52.000000 dbrepo-1.4.4rc0/tests/test_license.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14668 2024-05-17 21:25:33.000000 dbrepo-1.4.4rc0/tests/test_query.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)     1316 2024-05-17 21:25:33.000000 dbrepo-1.4.4rc0/tests/test_rest_client.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    29671 2024-05-17 21:25:33.000000 dbrepo-1.4.4rc0/tests/test_table.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    14697 2024-04-13 22:35:52.000000 dbrepo-1.4.4rc0/tests/test_user.py
+-rw-r--r--   0 mweise    (1000) mweise    (1000)    11997 2024-04-13 22:35:52.000000 dbrepo-1.4.4rc0/tests/test_view.py
```

### Comparing `dbrepo-1.4.3rc3/LICENSE` & `dbrepo-1.4.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc3/PKG-INFO` & `dbrepo-1.4.4rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.3rc3
+Version: 1.4.4rc0
 Summary: DBRepo Python Library
-Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
+Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -203,16 +203,16 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
-Project-URL: Homepage, https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.2/
-Project-URL: Documentation, https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.2/sphinx/
+Project-URL: Homepage, https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/
+Project-URL: Documentation, https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/sphinx/
 Project-URL: Issues, https://gitlab.phaidra.org/fair-data-austria-db-repository/fda-services/-/issues
 Project-URL: Source, https://gitlab.phaidra.org/fair-data-austria-db-repository/fda-services/
 Keywords: DBRepo,Database Repository
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
@@ -224,15 +224,15 @@
 Requires-Dist: pika
 Requires-Dist: pydantic
 Requires-Dist: tuspy
 Requires-Dist: pandas
 
 # DBRepo Python Library
 
-Official client library for [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/__APPVERSION__/), a database
+Official client library for [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/), a database
 repository to support research based
 on [requests](https://pypi.org/project/requests/), [pydantic](https://pypi.org/project/pydantic/), [tuspy](https://pypi.org/project/tuspy/)
 and [pika](https://pypi.org/project/pika/).
 
 ## Installing
 
 ```console
```

### Comparing `dbrepo-1.4.3rc3/README.md` & `dbrepo-1.4.4rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DBRepo Python Library
 
-Official client library for [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/__APPVERSION__/), a database
+Official client library for [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/), a database
 repository to support research based
 on [requests](https://pypi.org/project/requests/), [pydantic](https://pypi.org/project/pydantic/), [tuspy](https://pypi.org/project/tuspy/)
 and [pika](https://pypi.org/project/pika/).
 
 ## Installing
 
 ```console
```

### Comparing `dbrepo-1.4.3rc3/dbrepo/AmqpClient.py` & `dbrepo-1.4.4rc0/dbrepo/AmqpClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 
     def __init__(self,
                  broker_host: str = 'broker-service',
                  broker_port: int = 5672,
                  broker_virtual_host: str = '/',
                  username: str = None,
                  password: str = None) -> None:
-        logging.getLogger('requests').setLevel(logging.INFO)
-        logging.getLogger('urllib3').setLevel(logging.INFO)
         logging.basicConfig(format='%(asctime)s %(name)-12s %(levelname)-6s %(message)s', level=logging.DEBUG,
                             stream=sys.stdout)
         self.broker_host = os.environ.get('AMQP_API_HOST', broker_host)
         self.broker_port = os.environ.get('AMQP_API_PORT', broker_port)
         if os.environ.get('AMQP_API_VIRTUAL_HOST') is not None:
             self.broker_virtual_host = os.environ.get('AMQP_API_VIRTUAL_HOST')
         else:
```

### Comparing `dbrepo-1.4.3rc3/dbrepo/RestClient.py` & `dbrepo-1.4.4rc0/dbrepo/RestClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     secure: bool = None
 
     def __init__(self,
                  endpoint: str = 'http://gateway-service',
                  username: str = None,
                  password: str = None,
                  secure: bool = True) -> None:
-        logging.getLogger('requests').setLevel(logging.INFO)
-        logging.getLogger('urllib3').setLevel(logging.INFO)
         logging.basicConfig(format='%(asctime)s %(name)-12s %(levelname)-6s %(message)s', level=logging.DEBUG,
                             stream=sys.stdout)
         self.endpoint = os.environ.get('REST_API_ENDPOINT', endpoint)
         self.username = os.environ.get('REST_API_USERNAME', username)
         self.password = os.environ.get('REST_API_PASSWORD', password)
         if os.environ.get('REST_API_SECURE') is not None:
             self.secure = os.environ.get('REST_API_SECURE') == 'True'
@@ -516,14 +514,35 @@
             return
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to delete table: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to delete table: not found')
         raise ResponseCodeError(f'Failed to delete table: response code: {response.status_code} is not 202 (ACCEPTED)')
 
+    def get_table_metadata(self, database_id: int) -> Database:
+        """
+        Generate metadata of all system-versioned tables in a database with given id.
+
+        :param database_id: The database id.
+
+        :raises ResponseCodeError: If something went wrong with the retrieval.
+        :raises ForbiddenError: If the action is not allowed.
+        :raises NotExistsError: If the container does not exist.
+        """
+        url = f'/api/database/{database_id}/metadata/table'
+        response = self._wrapper(method="put", url=url, force_auth=True)
+        if response.status_code == 200:
+            body = response.json()
+            return Database.model_validate(body)
+        if response.status_code == 403:
+            raise ForbiddenError(f'Failed to get tables metadata: not allowed')
+        if response.status_code == 404:
+            raise NotExistsError(f'Failed to get tables metadata: not found')
+        raise ResponseCodeError(f'Failed to get tables metadata: response code: {response.status_code} is not 200 (OK)')
+
     def get_views(self, database_id: int) -> List[View]:
         """
         Gets views of a database with given database id.
 
         :param database_id: The database id.
 
         :returns: The list of views, if successful.
@@ -653,14 +672,35 @@
             raise MalformedError(f'Failed to get view data: service rejected malformed payload')
         if response.status_code == 403:
             raise ForbiddenError(f'Failed to get view data: not allowed')
         if response.status_code == 404:
             raise NotExistsError(f'Failed to get view data: not found')
         raise ResponseCodeError(f'Failed to get view data: response code: {response.status_code} is not 200 (OK)')
 
+    def get_views_metadata(self, database_id: int) -> Database:
+        """
+        Generate metadata of all views in a database with given id.
+
+        :param database_id: The database id.
+
+        :raises ResponseCodeError: If something went wrong with the retrieval.
+        :raises ForbiddenError: If the action is not allowed.
+        :raises NotExistsError: If the container does not exist.
+        """
+        url = f'/api/database/{database_id}/metadata/view'
+        response = self._wrapper(method="put", url=url, force_auth=True)
+        if response.status_code == 200:
+            body = response.json()
+            return Database.model_validate(body)
+        if response.status_code == 403:
+            raise ForbiddenError(f'Failed to get views metadata: not allowed')
+        if response.status_code == 404:
+            raise NotExistsError(f'Failed to get views metadata: not found')
+        raise ResponseCodeError(f'Failed to get views metadata: response code: {response.status_code} is not 200 (OK)')
+
     def get_table_data(self, database_id: int, table_id: int, page: int = 0, size: int = 10,
                        timestamp: datetime.datetime = None, df: bool = False) -> Result | DataFrame:
         """
         Get data of a table in a database with given database id and table id.
 
         :param database_id: The database id.
         :param table_id: The table id.
@@ -785,15 +825,15 @@
         :returns: The determined data types, if successful.
 
         :raises ResponseCodeError: If something went wrong with the analysis.
         :raises MalformedError: If the payload is rejected by the service.
         :raises NotExistsError: If the file was not found by the Analyse Service.
         """
         if upload:
-            client = UploadClient(endpoint=self.endpoint)
+            client = UploadClient(endpoint=f"{self.endpoint}/api/upload/files")
             filename = client.upload(file_path=file_path)
         else:
             filename = file_path
         params = [
             ('filename', filename),
             ('separator', separator),
             ('enum', enum),
@@ -1115,15 +1155,15 @@
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises MalformedError: If the payload is rejected by the service.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If the database, table or user does not exist.
         :raises QueryStoreError: The query store rejected the query.
         :raises MetadataConsistencyError: The service failed to parse columns from the metadata database.
         """
-        url = f'/api/database/{database_id}/query'
+        url = f'/api/database/{database_id}/subset'
         if page is not None and size is not None:
             url += f'?page={page}&size={size}'
         response = self._wrapper(method="post", url=url, force_auth=True,
                                  payload=ExecuteQuery(statement=query, timestamp=timestamp))
         if response.status_code == 202:
             body = response.json()
             return Result.model_validate(body)
@@ -1158,15 +1198,15 @@
         :raises MalformedError: If the payload is rejected by the service.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If the database, query or user does not exist.
         :raises QueryStoreError: The query store rejected the query.
         :raises MetadataConsistencyError: The service failed to parse columns from the metadata database.
         """
         headers = {}
-        url = f'/api/database/{database_id}/query/{query_id}/data'
+        url = f'/api/database/{database_id}/subset/{query_id}/data'
         if page is not None and size is not None:
             url += f'?page={page}&size={size}'
         response = self._wrapper(method="get", url=url, headers=headers)
         if response.status_code == 200:
             body = response.json()
             res = Result.model_validate(body)
             if df:
@@ -1199,15 +1239,15 @@
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises MalformedError: If the payload is rejected by the service.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If the database, query or user does not exist.
         :raises QueryStoreError: The query store rejected the query.
         :raises MetadataConsistencyError: The service failed to parse columns from the metadata database.
         """
-        url = f'/api/database/{database_id}/query/{query_id}/data'
+        url = f'/api/database/{database_id}/subset/{query_id}/data'
         if page is not None and size is not None:
             url += f'?page={page}&size={size}'
         response = self._wrapper(method="head", url=url)
         if response.status_code == 200:
             return int(response.headers.get('X-Count'))
         if response.status_code == 400:
             raise MalformedError(f'Failed to re-execute query: service rejected malformed payload')
@@ -1233,15 +1273,15 @@
 
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thedatabase, query or user does not exist.
         :raises QueryStoreError: The query store rejected the query.
         :raises MetadataConsistencyError: The service failed to parse columns from the metadata database.
         """
-        url = f'/api/database/{database_id}/query/{query_id}'
+        url = f'/api/database/{database_id}/subset/{query_id}'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
             return Query.model_validate(body)
         if response.status_code == 404:
             raise NotExistsError(f'Failed to find query: not found')
         if response.status_code == 403 or response.status_code == 405:
@@ -1263,15 +1303,15 @@
 
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises MalformedError: If the query is rejected by the service.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thedatabase or user does not exist.
         :raises QueryStoreError: The query store rejected the query.
         """
-        url = f'/api/database/{database_id}/query'
+        url = f'/api/database/{database_id}/subset'
         response = self._wrapper(method="get", url=url)
         if response.status_code == 200:
             body = response.json()
             return TypeAdapter(List[Query]).validate_python(body)
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to find queries: not allowed')
         if response.status_code == 404:
@@ -1295,15 +1335,15 @@
         :returns: The query, if successful.
 
         :raises ResponseCodeError: If something went wrong with the retrieval.
         :raises ForbiddenError: If the action is not allowed.
         :raises NotExistsError: If thedatabase or user does not exist.
         :raises QueryStoreError: The query store rejected the update.
         """
-        url = f'/api/database/{database_id}/query/{query_id}'
+        url = f'/api/database/{database_id}/subset/{query_id}'
         response = self._wrapper(method="put", url=url, force_auth=True, payload=UpdateQuery(persist=persist))
         if response.status_code == 202:
             body = response.json()
             return Query.model_validate(body)
         if response.status_code == 403 or response.status_code == 405:
             raise ForbiddenError(f'Failed to update query: not allowed')
         if response.status_code == 404:
@@ -1317,15 +1357,15 @@
                           publisher: str, creators: List[CreateIdentifierCreator], publication_year: int,
                           descriptions: List[CreateIdentifierDescription] = None,
                           funders: List[CreateIdentifierFunder] = None, licenses: List[License] = None,
                           language: Language = None, query_id: int = None, view_id: int = None, table_id: int = None,
                           publication_day: int = None, publication_month: int = None,
                           related_identifiers: List[CreateRelatedIdentifier] = None) -> Identifier:
         """
-        Create an identifier
+        Create an identifier draft.
 
         :param database_id: The database id of the created identifier.
         :param type: The type of the created identifier.
         :param titles: The titles of the created identifier.
         :param publisher: The publisher of the created identifier.
         :param creators: The creator(s) of the created identifier.
         :param publication_year: The publication year of the created identifier.
@@ -1341,15 +1381,15 @@
         :param related_identifiers: The related identifier(s) of the created identifier. Optional.
 
         :returns: The identifier, if successful.
 
         :raises ResponseCodeError: If something went wrong with the creation of the identifier.
         :raises ForbiddenError: If the action is not allowed.
         :raises MalformedError: If the payload is rejected by the service.
-        :raises NotExistsError: If the database, table/view/query or user does not exist.
+        :raises NotExistsError: If the database, table/view/subset or user does not exist.
         :raises ExternalSystemError: If the external system (DataCite) refused communication with the service.
         """
         url = f'/api/identifier'
         payload = CreateIdentifier(database_id=database_id, type=type, titles=titles, publisher=publisher,
                                    creators=creators, publication_year=publication_year, descriptions=descriptions,
                                    funders=funders, licenses=licenses, language=language, query_id=query_id,
                                    view_id=view_id, table_id=table_id, publication_day=publication_day,
@@ -1365,14 +1405,101 @@
         if response.status_code == 404:
             raise NotExistsError(f'Failed to create identifier: not found')
         if response.status_code == 503:
             raise ExternalSystemError(f'Failed to create identifier: external system rejected communication')
         raise ResponseCodeError(
             f'Failed to create identifier: response code: {response.status_code} is not 201 (CREATED)')
 
+    def save_identifier(self, identifier_id: int, database_id: int, type: IdentifierType,
+                        titles: List[CreateIdentifierTitle], publisher: str, creators: List[CreateIdentifierCreator],
+                        publication_year: int, descriptions: List[CreateIdentifierDescription] = None,
+                        funders: List[CreateIdentifierFunder] = None, licenses: List[License] = None,
+                        language: Language = None, query_id: int = None, view_id: int = None, table_id: int = None,
+                        publication_day: int = None, publication_month: int = None,
+                        related_identifiers: List[CreateRelatedIdentifier] = None) -> Identifier:
+        """
+        Save an existing identifier and update the metadata attached to it.
+
+        :param identifier_id: The identifier id.
+        :param database_id: The database id of the created identifier.
+        :param type: The type of the created identifier.
+        :param titles: The titles of the created identifier.
+        :param publisher: The publisher of the created identifier.
+        :param creators: The creator(s) of the created identifier.
+        :param publication_year: The publication year of the created identifier.
+        :param descriptions: The description(s) of the created identifier. Optional.
+        :param funders: The funders(s) of the created identifier. Optional.
+        :param licenses: The license(s) of the created identifier. Optional.
+        :param language: The language of the created identifier. Optional.
+        :param query_id: The query id of the created identifier. Required when type=SUBSET, otherwise invalid. Optional.
+        :param view_id: The view id of the created identifier. Required when type=VIEW, otherwise invalid. Optional.
+        :param table_id: The table id of the created identifier. Required when type=TABLE, otherwise invalid. Optional.
+        :param publication_day: The publication day of the created identifier. Optional.
+        :param publication_month: The publication month of the created identifier. Optional.
+        :param related_identifiers: The related identifier(s) of the created identifier. Optional.
+
+        :returns: The identifier, if successful.
+
+        :raises ResponseCodeError: If something went wrong with the creation of the identifier.
+        :raises ForbiddenError: If the action is not allowed.
+        :raises MalformedError: If the payload is rejected by the service.
+        :raises NotExistsError: If the database, table/view/subset or user does not exist.
+        :raises ExternalSystemError: If the external system (DataCite) refused communication with the service.
+        """
+        url = f'/api/identifier/{identifier_id}'
+        payload = CreateIdentifier(database_id=database_id, type=type, titles=titles, publisher=publisher,
+                                   creators=creators, publication_year=publication_year, descriptions=descriptions,
+                                   funders=funders, licenses=licenses, language=language, query_id=query_id,
+                                   view_id=view_id, table_id=table_id, publication_day=publication_day,
+                                   publication_month=publication_month, related_identifiers=related_identifiers)
+        response = self._wrapper(method="put", url=url, force_auth=True, payload=payload)
+        if response.status_code == 201:
+            body = response.json()
+            return Identifier.model_validate(body)
+        if response.status_code == 400:
+            raise MalformedError(f'Failed to save identifier: service rejected malformed payload')
+        if response.status_code == 403 or response.status_code == 405:
+            raise ForbiddenError(f'Failed to save identifier: not allowed')
+        if response.status_code == 404:
+            raise NotExistsError(f'Failed to save identifier: not found')
+        if response.status_code == 503:
+            raise ExternalSystemError(f'Failed to save identifier: external system rejected communication')
+        raise ResponseCodeError(
+            f'Failed to save identifier: response code: {response.status_code} is not 202 (ACCEPTED)')
+
+    def publish_identifier(self, identifier_id: int) -> Identifier:
+        """
+        Publish an identifier with given id.
+
+        :param identifier_id: The identifier id.
+
+        :returns: The identifier, if successful.
+
+        :raises ResponseCodeError: If something went wrong with the creation of the identifier.
+        :raises ForbiddenError: If the action is not allowed.
+        :raises MalformedError: If the payload is rejected by the service.
+        :raises NotExistsError: If the database, table/view/subset or user does not exist.
+        :raises ExternalSystemError: If the external system (DataCite) refused communication with the service.
+        """
+        url = f'/api/identifier/{identifier_id}/publish'
+        response = self._wrapper(method="put", url=url, force_auth=True)
+        if response.status_code == 201:
+            body = response.json()
+            return Identifier.model_validate(body)
+        if response.status_code == 400:
+            raise MalformedError(f'Failed to publish identifier: service rejected malformed payload')
+        if response.status_code == 403 or response.status_code == 405:
+            raise ForbiddenError(f'Failed to publish identifier: not allowed')
+        if response.status_code == 404:
+            raise NotExistsError(f'Failed to publish identifier: not found')
+        if response.status_code == 503:
+            raise ExternalSystemError(f'Failed to publish identifier: external system rejected communication')
+        raise ResponseCodeError(
+            f'Failed to publish identifier: response code: {response.status_code} is not 201 (CREATED)')
+
     def suggest_identifier(self, uri: str) -> Identifier:
         """
         Suggest identifier metadata for a given identifier URI. Example: ROR, ORCID, ISNI, GND, DOI.
 
         :param uri: The identifier URI.
 
         :returns: The identifier, if successful.
```

### Comparing `dbrepo-1.4.3rc3/dbrepo/UploadClient.py` & `dbrepo-1.4.4rc0/dbrepo/UploadClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     constructor parameters with the environment variables.
 
     :param endpoint: The REST API endpoint. Optional. Default: "http://gateway-service/api/upload/files"
     """
     endpoint: str = None
 
     def __init__(self, endpoint: str = 'http://gateway-service/api/upload/files') -> None:
-        logging.getLogger('requests').setLevel(logging.INFO)
-        logging.getLogger('urllib3').setLevel(logging.INFO)
         logging.basicConfig(format='%(asctime)s %(name)-12s %(levelname)-6s %(message)s', level=logging.DEBUG,
                             stream=sys.stdout)
         self.endpoint = os.environ.get('REST_UPLOAD_ENDPOINT', endpoint)
 
     def upload(self, file_path: str) -> str:
         """
         Imports a file through the Upload Service into the Storage Service.
```

### Comparing `dbrepo-1.4.3rc3/dbrepo/api/dto.py` & `dbrepo-1.4.4rc0/dbrepo/api/dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -620,14 +620,15 @@
     query_hash: str
     created: Timestamp
     creator: User
     internal_name: str
     is_public: bool
     initial_view: bool
     last_modified: Timestamp
+    columns: List[ViewColumn]
     identifiers: List[Identifier] = field(default_factory=list)
 
 
 class CreateView(BaseModel):
     name: str
     query: str
     is_public: bool
@@ -873,14 +874,15 @@
     table_id: int
     internal_name: str
     auto_generated: bool
     column_type: ColumnType
     is_public: bool
     is_null_allowed: bool
     alias: Optional[str] = None
+    description: Optional[str] = None
     size: Optional[int] = None
     d: Optional[int] = None
     mean: Optional[float] = None
     median: Optional[float] = None
     concept: Optional[Concept] = None
     unit: Optional[Unit] = None
     enums: Optional[List[str]] = field(default_factory=list)
@@ -892,14 +894,35 @@
     max_data_length: Optional[int] = None
     num_rows: Optional[int] = None
     val_min: Optional[float] = None
     val_max: Optional[float] = None
     std_dev: Optional[float] = None
 
 
+class ViewColumn(BaseModel):
+    id: int
+    name: str
+    database_id: int
+    internal_name: str
+    auto_generated: bool
+    column_type: ColumnType
+    is_public: bool
+    is_null_allowed: bool
+    alias: Optional[str] = None
+    size: Optional[int] = None
+    d: Optional[int] = None
+    mean: Optional[float] = None
+    median: Optional[float] = None
+    concept: Optional[Concept] = None
+    unit: Optional[Unit] = None
+    date_format: Optional[ImageDate] = None
+    index_length: Optional[int] = None
+    length: Optional[int] = None
+
+
 class Table(BaseModel):
     id: int
     database_id: int
     name: str
     creator: User
     owner: User
     created: Timestamp
```

### Comparing `dbrepo-1.4.3rc3/dbrepo/api/exceptions.py` & `dbrepo-1.4.4rc0/dbrepo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc3/dbrepo.egg-info/PKG-INFO` & `dbrepo-1.4.4rc0/dbrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dbrepo
-Version: 1.4.3rc3
+Version: 1.4.4rc0
 Summary: DBRepo Python Library
-Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo//
+Home-page: https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/
 Author: Martin Weise
 Author-email: "Martin Weise, TU Wien" <martin.weise@tuwien.ac.at>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -203,16 +203,16 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
-Project-URL: Homepage, https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.2/
-Project-URL: Documentation, https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.2/sphinx/
+Project-URL: Homepage, https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/
+Project-URL: Documentation, https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/sphinx/
 Project-URL: Issues, https://gitlab.phaidra.org/fair-data-austria-db-repository/fda-services/-/issues
 Project-URL: Source, https://gitlab.phaidra.org/fair-data-austria-db-repository/fda-services/
 Keywords: DBRepo,Database Repository
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
@@ -224,15 +224,15 @@
 Requires-Dist: pika
 Requires-Dist: pydantic
 Requires-Dist: tuspy
 Requires-Dist: pandas
 
 # DBRepo Python Library
 
-Official client library for [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/__APPVERSION__/), a database
+Official client library for [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/), a database
 repository to support research based
 on [requests](https://pypi.org/project/requests/), [pydantic](https://pypi.org/project/pydantic/), [tuspy](https://pypi.org/project/tuspy/)
 and [pika](https://pypi.org/project/pika/).
 
 ## Installing
 
 ```console
```

### Comparing `dbrepo-1.4.3rc3/dbrepo.egg-info/SOURCES.txt` & `dbrepo-1.4.4rc0/dbrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc3/pyproject.toml` & `dbrepo-1.4.4rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbrepo"
-version = "1.4.3rc3"
+version = "1.4.4rc0"
 description = "DBRepo Python Library"
 keywords = [
     "DBRepo",
     "Database Repository"
 ]
 authors = [
     { name = "Martin Weise, TU Wien", email = "martin.weise@tuwien.ac.at" }
@@ -30,11 +30,11 @@
 [build-system]
 requires = [
     "setuptools >= 61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
-Homepage = "https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.2/"
-Documentation = "https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.2/sphinx/"
+Homepage = "https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/"
+Documentation = "https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/1.4.3/sphinx/"
 Issues = "https://gitlab.phaidra.org/fair-data-austria-db-repository/fda-services/-/issues"
 Source = "https://gitlab.phaidra.org/fair-data-austria-db-repository/fda-services/"
```

### Comparing `dbrepo-1.4.3rc3/tests/test_analyse.py` & `dbrepo-1.4.4rc0/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc3/tests/test_container.py` & `dbrepo-1.4.4rc0/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc3/tests/test_database.py` & `dbrepo-1.4.4rc0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc3/tests/test_identifier.py` & `dbrepo-1.4.4rc0/tests/test_identifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 
 from dbrepo.RestClient import RestClient
 
 from dbrepo.api.dto import Identifier, IdentifierType, CreateIdentifierTitle, CreateIdentifierCreator, \
     IdentifierCreator, IdentifierTitle, IdentifierDescription, CreateIdentifierDescription, Language, \
     CreateIdentifierFunder, CreateRelatedIdentifier, RelatedIdentifierRelation, RelatedIdentifierType, IdentifierFunder, \
-    RelatedIdentifier
+    RelatedIdentifier, UserBrief, IdentifierStatusType
 from dbrepo.api.exceptions import MalformedError, ForbiddenError, NotExistsError, ExternalSystemError, \
     AuthenticationError
 
 
 class IdentifierTest(unittest.TestCase):
 
     def test_create_identifier_succeeds(self):
@@ -28,118 +28,129 @@
                              language=Language.EN,
                              descriptions=[IdentifierDescription(id=2, description='Test Description')],
                              titles=[IdentifierTitle(id=3, title='Test Title')],
                              funders=[IdentifierFunder(id=4, funder_name='FWF')],
                              related_identifiers=[
                                  RelatedIdentifier(id=7, value='10.12345/abc', relation=RelatedIdentifierRelation.CITES,
                                                    type=RelatedIdentifierType.DOI)],
-                             creators=[IdentifierCreator(id=5, creator_name='Carberry, Josiah')])
+                             creators=[IdentifierCreator(id=5, creator_name='Carberry, Josiah')],
+                             status=IdentifierStatusType.PUBLISHED,
+                             creator=UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise'))
             # mock
             mock.post('/api/identifier', json=exp.model_dump(), status_code=201)
             # test
             client = RestClient(username="a", password="b")
-            response = client.create_identifier(database_id=1, type=IdentifierType.VIEW,
-                                                titles=[CreateIdentifierTitle(title='Test Title')],
-                                                publisher='TU Wien', publication_year=2024,
-                                                language=Language.EN,
-                                                funders=[CreateIdentifierFunder(funder_name='FWF')],
-                                                related_identifiers=[CreateRelatedIdentifier(value='10.12345/abc',
-                                                                                             relation=RelatedIdentifierRelation.CITES,
-                                                                                             type=RelatedIdentifierType.DOI)],
-                                                descriptions=[
-                                                    CreateIdentifierDescription(description='Test Description')],
-                                                creators=[
-                                                    CreateIdentifierCreator(creator_name='Carberry, Josiah')])
+            response = client.create_identifier(
+                database_id=1, type=IdentifierType.VIEW,
+                titles=[CreateIdentifierTitle(title='Test Title')],
+                publisher='TU Wien', publication_year=2024,
+                language=Language.EN,
+                funders=[CreateIdentifierFunder(funder_name='FWF')],
+                related_identifiers=[CreateRelatedIdentifier(value='10.12345/abc',
+                                                             relation=RelatedIdentifierRelation.CITES,
+                                                             type=RelatedIdentifierType.DOI)],
+                descriptions=[CreateIdentifierDescription(description='Test Description')],
+                creators=[CreateIdentifierCreator(creator_name='Carberry, Josiah')])
             self.assertEqual(exp, response)
 
     def test_create_identifier_malformed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
             mock.post('/api/identifier', status_code=400)
             # test
             try:
                 client = RestClient(username="a", password="b")
-                response = client.create_identifier(database_id=1, type=IdentifierType.VIEW,
-                                                    titles=[CreateIdentifierTitle(title='Test Title')],
-                                                    publisher='TU Wien', publication_year=2024,
-                                                    creators=[
-                                                        CreateIdentifierCreator(creator_name='Carberry, Josiah')])
+                response = client.create_identifier(
+                    database_id=1, type=IdentifierType.VIEW,
+                    titles=[CreateIdentifierTitle(title='Test Title')],
+                    descriptions=[CreateIdentifierDescription(description='Test')],
+                    publisher='TU Wien', publication_year=2024,
+                    creators=[CreateIdentifierCreator(creator_name='Carberry, Josiah')])
             except MalformedError:
                 pass
 
     def test_create_identifier_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
             mock.post('/api/identifier', status_code=403)
             # test
             try:
                 client = RestClient(username="a", password="b")
-                response = client.create_identifier(database_id=1, type=IdentifierType.VIEW,
-                                                    titles=[CreateIdentifierTitle(title='Test Title')],
-                                                    publisher='TU Wien', publication_year=2024,
-                                                    creators=[
-                                                        CreateIdentifierCreator(creator_name='Carberry, Josiah')])
+                response = client.create_identifier(
+                    database_id=1, type=IdentifierType.VIEW,
+                    titles=[CreateIdentifierTitle(title='Test Title')],
+                    descriptions=[CreateIdentifierDescription(description='Test')],
+                    publisher='TU Wien', publication_year=2024,
+                    creators=[CreateIdentifierCreator(creator_name='Carberry, Josiah')])
             except ForbiddenError:
                 pass
 
     def test_create_identifier_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
             mock.post('/api/identifier', status_code=404)
             # test
             try:
                 client = RestClient(username="a", password="b")
-                response = client.create_identifier(database_id=1, type=IdentifierType.VIEW,
-                                                    titles=[CreateIdentifierTitle(title='Test Title')],
-                                                    publisher='TU Wien', publication_year=2024,
-                                                    creators=[
-                                                        CreateIdentifierCreator(creator_name='Carberry, Josiah')])
+                response = client.create_identifier(
+                    database_id=1, type=IdentifierType.VIEW,
+                    titles=[CreateIdentifierTitle(title='Test Title')],
+                    descriptions=[CreateIdentifierDescription(description='Test')],
+                    publisher='TU Wien', publication_year=2024,
+                    creators=[CreateIdentifierCreator(creator_name='Carberry, Josiah')])
             except NotExistsError:
                 pass
 
     def test_create_identifier_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
             mock.post('/api/identifier', status_code=503)
             # test
             try:
                 client = RestClient(username="a", password="b")
-                response = client.create_identifier(database_id=1, type=IdentifierType.VIEW,
-                                                    titles=[CreateIdentifierTitle(title='Test Title')],
-                                                    publisher='TU Wien', publication_year=2024,
-                                                    creators=[
-                                                        CreateIdentifierCreator(creator_name='Carberry, Josiah')])
+                response = client.create_identifier(
+                    database_id=1, type=IdentifierType.VIEW,
+                    titles=[CreateIdentifierTitle(title='Test Title')],
+                    descriptions=[CreateIdentifierDescription(description='Test')],
+                    publisher='TU Wien', publication_year=2024,
+                    creators=[CreateIdentifierCreator(creator_name='Carberry, Josiah')])
             except ExternalSystemError:
                 pass
 
     def test_create_identifier_not_auth_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
             mock.post('/api/identifier', status_code=503)
             # test
             try:
-                response = RestClient().create_identifier(database_id=1, type=IdentifierType.VIEW,
-                                                          titles=[CreateIdentifierTitle(title='Test Title')],
-                                                          publisher='TU Wien', publication_year=2024,
-                                                          creators=[
-                                                              CreateIdentifierCreator(creator_name='Carberry, Josiah')])
+                response = RestClient().create_identifier(
+                    database_id=1, type=IdentifierType.VIEW,
+                    titles=[CreateIdentifierTitle(title='Test Title')],
+                    descriptions=[CreateIdentifierDescription(description='Test')],
+                    publisher='TU Wien', publication_year=2024,
+                    creators=[CreateIdentifierCreator(creator_name='Carberry, Josiah')])
             except AuthenticationError:
                 pass
 
     def test_suggest_identifier_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = Identifier(id=10,
                              database_id=1,
                              publication_year=2024,
                              publisher='TU Wien',
+                             titles=[IdentifierTitle(id=10, title='Test Title')],
+                             descriptions=[IdentifierDescription(id=10, description='Test')],
                              created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                              last_modified=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                              type=IdentifierType.VIEW,
                              creators=[IdentifierCreator(id=5, creator_name='Carberry, Josiah',
-                                                         name_identifier='https://orcid.org/0000-0002-1825-0097')])
+                                                         name_identifier='https://orcid.org/0000-0002-1825-0097')],
+                             status=IdentifierStatusType.DRAFT,
+                             creator=UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise')
+                             )
             # mock
             mock.get('/api/identifier?url=https://orcid.org/0000-0002-1825-0097', json=exp.model_dump())
             # test
             response = RestClient().suggest_identifier("https://orcid.org/0000-0002-1825-0097")
             self.assertEqual(exp, response)
 
     def test_suggest_identifier_not_found_fails(self):
@@ -162,19 +173,20 @@
                               created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                               last_modified=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                               type=IdentifierType.VIEW,
                               language=Language.EN,
                               descriptions=[IdentifierDescription(id=2, description='Test Description')],
                               titles=[IdentifierTitle(id=3, title='Test Title')],
                               funders=[IdentifierFunder(id=4, funder_name='FWF')],
-                              related_identifiers=[
-                                  RelatedIdentifier(id=7, value='10.12345/abc',
-                                                    relation=RelatedIdentifierRelation.CITES,
-                                                    type=RelatedIdentifierType.DOI)],
-                              creators=[IdentifierCreator(id=5, creator_name='Carberry, Josiah')])]
+                              related_identifiers=[RelatedIdentifier(id=7, value='10.12345/abc',
+                                                                     relation=RelatedIdentifierRelation.CITES,
+                                                                     type=RelatedIdentifierType.DOI)],
+                              creators=[IdentifierCreator(id=5, creator_name='Carberry, Josiah')],
+                              status=IdentifierStatusType.PUBLISHED,
+                              creator=UserBrief(id='8638c043-5145-4be8-a3e4-4b79991b0a16', username='mweise'))]
             # mock
             mock.get('/api/pid', json=[exp[0].model_dump()], headers={"Accept": "application/json"})
             # test
             response = RestClient().get_identifiers()
             self.assertEqual(exp, response)
 
     def test_get_identifiers_ld_json_succeeds(self):
```

### Comparing `dbrepo-1.4.3rc3/tests/test_license.py` & `dbrepo-1.4.4rc0/tests/test_license.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc3/tests/test_query.py` & `dbrepo-1.4.4rc0/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,85 +17,85 @@
 
     def test_execute_query_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
                          headers=[{'id': 0, 'username': 1}],
                          id=None)
             # mock
-            mock.post('/api/database/1/query', json=exp.model_dump(), status_code=202)
+            mock.post('/api/database/1/subset', json=exp.model_dump(), status_code=202)
             # test
             client = RestClient(username="a", password="b")
             response = client.execute_query(database_id=1, page=0, size=10,
                                             query="SELECT id, username FROM some_table WHERE id IN (1,2)")
             self.assertEqual(exp, response)
 
     def test_execute_query_malformed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database/1/query', status_code=400)
+            mock.post('/api/database/1/subset', status_code=400)
             # test
             try:
                 client = RestClient(username="a", password="b")
                 response = client.execute_query(database_id=1,
                                                 query="SELECT id, username FROM some_table WHERE id IN (1,2)")
             except MalformedError:
                 pass
 
     def test_execute_query_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database/1/query', status_code=403)
+            mock.post('/api/database/1/subset', status_code=403)
             # test
             try:
                 client = RestClient(username="a", password="b")
                 response = client.execute_query(database_id=1,
                                                 query="SELECT id, username FROM some_table WHERE id IN (1,2)")
             except ForbiddenError:
                 pass
 
     def test_execute_query_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database/1/query', status_code=404)
+            mock.post('/api/database/1/subset', status_code=404)
             # test
             try:
                 client = RestClient(username="a", password="b")
                 response = client.execute_query(database_id=1,
                                                 query="SELECT id, username FROM some_table WHERE id IN (1,2)")
             except NotExistsError:
                 pass
 
     def test_execute_query_not_valid_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database/1/query', status_code=409)
+            mock.post('/api/database/1/subset', status_code=409)
             # test
             try:
                 client = RestClient(username="a", password="b")
                 response = client.execute_query(database_id=1,
                                                 query="SELECT id, username FROM some_table WHERE id IN (1,2)")
             except QueryStoreError:
                 pass
 
     def test_execute_query_not_expected_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database/1/query', status_code=417)
+            mock.post('/api/database/1/subset', status_code=417)
             # test
             try:
                 client = RestClient(username="a", password="b")
                 response = client.execute_query(database_id=1,
                                                 query="SELECT id, username FROM some_table WHERE id IN (1,2)")
             except MetadataConsistencyError:
                 pass
 
     def test_execute_query_not_auth_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.post('/api/database/1/query', status_code=417)
+            mock.post('/api/database/1/subset', status_code=417)
             # test
             try:
                 response = RestClient().execute_query(database_id=1,
                                                       query="SELECT id, username FROM some_table WHERE id IN (1,2)")
             except AuthenticationError:
                 pass
 
@@ -113,64 +113,64 @@
                         database_id=1,
                         query_hash='da5ff66c4a57683171e2ffcec25298ee684680d1e03633cd286f9067d6924ad8',
                         result_hash='464740ba612225913bb15b26f13377707949b55e65288e89c3f8b4c6469aecb4',
                         is_persisted=False,
                         result_number=None,
                         identifiers=[])
             # mock
-            mock.get('/api/database/1/query/6', json=exp.model_dump())
+            mock.get('/api/database/1/subset/6', json=exp.model_dump())
             # test
             response = RestClient().get_query(database_id=1, query_id=6)
             self.assertEqual(exp, response)
 
     def test_find_query_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query/6', status_code=403)
+            mock.get('/api/database/1/subset/6', status_code=403)
             # test
             try:
                 response = RestClient().get_query(database_id=1, query_id=6)
             except ForbiddenError:
                 pass
 
     def test_find_query_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query/6', status_code=404)
+            mock.get('/api/database/1/subset/6', status_code=404)
             # test
             try:
                 response = RestClient().get_query(database_id=1, query_id=6)
             except NotExistsError:
                 pass
 
     def test_find_query_not_valid_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query/6', status_code=501)
+            mock.get('/api/database/1/subset/6', status_code=501)
             # test
             try:
                 response = RestClient().get_query(database_id=1, query_id=6)
             except QueryStoreError:
                 pass
 
     def test_find_query_not_expected_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query/6', status_code=417)
+            mock.get('/api/database/1/subset/6', status_code=417)
             # test
             try:
                 response = RestClient().get_query(database_id=1, query_id=6)
             except MetadataConsistencyError:
                 pass
 
     def test_get_queries_empty_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = []
             # mock
-            mock.get('/api/database/1/query', json=[])
+            mock.get('/api/database/1/subset', json=[])
             # test
             response = RestClient().get_queries(database_id=1)
             self.assertEqual(exp, response)
 
     def test_get_queries_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = [Query(id=6,
@@ -185,166 +185,166 @@
                          database_id=1,
                          query_hash='da5ff66c4a57683171e2ffcec25298ee684680d1e03633cd286f9067d6924ad8',
                          result_hash='464740ba612225913bb15b26f13377707949b55e65288e89c3f8b4c6469aecb4',
                          is_persisted=False,
                          result_number=None,
                          identifiers=[])]
             # mock
-            mock.get('/api/database/1/query', json=[exp[0].model_dump()])
+            mock.get('/api/database/1/subset', json=[exp[0].model_dump()])
             # test
             response = RestClient().get_queries(database_id=1)
             self.assertEqual(exp, response)
 
     def test_get_queries_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query', status_code=403)
+            mock.get('/api/database/1/subset', status_code=403)
             # test
             try:
                 response = RestClient().get_queries(database_id=1)
             except ForbiddenError:
                 pass
 
     def test_get_queries_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query', status_code=404)
+            mock.get('/api/database/1/subset', status_code=404)
             # test
             try:
                 response = RestClient().get_queries(database_id=1)
             except NotExistsError:
                 pass
 
     def test_get_queries_not_valid_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query', status_code=501)
+            mock.get('/api/database/1/subset', status_code=501)
             # test
             try:
                 response = RestClient().get_queries(database_id=1)
             except QueryStoreError:
                 pass
 
     def test_get_queries_malformed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query', status_code=423)
+            mock.get('/api/database/1/subset', status_code=423)
             # test
             try:
                 response = RestClient().get_queries(database_id=1)
             except MalformedError:
                 pass
 
     def test_get_query_data_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
                          headers=[{'id': 0, 'username': 1}],
                          id=6)
             # mock
-            mock.get('/api/database/1/query/6/data', json=exp.model_dump())
+            mock.get('/api/database/1/subset/6/data', json=exp.model_dump())
             # test
             response = RestClient().get_query_data(database_id=1, query_id=6)
             self.assertEqual(exp, response)
 
     def test_get_query_data_dataframe_succeeds(self):
         with requests_mock.Mocker() as mock:
             res = Result(result=[{'id': 1, 'username': 'foo'}, {'id': 2, 'username': 'bar'}],
                          headers=[{'id': 0, 'username': 1}],
                          id=6)
             exp = DataFrame.from_records(res.model_dump()['result'])
             # mock
-            mock.get('/api/database/1/query/6/data', json=res.model_dump())
+            mock.get('/api/database/1/subset/6/data', json=res.model_dump())
             # test
             response = RestClient().get_query_data(database_id=1, query_id=6, df=True)
             self.assertEqual(exp.shape, response.shape)
             self.assertTrue(DataFrame.equals(exp, response))
 
     def test_get_query_data_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query/6/data', status_code=403)
+            mock.get('/api/database/1/subset/6/data', status_code=403)
             # test
             try:
                 response = RestClient().get_query_data(database_id=1, query_id=6)
             except ForbiddenError:
                 pass
 
     def test_get_query_data_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query/6/data', status_code=404)
+            mock.get('/api/database/1/subset/6/data', status_code=404)
             # test
             try:
                 response = RestClient().get_query_data(database_id=1, query_id=6)
             except NotExistsError:
                 pass
 
     def test_get_query_data_not_valid_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query/6/data', status_code=409)
+            mock.get('/api/database/1/subset/6/data', status_code=409)
             # test
             try:
                 response = RestClient().get_query_data(database_id=1, query_id=6)
             except QueryStoreError:
                 pass
 
     def test_get_query_data_not_consistent_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.get('/api/database/1/query/6/data', status_code=417)
+            mock.get('/api/database/1/subset/6/data', status_code=417)
             # test
             try:
                 response = RestClient().get_query_data(database_id=1, query_id=6)
             except MetadataConsistencyError:
                 pass
 
     def test_get_query_data_count_succeeds(self):
         with requests_mock.Mocker() as mock:
             exp = 2
             # mock
-            mock.head('/api/database/1/query/6/data', headers={'X-Count': str(exp)})
+            mock.head('/api/database/1/subset/6/data', headers={'X-Count': str(exp)})
             # test
             response = RestClient().get_query_data_count(database_id=1, query_id=6)
             self.assertEqual(exp, response)
 
     def test_get_query_data_count_not_allowed_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.head('/api/database/1/query/6/data', status_code=403)
+            mock.head('/api/database/1/subset/6/data', status_code=403)
             # test
             try:
                 response = RestClient().get_query_data_count(database_id=1, query_id=6)
             except ForbiddenError:
                 pass
 
     def test_get_query_data_count_not_found_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.head('/api/database/1/query/6/data', status_code=404)
+            mock.head('/api/database/1/subset/6/data', status_code=404)
             # test
             try:
                 response = RestClient().get_query_data_count(database_id=1, query_id=6)
             except NotExistsError:
                 pass
 
     def test_get_query_data_count_not_valid_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.head('/api/database/1/query/6/data', status_code=409)
+            mock.head('/api/database/1/subset/6/data', status_code=409)
             # test
             try:
                 response = RestClient().get_query_data_count(database_id=1, query_id=6)
             except QueryStoreError:
                 pass
 
     def test_get_query_data_count_not_consistent_fails(self):
         with requests_mock.Mocker() as mock:
             # mock
-            mock.head('/api/database/1/query/6/data', status_code=417)
+            mock.head('/api/database/1/subset/6/data', status_code=417)
             # test
             try:
                 response = RestClient().get_query_data_count(database_id=1, query_id=6)
             except MetadataConsistencyError:
                 pass
```

### Comparing `dbrepo-1.4.3rc3/tests/test_rest_client.py` & `dbrepo-1.4.4rc0/tests/test_rest_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,18 @@
         client = RestClient()
         self.assertEqual("http://gateway-service", client.endpoint)
         self.assertIsNone(client.username)
         self.assertIsNone(client.password)
         self.assertTrue(client.secure)
 
     @mock.patch.dict(os.environ, {
-        "DBREPO_ENDPOINT": "https://test.dbrepo.tuwien.ac.at",
-        "DBREPO_USERNAME": "foo",
-        "DBREPO_PASSWORD": "bar",
-        "DBREPO_SECURE": "False",
+        "REST_API_ENDPOINT": "https://test.dbrepo.tuwien.ac.at",
+        "REST_API_USERNAME": "foo",
+        "REST_API_PASSWORD": "bar",
+        "REST_API_SECURE": "false",
     })
     def test_constructor_environment_succeeds(self):
         # test
         client = RestClient()
         self.assertEqual("https://test.dbrepo.tuwien.ac.at", client.endpoint)
         self.assertEqual("foo", client.username)
         self.assertEqual("bar", client.password)
```

### Comparing `dbrepo-1.4.3rc3/tests/test_table.py` & `dbrepo-1.4.4rc0/tests/test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                                attributes=UserAttributes(theme='light')),
                     created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                     is_versioned=True,
                     created_by='8638c043-5145-4be8-a3e4-4b79991b0a16',
                     queue_name='test',
                     routing_key='dbrepo.test_database_1234.test',
                     is_public=True,
-                    constraints=Constraints(),
+                    constraints=Constraints(primary_key=["ID"], uniques=[], foreign_keys=[], checks=[]),
                     columns=[Column(id=1,
                                     name="ID",
                                     database_id=1,
                                     table_id=2,
                                     internal_name="id",
                                     auto_generated=True,
                                     is_primary_key=True,
@@ -131,15 +131,15 @@
                                     attributes=UserAttributes(theme='light')),
                          created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                          is_versioned=True,
                          created_by='8638c043-5145-4be8-a3e4-4b79991b0a16',
                          queue_name='test',
                          routing_key='dbrepo.test_database_1234.test',
                          is_public=True,
-                         constraints=Constraints(),
+                         constraints=Constraints(primary_key=["ID"], uniques=[], foreign_keys=[], checks=[]),
                          columns=[Column(id=1,
                                          name="ID",
                                          database_id=1,
                                          table_id=2,
                                          internal_name="id",
                                          auto_generated=True,
                                          is_primary_key=True,
@@ -165,15 +165,15 @@
                                    attributes=UserAttributes(theme='light')),
                         created=datetime.datetime(2024, 1, 1, 0, 0, 0, 0, datetime.timezone.utc),
                         is_versioned=True,
                         created_by='8638c043-5145-4be8-a3e4-4b79991b0a16',
                         queue_name='test',
                         routing_key='dbrepo.test_database_1234.test',
                         is_public=True,
-                        constraints=Constraints(),
+                        constraints=Constraints(primary_key=["ID"], uniques=[], foreign_keys=[], checks=[]),
                         columns=[Column(id=1,
                                         name="ID",
                                         database_id=1,
                                         table_id=2,
                                         internal_name="id",
                                         auto_generated=True,
                                         is_primary_key=True,
```

### Comparing `dbrepo-1.4.3rc3/tests/test_user.py` & `dbrepo-1.4.4rc0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `dbrepo-1.4.3rc3/tests/test_view.py` & `dbrepo-1.4.4rc0/tests/test_view.py`

 * *Files identical despite different names*

