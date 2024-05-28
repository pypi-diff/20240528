# Comparing `tmp/cela-0.0.1b0-py2.py3-none-any.whl.zip` & `tmp/cela-0.0.2b0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 9440 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 09:48 cela/__init__.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-24 09:48 cela/main.py
--rw-r--r--  2.0 unx     9859 b- defN 24-May-24 09:48 cela/util.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 09:48 cela/services/__init__.py
--rw-r--r--  2.0 unx     1121 b- defN 24-May-24 09:48 cela/services/create.py
--rw-r--r--  2.0 unx     1574 b- defN 24-May-24 09:48 cela/services/init.py
--rw-r--r--  2.0 unx     7196 b- defN 24-May-24 09:48 cela/services/migrate.py
--rw-r--r--  2.0 unx     1004 b- defN 24-May-24 09:48 cela/services/reset.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 09:48 cela-0.0.1b0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3782 b- defN 24-May-24 09:48 cela-0.0.1b0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-May-24 09:48 cela-0.0.1b0.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 24-May-24 09:48 cela-0.0.1b0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-24 09:48 cela-0.0.1b0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1077 b- defN 24-May-24 09:48 cela-0.0.1b0.dist-info/RECORD
-14 files, 26779 bytes uncompressed, 7658 bytes compressed:  71.4%
+Zip file size: 11521 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 08:59 cela/__init__.py
+-rw-r--r--  2.0 unx     1840 b- defN 24-May-28 08:59 cela/main.py
+-rw-r--r--  2.0 unx    11544 b- defN 24-May-28 08:59 cela/util.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 08:59 cela/services/__init__.py
+-rw-r--r--  2.0 unx     1181 b- defN 24-May-28 08:59 cela/services/create.py
+-rw-r--r--  2.0 unx     1909 b- defN 24-May-28 08:59 cela/services/init.py
+-rw-r--r--  2.0 unx     8282 b- defN 24-May-28 08:59 cela/services/migrate.py
+-rw-r--r--  2.0 unx     1028 b- defN 24-May-28 08:59 cela/services/reset.py
+-rw-r--r--  2.0 unx      408 b- defN 24-May-28 08:59 cela/services/version.py
+-rw-r--r--  2.0 unx     1060 b- defN 24-May-28 08:59 cela-0.0.2b0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5134 b- defN 24-May-28 08:59 cela-0.0.2b0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-28 08:59 cela-0.0.2b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 24-May-28 08:59 cela-0.0.2b0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-28 08:59 cela-0.0.2b0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1161 b- defN 24-May-28 08:59 cela-0.0.2b0.dist-info/RECORD
+15 files, 33702 bytes uncompressed, 9615 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -18,26 +18,29 @@
 
 Filename: cela/services/migrate.py
 Comment: 
 
 Filename: cela/services/reset.py
 Comment: 
 
-Filename: cela-0.0.1b0.dist-info/LICENSE
+Filename: cela/services/version.py
 Comment: 
 
-Filename: cela-0.0.1b0.dist-info/METADATA
+Filename: cela-0.0.2b0.dist-info/LICENSE
 Comment: 
 
-Filename: cela-0.0.1b0.dist-info/WHEEL
+Filename: cela-0.0.2b0.dist-info/METADATA
 Comment: 
 
-Filename: cela-0.0.1b0.dist-info/entry_points.txt
+Filename: cela-0.0.2b0.dist-info/WHEEL
 Comment: 
 
-Filename: cela-0.0.1b0.dist-info/top_level.txt
+Filename: cela-0.0.2b0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cela-0.0.1b0.dist-info/RECORD
+Filename: cela-0.0.2b0.dist-info/top_level.txt
+Comment: 
+
+Filename: cela-0.0.2b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cela/main.py

```diff
@@ -1,36 +1,54 @@
 import argparse
 import cela.services.init
 import cela.services.create
 import cela.services.migrate
 import cela.services.reset
+import cela.services.version
 
 
 def main():
     parser = argparse.ArgumentParser(description='Process migrations.')
     subparsers = parser.add_subparsers(dest='command')
 
     init_parser = subparsers.add_parser('init')
 
     create_parser = subparsers.add_parser('create')
-    create_parser.add_argument('--name', type=str, help='The name of the migration to create')
+    create_parser.add_argument('--name', type=str, help='The name of the migration to create.')
 
     migrate_parser = subparsers.add_parser('migrate')
 
+    rollback_parser = subparsers.add_parser('rollback')
+
     reset_parser = subparsers.add_parser('reset')
 
+    version_parser = subparsers.add_parser('version')
+
     args = parser.parse_args()
 
     if args.command == 'create':
         cela.services.create.run(args.name)
     elif args.command == 'migrate':
         cela.services.migrate.run('up')
+    elif args.command == 'rollback':
+        cela.services.migrate.run('down')
     elif args.command == 'init':
         cela.services.init.run()
     elif args.command == 'reset':
         cela.services.reset.run()
+    elif args.command == 'version':
+        cela.services.version.run()
     else:
-        print("Invalid command. Please choose 'create' or 'migrate'.")
+        print("Invalid command. Please follow the usage below.")
+        print("Usage: cela <command>")
+        print("Commands:")
+        print("  init        Initialize migration configuration. You should run this command first.")
+        print("  create      Create a new migration file.")
+        print("    --name    The name of the migration to create.")
+        print("  migrate     Run all pending migrations.")
+        print("  rollback    Rollback the last migration.")
+        print("  reset       Reset the migration version.")
+        print("  version     Show the current migration version.")
 
 
 if __name__ == '__main__':
     main()
```

## cela/util.py

```diff
@@ -1,36 +1,87 @@
 import os
 import glob
 
+MIGRATION_DIRECTORY = '.migrations'
+
+
+def migration_directory():
+    return MIGRATION_DIRECTORY
+
 
 # Check if the migration system has been initialized.
 def is_inited():
     return os.path.exists('migrations')
 
 
 # Get all migration files that have a version greater than the given version.
-def get_greater_migration_files(version):
-    all_files = glob.glob('migrations/*.yaml')
+def get_bigger_migration_files(version):
+    all_files = glob.glob(migration_directory() + '/*.yaml')
     migration_files = []
     for f in all_files:
         basename = os.path.basename(f)
         if not basename[:8].isdigit():
             continue
         if int(basename[:8]) > version:
             migration_files.append(f)
     migration_files = sorted(migration_files, key=lambda f: int(os.path.basename(f)[:8]))
     return migration_files
 
 
 # Get the migration file that has a version greater than the given version.
-def get_greater_migration_file(version):
-    migration_files = get_greater_migration_files(version)
+def get_bigger_migration_file(version):
+    migration_files = get_bigger_migration_files(version)
     return migration_files[0] if migration_files else None
 
 
+# Get all migration files that have a version smaller than the given version.
+def get_smaller_migration_files(version):
+    all_files = glob.glob(migration_directory() + '/*.yaml')
+    migration_files = []
+    for f in all_files:
+        basename = os.path.basename(f)
+        if not basename[:8].isdigit():
+            continue
+        if int(basename[:8]) < version:
+            migration_files.append(f)
+    migration_files = sorted(migration_files, key=lambda f: int(os.path.basename(f)[:8]), reverse=True)
+    return migration_files
+
+
+# Get the migration file that has a version smaller than the given version.
+def get_smaller_migration_file(version):
+    migration_files = get_smaller_migration_files(version)
+    return migration_files[0] if migration_files else None
+
+
+# Get the current version.
+def get_current_version(connection):
+    with connection.cursor() as cursor:
+        cursor.execute("SELECT `version` FROM migrations LIMIT 1")
+        result = cursor.fetchone()
+        return result[0] if result else None
+
+
+# Get the matching migration file.
+def get_matching_migration_file(current_version):
+    if current_version and current_version != 0:
+        all_files = glob.glob(migration_directory() + '/*.yaml')
+        for file in all_files:
+            basename = os.path.basename(file)
+            if basename[:8] == str(current_version).zfill(8):
+                return file
+    return None
+
+
+# Get the version from the migration file.
+def get_version_from_migration_file(filename):
+    basename = os.path.basename(filename)
+    return int(basename[:8])
+
+
 # Convert column to sql string.
 def column_to_sql(column):
     if column.get('type') in ['int', 'integer']:
         column_sql_string = 'INT'
     elif column.get('type') == 'text':
         column_sql_string = 'TEXT'
     elif column.get('type') == 'float':
```

## cela/services/create.py

```diff
@@ -3,23 +3,23 @@
 import os
 
 
 def run(name):
     if not cela.util.is_inited():
         print("Please run 'cela init' first.")
         exit(1)
-
-    files = os.listdir('migrations')
+    directory_name = cela.util.migration_directory()
+    files = os.listdir(directory_name)
     migration_files = [f for f in files if f[:8].isdigit()]
     if migration_files:
         max_number = max(int(f[:8]) for f in migration_files)
     else:
         max_number = 0
     new_number = str(max_number + 1).zfill(8)
-    file_name = f'migrations/{new_number}_{name}.yaml'
+    file_name = f'{directory_name}/{new_number}_{name}.yaml'
 
     data = {
         "database_name": "",
         "up": [
             {
                 "table_name": "",
                 "columns": [
```

## cela/services/init.py

```diff
@@ -1,14 +1,20 @@
 import os
 import yaml
 import pymysql
+import cela.util
 
 
 def run():
-    directory_name = 'migrations'
+    directory_name = cela.util.migration_directory()
+    config_file_path = directory_name + '/config.yaml'
+    if os.path.exists(config_file_path):
+        print("The migration configuration is existed.")
+        print(f"If you want to reinitialize the configuration, please remove the config file: {config_file_path}.")
+        exit(1)
     if not os.path.exists(directory_name):
         os.makedirs(directory_name)
     print("Starting configurate database connection, you can press CTRL+C to exit.")
     host = input("tell me the host: ")
     port = input("tell me the port: ")
     user = input("tell me the user: ")
     password = input("tell me the password: ")
@@ -16,15 +22,15 @@
     config = {
         'host': host,
         'port': int(port),
         'user': user,
         'password': password,
         'database': database
     }
-    with open('migrations/config.yaml', 'w') as file:
+    with open(directory_name + '/config.yaml', 'w') as file:
         yaml.dump(config, file)
     config.pop('database')
     connection = pymysql.connect(**config)
     try:
         with connection.cursor() as cursor:
             sql = f"CREATE DATABASE IF NOT EXISTS {database}"
             cursor.execute(sql)
@@ -45,8 +51,8 @@
             """
             cursor.execute(sql)
         connection.commit()
     finally:
         connection.close()
 
     print("Initialized migrations.")
-    print("Please check migrations/config.yaml to ensure the connection of database is correct.")
+    print(f"Please check {directory_name}/config.yaml to ensure the connection of database is correct.")
```

## cela/services/migrate.py

```diff
@@ -3,28 +3,35 @@
 import pymysql
 
 
 def run(action):
     if not cela.util.is_inited():
         print("Please run 'cela init' first.")
         exit(1)
-    with open('migrations/config.yaml', 'r') as file:
+    with open(cela.util.migration_directory() + '/config.yaml', 'r') as file:
         config = yaml.safe_load(file)
     connection = pymysql.connect(**config)
     database = config['database']
     try:
         with connection.cursor() as cursor:
             cursor.execute(f"USE {database}")
             while True:
                 try:
+                    # do up or down migration.
+                    current_version = cela.util.get_current_version(connection)
+                    if action == 'up':
+                        migration_file = cela.util.get_bigger_migration_file(current_version)
+                    else:
+                        migration_file = cela.util.get_matching_migration_file(current_version)
+
+                    if migration_file is None:
+                        print("No waiting migration files.")
+                        break
+
                     connection.begin()
-                    cursor.execute("SELECT `version` FROM migrations LIMIT 1")
-                    result = cursor.fetchone()
-                    latest_version = result[0] if result else None
-                    migration_file = cela.util.get_greater_migration_file(latest_version)
 
                     # break migrations if there is no greater migration file.
                     if not migration_file:
                         break
 
                     with open(migration_file, 'r') as file:
                         blueprint = yaml.safe_load(file)
@@ -119,17 +126,29 @@
                                 for column in table['columns']:
                                     column_sql_string = cela.util.column_to_sql(column)
                                     column_string_array.append(f"{column['name']} {column_sql_string} ")
                                 sql += ", ".join(column_string_array)
                                 sql += ")"
                                 cursor.execute(sql)
 
-                        # update version
-                        latest_version = latest_version + 1
-                        sql = f"UPDATE migrations SET version = {latest_version} LIMIT 1"
+                        # if action is up, the current version should be updated to the current filename.
+                        if action == 'up':
+                            current_version = cela.util.get_version_from_migration_file(migration_file)
+                        # if action is down, the current version should be updated to the smaller version filename.
+                        if action == 'down':
+                            smaller_migration_file = cela.util.get_smaller_migration_file(current_version)
+                            if smaller_migration_file is not None:
+                                current_version = cela.util.get_version_from_migration_file(smaller_migration_file)
+                            else:
+                                current_version = 0
+
+                        if current_version is None:
+                            raise Exception("Error: current version is None.")
+
+                        sql = f"UPDATE migrations SET version = {current_version} LIMIT 1"
                         cursor.execute(sql)
                         connection.commit()
                         print(f"Migration {migration_file} {action} successfully.")
                 except Exception as e:
                     raise
                     # connection.rollback()
                     # print(f"Error: {e}")
```

## cela/services/reset.py

```diff
@@ -3,15 +3,15 @@
 import yaml
 
 
 def run():
     if not cela.util.is_inited():
         print("Please run 'cela init' first.")
         exit(1)
-    with open('migrations/config.yaml', 'r') as file:
+    with open(cela.util.migration_directory() + '/config.yaml', 'r') as file:
         config = yaml.safe_load(file)
     connection = pymysql.connect(**config)
     try:
         connection.begin()
         with connection.cursor() as cursor:
             cursor.execute("SHOW TABLES")
             tables = cursor.fetchall()
```

## Comparing `cela-0.0.1b0.dist-info/RECORD` & `cela-0.0.2b0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 cela/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cela/main.py,sha256=SRLMcl-PaiqKyAbTla3Cw8O31mpvYcnjdxhegDGXtIc,1011
-cela/util.py,sha256=pM-S14W9lmwkpwd6AhXsDifrSOwqBQD6hqOF0Bl01ec,9859
+cela/main.py,sha256=nRBORZrVW7V1vLljn6RWb2zgTfIIesC45ejKPNndxq0,1840
+cela/util.py,sha256=EeRVXTERvwf-fiWe8y91P7UCCV7ImlKAHoR1I6bzIm8,11544
 cela/services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cela/services/create.py,sha256=EuhxLqajPSUMtx66US1ZGywIeqLZCB1i0nJ4yN75CKQ,1121
-cela/services/init.py,sha256=g_RoqUZqJWtOP3uUv0ihdr7qTO3auhkplKk3ussTNsA,1574
-cela/services/migrate.py,sha256=yg11PQJQvKr4q_RD5cg5xXPidjR8cZrWvT8yj-HwqpE,7196
-cela/services/reset.py,sha256=LrAV1oYakVeFb_slHqMg_Fy_h-SWeQXRMJdklFqMXjE,1004
-cela-0.0.1b0.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cela-0.0.1b0.dist-info/METADATA,sha256=qWt6GIrYHBUoy36nhR2c5aYdXgjNY1195aKuRh6NTLE,3782
-cela-0.0.1b0.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-cela-0.0.1b0.dist-info/entry_points.txt,sha256=LWM7Xlzng7LSBixy3ipdGeVdU83PNH--kdSwJ-16_To,40
-cela-0.0.1b0.dist-info/top_level.txt,sha256=JLeVRdYV3vd7_guWEGmG37VGqe-FWLGuLBqaPFGUzZo,5
-cela-0.0.1b0.dist-info/RECORD,,
+cela/services/create.py,sha256=faja9cAL3fFb3SFShYw6d-DNEkuiP-oq4KSujNiqW5U,1181
+cela/services/init.py,sha256=J5GXSZ9IUnz7a3xwPpPemz67ONh1-M4CtdgSqRwYEhA,1909
+cela/services/migrate.py,sha256=is81vNBPW-rsMjAa01vuS2IXtCqF8rxUeOixsFsGpGE,8282
+cela/services/reset.py,sha256=lpK3BNx5SD4iPRcaa49uit3XyhjwrZ7Xkpgxy5YtN-Q,1028
+cela/services/version.py,sha256=22MMkg9EX1DwozOTLWkdSsknX1P_Us6WLtaVmsKUHW0,408
+cela-0.0.2b0.dist-info/LICENSE,sha256=5WnAlznfotbwRBMGrH-urAnfVNpQJlrYtaMKcf6zoP0,1060
+cela-0.0.2b0.dist-info/METADATA,sha256=5e85c6T4mkzpWjFXjcWxs1V6ngqAfy2adTwZBkseLwo,5134
+cela-0.0.2b0.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+cela-0.0.2b0.dist-info/entry_points.txt,sha256=LWM7Xlzng7LSBixy3ipdGeVdU83PNH--kdSwJ-16_To,40
+cela-0.0.2b0.dist-info/top_level.txt,sha256=JLeVRdYV3vd7_guWEGmG37VGqe-FWLGuLBqaPFGUzZo,5
+cela-0.0.2b0.dist-info/RECORD,,
```

