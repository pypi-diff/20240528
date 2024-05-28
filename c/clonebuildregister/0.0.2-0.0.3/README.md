# Comparing `tmp/clonebuildregister-0.0.2.tar.gz` & `tmp/clonebuildregister-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonebuildregister-0.0.2.tar", last modified: Fri May 17 17:40:15 2024, max compression
+gzip compressed data, was "clonebuildregister-0.0.3.tar", last modified: Tue May 28 18:45:29 2024, max compression
```

## Comparing `clonebuildregister-0.0.2.tar` & `clonebuildregister-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jnsproul   (502) staff       (20)        0 2024-05-17 17:40:15.437828 clonebuildregister-0.0.2/
--rw-r--r--   0 jnsproul   (502) staff       (20)     1498 2023-06-19 12:37:56.000000 clonebuildregister-0.0.2/LICENSE
--rw-r--r--   0 jnsproul   (502) staff       (20)     6423 2024-05-17 17:40:15.437631 clonebuildregister-0.0.2/PKG-INFO
--rw-r--r--   0 jnsproul   (502) staff       (20)     5588 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/README.rst
-drwxr-xr-x   0 jnsproul   (502) staff       (20)        0 2024-05-17 17:40:15.436074 clonebuildregister-0.0.2/clonebuildregister/
--rw-r--r--   0 jnsproul   (502) staff       (20)       64 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/clonebuildregister/__init__.py
--rw-r--r--   0 jnsproul   (502) staff       (20)     5725 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/clonebuildregister/__main__.py
--rw-r--r--   0 jnsproul   (502) staff       (20)     2681 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/clonebuildregister/build_image.py
--rw-r--r--   0 jnsproul   (502) staff       (20)     1325 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/clonebuildregister/clone_repo.py
--rw-r--r--   0 jnsproul   (502) staff       (20)     3672 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/clonebuildregister/clonebuildregister.py
--rw-r--r--   0 jnsproul   (502) staff       (20)     2658 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/clonebuildregister/exceptions.py
--rw-r--r--   0 jnsproul   (502) staff       (20)     3033 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/clonebuildregister/register_image.py
-drwxr-xr-x   0 jnsproul   (502) staff       (20)        0 2024-05-17 17:40:15.437382 clonebuildregister-0.0.2/clonebuildregister.egg-info/
--rw-r--r--   0 jnsproul   (502) staff       (20)     6423 2024-05-17 17:40:15.000000 clonebuildregister-0.0.2/clonebuildregister.egg-info/PKG-INFO
--rw-r--r--   0 jnsproul   (502) staff       (20)      517 2024-05-17 17:40:15.000000 clonebuildregister-0.0.2/clonebuildregister.egg-info/SOURCES.txt
--rw-r--r--   0 jnsproul   (502) staff       (20)        1 2024-05-17 17:40:15.000000 clonebuildregister-0.0.2/clonebuildregister.egg-info/dependency_links.txt
--rw-r--r--   0 jnsproul   (502) staff       (20)        1 2024-05-16 15:36:52.000000 clonebuildregister-0.0.2/clonebuildregister.egg-info/not-zip-safe
--rw-r--r--   0 jnsproul   (502) staff       (20)       87 2024-05-17 17:40:15.000000 clonebuildregister-0.0.2/clonebuildregister.egg-info/requires.txt
--rw-r--r--   0 jnsproul   (502) staff       (20)       19 2024-05-17 17:40:15.000000 clonebuildregister-0.0.2/clonebuildregister.egg-info/top_level.txt
--rw-r--r--   0 jnsproul   (502) staff       (20)       38 2024-05-17 17:40:15.437870 clonebuildregister-0.0.2/setup.cfg
--rw-r--r--   0 jnsproul   (502) staff       (20)     1819 2024-05-17 16:24:15.000000 clonebuildregister-0.0.2/setup.py
+drwxr-xr-x   0 jnsproul   (502) staff       (20)        0 2024-05-28 18:45:29.791626 clonebuildregister-0.0.3/
+-rw-r--r--   0 jnsproul   (502) staff       (20)     1498 2023-06-19 12:37:56.000000 clonebuildregister-0.0.3/LICENSE
+-rw-r--r--   0 jnsproul   (502) staff       (20)     7019 2024-05-28 18:45:29.791389 clonebuildregister-0.0.3/PKG-INFO
+-rw-r--r--   0 jnsproul   (502) staff       (20)     6184 2024-05-28 18:45:24.000000 clonebuildregister-0.0.3/README.rst
+drwxr-xr-x   0 jnsproul   (502) staff       (20)        0 2024-05-28 18:45:29.788900 clonebuildregister-0.0.3/clonebuildregister/
+-rw-r--r--   0 jnsproul   (502) staff       (20)       64 2024-05-20 15:24:26.000000 clonebuildregister-0.0.3/clonebuildregister/__init__.py
+-rw-r--r--   0 jnsproul   (502) staff       (20)     6383 2024-05-22 15:33:21.000000 clonebuildregister-0.0.3/clonebuildregister/__main__.py
+-rw-r--r--   0 jnsproul   (502) staff       (20)     3305 2024-05-28 16:34:41.000000 clonebuildregister-0.0.3/clonebuildregister/build_image.py
+-rw-r--r--   0 jnsproul   (502) staff       (20)     1325 2024-05-20 15:24:26.000000 clonebuildregister-0.0.3/clonebuildregister/clone_repo.py
+-rw-r--r--   0 jnsproul   (502) staff       (20)     5075 2024-05-28 18:45:20.000000 clonebuildregister-0.0.3/clonebuildregister/clonebuildregister.py
+-rw-r--r--   0 jnsproul   (502) staff       (20)     2658 2024-05-20 15:24:26.000000 clonebuildregister-0.0.3/clonebuildregister/exceptions.py
+-rw-r--r--   0 jnsproul   (502) staff       (20)     3360 2024-05-22 15:31:39.000000 clonebuildregister-0.0.3/clonebuildregister/register_image.py
+drwxr-xr-x   0 jnsproul   (502) staff       (20)        0 2024-05-28 18:45:29.791084 clonebuildregister-0.0.3/clonebuildregister.egg-info/
+-rw-r--r--   0 jnsproul   (502) staff       (20)     7019 2024-05-28 18:45:29.000000 clonebuildregister-0.0.3/clonebuildregister.egg-info/PKG-INFO
+-rw-r--r--   0 jnsproul   (502) staff       (20)      517 2024-05-28 18:45:29.000000 clonebuildregister-0.0.3/clonebuildregister.egg-info/SOURCES.txt
+-rw-r--r--   0 jnsproul   (502) staff       (20)        1 2024-05-28 18:45:29.000000 clonebuildregister-0.0.3/clonebuildregister.egg-info/dependency_links.txt
+-rw-r--r--   0 jnsproul   (502) staff       (20)        1 2024-05-28 18:03:07.000000 clonebuildregister-0.0.3/clonebuildregister.egg-info/not-zip-safe
+-rw-r--r--   0 jnsproul   (502) staff       (20)       87 2024-05-28 18:45:29.000000 clonebuildregister-0.0.3/clonebuildregister.egg-info/requires.txt
+-rw-r--r--   0 jnsproul   (502) staff       (20)       19 2024-05-28 18:45:29.000000 clonebuildregister-0.0.3/clonebuildregister.egg-info/top_level.txt
+-rw-r--r--   0 jnsproul   (502) staff       (20)       38 2024-05-28 18:45:29.791676 clonebuildregister-0.0.3/setup.cfg
+-rw-r--r--   0 jnsproul   (502) staff       (20)     1819 2024-05-20 15:24:26.000000 clonebuildregister-0.0.3/setup.py
```

### Comparing `clonebuildregister-0.0.2/LICENSE` & `clonebuildregister-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clonebuildregister-0.0.2/PKG-INFO` & `clonebuildregister-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: clonebuildregister
-Version: 0.0.2
+Version: 0.0.3
 Summary: Model package for building container images and posting them to google cloud artifact registry
 Home-page: https://github.com/cznethub/clonebuildregister
-Download-URL: https://github.com/cznethub/clonebuildregister/tarball/0.0.2
+Download-URL: https://github.com/cznethub/clonebuildregister/tarball/0.0.3
 Author: Jude Sproul
 Author-email: jnsproul@ncsu.edu
 License: BSD3
 Keywords: docker image build
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -32,46 +32,55 @@
 
     >>> from clonebuildregister.clonebuildregister import clonebuildregister
     >>> clonebuildregister("cbcunc", "timage", "develop", "testimage", "v1", "timage", "testimage", "v1", "us-east1", "bimage-project", "bimage-repository")
     >>>
 
 To use clonebuildregister as a script:
 
-    usage: python -m clonebuildregister [-h] \
-                  github_org repo_name branch_or_tag local_image_name local_image_tag path_to_dockerfile target_image_name \
-                  target_image_tag region gcloudProjectId repositoryName
-    
-    Build a container image described in a GitHub repository and push that image to google cloud artifact registry.
-    
-    positional arguments:
-      ==================  ===================================================================================================
-      github_org          The GitHub organization of the repository
-      repo_name           The name of the repository in the organization
-      branch_or_tag       The branch or tag of the repository
-      local_image_name    The name of the image we create locally from the Dockerfile
-      local_image_tag     The tag of the image we create locally from the Dockerfile (v1, 1.0.1, version2.0)
-      path_to_dockerfile  The path to the docker file from the repository we cloned, usually the name of the repository
-      target_image_name   The target image name, i.e. the name of the image we store in the google cloud artifact registry
-      target_image_tag    The target image tag, i.e. the tag of the image we store in the google cloud artifact registry (v1,
-                          1.0.1, version2.0)
-      region              Region the image will be stored in the google cloud (e.g. us-east1, us, eu)
-      gcloudProjectId     The project id from which the image will be stored under in a google artifact registry
-      repositoryName      The name of the google cloud artifact registry that holds docker images
-      ==================  ===================================================================================================
-    
-    options:
-
-        - -h, --help          show this help message and exit
-        - --l L, -path_to_local_environment L
-                        The path to a local environment file with secrets not to be seen on github (e.g usr/home/clonebuildregister/.env). Defaults to .
-                        (default: None)
-        - --r R, -path_to_remote_environment R
-                        The path to the dummy environment files found on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: None)
-        - --p P, -platform P    The target platform of the image in the form of os[/arch[/variant]] (default: None)
-    
+    usage: clonebuildregister [-h] [-l PATH_TO_LOCAL_ENVIRONMENT] [-r PATH_TO_REMOTE_ENVIRONMENT] [-p PLATFORM] [-cn CLONE_NAME] [-dr DELETE_REPOSITORY]
+                          [-di DELETE_ALL_DOCKER_IMAGES]
+                          github_org repo_name branch_or_tag local_image_name local_image_tag path_to_dockerfile target_image_name target_image_tag region
+                          gcloudProjectId repositoryName
+
+
+positional arguments:
+  :github_org:            The GitHub organization of the repository
+  :repo_name:             The name of the repository in the organization
+  :branch_or_tag:         The branch or tag of the repository
+  :local_image_name:      The name of the image we create locally from the Dockerfile
+  :local_image_tag:       The tag of the image we create locally from the Dockerfile (v1, 1.0.1, version2.0)
+  :path_to_dockerfile:    The path to the docker file from the repository we cloned, usually the name of the repository
+  :target_image_name:     The target image name, i.e. the name of the image we store in the google cloud artifact registry
+  :target_image_tag:      The target image tag, i.e. the tag of the image we store in the google cloud artifact registry (v1, 1.0.1, version2.0)
+  :region:                Region the image will be stored in the google cloud (e.g. us-east1, us, eu)
+  :gcloudProjectId:       The project id from which the image will be stored under in a google artifact registry
+  :repositoryName:        The name of the google cloud artifact registry that holds docker images
+
+options:
+
+  -h, --help            show this help message and exit
+
+  -l PATH_TO_LOCAL_ENVIRONMENT, --path_to_local_environment PATH_TO_LOCAL_ENVIRONMENT
+                        The path to a local environment file with secrets not to be seen on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: )
+
+  -r PATH_TO_REMOTE_ENVIRONMENT, --path_to_remote_environment PATH_TO_REMOTE_ENVIRONMENT
+                        The path to the dummy environment files found on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: )
+
+  -p PLATFORM, --platform PLATFORM
+                        The target platform of the image in the form of os[/arch[/variant]] (default: )
+
+  -cn CLONE_NAME, --clone_name CLONE_NAME
+                        The name of the top level folder of the github repository will be named after cloning. (default: )
+
+  -dr DELETE_REPOSITORY, --delete_repository DELETE_REPOSITORY
+                        Boolean that tells the program to delete the github repository that it clones after it registers it to the google cloud AR (default: False)
+
+  -di DELETE_ALL_DOCKER_IMAGES, --delete_all_docker_images DELETE_ALL_DOCKER_IMAGES
+                        Boolean that tells the program to delete all docker images on the local system after the program puts the image on the google cloud artifact registry. Deletes using force. Similar to running this $ docker rmi -f $(docker images -aq) (default: False)
+
     example:
         $ python -m clonebuildregister cbcunc timage develop testimage v1 timage testimage v1 us-east1 bimage-project bimage-repository
 
 Use modules of clonebuildregister
 *********************************
 Use the module buildImage:
     >>> from clonebuildregister.buildImage import buildImage
@@ -98,19 +107,21 @@
 3. Go to the google cloud artifact registry and create a repository called bimage-repository ensure the repository zone is us-east1
 4. From there goto the terminal where you cloned bimage and ensure you have the gcloud CLI installed https://cloud.google.com/sdk/docs/install
 5. Make sure add to path and run $ gcloud init, ensuring you choose bimage-project
 6. Also ensure to run $ gcloud auth login, if needed
 7. Make sure $ cat ~/.docker/config.json contains us-east1. If not run $ gcloud auth configure-docker us-east1-docker.pkg.dev to add it.
 8. The test cases should now work assuming you also have docker running in the background and have already run $ python setup.py develop
 
-Install python dependencies
+Install Python dependencies
 ***************************
 1. Navigate to clonebuildregister top-level folder
 2. Create a python environment so that your default environment doesn't get cluttered
-3. Run $ conda install --file requirements.txt
+3. Run $ conda install --file environment.yml
+4. Ensure you have Docker installed.
 
 Run Tests
 *********
-1. Navigate to clonebuildregister top-level folder 
-2. $ python -m pytest
-3. If it doesn't work, do this. Replace all string instances of bimage-project-###### with the project id that you have been given. TODO: make it simpler so that you don't have to do the previous step.
+1. Navigate to clonebuildregister top-level folder
+2. Ensure you have google cloud, docker, and the required dependencies.
+3. Make sure clonebuildregister/test/testing_variables.py has the correct values for the setup you have.
+4. Run $ python -m pytest
```

### Comparing `clonebuildregister-0.0.2/README.rst` & `clonebuildregister-0.0.3/clonebuildregister.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: clonebuildregister
+Version: 0.0.3
+Summary: Model package for building container images and posting them to google cloud artifact registry
+Home-page: https://github.com/cznethub/clonebuildregister
+Download-URL: https://github.com/cznethub/clonebuildregister/tarball/0.0.3
+Author: Jude Sproul
+Author-email: jnsproul@ncsu.edu
+License: BSD3
+Keywords: docker image build
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: docker
+Requires-Dist: gitpython
+Requires-Dist: github3.py
+Requires-Dist: python-dotenv
+Requires-Dist: google-cloud-artifact-registry
+Requires-Dist: grpcio-status
+
 
 ******************
 clonebuildregister
 ******************
 
 Clones a repository, builds a docker image from that repository, and then pushes that image to google cloud artifact registry
 
@@ -9,46 +32,55 @@
 
     >>> from clonebuildregister.clonebuildregister import clonebuildregister
     >>> clonebuildregister("cbcunc", "timage", "develop", "testimage", "v1", "timage", "testimage", "v1", "us-east1", "bimage-project", "bimage-repository")
     >>>
 
 To use clonebuildregister as a script:
 
-    usage: python -m clonebuildregister [-h] \
-                  github_org repo_name branch_or_tag local_image_name local_image_tag path_to_dockerfile target_image_name \
-                  target_image_tag region gcloudProjectId repositoryName
-    
-    Build a container image described in a GitHub repository and push that image to google cloud artifact registry.
-    
-    positional arguments:
-      ==================  ===================================================================================================
-      github_org          The GitHub organization of the repository
-      repo_name           The name of the repository in the organization
-      branch_or_tag       The branch or tag of the repository
-      local_image_name    The name of the image we create locally from the Dockerfile
-      local_image_tag     The tag of the image we create locally from the Dockerfile (v1, 1.0.1, version2.0)
-      path_to_dockerfile  The path to the docker file from the repository we cloned, usually the name of the repository
-      target_image_name   The target image name, i.e. the name of the image we store in the google cloud artifact registry
-      target_image_tag    The target image tag, i.e. the tag of the image we store in the google cloud artifact registry (v1,
-                          1.0.1, version2.0)
-      region              Region the image will be stored in the google cloud (e.g. us-east1, us, eu)
-      gcloudProjectId     The project id from which the image will be stored under in a google artifact registry
-      repositoryName      The name of the google cloud artifact registry that holds docker images
-      ==================  ===================================================================================================
-    
-    options:
-
-        - -h, --help          show this help message and exit
-        - --l L, -path_to_local_environment L
-                        The path to a local environment file with secrets not to be seen on github (e.g usr/home/clonebuildregister/.env). Defaults to .
-                        (default: None)
-        - --r R, -path_to_remote_environment R
-                        The path to the dummy environment files found on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: None)
-        - --p P, -platform P    The target platform of the image in the form of os[/arch[/variant]] (default: None)
-    
+    usage: clonebuildregister [-h] [-l PATH_TO_LOCAL_ENVIRONMENT] [-r PATH_TO_REMOTE_ENVIRONMENT] [-p PLATFORM] [-cn CLONE_NAME] [-dr DELETE_REPOSITORY]
+                          [-di DELETE_ALL_DOCKER_IMAGES]
+                          github_org repo_name branch_or_tag local_image_name local_image_tag path_to_dockerfile target_image_name target_image_tag region
+                          gcloudProjectId repositoryName
+
+
+positional arguments:
+  :github_org:            The GitHub organization of the repository
+  :repo_name:             The name of the repository in the organization
+  :branch_or_tag:         The branch or tag of the repository
+  :local_image_name:      The name of the image we create locally from the Dockerfile
+  :local_image_tag:       The tag of the image we create locally from the Dockerfile (v1, 1.0.1, version2.0)
+  :path_to_dockerfile:    The path to the docker file from the repository we cloned, usually the name of the repository
+  :target_image_name:     The target image name, i.e. the name of the image we store in the google cloud artifact registry
+  :target_image_tag:      The target image tag, i.e. the tag of the image we store in the google cloud artifact registry (v1, 1.0.1, version2.0)
+  :region:                Region the image will be stored in the google cloud (e.g. us-east1, us, eu)
+  :gcloudProjectId:       The project id from which the image will be stored under in a google artifact registry
+  :repositoryName:        The name of the google cloud artifact registry that holds docker images
+
+options:
+
+  -h, --help            show this help message and exit
+
+  -l PATH_TO_LOCAL_ENVIRONMENT, --path_to_local_environment PATH_TO_LOCAL_ENVIRONMENT
+                        The path to a local environment file with secrets not to be seen on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: )
+
+  -r PATH_TO_REMOTE_ENVIRONMENT, --path_to_remote_environment PATH_TO_REMOTE_ENVIRONMENT
+                        The path to the dummy environment files found on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: )
+
+  -p PLATFORM, --platform PLATFORM
+                        The target platform of the image in the form of os[/arch[/variant]] (default: )
+
+  -cn CLONE_NAME, --clone_name CLONE_NAME
+                        The name of the top level folder of the github repository will be named after cloning. (default: )
+
+  -dr DELETE_REPOSITORY, --delete_repository DELETE_REPOSITORY
+                        Boolean that tells the program to delete the github repository that it clones after it registers it to the google cloud AR (default: False)
+
+  -di DELETE_ALL_DOCKER_IMAGES, --delete_all_docker_images DELETE_ALL_DOCKER_IMAGES
+                        Boolean that tells the program to delete all docker images on the local system after the program puts the image on the google cloud artifact registry. Deletes using force. Similar to running this $ docker rmi -f $(docker images -aq) (default: False)
+
     example:
         $ python -m clonebuildregister cbcunc timage develop testimage v1 timage testimage v1 us-east1 bimage-project bimage-repository
 
 Use modules of clonebuildregister
 *********************************
 Use the module buildImage:
     >>> from clonebuildregister.buildImage import buildImage
@@ -75,18 +107,21 @@
 3. Go to the google cloud artifact registry and create a repository called bimage-repository ensure the repository zone is us-east1
 4. From there goto the terminal where you cloned bimage and ensure you have the gcloud CLI installed https://cloud.google.com/sdk/docs/install
 5. Make sure add to path and run $ gcloud init, ensuring you choose bimage-project
 6. Also ensure to run $ gcloud auth login, if needed
 7. Make sure $ cat ~/.docker/config.json contains us-east1. If not run $ gcloud auth configure-docker us-east1-docker.pkg.dev to add it.
 8. The test cases should now work assuming you also have docker running in the background and have already run $ python setup.py develop
 
-Install python dependencies
+Install Python dependencies
 ***************************
 1. Navigate to clonebuildregister top-level folder
 2. Create a python environment so that your default environment doesn't get cluttered
-3. Run $ conda install --file requirements.txt
+3. Run $ conda install --file environment.yml
+4. Ensure you have Docker installed.
 
 Run Tests
 *********
-1. Navigate to clonebuildregister top-level folder 
-2. $ python -m pytest
-3. If it doesn't work, do this. Replace all string instances of bimage-project-###### with the project id that you have been given. TODO: make it simpler so that you don't have to do the previous step.
+1. Navigate to clonebuildregister top-level folder
+2. Ensure you have google cloud, docker, and the required dependencies.
+3. Make sure clonebuildregister/test/testing_variables.py has the correct values for the setup you have.
+4. Run $ python -m pytest
+
```

### Comparing `clonebuildregister-0.0.2/clonebuildregister/__main__.py` & `clonebuildregister-0.0.3/clonebuildregister/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
                           1.0.1, version2.0)
       region              Region the image will be stored in the google cloud
                           (e.g. us-east1, us, eu)
       gcloudProjectId     The project id from which the image will be stored under in a
                           google artifact registry
       repositoryName      The name of the google cloud artifact registry that holds docker images
 
+
     options:
         -h, --help     show help message and exit
 
     example:
         $ python clonebuildregister cbcunc timage develop testimage v1 timage testimage v1\
             us-east1 bimage-project bimage-repository
     """
@@ -89,18 +90,25 @@
                         help="The path to the dummy environment \
                 files found on github (e.g usr/home/clonebuildregister/.env). Defaults to "".",
                 default="")
     parser.add_argument("-p", "--platform", help="The target platform of the image in the \
                          form of os[/arch[/variant]]", default="")
     parser.add_argument("-cn", "--clone_name", help="The name of the top level folder of the github repository \
                         will be named after cloning.", default="")
+    parser.add_argument("-dr", "--delete_repository", help="Boolean that tells the program to delete the \
+                        github repository that it clones after it registers it to the google cloud AR", default=False)
+    parser.add_argument("-di", "--delete_all_docker_images", help="Boolean that tells the program to delete \
+              all docker images on the local system after the program puts the image on \
+              the google cloud artifact registry. Deletes using force. \
+              Similar to running this $ docker rmi -f $(docker images -aq)", default=False)
     args = parser.parse_args(argv)
     clonebuildregister(args.github_org, args.repo_name, args.branch_or_tag,
            args.local_image_name, args.local_image_tag,
            args.path_to_dockerfile, args.target_image_name,
            args.target_image_tag, args.region, args.gcloudProjectId,
            args.repositoryName, args.path_to_local_environment,
-           args.path_to_remote_environment, args.platform, args.clone_name)
+           args.path_to_remote_environment, args.platform, args.clone_name,
+           args.delete_repository, args.delete_all_docker_images)
 
 
 if __name__ == '__main__':
     main(sys.argv[1:])
```

### Comparing `clonebuildregister-0.0.2/clonebuildregister/build_image.py` & `clonebuildregister-0.0.3/clonebuildregister/build_image.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 """
 This module builds an image via dockerpy
 """
 
 import shutil
 
+from pprint import pprint
+import threading
 import docker
 from dotenv import dotenv_values
 
 from clonebuildregister.exceptions import BadCopyEnvException
 from clonebuildregister.exceptions import BuildImageException
 
 
@@ -38,36 +40,51 @@
             shutil.copyfile(path_to_local_environment, path_to_remote_environment)
         except Exception as exc:
             raise BadCopyEnvException(path_to_local_environment, path_to_remote_environment) from exc
     if (path_to_local_environment and not path_to_remote_environment):
         env_values = dotenv_values(path_to_local_environment)
     else:
         env_values = dotenv_values(".env")
-    client = docker.from_env()
+    
+    client = docker.APIClient(base_url='unix://var/run/docker.sock') #could be problem statement, could mess up the portability.
+    # events = client.events()
+    # threading.Thread(target=log_events_helper, name="log_events_helper", args=(client,)).start()
+    response = []
     try:
         if platform:
-            image = client.images.build(
-                rm=True,
-                path=f"./{target}/",
-                tag=name,
-                buildargs=dict(env_values),
-                platform=platform
-            )
+            
+            for line in client.build(rm=True, path=f"./{str(target)}/", tag=name, 
+                                     buildargs=dict(env_values), decode=True, platform=platform):
+                response.append(line)
+                print(line)
+            
+            pprint(response)
         else:
-            print(target)
-            print(name)
             
-            image = client.images.build(
-                rm=True,
-                path=f"./{str(target)}/",
-                tag=name,
-                buildargs=dict(env_values)
-            )
-        for item in image[1]:
-            for key, value in item.items():
-                if key == 'stream':
-                    text = value.strip()
-                    if text:
-                        print(text)
+            for line in client.build(rm=True, path=f"./{str(target)}/", tag=name, 
+                                     buildargs=dict(env_values), decode=True):
+                response.append(line)
+                print(line)
+            
+            
+            # pprint(response)
     except Exception as exc:
+        
         raise BuildImageException from exc
-    return image
+    
+    return response
+
+
+# Not used since events don't trigger on failure
+# def log_events_helper(client):
+#     """
+#     Helper to log events through Docker.
+#     @param events the event object that docker py created to help print logs
+#     """
+#     print("got here")
+#     i =0
+#     events = client.events()
+#     for event in events:
+#         i +=1
+#         print(i)
+#         pprint(event)
+#     print("it's ended")
```

### Comparing `clonebuildregister-0.0.2/clonebuildregister/clone_repo.py` & `clonebuildregister-0.0.3/clonebuildregister/clone_repo.py`

 * *Files identical despite different names*

### Comparing `clonebuildregister-0.0.2/clonebuildregister/exceptions.py` & `clonebuildregister-0.0.3/clonebuildregister/exceptions.py`

 * *Files identical despite different names*

### Comparing `clonebuildregister-0.0.2/clonebuildregister/register_image.py` & `clonebuildregister-0.0.3/clonebuildregister/register_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # from google.api_core.exceptions import NotFound
 
 from clonebuildregister.exceptions import GCloudRegisterImageException
 from clonebuildregister.exceptions import TagImageException
 
 
 def register_image(local_image_name: str, local_image_tag: str, target_image_name: str,
-                   target_image_tag: str, region: str, gcloud_project_id: str, repository_name: str):
+                   target_image_tag: str, region: str, gcloud_project_id: str, repository_name: str,
+                   delete_all_docker_images: bool = False):
     """
     The registerImage function.
 
         Parameters:
             local_image_name     The name of the local image that we are going to push to gcloud
             local_image_tag      The tag of the local image that we are going to push to gcloud
             target_image_name    The name of the image when it is pushed to gcloud
@@ -66,9 +67,13 @@
     if 'errorDetail' in response:
         pprint(response)
         raise GCloudRegisterImageException() from Exception()
 
     if gcloud_response:
         gcloud_request = artifactregistry_v1.DeleteVersionRequest(name=gcloud_response.version, force=True)
         gcloud_client.delete_version(request=gcloud_request)
-
+    if (delete_all_docker_images):
+        print("Attempting to delete remaining local images. Deleting using --force.")
+        for image in client.images.list():
+            print("Deleting image: ", image.tags)
+            client.images.remove(image.id, force=True)
     return response
```

### Comparing `clonebuildregister-0.0.2/clonebuildregister.egg-info/PKG-INFO` & `clonebuildregister-0.0.3/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: clonebuildregister
-Version: 0.0.2
-Summary: Model package for building container images and posting them to google cloud artifact registry
-Home-page: https://github.com/cznethub/clonebuildregister
-Download-URL: https://github.com/cznethub/clonebuildregister/tarball/0.0.2
-Author: Jude Sproul
-Author-email: jnsproul@ncsu.edu
-License: BSD3
-Keywords: docker image build
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Build Tools
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: docker
-Requires-Dist: gitpython
-Requires-Dist: github3.py
-Requires-Dist: python-dotenv
-Requires-Dist: google-cloud-artifact-registry
-Requires-Dist: grpcio-status
-
 
 ******************
 clonebuildregister
 ******************
 
 Clones a repository, builds a docker image from that repository, and then pushes that image to google cloud artifact registry
 
@@ -32,46 +9,55 @@
 
     >>> from clonebuildregister.clonebuildregister import clonebuildregister
     >>> clonebuildregister("cbcunc", "timage", "develop", "testimage", "v1", "timage", "testimage", "v1", "us-east1", "bimage-project", "bimage-repository")
     >>>
 
 To use clonebuildregister as a script:
 
-    usage: python -m clonebuildregister [-h] \
-                  github_org repo_name branch_or_tag local_image_name local_image_tag path_to_dockerfile target_image_name \
-                  target_image_tag region gcloudProjectId repositoryName
-    
-    Build a container image described in a GitHub repository and push that image to google cloud artifact registry.
-    
-    positional arguments:
-      ==================  ===================================================================================================
-      github_org          The GitHub organization of the repository
-      repo_name           The name of the repository in the organization
-      branch_or_tag       The branch or tag of the repository
-      local_image_name    The name of the image we create locally from the Dockerfile
-      local_image_tag     The tag of the image we create locally from the Dockerfile (v1, 1.0.1, version2.0)
-      path_to_dockerfile  The path to the docker file from the repository we cloned, usually the name of the repository
-      target_image_name   The target image name, i.e. the name of the image we store in the google cloud artifact registry
-      target_image_tag    The target image tag, i.e. the tag of the image we store in the google cloud artifact registry (v1,
-                          1.0.1, version2.0)
-      region              Region the image will be stored in the google cloud (e.g. us-east1, us, eu)
-      gcloudProjectId     The project id from which the image will be stored under in a google artifact registry
-      repositoryName      The name of the google cloud artifact registry that holds docker images
-      ==================  ===================================================================================================
-    
-    options:
-
-        - -h, --help          show this help message and exit
-        - --l L, -path_to_local_environment L
-                        The path to a local environment file with secrets not to be seen on github (e.g usr/home/clonebuildregister/.env). Defaults to .
-                        (default: None)
-        - --r R, -path_to_remote_environment R
-                        The path to the dummy environment files found on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: None)
-        - --p P, -platform P    The target platform of the image in the form of os[/arch[/variant]] (default: None)
-    
+    usage: clonebuildregister [-h] [-l PATH_TO_LOCAL_ENVIRONMENT] [-r PATH_TO_REMOTE_ENVIRONMENT] [-p PLATFORM] [-cn CLONE_NAME] [-dr DELETE_REPOSITORY]
+                          [-di DELETE_ALL_DOCKER_IMAGES]
+                          github_org repo_name branch_or_tag local_image_name local_image_tag path_to_dockerfile target_image_name target_image_tag region
+                          gcloudProjectId repositoryName
+
+
+positional arguments:
+  :github_org:            The GitHub organization of the repository
+  :repo_name:             The name of the repository in the organization
+  :branch_or_tag:         The branch or tag of the repository
+  :local_image_name:      The name of the image we create locally from the Dockerfile
+  :local_image_tag:       The tag of the image we create locally from the Dockerfile (v1, 1.0.1, version2.0)
+  :path_to_dockerfile:    The path to the docker file from the repository we cloned, usually the name of the repository
+  :target_image_name:     The target image name, i.e. the name of the image we store in the google cloud artifact registry
+  :target_image_tag:      The target image tag, i.e. the tag of the image we store in the google cloud artifact registry (v1, 1.0.1, version2.0)
+  :region:                Region the image will be stored in the google cloud (e.g. us-east1, us, eu)
+  :gcloudProjectId:       The project id from which the image will be stored under in a google artifact registry
+  :repositoryName:        The name of the google cloud artifact registry that holds docker images
+
+options:
+
+  -h, --help            show this help message and exit
+
+  -l PATH_TO_LOCAL_ENVIRONMENT, --path_to_local_environment PATH_TO_LOCAL_ENVIRONMENT
+                        The path to a local environment file with secrets not to be seen on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: )
+
+  -r PATH_TO_REMOTE_ENVIRONMENT, --path_to_remote_environment PATH_TO_REMOTE_ENVIRONMENT
+                        The path to the dummy environment files found on github (e.g usr/home/clonebuildregister/.env). Defaults to . (default: )
+
+  -p PLATFORM, --platform PLATFORM
+                        The target platform of the image in the form of os[/arch[/variant]] (default: )
+
+  -cn CLONE_NAME, --clone_name CLONE_NAME
+                        The name of the top level folder of the github repository will be named after cloning. (default: )
+
+  -dr DELETE_REPOSITORY, --delete_repository DELETE_REPOSITORY
+                        Boolean that tells the program to delete the github repository that it clones after it registers it to the google cloud AR (default: False)
+
+  -di DELETE_ALL_DOCKER_IMAGES, --delete_all_docker_images DELETE_ALL_DOCKER_IMAGES
+                        Boolean that tells the program to delete all docker images on the local system after the program puts the image on the google cloud artifact registry. Deletes using force. Similar to running this $ docker rmi -f $(docker images -aq) (default: False)
+
     example:
         $ python -m clonebuildregister cbcunc timage develop testimage v1 timage testimage v1 us-east1 bimage-project bimage-repository
 
 Use modules of clonebuildregister
 *********************************
 Use the module buildImage:
     >>> from clonebuildregister.buildImage import buildImage
@@ -98,19 +84,20 @@
 3. Go to the google cloud artifact registry and create a repository called bimage-repository ensure the repository zone is us-east1
 4. From there goto the terminal where you cloned bimage and ensure you have the gcloud CLI installed https://cloud.google.com/sdk/docs/install
 5. Make sure add to path and run $ gcloud init, ensuring you choose bimage-project
 6. Also ensure to run $ gcloud auth login, if needed
 7. Make sure $ cat ~/.docker/config.json contains us-east1. If not run $ gcloud auth configure-docker us-east1-docker.pkg.dev to add it.
 8. The test cases should now work assuming you also have docker running in the background and have already run $ python setup.py develop
 
-Install python dependencies
+Install Python dependencies
 ***************************
 1. Navigate to clonebuildregister top-level folder
 2. Create a python environment so that your default environment doesn't get cluttered
-3. Run $ conda install --file requirements.txt
+3. Run $ conda install --file environment.yml
+4. Ensure you have Docker installed.
 
 Run Tests
 *********
-1. Navigate to clonebuildregister top-level folder 
-2. $ python -m pytest
-3. If it doesn't work, do this. Replace all string instances of bimage-project-###### with the project id that you have been given. TODO: make it simpler so that you don't have to do the previous step.
-
+1. Navigate to clonebuildregister top-level folder
+2. Ensure you have google cloud, docker, and the required dependencies.
+3. Make sure clonebuildregister/test/testing_variables.py has the correct values for the setup you have.
+4. Run $ python -m pytest
```

### Comparing `clonebuildregister-0.0.2/clonebuildregister.egg-info/SOURCES.txt` & `clonebuildregister-0.0.3/clonebuildregister.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clonebuildregister-0.0.2/setup.py` & `clonebuildregister-0.0.3/setup.py`

 * *Files identical despite different names*

