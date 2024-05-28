# Comparing `tmp/dlt_init_openapi-0.1.0a2.tar.gz` & `tmp/dlt_init_openapi-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt_init_openapi-0.1.0a2.tar", max compression
+gzip compressed data, was "dlt_init_openapi-0.1.0a3.tar", max compression
```

## Comparing `dlt_init_openapi-0.1.0a2.tar` & `dlt_init_openapi-0.1.0a3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     2109 2024-05-26 19:54:27.713247 dlt_init_openapi-0.1.0a2/CHANGELOG.md
--rw-r--r--   0        0        0     1111 2024-05-10 11:31:42.794290 dlt_init_openapi-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     9996 2024-05-26 19:52:35.277719 dlt_init_openapi-0.1.0a2/README.md
--rw-r--r--   0        0        0     4763 2024-05-24 15:05:07.637826 dlt_init_openapi-0.1.0a2/dlt_init_openapi/__init__.py
--rw-r--r--   0        0        0       28 2024-05-23 04:47:13.947847 dlt_init_openapi-0.1.0a2/dlt_init_openapi/__main__.py
--rw-r--r--   0        0        0     4985 2024-05-26 18:27:39.544319 dlt_init_openapi-0.1.0a2/dlt_init_openapi/cli/__init__.py
--rw-r--r--   0        0        0     1197 2024-05-24 15:05:07.638151 dlt_init_openapi-0.1.0a2/dlt_init_openapi/cli/cli_endpoint_selection.py
--rw-r--r--   0        0        0     3611 2024-05-26 19:52:35.278119 dlt_init_openapi-0.1.0a2/dlt_init_openapi/config.py
--rw-r--r--   0        0        0       29 2024-05-23 04:47:13.948156 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/__init__.py
--rw-r--r--   0        0        0      664 2024-05-23 04:47:13.948219 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/base_detector.py
--rw-r--r--   0        0        0    22415 2024-05-24 15:05:07.638768 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/__init__.py
--rw-r--r--   0        0        0     1065 2024-05-24 15:05:07.639104 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/const.py
--rw-r--r--   0        0        0     1774 2024-05-23 04:47:13.948547 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/primary_key.py
--rw-r--r--   0        0        0      686 2024-05-23 04:47:13.948609 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/utils.py
--rw-r--r--   0        0        0     1573 2024-05-23 04:47:13.948668 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/warnings.py
--rw-r--r--   0        0        0     1903 2024-05-24 15:05:07.639228 dlt_init_openapi-0.1.0a2/dlt_init_openapi/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-23 04:47:13.948783 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/__init__.py
--rw-r--r--   0        0        0       57 2024-05-23 04:47:13.948849 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/config.py
--rw-r--r--   0        0        0       44 2024-05-23 04:47:13.948951 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/const.py
--rw-r--r--   0        0        0     2839 2024-05-23 04:47:13.949026 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/context.py
--rw-r--r--   0        0        0    10764 2024-05-26 19:52:35.278592 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/endpoints.py
--rw-r--r--   0        0        0     1376 2024-05-23 04:47:13.949244 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/errors.py
--rw-r--r--   0        0        0      704 2024-05-23 04:47:13.949307 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/info.py
--rw-r--r--   0        0        0    12896 2024-05-23 04:47:13.949454 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/models.py
--rw-r--r--   0        0        0     4112 2024-05-24 15:05:07.639975 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/openapi_parser.py
--rw-r--r--   0        0        0      670 2024-05-23 04:47:13.949606 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/pagination.py
--rw-r--r--   0        0        0     2766 2024-05-23 04:47:13.949686 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/parameters.py
--rw-r--r--   0        0        0        0 2024-05-23 04:47:13.949744 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/properties/__init__.py
--rw-r--r--   0        0        0     2365 2024-05-23 04:47:13.949854 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/properties/converter.py
--rw-r--r--   0        0        0      562 2024-05-23 07:11:02.288112 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/security.py
--rw-r--r--   0        0        0     2360 2024-05-23 04:47:13.950009 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/types.py
--rw-r--r--   0        0        0       26 2024-05-23 04:47:13.950067 dlt_init_openapi-0.1.0a2/dlt_init_openapi/py.typed
--rw-r--r--   0        0        0        0 2024-05-23 04:47:13.950094 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/__init__.py
--rw-r--r--   0        0        0      516 2024-05-23 04:47:13.950163 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/base_renderer.py
--rw-r--r--   0        0        0     6155 2024-05-24 15:05:07.640152 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/__init__.py
--rw-r--r--   0        0        0      932 2024-05-24 15:05:07.640271 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/README.md.j2
--rw-r--r--   0        0        0      519 2024-05-23 05:53:21.142183 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2
--rw-r--r--   0        0        0      279 2024-05-23 07:43:30.108700 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/dlt_secrets.toml.j2
--rw-r--r--   0        0        0       62 2024-05-23 07:43:30.108831 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/gitignore.j2
--rw-r--r--   0        0        0      479 2024-05-23 05:53:21.142413 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/pipeline.py.j2
--rw-r--r--   0        0        0       11 2024-05-23 04:47:13.950645 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/requirements.txt.j2
--rw-r--r--   0        0        0     4301 2024-05-26 19:52:35.278941 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/source.py.j2
--rw-r--r--   0        0        0      199 2024-05-23 04:47:13.950759 dlt_init_openapi-0.1.0a2/dlt_init_openapi/typing.py
--rw-r--r--   0        0        0        0 2024-05-23 04:47:13.950790 dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/__init__.py
--rw-r--r--   0        0        0     4137 2024-05-23 05:53:21.142935 dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/misc.py
--rw-r--r--   0        0        0     3851 2024-05-23 04:47:13.950988 dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/paths.py
--rw-r--r--   0        0        0     1167 2024-05-23 07:11:02.288801 dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/update_rest_api.py
--rw-r--r--   0        0        0     2539 2024-05-26 19:53:13.689616 dlt_init_openapi-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0    11587 1970-01-01 00:00:00.000000 dlt_init_openapi-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     2217 2024-05-27 16:07:45.217083 dlt_init_openapi-0.1.0a3/CHANGELOG.md
+-rw-r--r--   0        0        0     1111 2024-05-21 08:48:46.382581 dlt_init_openapi-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0    10033 2024-05-27 16:06:59.069647 dlt_init_openapi-0.1.0a3/README.md
+-rw-r--r--   0        0        0     4763 2024-05-23 15:54:53.848070 dlt_init_openapi-0.1.0a3/dlt_init_openapi/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-21 10:48:17.311493 dlt_init_openapi-0.1.0a3/dlt_init_openapi/__main__.py
+-rw-r--r--   0        0        0     4985 2024-05-27 13:40:11.345582 dlt_init_openapi-0.1.0a3/dlt_init_openapi/cli/__init__.py
+-rw-r--r--   0        0        0     1197 2024-05-23 15:54:53.849095 dlt_init_openapi-0.1.0a3/dlt_init_openapi/cli/cli_endpoint_selection.py
+-rw-r--r--   0        0        0     3611 2024-05-27 13:40:11.345952 dlt_init_openapi-0.1.0a3/dlt_init_openapi/config.py
+-rw-r--r--   0        0        0       29 2024-05-21 10:48:17.312788 dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/__init__.py
+-rw-r--r--   0        0        0      664 2024-05-21 10:48:17.312992 dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/base_detector.py
+-rw-r--r--   0        0        0    22415 2024-05-23 15:54:53.850824 dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/__init__.py
+-rw-r--r--   0        0        0     1065 2024-05-23 15:54:53.851684 dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/const.py
+-rw-r--r--   0        0        0     1774 2024-05-21 10:48:17.313932 dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/primary_key.py
+-rw-r--r--   0        0        0      686 2024-05-21 10:48:17.314162 dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/utils.py
+-rw-r--r--   0        0        0     1573 2024-05-21 10:48:17.314794 dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/warnings.py
+-rw-r--r--   0        0        0     1903 2024-05-23 15:54:53.852261 dlt_init_openapi-0.1.0a3/dlt_init_openapi/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:48:17.315259 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-21 10:48:17.315501 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/config.py
+-rw-r--r--   0        0        0       44 2024-05-21 10:48:17.315659 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/const.py
+-rw-r--r--   0        0        0     2839 2024-05-21 10:48:17.315866 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/context.py
+-rw-r--r--   0        0        0    10742 2024-05-27 16:06:59.070196 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/endpoints.py
+-rw-r--r--   0        0        0     1376 2024-05-21 10:48:17.316256 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/errors.py
+-rw-r--r--   0        0        0      704 2024-05-21 10:48:17.316445 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/info.py
+-rw-r--r--   0        0        0    12896 2024-05-21 10:48:17.316840 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/models.py
+-rw-r--r--   0        0        0     4112 2024-05-23 15:54:53.853568 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/openapi_parser.py
+-rw-r--r--   0        0        0      670 2024-05-21 10:48:17.317716 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/pagination.py
+-rw-r--r--   0        0        0     2766 2024-05-21 10:48:17.318056 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/parameters.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:48:17.318258 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/properties/__init__.py
+-rw-r--r--   0        0        0     2365 2024-05-21 10:48:17.318463 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/properties/converter.py
+-rw-r--r--   0        0        0      562 2024-05-23 09:23:18.941182 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/security.py
+-rw-r--r--   0        0        0     2360 2024-05-21 10:48:17.318971 dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/types.py
+-rw-r--r--   0        0        0       26 2024-05-21 10:48:17.319147 dlt_init_openapi-0.1.0a3/dlt_init_openapi/py.typed
+-rw-r--r--   0        0        0        0 2024-05-21 10:48:17.319244 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-21 10:48:17.319570 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/base_renderer.py
+-rw-r--r--   0        0        0     6155 2024-05-23 15:54:53.854060 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/__init__.py
+-rw-r--r--   0        0        0      932 2024-05-23 15:54:53.854540 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/README.md.j2
+-rw-r--r--   0        0        0      519 2024-05-22 10:51:36.172746 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2
+-rw-r--r--   0        0        0      279 2024-05-23 09:23:18.942359 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/dlt_secrets.toml.j2
+-rw-r--r--   0        0        0       62 2024-05-23 09:23:18.942598 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/gitignore.j2
+-rw-r--r--   0        0        0      479 2024-05-22 10:51:36.173291 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/pipeline.py.j2
+-rw-r--r--   0        0        0       11 2024-05-21 10:48:17.321138 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/requirements.txt.j2
+-rw-r--r--   0        0        0     4301 2024-05-27 13:40:11.347048 dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/source.py.j2
+-rw-r--r--   0        0        0      199 2024-05-21 10:48:17.321712 dlt_init_openapi-0.1.0a3/dlt_init_openapi/typing.py
+-rw-r--r--   0        0        0        0 2024-05-21 10:48:17.321833 dlt_init_openapi-0.1.0a3/dlt_init_openapi/utils/__init__.py
+-rw-r--r--   0        0        0     4137 2024-05-22 10:51:36.173648 dlt_init_openapi-0.1.0a3/dlt_init_openapi/utils/misc.py
+-rw-r--r--   0        0        0     3851 2024-05-21 10:48:17.322279 dlt_init_openapi-0.1.0a3/dlt_init_openapi/utils/paths.py
+-rw-r--r--   0        0        0     1167 2024-05-23 09:23:18.943730 dlt_init_openapi-0.1.0a3/dlt_init_openapi/utils/update_rest_api.py
+-rw-r--r--   0        0        0     2539 2024-05-27 16:07:17.110345 dlt_init_openapi-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0    11624 1970-01-01 00:00:00.000000 dlt_init_openapi-0.1.0a3/PKG-INFO
```

### Comparing `dlt_init_openapi-0.1.0a2/CHANGELOG.md` & `dlt_init_openapi-0.1.0a3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 [Go to GitHub Releases](https://github.com/dlt-hub/dlt-init-openapi/releases)
 
+0.1.0a3 - Getting ready for the first release
+* Remove left over print statement
+* Small udpates to readme
+
 0.1.0a2 - Getting ready for the first release
 * Updated Readme, reordered content blocks and made example nicer
 * Better rendering of required and non-required query args
 * Do not ask wether output directory should be written when in non-interactive mode
 
 0.1.0a1 - Getting ready for the first release
 * Remove init command from CLI. The same functionality is now the default command, see updated README file.
```

### Comparing `dlt_init_openapi-0.1.0a2/LICENSE` & `dlt_init_openapi-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/README.md` & `dlt_init_openapi-0.1.0a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,50 +22,56 @@
 
 ## A quick example
 
 You will need Python 3.9 or higher installed, as well as pip. You can run `pip install dlt-init-openapi` to install the current version.
 
 We will create a simple example pipeline from a [PokeAPI spec](https://pokeapi.co/) in our repo. You can point to any other OpenAPI Spec instead if you prefer.
 
-```console
+```sh
 # 1.a. Run the generator with a URL:
 $ dlt-init-openapi pokemon --url https://raw.githubusercontent.com/dlt-hub/dlt-init-openapi/devel/tests/cases/e2e_specs/pokeapi.yml --global-limit 2
 
 # 1.b. If you have a local file, you can use the --path flag:
 $ dlt-init-openapi pokemon --path ./my_specs/pokeapi.yml
 
 # 2. You can now pick both of the endpoints from the popup.
 
-# 3. After selecting your Pokemon endpoints and hitting Enter, your pipeline will be rendered.
+# 3. After selecting your Pokemon endpoints and hitting Enter, 
+#    your pipeline will be rendered.
 
-# 4. If you have any kind of authentication on your pipeline (this example does not), open the `.dlt/secrets.toml` and provide the credentials. You can find further settings in the `.dlt/config.toml`.
+# 4. If you have any kind of authentication on your pipeline (this example does not), 
+#    open the `.dlt/secrets.toml` and provide the credentials. You can find further 
+#    settings in the `.dlt/config.toml`.
 
 # 5. Go to the created pipeline folder and run your pipeline.
 $ cd pokemon-pipeline
 $ PROGRESS=enlighten python pipeline.py # we use enlighten for a nice progress bar :)
 
 # 6. Print the pipeline info to the console to see what got loaded.
 $ dlt pipeline pokemon_pipeline info
 
-# 7. You can now also install Streamlit to see a preview of the data; you should have loaded 40 Pokemons and their details.
+# 7. You can now also install Streamlit to see a preview of the data; you should 
+#    have loaded 40 Pokemons and their details.
 $ pip install pandas streamlit
 $ dlt pipeline pokemon_pipeline show
 
-# 8. You can go to our docs at https://dlthub.com/docs to learn how to modify the generated pipeline to load to many destinations, place schema contracts on your pipeline, and many other things.
-
-# NOTE: We used the `--global-limit 2` CLI flag to limit the requests to the PokeAPI for this example. This way, the Pokemon collection endpoint only gets queried twice, resulting in 2 x 20 Pokemon
-
- details being rendered.
+# 8. You can go to our docs at https://dlthub.com/docs to learn how to modify 
+#    the generated pipeline to load to many destinations, place schema contracts 
+#    on your pipeline, and many other things.
+
+# NOTE: We used the `--global-limit 2` CLI flag to limit the requests to the PokeAPI 
+#       for this example. This way, the Pokemon collection endpoint only gets queried 
+#       twice, resulting in 2 x 20 Pokemon details being rendered.
 ```
 
 ## What will be created?
 
 When you run the `init` command above, the following files will be generated:
 
-```
+```text
 pokemon_pipeline/
 ├── .dlt/
 │   ├── config.toml     # dlt config, learn more at dlthub.com/docs
 │   └── secrets.toml    # your secrets, only needed for APIs with auth
 ├── pokemon/
 │   └── __init__.py     # your rest_api dictionary, learn more below
 ├── rest_api/
@@ -80,15 +86,15 @@
 
 ## A closer look at your rest_api dictionary in pokemon/__init__.py
 
 This file contains the configuration dictionary for the [dlt rest_api](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) source which is the main result of running this generator. For our Pokemon example, we have used an OpenAPI 3 spec that works out of the box. The result of this dictionary depends on the quality of the spec you are using, whether the API you are querying actually adheres to this spec, and whether our heuristics manage to find the right values. You can edit this file to adapt the behavior of the dlt rest_api accordingly. Please read our [dlt rest_api](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) docs to learn how to do this and play with our detailed [Google Colab example](https://colab.research.google.com/drive/1MRZvguOTZj1MlkEGzjiso8lQ_wr1MJRI?usp=sharing#scrollTo=LHGxzf1Ev_yr).
 
 The generated dictionary will look something like this:
 
-```python
+```py
 {
     "client": {
         "base_url": base_url,
         # -> the detected common paginator
         "paginator": {
             ...
         },
@@ -130,15 +136,15 @@
         },
     ],
 }
 ```
 
 ## CLI command
 
-```console
+```sh
 $ dlt-init-openapi <source_name> [OPTIONS]
 # example:
 $ dlt-init-openapi pokemon --path ./path/to/my_spec.yml --no-interactive --output-path ./my_pipeline
 ```
 
 **Options**:
 
@@ -166,15 +172,15 @@
 ```yaml
 # config.yml
 package_name: "other_package_name"
 ```
 
 And use it with the config argument:
 
-```console
+```sh
 $ dlt-init-openapi pokemon --url ... --config config.yml
 ```
 
 ## Telemetry
 We track your usage of this tool similar to how we track other commands in the dlt core library. Read more about this and how to disable it here: https://dlthub.com/docs/reference/telemetry.
 
 ## Prior work
```

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/__init__.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/cli/__init__.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/cli/cli_endpoint_selection.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/cli/cli_endpoint_selection.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/config.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/config.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/base_detector.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/base_detector.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/__init__.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/const.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/const.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/primary_key.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/primary_key.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/utils.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/utils.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/warnings.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/detector/default/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/exceptions.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/context.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/context.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/endpoints.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         params = get_path_var_names(self.path)
         transformer_param = self.transformer.path_parameter_name if self.transformer else None
         return [p for p in params if p != transformer_param]
 
     @property
     def unresolvable_query_params(self) -> List[Parameter]:
         """returns a list of required query param names with params that are used by the paginator excluded"""
-        print("HERE")
         paginator_params = self.detected_pagination.param_names if self.detected_pagination else []
         query_params: List[Parameter] = []
         for param in self.list_all_parameters:
             if param.name not in paginator_params and param.location == "query":
                 query_params.append(param)
         return query_params
```

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/errors.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/errors.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/info.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/info.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/models.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/models.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/openapi_parser.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/openapi_parser.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/pagination.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/pagination.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/parameters.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/parameters.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/properties/converter.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/properties/converter.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/security.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/security.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/types.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/parser/types.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/base_renderer.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/base_renderer.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/__init__.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/README.md.j2` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/source.py.j2` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/renderer/default/templates/source.py.j2`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/misc.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/paths.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/utils/paths.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/update_rest_api.py` & `dlt_init_openapi-0.1.0a3/dlt_init_openapi/utils/update_rest_api.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a2/pyproject.toml` & `dlt_init_openapi-0.1.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt-init-openapi"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "Generate dlt Python clients from OpenAPI"
 homepage = "https://dlthub.com"
 repository = "https://github.com/dlt-hub/dlt-init-openapi"
 license = "MIT"
 keywords=["OpenAPI", "Client", "Generator"]
 authors = ["David Scharf <david@dlthub.com>"]
 classifiers = [
```

### Comparing `dlt_init_openapi-0.1.0a2/PKG-INFO` & `dlt_init_openapi-0.1.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt-init-openapi
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Generate dlt Python clients from OpenAPI
 Home-page: https://dlthub.com
 License: MIT
 Keywords: OpenAPI,Client,Generator
 Author: David Scharf
 Author-email: david@dlthub.com
 Requires-Python: >=3.9,<3.13
@@ -62,50 +62,56 @@
 
 ## A quick example
 
 You will need Python 3.9 or higher installed, as well as pip. You can run `pip install dlt-init-openapi` to install the current version.
 
 We will create a simple example pipeline from a [PokeAPI spec](https://pokeapi.co/) in our repo. You can point to any other OpenAPI Spec instead if you prefer.
 
-```console
+```sh
 # 1.a. Run the generator with a URL:
 $ dlt-init-openapi pokemon --url https://raw.githubusercontent.com/dlt-hub/dlt-init-openapi/devel/tests/cases/e2e_specs/pokeapi.yml --global-limit 2
 
 # 1.b. If you have a local file, you can use the --path flag:
 $ dlt-init-openapi pokemon --path ./my_specs/pokeapi.yml
 
 # 2. You can now pick both of the endpoints from the popup.
 
-# 3. After selecting your Pokemon endpoints and hitting Enter, your pipeline will be rendered.
+# 3. After selecting your Pokemon endpoints and hitting Enter, 
+#    your pipeline will be rendered.
 
-# 4. If you have any kind of authentication on your pipeline (this example does not), open the `.dlt/secrets.toml` and provide the credentials. You can find further settings in the `.dlt/config.toml`.
+# 4. If you have any kind of authentication on your pipeline (this example does not), 
+#    open the `.dlt/secrets.toml` and provide the credentials. You can find further 
+#    settings in the `.dlt/config.toml`.
 
 # 5. Go to the created pipeline folder and run your pipeline.
 $ cd pokemon-pipeline
 $ PROGRESS=enlighten python pipeline.py # we use enlighten for a nice progress bar :)
 
 # 6. Print the pipeline info to the console to see what got loaded.
 $ dlt pipeline pokemon_pipeline info
 
-# 7. You can now also install Streamlit to see a preview of the data; you should have loaded 40 Pokemons and their details.
+# 7. You can now also install Streamlit to see a preview of the data; you should 
+#    have loaded 40 Pokemons and their details.
 $ pip install pandas streamlit
 $ dlt pipeline pokemon_pipeline show
 
-# 8. You can go to our docs at https://dlthub.com/docs to learn how to modify the generated pipeline to load to many destinations, place schema contracts on your pipeline, and many other things.
-
-# NOTE: We used the `--global-limit 2` CLI flag to limit the requests to the PokeAPI for this example. This way, the Pokemon collection endpoint only gets queried twice, resulting in 2 x 20 Pokemon
-
- details being rendered.
+# 8. You can go to our docs at https://dlthub.com/docs to learn how to modify 
+#    the generated pipeline to load to many destinations, place schema contracts 
+#    on your pipeline, and many other things.
+
+# NOTE: We used the `--global-limit 2` CLI flag to limit the requests to the PokeAPI 
+#       for this example. This way, the Pokemon collection endpoint only gets queried 
+#       twice, resulting in 2 x 20 Pokemon details being rendered.
 ```
 
 ## What will be created?
 
 When you run the `init` command above, the following files will be generated:
 
-```
+```text
 pokemon_pipeline/
 ├── .dlt/
 │   ├── config.toml     # dlt config, learn more at dlthub.com/docs
 │   └── secrets.toml    # your secrets, only needed for APIs with auth
 ├── pokemon/
 │   └── __init__.py     # your rest_api dictionary, learn more below
 ├── rest_api/
@@ -120,15 +126,15 @@
 
 ## A closer look at your rest_api dictionary in pokemon/__init__.py
 
 This file contains the configuration dictionary for the [dlt rest_api](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) source which is the main result of running this generator. For our Pokemon example, we have used an OpenAPI 3 spec that works out of the box. The result of this dictionary depends on the quality of the spec you are using, whether the API you are querying actually adheres to this spec, and whether our heuristics manage to find the right values. You can edit this file to adapt the behavior of the dlt rest_api accordingly. Please read our [dlt rest_api](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) docs to learn how to do this and play with our detailed [Google Colab example](https://colab.research.google.com/drive/1MRZvguOTZj1MlkEGzjiso8lQ_wr1MJRI?usp=sharing#scrollTo=LHGxzf1Ev_yr).
 
 The generated dictionary will look something like this:
 
-```python
+```py
 {
     "client": {
         "base_url": base_url,
         # -> the detected common paginator
         "paginator": {
             ...
         },
@@ -170,15 +176,15 @@
         },
     ],
 }
 ```
 
 ## CLI command
 
-```console
+```sh
 $ dlt-init-openapi <source_name> [OPTIONS]
 # example:
 $ dlt-init-openapi pokemon --path ./path/to/my_spec.yml --no-interactive --output-path ./my_pipeline
 ```
 
 **Options**:
 
@@ -206,15 +212,15 @@
 ```yaml
 # config.yml
 package_name: "other_package_name"
 ```
 
 And use it with the config argument:
 
-```console
+```sh
 $ dlt-init-openapi pokemon --url ... --config config.yml
 ```
 
 ## Telemetry
 We track your usage of this tool similar to how we track other commands in the dlt core library. Read more about this and how to disable it here: https://dlthub.com/docs/reference/telemetry.
 
 ## Prior work
```

