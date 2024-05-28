# Comparing `tmp/echoss_query-0.0.9.tar.gz` & `tmp/echoss_query-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoss_query-0.0.9.tar", last modified: Fri Jan  5 05:14:58 2024, max compression
+gzip compressed data, was "echoss_query-0.1.0.tar", last modified: Tue May 28 06:08:57 2024, max compression
```

## Comparing `echoss_query-0.0.9.tar` & `echoss_query-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-05 05:14:58.877392 echoss_query-0.0.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2662 2024-01-05 05:14:58.877392 echoss_query-0.0.9/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2421 2023-07-26 03:06:41.000000 echoss_query-0.0.9/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-05 05:14:58.877392 echoss_query-0.0.9/echoss_query/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-09-18 00:04:27.000000 echoss_query-0.0.9/echoss_query/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-05 05:14:58.877392 echoss_query-0.0.9/echoss_query/project_control/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8840 2023-09-18 00:04:27.000000 echoss_query-0.0.9/echoss_query/project_control/project_generator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-05 05:14:58.877392 echoss_query-0.0.9/echoss_query/query/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-18 00:04:27.000000 echoss_query-0.0.9/echoss_query/query/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25347 2023-09-18 01:54:47.000000 echoss_query-0.0.9/echoss_query/query/echoss_query.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-05 05:14:58.877392 echoss_query-0.0.9/echoss_query.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2662 2024-01-05 05:14:58.000000 echoss_query-0.0.9/echoss_query.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2024-01-05 05:14:58.000000 echoss_query-0.0.9/echoss_query.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-05 05:14:58.000000 echoss_query-0.0.9/echoss_query.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2024-01-05 05:14:58.000000 echoss_query-0.0.9/echoss_query.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2024-01-05 05:14:58.000000 echoss_query-0.0.9/echoss_query.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-05 05:14:58.877392 echoss_query-0.0.9/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      839 2024-01-05 05:13:47.000000 echoss_query-0.0.9/setup.py
+drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-28 06:08:57.292635 echoss_query-0.1.0/
+-rw-r--r--   0 sin-incheol   (501) staff       (20)     2820 2024-05-28 06:08:57.292122 echoss_query-0.1.0/PKG-INFO
+-rw-r--r--   0 sin-incheol   (501) staff       (20)     2427 2024-05-28 05:52:53.000000 echoss_query-0.1.0/README.md
+drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-28 06:08:57.290565 echoss_query-0.1.0/echoss_query.egg-info/
+-rw-r--r--   0 sin-incheol   (501) staff       (20)     2820 2024-05-28 06:08:57.000000 echoss_query-0.1.0/echoss_query.egg-info/PKG-INFO
+-rw-r--r--   0 sin-incheol   (501) staff       (20)      237 2024-05-28 06:08:57.000000 echoss_query-0.1.0/echoss_query.egg-info/SOURCES.txt
+-rw-r--r--   0 sin-incheol   (501) staff       (20)        1 2024-05-28 06:08:57.000000 echoss_query-0.1.0/echoss_query.egg-info/dependency_links.txt
+-rw-r--r--   0 sin-incheol   (501) staff       (20)       77 2024-05-28 06:08:57.000000 echoss_query-0.1.0/echoss_query.egg-info/requires.txt
+-rw-r--r--   0 sin-incheol   (501) staff       (20)        6 2024-05-28 06:08:57.000000 echoss_query-0.1.0/echoss_query.egg-info/top_level.txt
+drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-28 06:08:57.291338 echoss_query-0.1.0/query/
+-rw-r--r--   0 sin-incheol   (501) staff       (20)        0 2024-05-28 05:52:53.000000 echoss_query-0.1.0/query/__init__.py
+-rw-r--r--   0 sin-incheol   (501) staff       (20)    26208 2024-05-28 05:53:49.000000 echoss_query-0.1.0/query/echoss_query.py
+-rw-r--r--   0 sin-incheol   (501) staff       (20)       38 2024-05-28 06:08:57.292783 echoss_query-0.1.0/setup.cfg
+-rw-r--r--   0 sin-incheol   (501) staff       (20)      689 2024-05-28 06:05:53.000000 echoss_query-0.1.0/setup.py
```

### Comparing `echoss_query-0.0.9/PKG-INFO` & `echoss_query-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: echoss_query
-Version: 0.0.9
-Summary: echoss AI Bigdata Solution - Query Package
-Home-page: 
-Author: incheolshin
-Author-email: incheolshin@12cm.co.kr
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-
 # echoss_query
 -------------
 사용 전 config(인증 정보) 폴더의 유무를 확인한 뒤 사용해야한다.
 
 ### Installaion
 -------------
 To install this package, please use Python 3.8 or higher. 
@@ -22,15 +12,15 @@
     cd ~/echoss_query
     pip install -r requirements.txt
 ```
 
 ### Quick Start
 -------------
 ```
-    from echoss_query import MysqlQuery, MongoQuery, ElasticSearch
+    from echoss_query.query import MysqlQuery, MongoQuery, ElasticSearch
 
     mysql = MysqlQuery('CONFIG_FILE_PATH' or dict)
     mongo = MongoQuery('CONFIG_FILE_PATH' or dict)
     elastic = ElasticSearch('CONFIG_FILE_PATH' or dict)
 
 
     #CREATE
@@ -109,8 +99,8 @@
         param1: The first parameter.
         param2: The second parameter.
 
     Returns:
         The return value. True for success, False otherwise.
 
     """
-```
+```
```

### Comparing `echoss_query-0.0.9/README.md` & `echoss_query-0.1.0/echoss_query.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: echoss-query
+Version: 0.1.0
+Summary: echoss AI Bigdata Solution - Query Package
+Home-page: 
+Author: incheolshin
+Author-email: incheolshin@12cm.co.kr
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+Requires-Dist: pandas>=1.5.3
+Requires-Dist: pymongo>=4.3.3
+Requires-Dist: PyMySQL>=1.0.2
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: opensearch-py>=2.2.0
+
 # echoss_query
 -------------
 사용 전 config(인증 정보) 폴더의 유무를 확인한 뒤 사용해야한다.
 
 ### Installaion
 -------------
 To install this package, please use Python 3.8 or higher. 
@@ -12,15 +27,15 @@
     cd ~/echoss_query
     pip install -r requirements.txt
 ```
 
 ### Quick Start
 -------------
 ```
-    from echoss_query import MysqlQuery, MongoQuery, ElasticSearch
+    from echoss_query.query import MysqlQuery, MongoQuery, ElasticSearch
 
     mysql = MysqlQuery('CONFIG_FILE_PATH' or dict)
     mongo = MongoQuery('CONFIG_FILE_PATH' or dict)
     elastic = ElasticSearch('CONFIG_FILE_PATH' or dict)
 
 
     #CREATE
@@ -99,8 +114,8 @@
         param1: The first parameter.
         param2: The second parameter.
 
     Returns:
         The return value. True for success, False otherwise.
 
     """
-```
+```
```

### Comparing `echoss_query-0.0.9/echoss_query/query/echoss_query.py` & `echoss_query-0.1.0/query/echoss_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
             self.charset = conn_info['mysql']['charset']
         else:
             print('mysql : config info not exist')
 
     @staticmethod
     def _parsing(query: str) -> str:
         if ';' not in query:
-            result = query + ';'
-        return result
+            return query + ';'
+        return query
 
     def _connect_db(self) -> None:
         try:
             self.conn = pymysql.connect(
                 user=self.user,
                 passwd=self.passwd,
                 host=self.host,
@@ -784,8 +784,29 @@
         return self.conn.info()
     
     def exists(self, id:str or int=None) -> bool:
         """
         Args:
             echoss_query_env(env_var) : Region Name
             ex export echoss_query=kr_local
-    """
+    """
+if __name__ == '__main__':
+    # import os
+    import yaml
+
+    #### region = os.environ['echoss_query_env']
+    # 환경 변수를 가져와서 인자 값으로 할당하는 방식
+    #
+    with open('../config/config.yaml', 'r') as file:
+        yaml_info = yaml.load(file, Loader=yaml.FullLoader)
+
+    # mysql = MysqlQuery(yaml_info['kr_local'])
+    mq = MongoQuery(yaml_info['kr_stag'])
+
+    mq.ping()
+    # print(mongo.new_index('project_info', 'project_number'))
+    # # print(mysql.update("""UPDATE PROJECT_INFO SET PROJECT_NUMBER = 777 WHERE = PROJECT_NAME = 'abalone'"""))
+    # # print(mysql.select_list('SELECT 영수증번호 FROM sys.`ppcd_df-001.csv` WHERE 고객번호 = 1'))
+    # # print(mongo.select('ppcd_df', {'고객번호':1}))
+    # # print(mysql.databases())
+    # # print(mongo.databases())
+    # print(mongo.create('test_collection2'))
```

### Comparing `echoss_query-0.0.9/echoss_query.egg-info/PKG-INFO` & `echoss_query-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
-Name: echoss-query
-Version: 0.0.9
+Name: echoss_query
+Version: 0.1.0
 Summary: echoss AI Bigdata Solution - Query Package
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
+Requires-Dist: pandas>=1.5.3
+Requires-Dist: pymongo>=4.3.3
+Requires-Dist: PyMySQL>=1.0.2
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: opensearch-py>=2.2.0
 
 # echoss_query
 -------------
 사용 전 config(인증 정보) 폴더의 유무를 확인한 뒤 사용해야한다.
 
 ### Installaion
 -------------
@@ -22,15 +27,15 @@
     cd ~/echoss_query
     pip install -r requirements.txt
 ```
 
 ### Quick Start
 -------------
 ```
-    from echoss_query import MysqlQuery, MongoQuery, ElasticSearch
+    from echoss_query.query import MysqlQuery, MongoQuery, ElasticSearch
 
     mysql = MysqlQuery('CONFIG_FILE_PATH' or dict)
     mongo = MongoQuery('CONFIG_FILE_PATH' or dict)
     elastic = ElasticSearch('CONFIG_FILE_PATH' or dict)
 
 
     #CREATE
```

### Comparing `echoss_query-0.0.9/setup.py` & `echoss_query-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 package_name = "echoss_query"
 
-packages = [
-    package
-    for package in find_packages(where=".")
-    if package == package_name or package.startswith(package_name + ".")
-]
-
 setup(
     name='echoss_query',
-    version='0.0.9',
+    version='0.1.0',
     url='',
     install_requires=[
         'pandas>=1.5.3',
         'pymongo>=4.3.3',
         'PyMySQL>=1.0.2',
         'PyYAML>=6.0',
         'opensearch-py>=2.2.0'
-        ],
+    ],
     license='',
     author='incheolshin',
     author_email='incheolshin@12cm.co.kr',
     description='echoss AI Bigdata Solution - Query Package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     package_data={},
     python_requires= '>3.7',
-)
+)
```

