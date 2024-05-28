# Comparing `tmp/inception_reports-0.3.2.tar.gz` & `tmp/inception_reports-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inception_reports-0.3.2.tar", last modified: Thu May 16 10:10:46 2024, max compression
+gzip compressed data, was "inception_reports-0.4.1.tar", last modified: Tue May 28 01:11:14 2024, max compression
```

## Comparing `inception_reports-0.3.2.tar` & `inception_reports-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 10:10:46.418055 inception_reports-0.3.2/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    11357 2023-09-25 12:56:28.000000 inception_reports-0.3.2/LICENSE
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       72 2024-05-16 10:10:41.000000 inception_reports-0.3.2/MANIFEST.in
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      752 2023-11-07 13:15:00.000000 inception_reports-0.3.2/NOTICE.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2065 2024-05-16 10:10:46.418055 inception_reports-0.3.2/PKG-INFO
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1376 2024-04-30 00:10:18.000000 inception_reports-0.3.2/README.md
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 10:10:46.414055 inception_reports-0.3.2/inception_reports/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-04-02 01:14:36.000000 inception_reports-0.3.2/inception_reports/__init__.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1704 2024-04-29 23:24:38.000000 inception_reports-0.3.2/inception_reports/__main__.py
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 10:10:46.414055 inception_reports-0.3.2/inception_reports/data/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-05-16 09:38:16.000000 inception_reports-0.3.2/inception_reports/data/__init__.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    19092 2024-05-15 09:37:35.000000 inception_reports-0.3.2/inception_reports/data/document_types.json
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1337 2024-05-15 09:37:35.000000 inception_reports-0.3.2/inception_reports/data/specialties.json
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     6443 2024-05-16 09:44:28.000000 inception_reports-0.3.2/inception_reports/generate_reports_lead.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    16666 2024-05-16 09:44:22.000000 inception_reports-0.3.2/inception_reports/generate_reports_manager.py
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 10:10:46.418055 inception_reports-0.3.2/inception_reports.egg-info/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2065 2024-05-16 10:10:46.000000 inception_reports-0.3.2/inception_reports.egg-info/PKG-INFO
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      645 2024-05-16 10:10:46.000000 inception_reports-0.3.2/inception_reports.egg-info/SOURCES.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)        1 2024-05-16 10:10:46.000000 inception_reports-0.3.2/inception_reports.egg-info/dependency_links.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       70 2024-05-16 10:10:46.000000 inception_reports-0.3.2/inception_reports.egg-info/entry_points.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       52 2024-05-16 10:10:46.000000 inception_reports-0.3.2/inception_reports.egg-info/requires.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       18 2024-05-16 10:10:46.000000 inception_reports-0.3.2/inception_reports.egg-info/top_level.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      944 2024-05-16 10:10:35.000000 inception_reports-0.3.2/pyproject.toml
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       38 2024-05-16 10:10:46.418055 inception_reports-0.3.2/setup.cfg
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-16 10:10:46.418055 inception_reports-0.3.2/tests/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     3565 2024-05-15 09:37:35.000000 inception_reports-0.3.2/tests/test_generate_reports_lead.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     4262 2024-05-07 01:00:49.000000 inception_reports-0.3.2/tests/test_generate_reports_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:14.472260 inception_reports-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 01:11:10.000000 inception_reports-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 01:11:10.000000 inception_reports-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-28 01:11:10.000000 inception_reports-0.4.1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-28 01:11:14.472260 inception_reports-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-28 01:11:10.000000 inception_reports-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:14.468260 inception_reports-0.4.1/inception_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-28 01:11:10.000000 inception_reports-0.4.1/inception_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-28 01:11:10.000000 inception_reports-0.4.1/inception_reports/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:14.472260 inception_reports-0.4.1/inception_reports/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    19092 2024-05-28 01:11:10.000000 inception_reports-0.4.1/inception_reports/data/document_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-28 01:11:10.000000 inception_reports-0.4.1/inception_reports/data/specialties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-28 01:11:10.000000 inception_reports-0.4.1/inception_reports/generate_reports_lead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-05-28 01:11:10.000000 inception_reports-0.4.1/inception_reports/generate_reports_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:14.472260 inception_reports-0.4.1/inception_reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-28 01:11:14.000000 inception_reports-0.4.1/inception_reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-28 01:11:14.000000 inception_reports-0.4.1/inception_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:11:14.000000 inception_reports-0.4.1/inception_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 01:11:14.000000 inception_reports-0.4.1/inception_reports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 01:11:14.000000 inception_reports-0.4.1/inception_reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 01:11:14.000000 inception_reports-0.4.1/inception_reports.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-28 01:11:10.000000 inception_reports-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:11:14.472260 inception_reports-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:14.472260 inception_reports-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-28 01:11:10.000000 inception_reports-0.4.1/tests/test_generate_reports_lead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-28 01:11:10.000000 inception_reports-0.4.1/tests/test_generate_reports_manager.py
```

### Comparing `inception_reports-0.3.2/LICENSE` & `inception_reports-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3.2/NOTICE.txt` & `inception_reports-0.4.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3.2/PKG-INFO` & `inception_reports-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inception_reports
-Version: 0.3.2
+Version: 0.4.1
 Summary: Generate plots that report the progress of an INCEpTION project.
 Author-email: Serwar <serwar.basch@tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/inception-project/inception-reporting-dashboard
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `inception_reports-0.3.2/README.md` & `inception_reports-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3.2/inception_reports/__init__.py` & `inception_reports-0.4.1/inception_reports/__init__.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3.2/inception_reports/__main__.py` & `inception_reports-0.4.1/inception_reports/__main__.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3.2/inception_reports/data/document_types.json` & `inception_reports-0.4.1/inception_reports/data/document_types.json`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3.2/inception_reports/data/specialties.json` & `inception_reports-0.4.1/inception_reports/data/specialties.json`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3.2/inception_reports/generate_reports_lead.py` & `inception_reports-0.4.1/inception_reports/generate_reports_lead.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     """
 
     st.sidebar.write(
         "Please input the path to the folder containing the INCEpTION projects."
     )
     projects_folder = st.sidebar.text_input(
         "Projects Folder:",
-        value="/home/basch/Documents/projects/gemtex_demo_exported_data/",
+        value="",
     )
     button = st.sidebar.button("Generate Reports")
     if button:
         st.session_state["initialized"] = True
         st.session_state["projects"] = read_dir(projects_folder)
         button = False
         set_sidebar_state("collapsed")
```

### Comparing `inception_reports-0.3.2/inception_reports/generate_reports_manager.py` & `inception_reports-0.4.1/inception_reports/generate_reports_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,45 +106,47 @@
         with open(translation_path, "r") as f:
             translation = json.load(f)
         if tag in translation:
             return translation[tag]
         else:
             return tag
     else:
-        data_path = importlib.resources.files('inception_reports.data')
+        data_path = importlib.resources.files("inception_reports.data")
         with open(data_path.joinpath("specialties.json"), "r") as f:
             specialties = json.load(f)
         with open(data_path.joinpath("document_types.json"), "r") as f:
             document_types = json.load(f)
 
         if tag in specialties:
             return specialties[tag]
         elif tag in document_types:
             return document_types[tag]
         else:
             return tag
 
 
-def read_dir(dir_path: str) -> list[dict]:
+def read_dir(dir_path: str, selected_projects: list = None) -> list[dict]:
     """
     Reads a directory containing zip files, extracts the contents, and retrieves project metadata and annotations.
 
-    Args:
+    Parameters:
         dir_path (str): The path to the directory containing the zip files.
 
     Returns:
         list[dict]: A list of dictionaries, where each dictionary represents a project and contains the following keys:
             - "name": The name of the zip file.
             - "tags": A list of tags extracted from the project metadata.
             - "documents": A list of source documents from the project metadata.
             - "annotations": A dictionary mapping annotation subfolder names to their corresponding CAS objects.
     """
     projects = []
 
     for file_name in os.listdir(dir_path):
+        if selected_projects and file_name.split(".")[0] not in selected_projects:
+            continue
         file_path = os.path.join(dir_path, file_name)
         if zipfile.is_zipfile(file_path):
             with zipfile.ZipFile(file_path, "r") as zip_file:
                 zip_path = f"{dir_path}/{file_name.split('.')[0]}"
                 zip_file.extractall(path=zip_path)
 
                 # Find project metadata file
@@ -173,15 +175,15 @@
                     with zip_file.open(annotation_file) as cas_file:
                         cas = cassis.load_cas_from_json(cas_file)
                         annotations[subfolder_name] = cas
 
                 projects.append(
                     {
                         "name": file_name,
-                        "tags": project_tags,
+                        "tags": project_tags if project_tags else None,
                         "documents": project_documents,
                         "annotations": annotations,
                     }
                 )
 
                 # Clean up extracted files
                 shutil.rmtree(zip_path)
@@ -215,55 +217,71 @@
 
 def select_method_to_import_data():
     """
     Allows the user to select a method to import data for generating reports.
     """
 
     method = st.sidebar.radio(
-        "Choose your method to import data:", ("Manually", "API"), index=0
+        "Choose your method to import data:", ("Manually", "API"), index=1
     )
 
     if method == "Manually":
         st.sidebar.write(
             "Please input the path to the folder containing the INCEpTION projects."
         )
-        projects_folder = st.sidebar.text_input(
-            "Projects Folder:", value="data/gemtex_demo_projects/"
-        )
+        projects_folder = st.sidebar.text_input("Projects Folder:", value="")
         button = st.sidebar.button("Generate Reports")
         if button:
-            st.session_state["initialized"] = True
             st.session_state["method"] = "Manually"
             st.session_state["projects"] = read_dir(projects_folder)
             button = False
             set_sidebar_state("collapsed")
     elif method == "API":
+        projects_folder = f"{os.path.expanduser('~')}/.inception_reports/projects"
+        os.makedirs(os.path.dirname(projects_folder), exist_ok=True)
         api_url = st.sidebar.text_input("Enter API URL:", "")
         username = st.sidebar.text_input("Username:", "")
         password = st.sidebar.text_input("Password:", type="password", value="")
-        inception_status, inception_client = login_to_inception(
-            api_url, username, password
-        )
-        if inception_status:
+        inception_status = st.session_state.get("inception_status", False)
+        inception_client = st.session_state.get("inception_client", None)
+        if not inception_status:
+            inception_status, inception_client = login_to_inception(api_url, username, password)
+            st.session_state["inception_status"] = inception_status
+            st.session_state["inception_client"] = inception_client
+
+        if inception_status and "available_projects" not in st.session_state:
             inception_projects = inception_client.api.projects()
-            st.sidebar.write("Following projects got imported:")
-            for inception_project in inception_projects:
-                st.sidebar.write(inception_project.project_name)
-                project_export = inception_client.api.export_project(
-                    inception_project, "jsoncas"
-                )
-                with open(
-                    f"{os.path.expanduser('~')}/.inception_reports/projects/{inception_project}.zip",
-                    "wb",
-                ) as f:
-                    f.write(project_export)
-            st.session_state["initialized"] = True
-            st.session_state["method"] = "API"
-            st.session_state["projects"] = read_dir(projects_folder)
-            set_sidebar_state("collapsed")
+            st.session_state["available_projects"] = inception_projects
+
+        if inception_status and "available_projects" in st.session_state:
+            st.sidebar.write("Select the projects to import:")
+            selected_projects = st.session_state.get("selected_projects", {})
+            
+            for inception_project in st.session_state["available_projects"]:
+                project_name = inception_project.project_name
+                project_id = inception_project.project_id
+                selected_projects[project_id] = st.sidebar.checkbox(project_name, value=False)
+                st.session_state["selected_projects"] = selected_projects
+            
+            selected_projects_names = []
+            button = st.sidebar.button("Generate Reports")
+            if button:
+                for project_id, is_selected in selected_projects.items():
+                    if is_selected:
+                        project = inception_client.api.project(project_id)
+                        selected_projects_names.append(project.project_name)
+                        file_path = f"{projects_folder}/{project.project_name}.zip"
+                        st.sidebar.write(f"Importing project: {project.project_name}")
+                        project_export = inception_client.api.export_project(project, "jsoncas")
+                        with open(file_path, "wb") as f:
+                            f.write(project_export)
+                
+                st.session_state["method"] = "API"
+                st.session_state["projects"] = read_dir(projects_folder, selected_projects_names)
+                set_sidebar_state("collapsed")
 
 
 def find_element_by_name(element_list, name):
     """
     Finds an element in the given element list by its name.
 
     Args:
@@ -286,16 +304,15 @@
     Args:
         annotations (dict): A dictionary containing the annotations.
 
     Returns:
         dict: A dictionary containing the count of each type.
     """
     count_dict = {}
-
-    layerDefinition = annotations.popitem()[1].select(
+    layerDefinition = next(iter(annotations.values())).select(
         "de.tudarmstadt.ukp.clarin.webanno.api.type.LayerDefinition"
     )
     for doc in annotations:
         type_names = [
             (
                 find_element_by_name(layerDefinition, t.name),
                 len(annotations[doc].select(t.name)),
@@ -354,25 +371,31 @@
     compared to the estimated time for remaining documents.
 
     Parameters:
         project (dict): A dict containing project information, namely the name, tags, annotations, and logs.
 
     """
 
-    st.write(
-        f"<div style='text-align: center; font-size: 18px;'><b>Project Name</b>: {project['name']} <br> <b>Tags</b>: {', '.join(project['tags'])}</div>",
-        unsafe_allow_html=True,
-    )
-
     # df = project["logs"]
     project_name = project["name"].strip(".zip")
     project_tags = project["tags"]
     project_annotations = project["annotations"]
     project_documents = project["documents"]
 
+    if project_tags:
+        st.write(
+            f"<div style='text-align: center; font-size: 18px;'><b>Project Name</b>: {project_name} <br> <b>Tags</b>: {', '.join(project['tags'])}</div>",
+            unsafe_allow_html=True,
+        )
+    else:
+        st.write(
+            f"<div style='text-align: center; font-size: 18px;'><b>Project Name</b>: {project_name} <br> <b>Tags</b>: No tags available</div>",
+            unsafe_allow_html=True,
+        )
+
     doc_categories = {
         "ANNOTATION_IN_PROGRESS": 0,
         "ANNOTATION_FINISHED": 0,
         "CURATION_IN_PROGRESS": 0,
         "CURATION_FINISHED": 0,
         "NEW": 0,
     }
@@ -415,19 +438,19 @@
             "Types": [type for type, _ in type_counts.items()],
             "Counts": list(type_counts.values()),
         }
     )
 
     pie_chart = go.Figure(
         go.Pie(
-            labels=df_pie['Labels'],
-            values=df_pie['Sizes'],
+            labels=df_pie["Labels"],
+            values=df_pie["Sizes"],
             sort=False,
             hole=0.4,
-            hoverinfo="label+value"
+            hoverinfo="label+value",
         )
     )
 
     pie_chart.update_layout(
         title=dict(
             text="Documents Status",
             font=dict(size=24),
@@ -435,43 +458,43 @@
             x=0.5,
             xanchor="center",
         ),
         font=dict(size=18),
         legend=dict(font=dict(size=12), y=0.5),
         paper_bgcolor="rgba(0,0,0,0)",
         plot_bgcolor="rgba(0,0,0,0)",
-        margin=dict(l=40, r=40)
+        margin=dict(l=40, r=40),
     )
 
     bar_chart = go.Figure()
 
     for _, row in df_bar.iterrows():
         bar_chart.add_trace(
             go.Bar(
                 y=[row["Types"]],
                 x=[row["Counts"]],
                 orientation="h",
                 name=row["Types"],
                 legendgroup=row["Types"],
                 showlegend=True,
-                hoverinfo="x+y"
+                hoverinfo="x+y",
             )
         )
 
     bar_chart.update_layout(
         title=dict(
             text="Types of Annotations",
             font=dict(size=24),
             y=0.95,
             x=0.45,
             xanchor="center",
         ),
         xaxis_title="Number of Annotations",
         barmode="overlay",
-        height=50 * len(df_bar),
+        height= 60 * len(df_bar),
         font=dict(size=18),
         legend=dict(font=dict(size=12)),
         paper_bgcolor="rgba(0,0,0,0)",
         plot_bgcolor="rgba(0,0,0,0)",
         margin=dict(l=40, r=40),
         colorway=px.colors.qualitative.Plotly,
     )
```

### Comparing `inception_reports-0.3.2/inception_reports.egg-info/PKG-INFO` & `inception_reports-0.4.1/inception_reports.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inception_reports
-Version: 0.3.2
+Version: 0.4.1
 Summary: Generate plots that report the progress of an INCEpTION project.
 Author-email: Serwar <serwar.basch@tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/inception-project/inception-reporting-dashboard
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `inception_reports-0.3.2/inception_reports.egg-info/SOURCES.txt` & `inception_reports-0.4.1/inception_reports.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,11 @@
 inception_reports/generate_reports_manager.py
 inception_reports.egg-info/PKG-INFO
 inception_reports.egg-info/SOURCES.txt
 inception_reports.egg-info/dependency_links.txt
 inception_reports.egg-info/entry_points.txt
 inception_reports.egg-info/requires.txt
 inception_reports.egg-info/top_level.txt
-inception_reports/data/__init__.py
 inception_reports/data/document_types.json
 inception_reports/data/specialties.json
 tests/test_generate_reports_lead.py
 tests/test_generate_reports_manager.py
```

### Comparing `inception_reports-0.3.2/pyproject.toml` & `inception_reports-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inception_reports"
 description = "Generate plots that report the progress of an INCEpTION project."
-version = "0.3.2"
+version = "0.4.1"
 authors = [
     { name = "Serwar", email = "serwar.basch@tu-darmstadt.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 
 dependencies = [
```

### Comparing `inception_reports-0.3.2/tests/test_generate_reports_lead.py` & `inception_reports-0.4.1/tests/test_generate_reports_lead.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.3.2/tests/test_generate_reports_manager.py` & `inception_reports-0.4.1/tests/test_generate_reports_manager.py`

 * *Files identical despite different names*

