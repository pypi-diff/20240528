# Comparing `tmp/datawarehouse_connector-0.1.2.tar.gz` & `tmp/datawarehouse_connector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawarehouse_connector-0.1.2.tar", last modified: Fri May 24 13:26:03 2024, max compression
+gzip compressed data, was "datawarehouse_connector-0.1.3.tar", last modified: Tue May 28 15:05:33 2024, max compression
```

## Comparing `datawarehouse_connector-0.1.2.tar` & `datawarehouse_connector-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 13:26:03.414148 datawarehouse_connector-0.1.2/
--rw-rw-rw-   0        0        0     1090 2024-05-22 10:02:14.000000 datawarehouse_connector-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3869 2024-05-24 13:26:03.413148 datawarehouse_connector-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2594 2024-05-24 13:20:57.000000 datawarehouse_connector-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 13:26:03.388149 datawarehouse_connector-0.1.2/datawarehouse_connector/
--rw-rw-rw-   0        0        0       36 2024-05-24 11:16:12.000000 datawarehouse_connector-0.1.2/datawarehouse_connector/__init__.py
--rw-rw-rw-   0        0        0     1964 2024-05-24 13:21:55.000000 datawarehouse_connector-0.1.2/datawarehouse_connector/connector.py
--rw-rw-rw-   0        0        0      306 2024-05-24 08:40:26.000000 datawarehouse_connector-0.1.2/datawarehouse_connector/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:26:03.410148 datawarehouse_connector-0.1.2/datawarehouse_connector.egg-info/
--rw-rw-rw-   0        0        0     3869 2024-05-24 13:26:03.000000 datawarehouse_connector-0.1.2/datawarehouse_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-05-24 13:26:03.000000 datawarehouse_connector-0.1.2/datawarehouse_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 13:26:03.000000 datawarehouse_connector-0.1.2/datawarehouse_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2024-05-24 13:26:03.000000 datawarehouse_connector-0.1.2/datawarehouse_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-24 13:26:03.000000 datawarehouse_connector-0.1.2/datawarehouse_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 13:26:03.415151 datawarehouse_connector-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-05-24 13:24:49.000000 datawarehouse_connector-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 15:05:33.977817 datawarehouse_connector-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-22 10:02:14.000000 datawarehouse_connector-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6265 2024-05-28 15:05:33.976529 datawarehouse_connector-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4649 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 15:05:33.935384 datawarehouse_connector-0.1.3/datawarehouse_connector/
+-rw-rw-rw-   0        0        0      370 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/datawarehouse_connector/__init__.py
+-rw-rw-rw-   0        0        0      975 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/datawarehouse_connector/connector.py
+-rw-rw-rw-   0        0        0      614 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/datawarehouse_connector/constants.py
+-rw-rw-rw-   0        0        0     1114 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/datawarehouse_connector/postgres_session.py
+-rw-rw-rw-   0        0        0     4101 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/datawarehouse_connector/redshift_session.py
+-rw-rw-rw-   0        0        0     1338 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/datawarehouse_connector/snowflake_session.py
+-rw-rw-rw-   0        0        0      317 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/datawarehouse_connector/utils.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 13:39:23.000000 datawarehouse_connector-0.1.3/datawarehouse_connector/validate.py
+drwxrwxrwx   0        0        0        0 2024-05-28 15:05:33.975077 datawarehouse_connector-0.1.3/datawarehouse_connector.egg-info/
+-rw-rw-rw-   0        0        0     6265 2024-05-28 15:05:33.000000 datawarehouse_connector-0.1.3/datawarehouse_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2024-05-28 15:05:33.000000 datawarehouse_connector-0.1.3/datawarehouse_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 15:05:33.000000 datawarehouse_connector-0.1.3/datawarehouse_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2024-05-28 15:05:33.000000 datawarehouse_connector-0.1.3/datawarehouse_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-28 15:05:33.000000 datawarehouse_connector-0.1.3/datawarehouse_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 15:05:33.977817 datawarehouse_connector-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      906 2024-05-28 15:04:39.000000 datawarehouse_connector-0.1.3/setup.py
```

### Comparing `datawarehouse_connector-0.1.2/LICENSE` & `datawarehouse_connector-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datawarehouse_connector-0.1.2/PKG-INFO` & `datawarehouse_connector-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,138 @@
-Metadata-Version: 2.1
-Name: datawarehouse_connector
-Version: 0.1.2
-Summary: A package for database session management
-Home-page: https://github.com/Chandani7250/datawarehouse_connector
-Author: Poonam Saroj
-Author-email: poonam@coditation.com
-License: UNKNOWN
-Description: # Data Warehouse Connector
-        A Python module to establish connections to various data warehouses like Snowflake, Redshift, and PostgreSQL.
-        
-        # Overview
-        
-        This `README.md` file provides comprehensive instructions for installing, setting up, and using the `Data Warehouse Connector` module, ensuring users can easily establish connections to their data warehouses.
-        
-        ---
-        
-        # Data Warehouses
-        
-        ## Snowflake
-        
-        Requires `DB_SOURCE`, `USERNAME`, `HOST`, `PASSWORD`, `ROLE`, `WAREHOUSE`, and `DATABASE`.
-        
-        ```python
-        from datawarehouse_connector.connector import get_session
-        
-        snowflake_creds = {
-           "db_source": "snowflake",
-           "user": "user",
-           "password": "password",
-           "role": "role",
-           "warehouse": "warehouse",
-           "database": "database",
-           "host": "host",
-        }
-        
-        session = get_session(snowflake_creds)
-        session.close()
-        ```
-        
-        ## Redshift
-        
-        Requires `DB_SOURCE`, `USERNAME`, `HOST`, `PASSWORD`, and `DATABASE`.
-        
-        ```python
-        from datawarehouse_connector.connector import get_session
-        
-        redshift_creds = {
-           "db_source": "redshift",
-           "user": "user",
-           "password": "password",
-           "database": "database",
-           "host": "host",
-        }
-        
-        session = get_session(redshift_creds)
-        session.close()
-        ```
-        
-        ## PostgreSQL
-        
-        Requires `DB_SOURCE`, `USERNAME`, `HOST`, `PASSWORD`, and `DATABASE`.
-        
-        ```python
-        from datawarehouse_connector.connector import get_session
-        
-        postgresql_creds = {
-           "db_source": "postgresql",
-           "user": "user",
-           "password": "password",
-           "database": "database",
-           "host": "host",
-        }
-        
-        session = get_session(postgresql_creds)
-        session.close()
-        ```
-        
-        ---
-        
-        # Handling Connection
-        
-        Once the session is established, you can interact with your data warehouse using SQLAlchemy's ORM capabilities.
-        
-        ---
-        
-        # Troubleshooting
-        
-        ## Common Issues
-        
-        - Invalid Credentials: Ensure that the USERNAME and PASSWORD are correct.
-        - Host Unreachable: Verify the HOST address and network connectivity.
-        - Unsupported Data Source: Check if the DB_SOURCE is among the supported ones (snowflake, redshift, postgresql).
-        
-        ## Error Handling
-        
-        The `get_session` method prints exceptions to help identify issues during the connection process. Ensure that the provided connection details are accurate and the data warehouse is accessible.
-        
-        ---
-        
-        # Conclusion
-        
-        This module simplifies the process of connecting to various data warehouses. Follow the setup instructions carefully, and refer to the examples for guidance on using the `get_session` function. For further assistance, check the documentation or raise an issue on the project's GitHub repository.
-        ```
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# Data Warehouse Connector
+A Python module to establish connections to various data warehouses like Snowflake, Redshift, and PostgreSQL.
+
+# Overview
+
+This `README.md` file provides comprehensive instructions for installing, setting up, and using the `Data Warehouse Connector` module, ensuring users can easily establish connections to their data warehouses.
+
+---
+
+# Data Warehouses
+
+## Snowflake
+
+Requires `DB_SOURCE`, `USERNAME`, `HOST`, `PASSWORD`, `ROLE`, `WAREHOUSE`, and `DATABASE`.
+
+```python
+from datawarehouse_connector.connector import get_session
+
+snowflake_creds = {
+   "db_source": "snowflake",
+   "user": "user",
+   "password": "password",
+   "role": "role",
+   "warehouse": "warehouse",
+   "database": "database",
+   "host": "host",
+}
+
+session = get_session(snowflake_creds)
+session.close()
+```
+
+### Whitelisting
+If network policy is activated in the snowflake account and incoming ips are not allowed or restricted then need to whitelist our StepFunction IP : 
+
+Please follow the below steps for the same :
+1. Navigate to the Admin->Security section by clicking on "Admin" in the left navigation panel
+2. Switch to Network Rules. Create a new rule by clicking on + Network Rule button
+   a. Name: SFN_RULE
+   b. Choose Type: IPv4 and Mode: Ingress
+   c. Under Identifiers -> Add IP 18.210.244.167
+3. Switch to Network Policy. Create a new policy by clicking on + Network Policy button
+   a. Name: SFN_POLICY
+   b. Under Allowed Section & Under Select Rule Dropdown select SFN_RULE then click on Create button to create the policy.
+   c. Click on the dotted icon(...) at the end of the policy name and click Activate to start the policy. 
+4.   Navigate back to the worksheet and replace placeholder <IP> with the StepFunctions public IP address.
+	
+     ALTER NETWORK POLICY SFN_POLICY SET ALLOWED_IP_LIST=('18.210.244.167')
+
+## Redshift
+
+Requires `DB_SOURCE`, `USERNAME`, `HOST`, `PASSWORD`, and `DATABASE`.
+
+```python
+### Direct Connection (Redshift in Public Subnet)
+from datawarehouse_connector.connector import get_session
+
+**Database Connection Configuration**
+   redshift_creds = {
+   "db_source": "redshift",
+   "user": "user",
+   "password": "password",
+   "database": "database",
+   "host": "host"
+   }
+
+session = get_session(redshift_creds)
+session.close()
+
+### SSH Tunnel Connection (Redshift in Private Subnet)
+#### Purpose
+Connect to Amazon Redshift via an SSH tunnel when it's located in a private subnet, and the connecting instance (EC2) is in a public subnet.
+you need to provide the SSH details and private key content to establish an SSH tunnel. 
+#### Prerequisites
+SSH Host: The hostname or IP address of the EC2 instance that has access to the Redshift cluster.
+SSH Username: The username to log into the EC2 instance.
+SSH PEM File Content: The content of the PEM file (private key) used to authenticate the SSH connection.
+
+redshift_creds = {
+   "db_source": "redshift",
+   "user": "user",
+   "password": "password",
+   "database": "database",
+   "host": "host",
+   'ssh_host': 'ssh_host',
+   'ssh_username': 'ssh_username',
+   'ssh_pem_file_content': '''ssh_pem_file_content'''
+}
+
+session = get_session(redshift_creds)
+session.close()
+```
+
+## PostgreSQL
+
+Requires `DB_SOURCE`, `USERNAME`, `HOST`, `PASSWORD`, and `DATABASE`.
+
+```python
+from datawarehouse_connector.connector import get_session
+
+postgresql_creds = {
+   "db_source": "postgresql",
+   "user": "user",
+   "password": "password",
+   "database": "database",
+   "host": "host",
+}
+
+session = get_session(postgresql_creds)
+session.close()
+```
+
+---
+
+# Handling Connection
+
+Once the session is established, you can interact with your data warehouse using SQLAlchemy's ORM capabilities.
+
+---
+
+# Troubleshooting
+
+## Common Issues
+
+- Invalid Credentials: Ensure that the USERNAME and PASSWORD are correct.
+- Host Unreachable: Verify the HOST address and network connectivity.
+- Unsupported Data Source: Check if the DB_SOURCE is among the supported ones (snowflake, redshift, postgresql).
+
+## Error Handling
+
+The `get_session` method prints exceptions to help identify issues during the connection process. Ensure that the provided connection details are accurate and the data warehouse is accessible.
+
+---
+
+# Conclusion
+
+This module simplifies the process of connecting to various data warehouses. Follow the setup instructions carefully, and refer to the examples for guidance on using the `get_session` function. For further assistance, check the documentation or raise an issue on the project's GitHub repository.
+```
```

### Comparing `datawarehouse_connector-0.1.2/datawarehouse_connector.egg-info/PKG-INFO` & `datawarehouse_connector-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: datawarehouse-connector
-Version: 0.1.2
+Name: datawarehouse_connector
+Version: 0.1.3
 Summary: A package for database session management
 Home-page: https://github.com/Chandani7250/datawarehouse_connector
-Author: Poonam Saroj
-Author-email: poonam@coditation.com
+Author: Chandani Kumari
+Author-email: Chandani@coditation.com
 License: UNKNOWN
 Description: # Data Warehouse Connector
         A Python module to establish connections to various data warehouses like Snowflake, Redshift, and PostgreSQL.
         
         # Overview
         
         This `README.md` file provides comprehensive instructions for installing, setting up, and using the `Data Warehouse Connector` module, ensuring users can easily establish connections to their data warehouses.
@@ -34,27 +34,69 @@
            "host": "host",
         }
         
         session = get_session(snowflake_creds)
         session.close()
         ```
         
+        ### Whitelisting
+        If network policy is activated in the snowflake account and incoming ips are not allowed or restricted then need to whitelist our StepFunction IP : 
+        
+        Please follow the below steps for the same :
+        1. Navigate to the Admin->Security section by clicking on "Admin" in the left navigation panel
+        2. Switch to Network Rules. Create a new rule by clicking on + Network Rule button
+           a. Name: SFN_RULE
+           b. Choose Type: IPv4 and Mode: Ingress
+           c. Under Identifiers -> Add IP 18.210.244.167
+        3. Switch to Network Policy. Create a new policy by clicking on + Network Policy button
+           a. Name: SFN_POLICY
+           b. Under Allowed Section & Under Select Rule Dropdown select SFN_RULE then click on Create button to create the policy.
+           c. Click on the dotted icon(...) at the end of the policy name and click Activate to start the policy. 
+        4.   Navigate back to the worksheet and replace placeholder <IP> with the StepFunctions public IP address.
+        	
+             ALTER NETWORK POLICY SFN_POLICY SET ALLOWED_IP_LIST=('18.210.244.167')
+        
         ## Redshift
         
         Requires `DB_SOURCE`, `USERNAME`, `HOST`, `PASSWORD`, and `DATABASE`.
         
         ```python
+        ### Direct Connection (Redshift in Public Subnet)
         from datawarehouse_connector.connector import get_session
         
+        **Database Connection Configuration**
+           redshift_creds = {
+           "db_source": "redshift",
+           "user": "user",
+           "password": "password",
+           "database": "database",
+           "host": "host"
+           }
+        
+        session = get_session(redshift_creds)
+        session.close()
+        
+        ### SSH Tunnel Connection (Redshift in Private Subnet)
+        #### Purpose
+        Connect to Amazon Redshift via an SSH tunnel when it's located in a private subnet, and the connecting instance (EC2) is in a public subnet.
+        you need to provide the SSH details and private key content to establish an SSH tunnel. 
+        #### Prerequisites
+        SSH Host: The hostname or IP address of the EC2 instance that has access to the Redshift cluster.
+        SSH Username: The username to log into the EC2 instance.
+        SSH PEM File Content: The content of the PEM file (private key) used to authenticate the SSH connection.
+        
         redshift_creds = {
            "db_source": "redshift",
            "user": "user",
            "password": "password",
            "database": "database",
            "host": "host",
+           'ssh_host': 'ssh_host',
+           'ssh_username': 'ssh_username',
+           'ssh_pem_file_content': '''ssh_pem_file_content'''
         }
         
         session = get_session(redshift_creds)
         session.close()
         ```
         
         ## PostgreSQL
```

### Comparing `datawarehouse_connector-0.1.2/setup.py` & `datawarehouse_connector-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='datawarehouse_connector',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'psycopg2-binary',
         'redshift-connector',
         'snowflake-connector-python',
         'snowflake-sqlalchemy',
         'SQLAlchemy',
         'sqlalchemy-redshift',
         'urllib3'
     ],
-    author='Poonam Saroj',
-    author_email='poonam@coditation.com',
+    author='Chandani Kumari',
+    author_email='Chandani@coditation.com',
     description='A package for database session management',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Chandani7250/datawarehouse_connector',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

