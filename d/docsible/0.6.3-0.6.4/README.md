# Comparing `tmp/docsible-0.6.3.tar.gz` & `tmp/docsible-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsible-0.6.3.tar", max compression
+gzip compressed data, was "docsible-0.6.4.tar", max compression
```

## Comparing `docsible-0.6.3.tar` & `docsible-0.6.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2023-09-05 22:49:19.991131 docsible-0.6.3/LICENSE
--rw-r--r--   0        0        0     4605 2024-05-22 21:24:33.324940 docsible-0.6.3/README.md
--rw-r--r--   0        0        0        0 2023-09-05 22:00:43.145585 docsible-0.6.3/docsible/__init__.py
--rw-r--r--   0        0        0    11869 2024-05-22 21:17:22.510430 docsible-0.6.3/docsible/cli.py
--rw-r--r--   0        0        0     6777 2024-05-22 21:20:24.843572 docsible-0.6.3/docsible/markdown_template.py
--rw-r--r--   0        0        0        0 2023-09-11 08:20:14.156264 docsible-0.6.3/docsible/utils/__init__.py
--rw-r--r--   0        0        0    12952 2024-05-21 16:02:16.433270 docsible-0.6.3/docsible/utils/mermaid.py
--rw-r--r--   0        0        0     1823 2024-05-21 16:02:16.433270 docsible-0.6.3/docsible/utils/special_tasks_keys.py
--rw-r--r--   0        0        0     4749 2024-05-21 16:02:16.437269 docsible-0.6.3/docsible/utils/yaml.py
--rw-r--r--   0        0        0      860 2024-05-22 21:17:22.506430 docsible-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     5669 1970-01-01 00:00:00.000000 docsible-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-09-05 22:49:19.991131 docsible-0.6.4/LICENSE
+-rw-r--r--   0        0        0     4605 2024-05-22 21:32:29.531219 docsible-0.6.4/README.md
+-rw-r--r--   0        0        0        0 2023-09-05 22:00:43.145585 docsible-0.6.4/docsible/__init__.py
+-rw-r--r--   0        0        0    12792 2024-05-28 21:12:02.502456 docsible-0.6.4/docsible/cli.py
+-rw-r--r--   0        0        0     6777 2024-05-22 21:32:29.531219 docsible-0.6.4/docsible/markdown_template.py
+-rw-r--r--   0        0        0        0 2023-09-11 08:20:14.156264 docsible-0.6.4/docsible/utils/__init__.py
+-rw-r--r--   0        0        0    12952 2024-05-21 16:02:16.433270 docsible-0.6.4/docsible/utils/mermaid.py
+-rw-r--r--   0        0        0     1823 2024-05-21 16:02:16.433270 docsible-0.6.4/docsible/utils/special_tasks_keys.py
+-rw-r--r--   0        0        0     4749 2024-05-21 16:02:16.437269 docsible-0.6.4/docsible/utils/yaml.py
+-rw-r--r--   0        0        0      860 2024-05-28 21:10:05.965223 docsible-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     5669 1970-01-01 00:00:00.000000 docsible-0.6.4/PKG-INFO
```

### Comparing `docsible-0.6.3/LICENSE` & `docsible-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docsible-0.6.3/README.md` & `docsible-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `docsible-0.6.3/docsible/cli.py` & `docsible-0.6.4/docsible/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from docsible.markdown_template import static_template, collection_template
 from docsible.utils.mermaid import generate_mermaid_playbook, generate_mermaid_role_tasks_per_file
 from docsible.utils.yaml import load_yaml_generic, load_yaml_files_from_dir_custom, get_task_commensts
 from docsible.utils.special_tasks_keys import process_special_task_keys
 
 DOCSIBLE_START_TAG = "<!-- DOCSIBLE START -->"
 DOCSIBLE_END_TAG = "<!-- DOCSIBLE END -->"
+timestamp = datetime.now().strftime('%Y%m%d%H%M%S')
 
 def get_version():
-    return "0.6.3"
+    return "0.6.4"
 
 def manage_docsible_file_keys(docsible_path):
     default_data = {
         'description': None,
         'requester': None,
         'users': None,
         'dt_dev': None,
@@ -84,82 +85,96 @@
     else:
         final_content = new_content
     
     with open(output_path, 'w', encoding='utf-8') as readme_file:
         readme_file.write(final_content)
     print(f"Collection README.md written at: {output_path}")
 
-def document_collection_roles(collection_path, playbook, graph, no_backup, no_docsible, comments, md_template, append):
+def document_collection_roles(collection_path, playbook, graph, no_backup, no_docsible, comments, md_template, append, output):
     """
     Document all roles in a collection, extracting metadata from galaxy.yml or galaxy.yaml.
     """
     for root, dirs, files in os.walk(collection_path):
         galaxy_file = next((f for f in files if f in ['galaxy.yml', 'galaxy.yaml']), None)
         if galaxy_file:
             galaxy_path = os.path.join(root, galaxy_file)
             with open(galaxy_path, 'r') as f:
                 collection_metadata = yaml.safe_load(f)
-            readme_path = os.path.join(root, collection_metadata.get('readme', 'README.md'))
+                if output == "README.md":
+                    readme_path = os.path.join(root, collection_metadata.get('readme', output))
+                else:
+                    readme_path = os.path.join(root, output)
 
             if os.path.exists(readme_path) and not no_backup:
-                backup_path = readme_path + '_backup_' + datetime.now().strftime('%Y%m%d%H%M%S')
+                backup_path = f"{ readme_path[:readme_path.lower().rfind('.md')] }_backup_{timestamp}.md"
                 copyfile(readme_path, backup_path)
-                print(f"Backup of existing README.md created at: {backup_path}")
+                print(f"Backup of existing {output} created at: {backup_path}")
 
             roles_dir = os.path.join(root, 'roles')
             roles_info = []
             if os.path.exists(roles_dir) and os.path.isdir(roles_dir):
                 for role in os.listdir(roles_dir):
                     role_path = os.path.join(roles_dir, role)
                     if os.path.isdir(role_path):
-                        role_info = document_role(role_path, playbook, graph, no_backup, no_docsible, comments, md_template, belongs_to_collection=collection_metadata, append=append)
+                        if playbook:
+                            playbook_content = None
+                            role_playbook_path = os.path.join(role_path, playbook)
+                            try:
+                                with open(role_playbook_path, 'r') as f:
+                                    playbook_content = f.read()
+                            except FileNotFoundError:
+                                print(f'{role} not found:', role_playbook_path)
+                            except Exception as e:
+                                print(f'{playbook} import for {role} error:', e)
+                        role_info = document_role(role_path, playbook_content, graph, no_backup, no_docsible, comments, md_template, belongs_to_collection=collection_metadata, append=append, output=output)
                         roles_info.append(role_info)
 
             render_readme_template(collection_metadata, roles_info, readme_path, append)
 
 @click.command()
 @click.option('--role', default=None, help='Path to the Ansible role directory.')
 @click.option('--collection', default=None, help='Path to the Ansible collection directory.')
-@click.option('--playbook', default=None, help='Path to the playbook file.')
+@click.option('--playbook', default='tests/test.yml', help='Path to the playbook file.')
 @click.option('--graph', is_flag=True, help='Generate Mermaid graph for tasks.')
 @click.option('--no-backup', is_flag=True, help='Do not backup the readme before remove.')
 @click.option('--no-docsible', is_flag=True, help='Do not generate .docsible file and do not include it in README.md.')
 @click.option('--comments', is_flag=True, help='Read comments from tasks files')
 @click.option('--md-template', default=None, help='Path to the markdown template file.')
 @click.option('--append', is_flag=True, help='Append to the existing README.md instead of replacing it.')
+@click.option('--output', default='README.md', help='Output readme file name.')
 @click.version_option(version=get_version(), help="Show the module version.")
 
-def doc_the_role(role, collection, playbook, graph, no_backup, no_docsible, comments, md_template, append):
+def doc_the_role(role, collection, playbook, graph, no_backup, no_docsible, comments, md_template, append, output):
     if collection:
         collection_path = os.path.abspath(collection)
         if not os.path.exists(collection_path) or not os.path.isdir(collection_path):
             print(f"Folder {collection_path} does not exist.")
             return
-        document_collection_roles(collection_path, playbook, graph, no_backup, no_docsible, comments, md_template, append)
+        document_collection_roles(collection_path, playbook, graph, no_backup, no_docsible, comments, md_template, append, output)
     elif role:
         role_path = os.path.abspath(role)
         if not os.path.exists(role_path) or not os.path.isdir(role_path):
             print(f"Folder {role_path} does not exist.")
             return
         playbook_content = None
         if playbook:
             try:
                 with open(playbook, 'r') as f:
                     playbook_content = f.read()
             except FileNotFoundError:
                 print('playbook not found:', playbook)
             except Exception as e:
                 print('playbook import error:', e)
-        document_role(role_path, playbook_content, graph, no_backup, no_docsible, comments, md_template, belongs_to_collection=False, append=append)
+        document_role(role_path, playbook_content, graph, no_backup, no_docsible, comments, md_template, belongs_to_collection=False, append=append, output=output)
     else:
         print("Please specify either a role or a collection path.")
 
-def document_role(role_path, playbook_content, generate_graph, no_backup, no_docsible, comments, md_template, belongs_to_collection, append):
+def document_role(role_path, playbook_content, generate_graph, no_backup, no_docsible, comments, md_template, belongs_to_collection, append, output):
     role_name = os.path.basename(role_path)
-    readme_path = os.path.join(role_path, "README.md")
+    readme_path = os.path.join(role_path, output)
     meta_path = os.path.join(role_path, "meta", "main.yml")
     docsible_path = os.path.join(role_path, ".docsible")
     if not no_docsible:
         manage_docsible_file_keys(docsible_path)
 
     # Check if meta/main.yml exist, otherwise try meta/main.yaml
     if not os.path.exists(meta_path):
@@ -208,16 +223,15 @@
                                 task_info['tasks'].extend(processed_tasks)
                                 task_info['mermaid'].extend([task])
 
                         role_info["tasks"].append(task_info)
 
     if os.path.exists(readme_path):
         if not no_backup:
-            timestamp = datetime.now().strftime('%Y%m%d%H%M%S')
-            backup_readme_path = os.path.join(role_path, f"README_backup_{timestamp}.md")
+            backup_readme_path = os.path.join(role_path, f"{ output[:output.lower().rfind('.md')] }_backup_{timestamp}.md")
             copyfile(readme_path, backup_readme_path)
             print(f'Readme file backed up as: {backup_readme_path}')
         if not append:
             os.remove(readme_path)
 
     mermaid_code_per_file = {}
     if generate_graph:
```

### Comparing `docsible-0.6.3/docsible/markdown_template.py` & `docsible-0.6.4/docsible/markdown_template.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.3/docsible/utils/mermaid.py` & `docsible-0.6.4/docsible/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.3/docsible/utils/special_tasks_keys.py` & `docsible-0.6.4/docsible/utils/special_tasks_keys.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.3/docsible/utils/yaml.py` & `docsible-0.6.4/docsible/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.3/pyproject.toml` & `docsible-0.6.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docsible"
-version = "0.6.3"
+version = "0.6.4"
 description = "Document generator for ansible role/collection"
 authors = ["Lucian BLETAN <neuraluc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `docsible-0.6.3/PKG-INFO` & `docsible-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docsible
-Version: 0.6.3
+Version: 0.6.4
 Summary: Document generator for ansible role/collection
 License: MIT
 Author: Lucian BLETAN
 Author-email: neuraluc@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

