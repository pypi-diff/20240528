# Comparing `tmp/datagrok_api-0.0.1.tar.gz` & `tmp/datagrok_api-0.0.2.tar.gz`

## Comparing `datagrok_api-0.0.1.tar` & `datagrok_api-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/example.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/iris.csv
--rw-r--r--   0        0        0    53649 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/iris.layout
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/datagrok_api/__init__.py
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/datagrok_api/datagrok_client.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/.gitignore
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 datagrok_api-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/example.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/iris.csv
+-rw-r--r--   0        0        0    53649 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/iris.layout
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/datagrok_api/__init__.py
+-rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/datagrok_api/datagrok_client.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 datagrok_api-0.0.2/PKG-INFO
```

### Comparing `datagrok_api-0.0.1/example.py` & `datagrok_api-0.0.2/example.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 })
 
 # Downloads file from a given connection
 res = api.download_file('system.demofiles', 'demog.csv')
 print(res.head())
 
 # Uploads iris dataset as a table
-iris_id = api.upload_table('iris', pd.DataFrame(load_iris()['data']))
+iris_id = api.upload_table('iris', pd.DataFrame(load_iris()['data']))['ID']
 
 # Iris also can be uploaded as a file
 # api.upload_file('system.demofiles', 'iris.csv', 'iris.csv')
 
 # Fetches freshly uploaded Iris table 
 res = api.download_table(iris_id)
 print(res.head())
 
 # Creates dashboard from iris table with layout uploaded from file "iris.layout"
-dashboard_id = api.create_dashboard('python-test', iris_id, layout_filename='iris.layout')
+dashboard_id = api.create_dashboard('python-test', iris_id, layout_filename='iris.layout')['ID']
 
 # Shares dashboard with admin
 api.share_dashboard(dashboard_id, 'Test')
```

### Comparing `datagrok_api-0.0.1/iris.csv` & `datagrok_api-0.0.2/iris.csv`

 * *Files identical despite different names*

### Comparing `datagrok_api-0.0.1/iris.layout` & `datagrok_api-0.0.2/iris.layout`

 * *Files identical despite different names*

### Comparing `datagrok_api-0.0.1/datagrok_api/datagrok_client.py` & `datagrok_api-0.0.2/datagrok_api/datagrok_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             Several options supppored: UUID, Grok names (e.g. Namespace.Project.Table)
         
         Returns
         -------
         pandas.DataFrame
             Dataframe with table data
         '''
+        name = name.replace(':', '.')
         endpoint = f"/public/v1/tables/{name}"
         response = self._request('GET', endpoint, content_type="text/plain")
         return pd.read_csv(StringIO(response.text))
 
     def upload_table(self, name, dataframe):
         '''
         Uploads a table to Datagrok.
@@ -59,14 +60,15 @@
             table data to save
 
         Returns
         -------
         object
             set of identifiers for the uploaded table
         '''
+        name = name.replace(':', '.')
         endpoint = f"/public/v1/tables/{name}"
         csv_data = dataframe.to_csv(index=False)
         response = self._request('POST', endpoint, content_type="text/csv", data=csv_data)
         return response.json()
 
     def download_file(self, connector, path):
         '''
@@ -81,14 +83,15 @@
 
         Returns
         -------
         object
             If requested file is csv, returns corresponding pd.Datafrme.
             Otherwise returns list of bytes with file content.
         '''
+        connector = connector.replace(':', '.')
         endpoint = f"/public/v1/files/{connector}/{path}"
         response = self._request('GET', endpoint, content_type="application/octet-stream")
         if path.endswith('.csv'):
             return pd.read_csv(StringIO(response.content.decode('utf-8')))
         return response.content
 
     def upload_file(self, connector, path, file_path):
@@ -100,14 +103,15 @@
         connector: str
             Identifier of a connector: ID or Grok name.
         path: str
             Path to file in a connector
         file_path: str
             Path to local file that needs to be uploaded
         '''
+        connector = connector.replace(':', '.')
         endpoint = f"/public/v1/files/{connector}/{path}"
         with open(file_path, 'rb') as file:
             self._request('POST', endpoint, content_type="application/octet-stream", data=file)
 
     def share_dashboard(self, id, groups, access="View"):
         '''
         Shares a dashboard.
@@ -117,14 +121,15 @@
         id: str
             Identifier of a project: ID or Grok name.
         groups: str
             Comma-separated list of group/user names
         access: str
             Either 'View' or 'Edit'
         '''
+        id = id.replace(':', '.')
         endpoint = f"/public/v1/dashboards/{id}/shares"
         params = {
             'groups': groups,
             'access': access
         }
         self._request('GET', endpoint, params=params)
 
@@ -142,14 +147,16 @@
             Optional. Filename for a project layout.
 
         Returns
         -------
         object
             Identifiers of a project.
         '''
+        name = name.replace(':', '.')
+        table_ids = table_ids.replace(':', '.')
         endpoint = f"/public/v1/dashboards/{name}/{table_ids}"
         if layout_filename:
             with open(layout_filename, 'r') as layout_file:
                 layout = json.load(layout_file)
             response = self._request('POST', endpoint, json=layout, content_type="application/json")
         else:
             response = self._request('POST', endpoint, content_type="application/json")
@@ -167,18 +174,22 @@
             Dict with parameter values for function call.
 
         Returns
         -------
         object
             Result of invocation: either a single value or a list or outputs.
         '''
+        name = name.replace(':', '.')
         endpoint = f"/public/v1/{name}/call"
         response = self._request('POST', endpoint, json=invocation_parameters, content_type="application/json")
         return response.json()
 
     def _request(self, method, endpoint, content_type="application/json", **kwargs):
         url = f"{self.base_url}{endpoint}"
         headers = self.headers.copy()
         headers["Content-Type"] = content_type
         response = requests.request(method, url, headers=headers, **kwargs)
         response.raise_for_status()
+        content = response.content.decode()
+        if 'ApiError' in content:
+            raise Exception(content)
         return response
```

### Comparing `datagrok_api-0.0.1/.gitignore` & `datagrok_api-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `datagrok_api-0.0.1/README.md` & `datagrok_api-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,26 @@
+Metadata-Version: 2.3
+Name: datagrok-api
+Version: 0.0.2
+Summary: Client library for integration with datagrok API
+Project-URL: Homepage, https://github.com/datagrok-ai/public
+Project-URL: Issues, https://github.com/datagrok-ai/public/issues
+Author-email: Andrew Skalkin <askalkin@datagrok.ai>, Amelichev Konstantin <kamelichev@datagrok.ai>
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+
 # Datagrok python client library
 
 This library can be used for integration with datagrok. It is a python wrapper for public API, that has OpenAPI specification available [here](http://public.datagrok.ai/api/public/api.yaml).
 
+Refer to [Help](http://datagrok.ai/help) for more information.
+
 ## Installation
 
 To install package, use [pip](https://pypi.org/project/pip/).
 
 ```shell
 pip install datagrok-api
 ```
@@ -25,40 +40,37 @@
 See [License.md](https://github.com/datagrok-ai/public/blob/master/LICENSE.md).
 
 ## Examples
 
 The package uses Pandas for representation of tables and dataframes.
 
 ```python
-from datagrok_api import DatagrokClient
 import pandas as pd
 from sklearn.datasets import load_iris
 
-api = DatagrokClient('your token', 'datagrok url')
-
 # Calls a Datagrok function
 # Dataframes, columns and primitive data types are supported
 api.call_function('Abs', {
 	'x': -3
 })
 
 # Downloads file from a given connection
 res = api.download_file('system.demofiles', 'demog.csv')
 print(res.head())
 
 # Uploads iris dataset as a table
-iris_id = api.upload_table('iris', pd.DataFrame(load_iris()['data']))
+iris_id = api.upload_table('iris', pd.DataFrame(load_iris()['data']))['ID']
 
 # Iris also can be uploaded as a file
 # api.upload_file('system.demofiles', 'iris.csv', 'iris.csv')
 
 # Fetches freshly uploaded Iris table 
 res = api.download_table(iris_id)
 print(res.head())
 
 # Creates dashboard from iris table with layout uploaded from file "iris.layout"
-dashboard_id = api.create_dashboard('python-test', iris_id, layout_filename='iris.layout')
+dashboard_id = api.create_dashboard('python-test', iris_id, layout_filename='iris.layout')['ID']
 
 # Shares dashboard with admin
 api.share_dashboard(dashboard_id, 'Test')
 
 ```
```

### Comparing `datagrok_api-0.0.1/pyproject.toml` & `datagrok_api-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "datagrok-api"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Andrew Skalkin", email="askalkin@datagrok.ai" },
   { name="Amelichev Konstantin", email="kamelichev@datagrok.ai" },
 ]
 description = "Client library for integration with datagrok API"
 readme = "README.md"
 requires-python = ">=3.5"
```

### Comparing `datagrok_api-0.0.1/PKG-INFO` & `datagrok_api-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.3
-Name: datagrok-api
-Version: 0.0.1
-Summary: Client library for integration with datagrok API
-Project-URL: Homepage, https://github.com/datagrok-ai/public
-Project-URL: Issues, https://github.com/datagrok-ai/public/issues
-Author-email: Andrew Skalkin <askalkin@datagrok.ai>, Amelichev Konstantin <kamelichev@datagrok.ai>
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-
 # Datagrok python client library
 
 This library can be used for integration with datagrok. It is a python wrapper for public API, that has OpenAPI specification available [here](http://public.datagrok.ai/api/public/api.yaml).
 
+Refer to [Help](http://datagrok.ai/help) for more information.
+
 ## Installation
 
 To install package, use [pip](https://pypi.org/project/pip/).
 
 ```shell
 pip install datagrok-api
 ```
@@ -38,40 +27,37 @@
 See [License.md](https://github.com/datagrok-ai/public/blob/master/LICENSE.md).
 
 ## Examples
 
 The package uses Pandas for representation of tables and dataframes.
 
 ```python
-from datagrok_api import DatagrokClient
 import pandas as pd
 from sklearn.datasets import load_iris
 
-api = DatagrokClient('your token', 'datagrok url')
-
 # Calls a Datagrok function
 # Dataframes, columns and primitive data types are supported
 api.call_function('Abs', {
 	'x': -3
 })
 
 # Downloads file from a given connection
 res = api.download_file('system.demofiles', 'demog.csv')
 print(res.head())
 
 # Uploads iris dataset as a table
-iris_id = api.upload_table('iris', pd.DataFrame(load_iris()['data']))
+iris_id = api.upload_table('iris', pd.DataFrame(load_iris()['data']))['ID']
 
 # Iris also can be uploaded as a file
 # api.upload_file('system.demofiles', 'iris.csv', 'iris.csv')
 
 # Fetches freshly uploaded Iris table 
 res = api.download_table(iris_id)
 print(res.head())
 
 # Creates dashboard from iris table with layout uploaded from file "iris.layout"
-dashboard_id = api.create_dashboard('python-test', iris_id, layout_filename='iris.layout')
+dashboard_id = api.create_dashboard('python-test', iris_id, layout_filename='iris.layout')['ID']
 
 # Shares dashboard with admin
 api.share_dashboard(dashboard_id, 'Test')
 
 ```
```

