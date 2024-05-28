# Comparing `tmp/aurora_ssg-0.0.1.tar.gz` & `tmp/aurora_ssg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora_ssg-0.0.1.tar", last modified: Mon May 27 15:43:55 2024, max compression
+gzip compressed data, was "aurora_ssg-0.0.2.tar", last modified: Tue May 28 10:09:32 2024, max compression
```

## Comparing `aurora_ssg-0.0.1.tar` & `aurora_ssg-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-27 15:43:55.239232 aurora_ssg-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)     1061 2024-05-27 15:17:29.000000 aurora_ssg-0.0.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     6255 2024-05-27 15:43:55.238887 aurora_ssg-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     5294 2024-05-27 15:42:54.000000 aurora_ssg-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-27 15:43:55.236087 aurora_ssg-0.0.1/aurora/
--rw-r--r--   0 james      (501) staff       (20)       22 2024-05-27 15:43:42.000000 aurora_ssg-0.0.1/aurora/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1250 2024-05-27 15:43:43.000000 aurora_ssg-0.0.1/aurora/cli.py
--rw-r--r--   0 james      (501) staff       (20)      728 2024-05-27 15:43:42.000000 aurora_ssg-0.0.1/aurora/date_helpers.py
--rw-r--r--   0 james      (501) staff       (20)    20203 2024-05-27 15:43:43.000000 aurora_ssg-0.0.1/aurora/graph.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-27 15:43:55.237904 aurora_ssg-0.0.1/aurora_ssg.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     6255 2024-05-27 15:43:55.000000 aurora_ssg-0.0.1/aurora_ssg.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      304 2024-05-27 15:43:55.000000 aurora_ssg-0.0.1/aurora_ssg.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-05-27 15:43:55.000000 aurora_ssg-0.0.1/aurora_ssg.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       43 2024-05-27 15:43:55.000000 aurora_ssg-0.0.1/aurora_ssg.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)      147 2024-05-27 15:43:55.000000 aurora_ssg-0.0.1/aurora_ssg.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        7 2024-05-27 15:43:55.000000 aurora_ssg-0.0.1/aurora_ssg.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2024-05-27 15:43:55.239297 aurora_ssg-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1569 2024-05-27 15:43:42.000000 aurora_ssg-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:09:32.647052 aurora_ssg-0.0.2/
+-rw-r--r--   0 james      (501) staff       (20)      544 2024-05-28 10:09:29.000000 aurora_ssg-0.0.2/CHANGELOG.md
+-rw-r--r--   0 james      (501) staff       (20)     1061 2024-05-28 08:11:52.000000 aurora_ssg-0.0.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     6779 2024-05-28 10:09:32.646730 aurora_ssg-0.0.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     5787 2024-05-28 08:11:52.000000 aurora_ssg-0.0.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:09:32.643949 aurora_ssg-0.0.2/aurora/
+-rw-r--r--   0 james      (501) staff       (20)       22 2024-05-28 10:07:42.000000 aurora_ssg-0.0.2/aurora/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1250 2024-05-28 09:09:39.000000 aurora_ssg-0.0.2/aurora/cli.py
+-rw-r--r--   0 james      (501) staff       (20)      728 2024-05-28 08:11:52.000000 aurora_ssg-0.0.2/aurora/date_helpers.py
+-rw-r--r--   0 james      (501) staff       (20)    19826 2024-05-28 09:57:26.000000 aurora_ssg-0.0.2/aurora/graph.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-28 10:09:32.645864 aurora_ssg-0.0.2/aurora_ssg.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     6779 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      328 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       43 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      153 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        7 2024-05-28 10:09:32.000000 aurora_ssg-0.0.2/aurora_ssg.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)   923054 2024-05-28 08:11:52.000000 aurora_ssg-0.0.2/banner.png
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-05-28 10:09:32.647122 aurora_ssg-0.0.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1563 2024-05-28 09:57:24.000000 aurora_ssg-0.0.2/setup.py
```

### Comparing `aurora_ssg-0.0.1/LICENSE` & `aurora_ssg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.1/PKG-INFO` & `aurora_ssg-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aurora-ssg
-Version: 0.0.1
-Summary: A fast static site generator for Python.
+Version: 0.0.2
+Summary: A fast static site generator implemented in Python.
 Home-page: https://github.com/capjamesg/aurora
 Author: capjamesg
 Author-email: readers@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,14 +14,15 @@
 Requires-Dist: jinja2
 Requires-Dist: watchdog
 Requires-Dist: toposort
 Requires-Dist: pyromark
 Requires-Dist: python-frontmatter
 Requires-Dist: requests
 Requires-Dist: progress
+Requires-Dist: click
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black==22.3.0; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
@@ -38,14 +39,18 @@
 [![python-version](https://img.shields.io/pypi/pyversions/aurora-ssg)](https://badge.fury.io/py/aurora-ssg)
 </div>
 
 # Aurora
 
 Aurora is a static site generator implemented in Python.
 
+## Demo
+
+https://github.com/capjamesg/aurora/assets/37276661/59e4f3e6-f470-46bd-8812-0b475be40e88
+
 ## Get Started
 
 ### Install Aurora
 
 First, install Aurora:
 
 ```bash
@@ -198,12 +203,22 @@
 REGISTERED_HOOKS = {
     "hook_file_name": ["hook1", "hook2", "hook3"],
 }
 ```
 
 ## Performance
 
-TODO
+In a test on a website with 1763 files, Aurora built the website in `0:00:04.23`.
+
+The files were a combination of blog posts, static pages, and programmatic archives for blog posts (date pages, category pages).
+
+## Users
+
+The following sites are built with Aurora:
+
+- [James' Coffee Blog](https://jamesg.blog) (1,500+ pages)
+
+Have you made a website with Aurora? File a PR and add it to the list!
 
 ## License
 
 This project is licensed under an [MIT license](LICENSE).
```

### Comparing `aurora_ssg-0.0.1/README.md` & `aurora_ssg-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 [![python-version](https://img.shields.io/pypi/pyversions/aurora-ssg)](https://badge.fury.io/py/aurora-ssg)
 </div>
 
 # Aurora
 
 Aurora is a static site generator implemented in Python.
 
+## Demo
+
+https://github.com/capjamesg/aurora/assets/37276661/59e4f3e6-f470-46bd-8812-0b475be40e88
+
 ## Get Started
 
 ### Install Aurora
 
 First, install Aurora:
 
 ```bash
@@ -168,12 +172,22 @@
 REGISTERED_HOOKS = {
     "hook_file_name": ["hook1", "hook2", "hook3"],
 }
 ```
 
 ## Performance
 
-TODO
+In a test on a website with 1763 files, Aurora built the website in `0:00:04.23`.
+
+The files were a combination of blog posts, static pages, and programmatic archives for blog posts (date pages, category pages).
+
+## Users
+
+The following sites are built with Aurora:
+
+- [James' Coffee Blog](https://jamesg.blog) (1,500+ pages)
+
+Have you made a website with Aurora? File a PR and add it to the list!
 
 ## License
 
-This project is licensed under an [MIT license](LICENSE).
+This project is licensed under an [MIT license](LICENSE).
```

### Comparing `aurora_ssg-0.0.1/aurora/cli.py` & `aurora_ssg-0.0.2/aurora/cli.py`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.1/aurora/date_helpers.py` & `aurora_ssg-0.0.2/aurora/date_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora_ssg-0.0.1/aurora/graph.py` & `aurora_ssg-0.0.2/aurora/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,85 @@
 import os
 import sys
 
 if not os.path.exists("config.py"):
     raise Exception("config.py not found")
 
 import datetime
-import optparse
 import re
 import time
 
 import pyromark
 from frontmatter import loads
-from jinja2 import (Environment, FileSystemLoader, environment, exceptions,
-                    meta, nodes)
+from jinja2 import (Environment, FileSystemLoader, Template, environment,
+                    exceptions, meta, nodes)
 from jinja2.visitor import NodeVisitor
 from progress.bar import IncrementalBar
 from toposort import toposort, toposort_flatten
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 
 from .date_helpers import (archive_date, date_to_xml_string, list_archive_date,
                            long_date, month_number_to_written_month)
 
 module_dir = os.getcwd()
 os.chdir(module_dir)
-# add to path
 sys.path.append(module_dir)
+
 from config import (BASE_URL, LAYOUTS_BASE_DIR, REGISTERED_HOOKS, ROOT_DIR,
                     SITE_DIR, SITE_ENV)
 
-# for hook in registered hook, get all funcs
 for hook in REGISTERED_HOOKS:
     REGISTERED_HOOKS[hook] = [
         getattr(__import__(hook), func) for func in REGISTERED_HOOKS[hook]
     ]
 
-# get date of today w/ no time
 today = datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)
 state = {
     "posts": [],
     "site": {"root_url": BASE_URL},
     "build_date": today.strftime("%m-%d"),
+    "pages": [],
 }
 start = datetime.datetime.now()
 
 if not os.path.exists(SITE_DIR):
     os.makedirs(SITE_DIR)
 else:
     # remove all files in _site
     for root, dirs, files in os.walk(SITE_DIR):
         for file in files:
             os.remove(os.path.join(root, file))
 
 JINJA2_ENV = Environment(loader=FileSystemLoader(ROOT_DIR), cache_size=2000)
 
 
-def slugify(value):
+def slugify(value: str) -> str:
+    """
+    Turn a string into a slug for use in saving data to a file.
+    """
     return value.lower().replace(" ", "-")
 
 
+class Watcher(FileSystemEventHandler):
+    def on_modified(self, event):
+        print(f"Detected change in {event.src_path}. Rebuilding.")
+        file_name = event.src_path
+        file_name = file_name.replace(os.getcwd() + "/", "")
+        file_dependencies = all_dependencies[file_name]
+        file_dependencies.add(file_name)
+
+        main(deps=file_dependencies)
+
+
 class VariableVisitor(NodeVisitor):
+    """
+    Find all variables in a jinja2 template.
+    """
+
     def __init__(self):
         self.variables = set()
 
     def visit_Name(self, node, *args, **kwargs):
         self.variables.add(node.name)
         self.generic_visit(node, *args, **kwargs)
 
@@ -82,45 +98,58 @@
 
 JINJA2_ENV.filters["long_date"] = long_date
 JINJA2_ENV.filters["date_to_xml_string"] = date_to_xml_string
 JINJA2_ENV.filters["archive_date"] = archive_date
 JINJA2_ENV.filters["list_archive_date"] = list_archive_date
 JINJA2_ENV.filters["month_number_to_written_month"] = month_number_to_written_month
 
+ALLOWED_EXTENSIONS = ["html", "md", "css", "js", "txt", "xml"]
+
 all_pages = []
 
 for root, dirs, files in os.walk(ROOT_DIR):
     for file in files:
+        ext = os.path.splitext(file)[-1].replace(".", "")
+        if ext not in ALLOWED_EXTENSIONS:
+            continue
+
         all_pages.append(os.path.join(root, file))
 
 all_opened_pages = {}
+all_page_contents = {}
 
 for page in all_pages:
     with open(page, "r") as f:
+        contents = f.read()
         try:
             if page.endswith(".md"):
-                all_opened_pages[page] = f.read()
+                all_opened_pages[page] = contents
             else:
-                all_opened_pages[page] = JINJA2_ENV.from_string(f.read())
+                all_opened_pages[page] = JINJA2_ENV.from_string(contents)
+
+            all_page_contents[page] = loads(contents)
         except:
             print(f"Error reading {page}")
             pass
 
 
 all_dependencies = {}
 all_parsed_pages = {}
 
 
-def get_file_dependencies_and_evaluated_contents(file_name, contents):
-    if isinstance(contents, str):
-        template = JINJA2_ENV.parse(contents)
-    else:
-        # TODO: Make this more efficient
-        with open(file_name, "r") as f:
-            template = JINJA2_ENV.parse(f.read())
+def get_file_dependencies_and_evaluated_contents(
+    file_name: str, contents: Template
+) -> tuple:
+    """
+    Get all dependencies of a file. Dependencies are:
+
+    1. Other files that are included in the file, and;
+    2. Variables whose values are defined by the site generator (i.e. `site.*`).
+    """
+    template = JINJA2_ENV.parse(contents)
 
     includes = []
     included_variables = []
 
     for node in meta.find_referenced_templates(template):
         includes.append(node)
 
@@ -141,98 +170,67 @@
     for variable in included_variables:
         if not variable.startswith("site."):
             continue
 
         variable = variable.replace("site.", "")
         dependencies.add(f"{ROOT_DIR}/{variable}")
 
-    parsed_content = None
+    parsed_content = all_page_contents[file_name]
 
-    rendered_template = contents
+    parsed_content["slug"] = file_name.split("/")[-1].replace(".html", "")
 
-    try:
-        if (
-            isinstance(rendered_template, environment.Template)
-            and not file_name.startswith("pages/_layouts")
-            and not file_name.startswith("pages/_includes")
-            and not file_name.startswith("pages/templates")
-        ):
-            state["categories"] = []
-            state["stream"] = []
-            rendered_template = rendered_template.render(page=state, site=state)
-        else:
-            # open file and render
-            with open(file_name, "r") as f:
-                rendered_template = f.read()
-
-        parsed_content = loads(rendered_template)
-        parsed_content["slug"] = file_name.split("/")[-1].replace(".html", "")
-        # if no categories, add
-        # ADD ROOT URL
-        parsed_content["contents"] = pyromark.markdown(parsed_content.content)
-        parsed_content[
-            "url"
-        ] = f"{BASE_URL}/{file_name.replace(ROOT_DIR + '/posts/', '')}"
-        if "categories" not in parsed_content:
-            parsed_content["categories"] = []
-        # slug = parsed_content.get("slug")
-        # extract date slug w/ regex
-        slug = file_name.split("/")[-1].replace(".html", "")
-
-        slug = slug.replace("posts/", "")
+    parsed_content["url"] = f"{BASE_URL}/{file_name.replace(ROOT_DIR + '/posts/', '')}"
+    if "categories" not in parsed_content:
+        parsed_content["categories"] = []
+    # slug = parsed_content.get("slug")
+    # extract date slug w/ regex
+    slug = file_name.split("/")[-1].replace(".html", "")
+
+    slug = slug.replace("posts/", "")
+
+    if slug[0].isdigit():
+        date_slug = re.search(r"\d{4}-\d{2}-\d{2}", slug)
+
+        if date_slug:
+            date_slug = date_slug.group(0)
+            if not parsed_content.get("post"):
+                parsed_content["post"] = {}
+            if not parsed_content.get("page"):
+                parsed_content["page"] = {}
+            parsed_content["post"]["date"] = datetime.datetime.strptime(
+                date_slug, "%Y-%m-%d"
+            )
 
-        if slug:
-            date_slug = re.search(r"\d{4}-\d{2}-\d{2}", slug)
-            if date_slug:
-                # print(date_slug)
-                date_slug = date_slug.group(0)
-                if not parsed_content.get("post"):
-                    parsed_content["post"] = {}
-                if not parsed_content.get("page"):
-                    parsed_content["page"] = {}
-                parsed_content["post"]["date"] = datetime.datetime.strptime(
-                    date_slug, "%Y-%m-%d"
+            parsed_content["post"]["date_without_year"] = parsed_content["post"][
+                "date"
+            ].strftime("%m-%d")
+            parsed_content["date_without_year"] = parsed_content["post"][
+                "date_without_year"
+            ]
+
+            parsed_content["post"]["full_date"] = parsed_content["post"][
+                "date"
+            ].strftime("%B %d, %Y")
+            parsed_content["date"] = parsed_content["post"]["date"]
+
+            parsed_content["page"]["date"] = parsed_content["post"]["date"]
+
+            if "description" not in parsed_content:
+                parsed_content["description"] = pyromark.markdown(
+                    parsed_content.content.split("\n")[0]
                 )
-                # date_without_year
-                parsed_content["post"]["date_without_year"] = parsed_content["post"][
-                    "date"
-                ].strftime("%m-%d")
-                parsed_content["date_without_year"] = parsed_content["post"][
-                    "date_without_year"
-                ]
 
-                parsed_content["post"]["full_date"] = parsed_content["post"][
-                    "date"
-                ].strftime("%B %d, %Y")
-                parsed_content["date"] = parsed_content["post"]["date"]
-                # add page.date
-                parsed_content["page"]["date"] = parsed_content["post"]["date"]
-                # add description
-                if "description" not in parsed_content:
-                    parsed_content["description"] = pyromark.markdown(
-                        parsed_content.content.split("\n")[0]
-                    )
-
-        if "layout" in parsed_content:
-            dependencies.add(
-                f"{ROOT_DIR}/{LAYOUTS_BASE_DIR}/{parsed_content['layout']}.html"
-            )
-            # if layout is post, add to state global
-            # if parsed_content["layout"] == "post":
-            if not state.get(parsed_content["layout"] + "s"):
-                state[parsed_content["layout"] + "s"] = []
-
-            state[parsed_content["layout"] + "s"].append(parsed_content)
-    except exceptions.UndefinedError as e:
-        raise e
-    except Exception as e:
-        # raise e
-        print(f"Error parsing {file_name}")
-        pass
+    if "layout" in parsed_content:
+        dependencies.add(
+            f"{ROOT_DIR}/{LAYOUTS_BASE_DIR}/{parsed_content['layout']}.html"
+        )
+        if not state.get(parsed_content["layout"] + "s"):
+            state[parsed_content["layout"] + "s"] = []
 
+        state[parsed_content["layout"] + "s"].append(parsed_content)
     return dependencies, parsed_content
 
 
 for page, contents in all_opened_pages.items():
     dependencies, parsed_page = get_file_dependencies_and_evaluated_contents(
         page, contents
     )
@@ -240,15 +238,14 @@
     all_parsed_pages[page] = parsed_page
 
     if page.startswith("posts/"):
         state["posts"].append(parsed_page)
 
 posts = [key for key in all_opened_pages.keys() if key.startswith(ROOT_DIR + "/posts")]
 
-# get all dates
 dates = set()
 years = {}
 
 for post in posts:
     if not hasattr(all_parsed_pages[post], "metadata"):
         continue
 
@@ -262,93 +259,108 @@
         if date.day not in years[date.year][date.month]:
             years[date.year][date.month][date.day] = []
         years[date.year][date.month][date.day].append(post)
 
 state["years"] = years
 
 state["posts"] = sorted(
-    # sort by file name
     state["posts"],
     key=lambda x: x["slug"],
     reverse=True,
 )
 
 
 sorted_files = toposort(all_dependencies)
 
 
 def make_any_nonexistent_directories(path):
     if not os.path.exists(path):
         os.makedirs(path)
 
 
-# this needs to be a recursive function that builds up the page template
-# every page has a --- front matter block with a layout key
-# the layout key is the name of the layout to use
-# the layout is a jinja2 template that is in _layouts
-# the layout is rendered with the page content as the content variable
-# this needs to happen recursively until there is no layout key in the front matter
 def recursively_build_page_template_with_front_matter(
-    front_matter, state, current_contents=""
+    front_matter: dict, state: dict, current_contents: str = ""
 ):
+    """
+    Recursively build a page template with front matter.
+
+    This function is called recursively until there is no layout key in the front matter.
+    """
+
     if front_matter and "layout" in front_matter.metadata:
         layout = front_matter.metadata["layout"]
         layout_path = f"{ROOT_DIR}/{LAYOUTS_BASE_DIR}/{layout}.html"
+
+        page_fm = type(
+            "Page", (object,), front_matter.metadata.get("page", front_matter.metadata)
+        )()
+
         current_contents = loads(
             all_opened_pages[layout_path].render(
-                state, content=current_contents, page=front_matter.metadata
+                page=page_fm,
+                site=state,
+                content=current_contents,
+                post=front_matter.metadata,
             )
         ).content
 
         layout_front_matter = all_parsed_pages[layout_path]
 
+        # combine current front matter so that we can access it in the layout
+        if "page" in layout_front_matter.metadata:
+            layout_front_matter["page"] = {
+                **layout_front_matter.metadata["page"],
+                **front_matter.metadata,
+            }
+        else:
+            layout_front_matter["page"] = front_matter.metadata
+
         return recursively_build_page_template_with_front_matter(
             layout_front_matter, state, current_contents.strip()
         )
 
     return current_contents
 
 
-def render_page(file):
+def render_page(file: str) -> None:
+    """
+    Render a page with the Aurora static site generator.
+    """
     try:
         contents = all_opened_pages[file]
     except:
         print(f"Error reading {file}")
         return
 
-    # print(f"Rendering {file}")
-
     page_state = state.copy()
 
     if all_parsed_pages[file]:
         slug = file.split("/")[-1].replace(".html", "")
 
         slug = slug.replace("posts/", "")
 
-        # print(all_parsed_pages[file], )
-
         page_state["page"] = all_parsed_pages[file].metadata
         page_state["post"] = all_parsed_pages[file].metadata
         if not page_state["page"].get("permalink"):
             page_state["page"]["permalink"] = slug.strip("/")
+
         page_state["page"]["generated_on"] = datetime.datetime.now()
 
-        if slug:
+        if slug[0].isdigit():
             date_slug = re.search(r"\d{4}-\d{2}-\d{2}", slug)
             if date_slug:
                 date_slug = date_slug.group(0)
                 page_state["post"]["date"] = datetime.datetime.strptime(
                     date_slug, "%Y-%m-%d"
                 )
                 page_state["post"]["full_date"] = page_state["post"]["date"].strftime(
                     "%B %d, %Y"
                 )
                 page_state["date"] = page_state["post"]["date"]
                 page_state["full_date"] = page_state["post"]["full_date"]
-                # generate description using first paragraph
                 if "description" not in page_state["post"]:
                     page_state["post"]["description"] = all_parsed_pages[
                         file
                     ].content.split("\n")[0]
             page_state["is_article"] = True
 
         if page_state.get("date"):
@@ -378,23 +390,20 @@
 
     # run hooks on page_state
     for hook, hooks in REGISTERED_HOOKS.items():
         for hook in hooks:
             page_state = hook(file, page_state, state)
 
     try:
-        if file.endswith(".md") and file.startswith("pages/posts"):
-            contents = pyromark.markdown(loads(contents).content)
-        elif file.endswith(".md"):
-            contents = pyromark.markdown(contents)
+        if file.endswith(".md"):
+            contents = pyromark.markdown(loads(all_opened_pages[file]).content)
         else:
             contents = loads(contents.render(page=page_state, site=state)).content
     except Exception as e:
         print(f"Error rendering {file}")
-        print(e)
         return
 
     rendered = recursively_build_page_template_with_front_matter(
         all_parsed_pages[file], page_state, contents
     )
 
     file = file.replace(ROOT_DIR + "/", "")
@@ -404,72 +413,81 @@
 
     if file.endswith(".md"):
         file = file[:-3] + ".html"
 
     permalink = file
 
     # if permalink is _site/templates/index.html, make it _site/index.html
-
     if file == "templates/index.html":
-        # delete index.html dir
         if os.path.exists(os.path.join(SITE_DIR, "index.html")):
             os.remove(os.path.join(SITE_DIR, "index.html"))
         with open(os.path.join(SITE_DIR, "index.html"), "w") as f:
             f.write(rendered)
 
         return
 
-    # print(f"Rendering {permalink}")
-
-    if file.startswith("templates/"):
+    if file.startswith("templates/") and any(
+        file.endswith(ext) for ext in [".html", ".md"]
+    ):
         if hasattr(page_state["page"], "permalink"):
             permalink = os.path.join(
                 page_state["page"].permalink.strip("/"), "index.html"
             )
-            print(f"Permalink: {permalink}")
         else:
             permalink = file.replace("templates/", "")
+    else:
+        permalink = file.replace("templates/", "")
 
     make_any_nonexistent_directories(os.path.dirname(os.path.join(SITE_DIR, permalink)))
 
     permalink = os.path.join(SITE_DIR, permalink)
 
     try:
         with open(permalink, "w") as f:
             f.write(rendered)
     except Exception as e:
         print(f"Error writing {permalink}")
         print(e)
 
+    state["pages"].append({"url": f"{BASE_URL}/{permalink}", "file": file})
 
-def process_date_archives():
-    # print len of all posts
-    # get all keys in all_opened_pages starting with ROOT_DIR + posts
+
+def process_date_archives() -> None:
+    """
+    Generate date archives for all posts.
+
+    For example, if there are posts on 2022-01-01 and 2022-01-02, generate:
+
+    - /2022/index.html
+    - /2022/01/index.html
+    - /2022/01/01/index.html
+    """
     posts = [
         key for key in all_opened_pages.keys() if key.startswith(ROOT_DIR + "/posts")
     ]
 
-    # get all dates
     dates = set()
     years = {}
 
     for post in posts:
         if not hasattr(all_parsed_pages[post], "metadata"):
             continue
 
-        if all_parsed_pages[post].metadata.get("date"):
-            date = all_parsed_pages[post].metadata["date"]
-            dates.add(date)
-            if date.year not in years:
-                years[date.year] = {}
-            if date.month not in years[date.year]:
-                years[date.year][date.month] = {}
-            if date.day not in years[date.year][date.month]:
-                years[date.year][date.month][date.day] = []
-            years[date.year][date.month][date.day].append(post)
+        if not all_parsed_pages[post].metadata.get("date"):
+            continue
+
+        date = all_parsed_pages[post].metadata["date"]
+        dates.add(date)
+        if date.year not in years:
+            years[date.year] = {}
+        if date.month not in years[date.year]:
+            years[date.year][date.month] = {}
+        if date.day not in years[date.year][date.month]:
+            years[date.year][date.month][date.day] = []
+        years[date.year][date.month][date.day].append(post)
 
     for year in years:
         make_any_nonexistent_directories(os.path.join(SITE_DIR, str(year)))
 
         for month in years[year]:
             make_any_nonexistent_directories(
                 os.path.join(SITE_DIR, str(year), str(month))
@@ -477,49 +495,55 @@
 
             for day in years[year][month]:
                 make_any_nonexistent_directories(
                     os.path.join(SITE_DIR, str(year), str(month), str(day))
                 )
 
                 date_archive_state = state.copy()
-                date_archive_state["date"] = datetime.datetime(year, month, day)
+                current_date = datetime.datetime(year, month, day)
+                date_archive_state["date"] = current_date
                 date_archive_state["posts"] = [
                     all_parsed_pages[post].metadata
                     for post in posts
-                    if hasattr(all_parsed_pages[post], "metadata")
-                    and all_parsed_pages[post].metadata.get("date")
-                    == datetime.datetime(year, month, day)
+                    if all_parsed_pages[post].metadata.get("date") == current_date
                 ]
-                # render _layouts/date_archive.html
+
                 date_archive_layout = f"{ROOT_DIR}/{LAYOUTS_BASE_DIR}/date_archive.html"
                 date_archive_contents = all_opened_pages[date_archive_layout]
+
                 rendered_page = date_archive_contents.render(
                     date_archive_state,
                     site=date_archive_state,
                     posts=date_archive_state["posts"],
                     page=date_archive_state,
                 )
 
                 rendered_page = recursively_build_page_template_with_front_matter(
                     all_parsed_pages[date_archive_layout],
                     date_archive_state,
-                    loads(rendered_page).content,
+                    rendered_page,
                 )
 
                 with open(
                     os.path.join(
                         SITE_DIR, str(year), str(month), str(day), "index.html"
                     ),
                     "w",
                 ) as f:
                     f.write(rendered_page)
 
 
 def process_category_archives():
-    # get all categories
+    """
+    Generate category archives for all posts.
+
+    For example, if you have a post with the `category` key set to `writing`, generate:
+
+    - /writing/index.html
+    """
     categories = set()
     for post in state["posts"]:
         if not post.get("categories"):
             continue
 
         for category in post["categories"]:
             categories.add(category)
@@ -541,27 +565,33 @@
             posts=category_archive_state["posts"],
             page=category_archive_state,
         )
 
         rendered_page = recursively_build_page_template_with_front_matter(
             all_parsed_pages[category_archive_layout],
             category_archive_state,
-            loads(rendered_page).content,
+            rendered_page,
         )
 
         with open(os.path.join(SITE_DIR, slugify(category), "index.html"), "w") as f:
             f.write(rendered_page)
 
 
-def main(deps=None, watch=False):
-    # remove _layouts from all_dependencies
+def main(deps: list = None, watch: bool = False) -> None:
+    """
+    The Aurora runtime.
+
+    Aurora can be run in two ways:
+
+    - `aurora build` to build the site once, and;
+    - `aurora serve` to watch for changes in the `pages` directory and rebuild the site in real time.
+    """
+
     dependencies = list(toposort_flatten(all_dependencies)) if not deps else deps
 
-    # filter if starts with pages/_
-    # because templates do not need to be directly rendered
     dependencies = [
         dependency
         for dependency in dependencies
         if not dependency.startswith("pages/_")
     ]
 
     for file in IncrementalBar("Building website...").iter(dependencies):
@@ -574,29 +604,21 @@
                     render_page(os.path.join(root, file))
         else:
             render_page(file)
 
     process_date_archives()
     process_category_archives()
 
-    class Watcher(FileSystemEventHandler):
-        def on_modified(self, event):
-            print(f"Detected change in {event.src_path}. Rebuilding.")
-            file_name = event.src_path
-            file_name = file_name.replace(os.getcwd() + "/", "")
-            file_dependencies = all_dependencies[file_name]
-            file_dependencies.add(file_name)
-
-            main(deps=file_dependencies)
-
     if watch:
         observer = Observer()
         observer.schedule(Watcher(), path="pages", recursive=True)
         observer.start()
 
-        print("Watching for changes in pages directory")
+        print("Watching for changes...")
+        print("View your site at ", os.path.join(os.getcwd(), SITE_DIR, "index.html"))
+        print("Press Ctrl+C to stop.")
 
         try:
             while True:
                 time.sleep(1)
         except KeyboardInterrupt:
             observer.stop()
```

### Comparing `aurora_ssg-0.0.1/aurora_ssg.egg-info/PKG-INFO` & `aurora_ssg-0.0.2/aurora_ssg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aurora-ssg
-Version: 0.0.1
-Summary: A fast static site generator for Python.
+Version: 0.0.2
+Summary: A fast static site generator implemented in Python.
 Home-page: https://github.com/capjamesg/aurora
 Author: capjamesg
 Author-email: readers@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,14 +14,15 @@
 Requires-Dist: jinja2
 Requires-Dist: watchdog
 Requires-Dist: toposort
 Requires-Dist: pyromark
 Requires-Dist: python-frontmatter
 Requires-Dist: requests
 Requires-Dist: progress
+Requires-Dist: click
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black==22.3.0; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
@@ -38,14 +39,18 @@
 [![python-version](https://img.shields.io/pypi/pyversions/aurora-ssg)](https://badge.fury.io/py/aurora-ssg)
 </div>
 
 # Aurora
 
 Aurora is a static site generator implemented in Python.
 
+## Demo
+
+https://github.com/capjamesg/aurora/assets/37276661/59e4f3e6-f470-46bd-8812-0b475be40e88
+
 ## Get Started
 
 ### Install Aurora
 
 First, install Aurora:
 
 ```bash
@@ -198,12 +203,22 @@
 REGISTERED_HOOKS = {
     "hook_file_name": ["hook1", "hook2", "hook3"],
 }
 ```
 
 ## Performance
 
-TODO
+In a test on a website with 1763 files, Aurora built the website in `0:00:04.23`.
+
+The files were a combination of blog posts, static pages, and programmatic archives for blog posts (date pages, category pages).
+
+## Users
+
+The following sites are built with Aurora:
+
+- [James' Coffee Blog](https://jamesg.blog) (1,500+ pages)
+
+Have you made a website with Aurora? File a PR and add it to the list!
 
 ## License
 
 This project is licensed under an [MIT license](LICENSE).
```

### Comparing `aurora_ssg-0.0.1/setup.py` & `aurora_ssg-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,28 @@
     long_description = fh.read()
 
 setuptools.setup(
     name="aurora-ssg",
     version=version,
     author="capjamesg",
     author_email="readers@jamesg.blog",
-    description="A fast static site generator for Python.",
+    description="A fast static site generator implemented in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/capjamesg/aurora",
     install_requires=[
         "jinja2",
         "watchdog",
         "toposort",
         "pyromark",
         "python-frontmatter",
         "requests",
         "progress",
+        "click",
     ],
-    # allow models.csv in package
     include_package_data=True,
     package_data={"": ["models.csv"]},
     packages=find_packages(exclude=("tests",)),
     entry_points={
         "console_scripts": [
             "aurora = aurora.cli:main",
         ],
```

