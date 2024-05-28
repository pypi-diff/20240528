# Comparing `tmp/poetry_dockerize_plugin-1.0.1.tar.gz` & `tmp/poetry_dockerize_plugin-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_dockerize_plugin-1.0.1.tar", max compression
+gzip compressed data, was "poetry_dockerize_plugin-1.1.0.tar", max compression
```

## Comparing `poetry_dockerize_plugin-1.0.1.tar` & `poetry_dockerize_plugin-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-05-15 09:49:08.898501 poetry_dockerize_plugin-1.0.1/LICENSE
--rw-r--r--   0        0        0     4736 2024-05-15 09:49:08.898501 poetry_dockerize_plugin-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-15 09:49:08.898501 poetry_dockerize_plugin-1.0.1/poetry_dockerize_plugin/__init__.py
--rw-r--r--   0        0        0    13501 2024-05-15 09:49:08.898501 poetry_dockerize_plugin-1.0.1/poetry_dockerize_plugin/builder.py
--rw-r--r--   0        0        0     1239 2024-05-15 09:49:08.898501 poetry_dockerize_plugin-1.0.1/poetry_dockerize_plugin/plugin.py
--rw-r--r--   0        0        0     1997 2024-05-15 09:49:08.898501 poetry_dockerize_plugin-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6565 1970-01-01 00:00:00.000000 poetry_dockerize_plugin-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-28 15:35:37.425372 poetry_dockerize_plugin-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4857 2024-05-28 15:35:37.425372 poetry_dockerize_plugin-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 15:35:37.425372 poetry_dockerize_plugin-1.1.0/poetry_dockerize_plugin/__init__.py
+-rw-r--r--   0        0        0    13564 2024-05-28 15:35:37.425372 poetry_dockerize_plugin-1.1.0/poetry_dockerize_plugin/builder.py
+-rw-r--r--   0        0        0     1239 2024-05-28 15:35:37.425372 poetry_dockerize_plugin-1.1.0/poetry_dockerize_plugin/plugin.py
+-rw-r--r--   0        0        0     2024 2024-05-28 15:35:37.425372 poetry_dockerize_plugin-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6728 1970-01-01 00:00:00.000000 poetry_dockerize_plugin-1.1.0/PKG-INFO
```

### Comparing `poetry_dockerize_plugin-1.0.1/LICENSE` & `poetry_dockerize_plugin-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_dockerize_plugin-1.0.1/README.md` & `poetry_dockerize_plugin-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 * Highly configurable. You can configure the image by adding a section in the `pyproject.toml` configuration file.
 
 ## Installation
 
 In order to install the plugin you need to have installed a poetry version `>=1.2.0` and type:
 
 ```bash
-poetry self add poetry-dockerize-plugin
+poetry self add poetry-dockerize-plugin@latest
 ```
 
 ## Quickstart
 
 No configuration needed! Just type:
 ```bash
 poetry dockerize
@@ -51,15 +51,15 @@
   login:
     runs-on: ubuntu-latest
     steps:
         - name: Install Poetry
           uses: snok/install-poetry@v1
 
         - name: Install poetry-dockerize-plugin
-          run: poetry self add poetry-dockerize-plugin
+          run: poetry self add poetry-dockerize-plugin@latest
 
         - name: Build and package
           run: |
             poetry install
             poetry run pytest
             poetry dockerize
 
@@ -136,16 +136,18 @@
 
 ```bash
 poetry dockerize --debug
 ```
 
 ## Generate Dockerfile
 
-To store the generated Dockerfile, you can use the `--generate` flag.
+To only generate the Dockerfile, you can use the `--generate` flag.
 
 ```bash
 poetry dockerize --generate
 ```
 
+Then you can store the Dockerfile on the repository and use it as a template and customize it as you need. 
+
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,54 +1,56 @@
 # Poetry Dockerize Plugin
                         _[_P_y_P_I_]_[_D_o_w_n_l_o_a_d_s_][Py versions]
 Key features: * Automatically generate a docker image from your Poetry
 application. * Highly configurable. You can configure the image by adding a
 section in the `pyproject.toml` configuration file. ## Installation In order to
 install the plugin you need to have installed a poetry version `>=1.2.0` and
-type: ```bash poetry self add poetry-dockerize-plugin ``` ## Quickstart No
-configuration needed! Just type: ```bash poetry dockerize >Building image:
+type: ```bash poetry self add poetry-dockerize-plugin@latest ``` ## Quickstart
+No configuration needed! Just type: ```bash poetry dockerize >Building image:
 poetry-sample-app:latest >Successfully built image: poetry-sample-app:latest
 docker run --rm -it poetry-sample-app:latest >hello world! ``` ### Usage in
 GitHub Actions You just need to run the quickstart command in your GitHub
 Actions workflow: ```yaml name: Build and publish latest on: push: branches:
 main jobs: login: runs-on: ubuntu-latest steps: - name: Install Poetry uses:
 snok/install-poetry@v1 - name: Install poetry-dockerize-plugin run: poetry self
-add poetry-dockerize-plugin - name: Build and package run: | poetry install
-poetry run pytest poetry dockerize - name: Login to Docker Hub uses: docker/
-login-action@v3 with: username: ${{ secrets.DOCKERHUB_USERNAME }} password: ${
-{ secrets.DOCKERHUB_TOKEN }} - name: Push to Docker Hub run: docker push my-
-app:latest ``` ## Configuration To customize some options, you can add a `
-[tool.dockerize]` section in your `pyproject.toml` file. For example to change
-the image name: ```toml [tool.dockerize] name = "myself/myproject-app" ``` ##
-Configuration API Reference This examples shows a complete configuration of the
-docker image: ```toml [tool.dockerize] name = "alternative-image-name" python =
-"3.12" base-image = "python:3.12-slim" tags = ["latest-dev"] entrypoint =
-["python", "-m", "whatever"] ports = [5000] env = {"MY_APP_ENV" = "dev"} labels
-= {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-run-instructions =
-["RUN curl https://huggingface.co/transformers/"] # Only for build docker layer
-build-apt-packages = ["gcc"] extra-build-instructions = ["RUN poetry config
-http-basic.foo "] build-poetry-install-args = ["-E", "all", "--no-root"] ``` *
-`name` customizes the docker image name. * `python` python version to use. If
-not specified, will try to be extracted from `tool.poetry.dependencies.python`.
-Default is `3.11` * `base-image` customizes the base image. If not defined, the
-default base image is `python:-slim-bookworm`. * `tags` declares a list of tags
-for the image. * `entrypoint` customizes the entrypoint of the image. If not
-provided, the default entrypoint is retrieved from the `packages`
-configuration. * `ports` exposes ports * `env` declares environment variables
-inside the docker image. * `labels` append labels to the docker image. Default
-labels are added following the opencontainers specification. * `apt-packages`
-installs apt packages inside the docker image. * `extra-run-instructions` adds
-extra instructions to the docker run (after poetry install). Any modification
-to the filesystem will be kept after the poetry install. For the build step: *
-`build-apt-packages` installs apt packages inside the build docker container. *
-`extra-build-instructions` adds extra instructions to the docker build (before
-poetry install). Any modification to the filesystem will be lost after the
-poetry install. If you need to add files to the image, use the `extra-run-
-instructions`. * `build-poetry-install-args` adds additional arguments to the
-`poetry install` command in the build step. ## Command-Line options All command
-line options provided by the `poetry-dockerize-plugin` may be accessed by
-typing: ```bash poetry dockerize --help ``` ## Troubleshooting To troubleshoot
-the plugin, you can use the `--debug` flag to get more information about the
-execution. ```bash poetry dockerize --debug ``` ## Generate Dockerfile To store
-the generated Dockerfile, you can use the `--generate` flag. ```bash poetry
-dockerize --generate ``` ## License This project is licensed under the terms of
-the MIT license.
+add poetry-dockerize-plugin@latest - name: Build and package run: | poetry
+install poetry run pytest poetry dockerize - name: Login to Docker Hub uses:
+docker/login-action@v3 with: username: ${{ secrets.DOCKERHUB_USERNAME }}
+password: ${{ secrets.DOCKERHUB_TOKEN }} - name: Push to Docker Hub run: docker
+push my-app:latest ``` ## Configuration To customize some options, you can add
+a `[tool.dockerize]` section in your `pyproject.toml` file. For example to
+change the image name: ```toml [tool.dockerize] name = "myself/myproject-app"
+``` ## Configuration API Reference This examples shows a complete configuration
+of the docker image: ```toml [tool.dockerize] name = "alternative-image-name"
+python = "3.12" base-image = "python:3.12-slim" tags = ["latest-dev"]
+entrypoint = ["python", "-m", "whatever"] ports = [5000] env = {"MY_APP_ENV" =
+"dev"} labels = {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-run-
+instructions = ["RUN curl https://huggingface.co/transformers/"] # Only for
+build docker layer build-apt-packages = ["gcc"] extra-build-instructions =
+["RUN poetry config http-basic.foo "] build-poetry-install-args = ["-E", "all",
+"--no-root"] ``` * `name` customizes the docker image name. * `python` python
+version to use. If not specified, will try to be extracted from
+`tool.poetry.dependencies.python`. Default is `3.11` * `base-image` customizes
+the base image. If not defined, the default base image is `python:-slim-
+bookworm`. * `tags` declares a list of tags for the image. * `entrypoint`
+customizes the entrypoint of the image. If not provided, the default entrypoint
+is retrieved from the `packages` configuration. * `ports` exposes ports * `env`
+declares environment variables inside the docker image. * `labels` append
+labels to the docker image. Default labels are added following the
+opencontainers specification. * `apt-packages` installs apt packages inside the
+docker image. * `extra-run-instructions` adds extra instructions to the docker
+run (after poetry install). Any modification to the filesystem will be kept
+after the poetry install. For the build step: * `build-apt-packages` installs
+apt packages inside the build docker container. * `extra-build-instructions`
+adds extra instructions to the docker build (before poetry install). Any
+modification to the filesystem will be lost after the poetry install. If you
+need to add files to the image, use the `extra-run-instructions`. * `build-
+poetry-install-args` adds additional arguments to the `poetry install` command
+in the build step. ## Command-Line options All command line options provided by
+the `poetry-dockerize-plugin` may be accessed by typing: ```bash poetry
+dockerize --help ``` ## Troubleshooting To troubleshoot the plugin, you can use
+the `--debug` flag to get more information about the execution. ```bash poetry
+dockerize --debug ``` ## Generate Dockerfile To only generate the Dockerfile,
+you can use the `--generate` flag. ```bash poetry dockerize --generate ``` Then
+you can store the Dockerfile on the repository and use it as a template and
+customize it as you need. ## License This project is licensed under the terms
+of the MIT license.
```

### Comparing `poetry_dockerize_plugin-1.0.1/poetry_dockerize_plugin/builder.py` & `poetry_dockerize_plugin-1.1.0/poetry_dockerize_plugin/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,15 @@
             config.entrypoint = ["python", "-m", name]
 
     if not config.entrypoint:
         raise ValueError('No package found in pyproject.toml and no entrypoint specified in dockerize section')
 
     config.runtime_apt_packages = dockerize_section.apt_packages or []
     config.build_apt_packages = dockerize_section.build_apt_packages or []
+    config.build_apt_packages.append("gcc")
     config.build_poetry_install_args = dockerize_section.build_poetry_install_args or []
     if 'packages' in tool_poetry:
         config.app_packages += [package["include"] for package in tool_poetry['packages']]
 
     if "dependencies" in tool_poetry:
         for dep in tool_poetry["dependencies"]:
             if isinstance(tool_poetry["dependencies"][dep], dict):
@@ -268,14 +269,15 @@
         real_context_path = os.path.realpath(root_path)
         content = generate_docker_file_content(config, real_context_path)
         if generate:
             generate_dockerfile_path = os.path.join(real_context_path, "Dockerfile")
             with open(generate_dockerfile_path, "w") as f:
                 f.write(content)
             print(f"Stored Dockerfile to {generate_dockerfile_path} 📄")
+            return
         tmp.write(content.encode("utf-8"))
         tmp.flush()
         if verbose:
             print("Building with dockerfile content: \n===[Dockerfile]==\n" + content + "\n===[/Dockerfile]==\n")
 
         dockerignore = os.path.join(real_context_path, ".dockerignore")
         dockerignore_created = write_dockerignore_if_needed(dockerignore)
```

### Comparing `poetry_dockerize_plugin-1.0.1/poetry_dockerize_plugin/plugin.py` & `poetry_dockerize_plugin-1.1.0/poetry_dockerize_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_dockerize_plugin-1.0.1/pyproject.toml` & `poetry_dockerize_plugin-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-dockerize-plugin"
-version = "1.0.1"
+version = "1.1.0"
 description = "Poetry application to Docker, automatically."
 authors = ["Nicolò Boschi <boschi1997@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["poetry", "packaging", "docker"]
 repository = "https://github.com/nicoloboschi/poetry-dockerize-plugin"
 documentation = "https://github.com/nicoloboschi/poetry-dockerize-plugin"
@@ -34,18 +34,19 @@
     {include = "poetry_dockerize_plugin", from = "."}
 ]
 
 [tool.poetry.plugins."poetry.application.plugin"]
 dockerize = "poetry_dockerize_plugin.plugin:DockerApplicationPlugin"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<4.0"
 poetry = "^1.7.1"
 poetry-core = "^1.8.1"
-docker = "^6.1.3"
+docker = "^7.1.0"
+requests = "^2.32.2"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.4"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `poetry_dockerize_plugin-1.0.1/PKG-INFO` & `poetry_dockerize_plugin-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-dockerize-plugin
-Version: 1.0.1
+Version: 1.1.0
 Summary: Poetry application to Docker, automatically.
 Home-page: https://github.com/nicoloboschi/poetry-dockerize-plugin
 License: MIT
 Keywords: poetry,packaging,docker
 Author: Nicolò Boschi
 Author-email: boschi1997@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -26,17 +26,18 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Software Distribution
-Requires-Dist: docker (>=6.1.3,<7.0.0)
+Requires-Dist: docker (>=7.1.0,<8.0.0)
 Requires-Dist: poetry (>=1.7.1,<2.0.0)
 Requires-Dist: poetry-core (>=1.8.1,<2.0.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
 Project-URL: Documentation, https://github.com/nicoloboschi/poetry-dockerize-plugin
 Project-URL: Repository, https://github.com/nicoloboschi/poetry-dockerize-plugin
 Description-Content-Type: text/markdown
 
 # Poetry Dockerize Plugin
 
 <p align="center">
@@ -58,15 +59,15 @@
 * Highly configurable. You can configure the image by adding a section in the `pyproject.toml` configuration file.
 
 ## Installation
 
 In order to install the plugin you need to have installed a poetry version `>=1.2.0` and type:
 
 ```bash
-poetry self add poetry-dockerize-plugin
+poetry self add poetry-dockerize-plugin@latest
 ```
 
 ## Quickstart
 
 No configuration needed! Just type:
 ```bash
 poetry dockerize
@@ -90,15 +91,15 @@
   login:
     runs-on: ubuntu-latest
     steps:
         - name: Install Poetry
           uses: snok/install-poetry@v1
 
         - name: Install poetry-dockerize-plugin
-          run: poetry self add poetry-dockerize-plugin
+          run: poetry self add poetry-dockerize-plugin@latest
 
         - name: Build and package
           run: |
             poetry install
             poetry run pytest
             poetry dockerize
 
@@ -175,17 +176,19 @@
 
 ```bash
 poetry dockerize --debug
 ```
 
 ## Generate Dockerfile
 
-To store the generated Dockerfile, you can use the `--generate` flag.
+To only generate the Dockerfile, you can use the `--generate` flag.
 
 ```bash
 poetry dockerize --generate
 ```
 
+Then you can store the Dockerfile on the repository and use it as a template and customize it as you need. 
+
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-dockerize-plugin Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: poetry-dockerize-plugin Version: 1.1.0 Summary:
 Poetry application to Docker, automatically. Home-page: https://github.com/
 nicoloboschi/poetry-dockerize-plugin License: MIT Keywords:
 poetry,packaging,docker Author: NicolÃ² Boschi Author-email:
 boschi1997@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
@@ -14,65 +14,68 @@
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Topic :: Software Development Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System :: Archiving :: Packaging Classifier: Topic ::
 System :: Installation/Setup Classifier: Topic :: System :: Software
-Distribution Requires-Dist: docker (>=6.1.3,<7.0.0) Requires-Dist: poetry
-(>=1.7.1,<2.0.0) Requires-Dist: poetry-core (>=1.8.1,<2.0.0) Project-URL:
-Documentation, https://github.com/nicoloboschi/poetry-dockerize-plugin Project-
-URL: Repository, https://github.com/nicoloboschi/poetry-dockerize-plugin
-Description-Content-Type: text/markdown # Poetry Dockerize Plugin
+Distribution Requires-Dist: docker (>=7.1.0,<8.0.0) Requires-Dist: poetry
+(>=1.7.1,<2.0.0) Requires-Dist: poetry-core (>=1.8.1,<2.0.0) Requires-Dist:
+requests (>=2.32.2,<3.0.0) Project-URL: Documentation, https://github.com/
+nicoloboschi/poetry-dockerize-plugin Project-URL: Repository, https://
+github.com/nicoloboschi/poetry-dockerize-plugin Description-Content-Type: text/
+markdown # Poetry Dockerize Plugin
                         _[_P_y_P_I_]_[_D_o_w_n_l_o_a_d_s_][Py versions]
 Key features: * Automatically generate a docker image from your Poetry
 application. * Highly configurable. You can configure the image by adding a
 section in the `pyproject.toml` configuration file. ## Installation In order to
 install the plugin you need to have installed a poetry version `>=1.2.0` and
-type: ```bash poetry self add poetry-dockerize-plugin ``` ## Quickstart No
-configuration needed! Just type: ```bash poetry dockerize >Building image:
+type: ```bash poetry self add poetry-dockerize-plugin@latest ``` ## Quickstart
+No configuration needed! Just type: ```bash poetry dockerize >Building image:
 poetry-sample-app:latest >Successfully built image: poetry-sample-app:latest
 docker run --rm -it poetry-sample-app:latest >hello world! ``` ### Usage in
 GitHub Actions You just need to run the quickstart command in your GitHub
 Actions workflow: ```yaml name: Build and publish latest on: push: branches:
 main jobs: login: runs-on: ubuntu-latest steps: - name: Install Poetry uses:
 snok/install-poetry@v1 - name: Install poetry-dockerize-plugin run: poetry self
-add poetry-dockerize-plugin - name: Build and package run: | poetry install
-poetry run pytest poetry dockerize - name: Login to Docker Hub uses: docker/
-login-action@v3 with: username: ${{ secrets.DOCKERHUB_USERNAME }} password: ${
-{ secrets.DOCKERHUB_TOKEN }} - name: Push to Docker Hub run: docker push my-
-app:latest ``` ## Configuration To customize some options, you can add a `
-[tool.dockerize]` section in your `pyproject.toml` file. For example to change
-the image name: ```toml [tool.dockerize] name = "myself/myproject-app" ``` ##
-Configuration API Reference This examples shows a complete configuration of the
-docker image: ```toml [tool.dockerize] name = "alternative-image-name" python =
-"3.12" base-image = "python:3.12-slim" tags = ["latest-dev"] entrypoint =
-["python", "-m", "whatever"] ports = [5000] env = {"MY_APP_ENV" = "dev"} labels
-= {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-run-instructions =
-["RUN curl https://huggingface.co/transformers/"] # Only for build docker layer
-build-apt-packages = ["gcc"] extra-build-instructions = ["RUN poetry config
-http-basic.foo "] build-poetry-install-args = ["-E", "all", "--no-root"] ``` *
-`name` customizes the docker image name. * `python` python version to use. If
-not specified, will try to be extracted from `tool.poetry.dependencies.python`.
-Default is `3.11` * `base-image` customizes the base image. If not defined, the
-default base image is `python:-slim-bookworm`. * `tags` declares a list of tags
-for the image. * `entrypoint` customizes the entrypoint of the image. If not
-provided, the default entrypoint is retrieved from the `packages`
-configuration. * `ports` exposes ports * `env` declares environment variables
-inside the docker image. * `labels` append labels to the docker image. Default
-labels are added following the opencontainers specification. * `apt-packages`
-installs apt packages inside the docker image. * `extra-run-instructions` adds
-extra instructions to the docker run (after poetry install). Any modification
-to the filesystem will be kept after the poetry install. For the build step: *
-`build-apt-packages` installs apt packages inside the build docker container. *
-`extra-build-instructions` adds extra instructions to the docker build (before
-poetry install). Any modification to the filesystem will be lost after the
-poetry install. If you need to add files to the image, use the `extra-run-
-instructions`. * `build-poetry-install-args` adds additional arguments to the
-`poetry install` command in the build step. ## Command-Line options All command
-line options provided by the `poetry-dockerize-plugin` may be accessed by
-typing: ```bash poetry dockerize --help ``` ## Troubleshooting To troubleshoot
-the plugin, you can use the `--debug` flag to get more information about the
-execution. ```bash poetry dockerize --debug ``` ## Generate Dockerfile To store
-the generated Dockerfile, you can use the `--generate` flag. ```bash poetry
-dockerize --generate ``` ## License This project is licensed under the terms of
-the MIT license.
+add poetry-dockerize-plugin@latest - name: Build and package run: | poetry
+install poetry run pytest poetry dockerize - name: Login to Docker Hub uses:
+docker/login-action@v3 with: username: ${{ secrets.DOCKERHUB_USERNAME }}
+password: ${{ secrets.DOCKERHUB_TOKEN }} - name: Push to Docker Hub run: docker
+push my-app:latest ``` ## Configuration To customize some options, you can add
+a `[tool.dockerize]` section in your `pyproject.toml` file. For example to
+change the image name: ```toml [tool.dockerize] name = "myself/myproject-app"
+``` ## Configuration API Reference This examples shows a complete configuration
+of the docker image: ```toml [tool.dockerize] name = "alternative-image-name"
+python = "3.12" base-image = "python:3.12-slim" tags = ["latest-dev"]
+entrypoint = ["python", "-m", "whatever"] ports = [5000] env = {"MY_APP_ENV" =
+"dev"} labels = {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-run-
+instructions = ["RUN curl https://huggingface.co/transformers/"] # Only for
+build docker layer build-apt-packages = ["gcc"] extra-build-instructions =
+["RUN poetry config http-basic.foo "] build-poetry-install-args = ["-E", "all",
+"--no-root"] ``` * `name` customizes the docker image name. * `python` python
+version to use. If not specified, will try to be extracted from
+`tool.poetry.dependencies.python`. Default is `3.11` * `base-image` customizes
+the base image. If not defined, the default base image is `python:-slim-
+bookworm`. * `tags` declares a list of tags for the image. * `entrypoint`
+customizes the entrypoint of the image. If not provided, the default entrypoint
+is retrieved from the `packages` configuration. * `ports` exposes ports * `env`
+declares environment variables inside the docker image. * `labels` append
+labels to the docker image. Default labels are added following the
+opencontainers specification. * `apt-packages` installs apt packages inside the
+docker image. * `extra-run-instructions` adds extra instructions to the docker
+run (after poetry install). Any modification to the filesystem will be kept
+after the poetry install. For the build step: * `build-apt-packages` installs
+apt packages inside the build docker container. * `extra-build-instructions`
+adds extra instructions to the docker build (before poetry install). Any
+modification to the filesystem will be lost after the poetry install. If you
+need to add files to the image, use the `extra-run-instructions`. * `build-
+poetry-install-args` adds additional arguments to the `poetry install` command
+in the build step. ## Command-Line options All command line options provided by
+the `poetry-dockerize-plugin` may be accessed by typing: ```bash poetry
+dockerize --help ``` ## Troubleshooting To troubleshoot the plugin, you can use
+the `--debug` flag to get more information about the execution. ```bash poetry
+dockerize --debug ``` ## Generate Dockerfile To only generate the Dockerfile,
+you can use the `--generate` flag. ```bash poetry dockerize --generate ``` Then
+you can store the Dockerfile on the repository and use it as a template and
+customize it as you need. ## License This project is licensed under the terms
+of the MIT license.
```

