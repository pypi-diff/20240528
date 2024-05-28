# Comparing `tmp/launchcontainers-0.1.1.tar.gz` & `tmp/launchcontainers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchcontainers-0.1.1.tar", max compression
+gzip compressed data, was "launchcontainers-0.2.0.tar", max compression
```

## Comparing `launchcontainers-0.1.1.tar` & `launchcontainers-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1268 2024-02-08 05:43:54.013272 launchcontainers-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     1517 2024-02-08 05:43:54.014995 launchcontainers-0.1.1/README.md
--rwxr-xr-x   0        0        0     1435 2024-02-08 06:05:02.345356 launchcontainers-0.1.1/pyproject.toml
--rwxr-xr-x   0        0        0      815 2024-02-08 05:43:54.050335 launchcontainers-0.1.1/src/__init__.py
--rwxr-xr-x   0        0        0    16680 2024-02-08 05:43:54.051125 launchcontainers-0.1.1/src/launch.py
--rwxr-xr-x   0        0        0      814 2024-02-08 05:43:54.052341 launchcontainers-0.1.1/src/prepare_inputs/__init__.py
--rwxr-xr-x   0        0        0    23960 2024-02-08 05:43:54.053822 launchcontainers-0.1.1/src/prepare_inputs/_version.py
--rwxr-xr-x   0        0        0     9332 2024-02-08 05:43:54.056200 launchcontainers-0.1.1/src/prepare_inputs/check_parser.py
--rwxr-xr-x   0        0        0     6700 2024-02-08 05:43:54.057139 launchcontainers-0.1.1/src/prepare_inputs/dask_scheduler_config.py
--rwxr-xr-x   0        0        0    15373 2024-02-08 05:43:54.058122 launchcontainers-0.1.1/src/prepare_inputs/prepare.py
--rwxr-xr-x   0        0        0    32212 2024-02-07 01:13:39.126252 launchcontainers-0.1.1/src/prepare_inputs/prepare_dwi.py
--rwxr-xr-x   0        0        0      620 2024-02-08 05:43:54.058911 launchcontainers-0.1.1/src/prepare_inputs/prepare_prf.py
--rwxr-xr-x   0        0        0     9261 2024-02-08 05:43:54.059800 launchcontainers-0.1.1/src/prepare_inputs/utils.py
--rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 launchcontainers-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1268 2024-03-13 13:14:08.835946 launchcontainers-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     1517 2024-05-28 10:11:57.442938 launchcontainers-0.2.0/README.md
+-rwxr-xr-x   0        0        0     1435 2024-05-28 10:12:28.089313 launchcontainers-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0      815 2024-03-13 13:14:10.126085 launchcontainers-0.2.0/src/__init__.py
+-rwxr-xr-x   0        0        0    21045 2024-05-28 10:11:57.748009 launchcontainers-0.2.0/src/launch.py
+-rwxr-xr-x   0        0        0      814 2024-03-13 13:14:10.217982 launchcontainers-0.2.0/src/prepare_inputs/__init__.py
+-rwxr-xr-x   0        0        0    23960 2024-03-13 13:14:10.286713 launchcontainers-0.2.0/src/prepare_inputs/_version.py
+-rwxr-xr-x   0        0        0     9332 2024-03-13 13:14:10.332443 launchcontainers-0.2.0/src/prepare_inputs/check_parser.py
+-rwxr-xr-x   0        0        0     7166 2024-05-28 10:11:57.783613 launchcontainers-0.2.0/src/prepare_inputs/dask_scheduler_config.py
+-rwxr-xr-x   0        0        0    17635 2024-05-28 10:11:58.459389 launchcontainers-0.2.0/src/prepare_inputs/prepare.py
+-rwxr-xr-x   0        0        0    33548 2024-05-28 10:11:58.518098 launchcontainers-0.2.0/src/prepare_inputs/prepare_dwi.py
+-rwxr-xr-x   0        0        0      620 2024-03-13 13:14:10.452740 launchcontainers-0.2.0/src/prepare_inputs/prepare_prf.py
+-rwxr-xr-x   0        0        0     9275 2024-05-28 10:11:59.148485 launchcontainers-0.2.0/src/prepare_inputs/utils.py
+-rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 launchcontainers-0.2.0/PKG-INFO
```

### Comparing `launchcontainers-0.1.1/LICENSE` & `launchcontainers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.1.1/README.md` & `launchcontainers-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 1. Prepare folder structures and input files automatically
 2. Backup the input configs for data provenance
 3. Launching containers in BCBL or DIPC
 
 Currently, **launchcontainers** works along with [anatROIs](https://github.com/garikoitz/anatROIs), [RTP-preproc](https://github.com/garikoitz/rtp-preproc), and [RTP2-pipeline](https://github.com/garikoitz/rtp-pipeline).
 
 ## NEW FEATURES
-Now you can `pip install launchcontainers==0.0.6 ` and use it in the command line! check the [How to use]() for more information
+Now you can `pip install launchcontainers==0.1.1 ` and use it in the command line! check the [How to use]() for more information
 
 # Check also:
 * [Home](https://github.com/garikoitz/launchcontainers/wiki/Home)
 * [Installation](https://github.com/garikoitz/launchcontainers/wiki/Installation)
 * [Manual](https://github.com/garikoitz/launchcontainers/wiki/Manual)
     - [Edit configs](https://github.com/garikoitz/launchcontainers/wiki/Manual)
     - [Launch `prepare` mode](https://github.com/garikoitz/launchcontainers/wiki/Manual)
```

### Comparing `launchcontainers-0.1.1/pyproject.toml` & `launchcontainers-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "launchcontainers"
-version = "0.1.1"
+version = "0.2.0"
 description = "Launch Containers Package"
 authors = [ "BCBL", 
             "Garikoitz Lerma-Usabiaga",
             "Leandro Lecca",
             "Mengxing Liu",
             "Yongning Lei"
             ]
```

### Comparing `launchcontainers-0.1.1/src/__init__.py` & `launchcontainers-0.2.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.1.1/src/launch.py` & `launchcontainers-0.2.0/src/prepare_inputs/prepare.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,437 +1,388 @@
-# -*- coding: utf-8 -*-
 """
 MIT License
 
-Copyright (c) 2020-2024 Garikoitz Lerma-Usabiaga
+Copyright (c) 2020-2023 Garikoitz Lerma-Usabiaga
 Copyright (c) 2020-2022 Mengxing Liu
-Copyright (c) 2022-2023 Leandro Lecca
-Copyright (c) 2022-2024 Yongning Lei
+Copyright (c) 2022-2024 Leandro Lecca
+Copyright (c) 2022-2023 Yongning Lei
 Copyright (c) 2023 David Linhardt
 Copyright (c) 2023 Iñigo Tellaetxe
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 """
-import os
-import subprocess as sp
-import numpy as np
-import logging
-
-# modules in lc
-
-from bids import BIDSLayout
-from dask.distributed import progress
-
-from prepare_inputs import dask_scheduler_config as dsq
-from prepare_inputs import prepare as prepare
-from prepare_inputs import utils as do
-
-logger = logging.getLogger("GENERAL")
-
 
-# %% launchcontainers
-def generate_cmd(
-    lc_config, sub, ses, dir_analysis, lst_container_specific_configs, run_lc
-):
-    """Puts together the command to send to the container.
+import logging
+import os
+import os.path as path
+from os import rename
+from os import path, symlink, unlink
+import sys
+import json
+from glob import glob
+
+import numpy as np 
+from scipy.io import loadmat
+
+from . import utils as do
+from . import prepare_dwi as dwipre
+
+logger=logging.getLogger("GENERAL")
+
+
+#%% copy configs or create new analysis
+def prepare_analysis_folder(parser_namespace, lc_config):
+    '''
+    this function is the very very first step of everything, it is IMPORTANT, 
+    it will provide a check if your desired analysis has been running before
+    and it will help you keep track of your input parameters so that you know what you are doing in your analysis    
+
+    the option force will not be useful at the analysis_folder level, if you insist to do so, you need to delete the old analysis folder by hand
+    
+    after determine the analysis folder, this function will copy your input configs to the analysis folder, and it will read only from there
+    '''
+    # read parameters from lc_config
+    
+    basedir = lc_config['general']['basedir']
+    container = lc_config['general']['container']
+    force = lc_config["general"]["force"]
+    analysis_name= lc_config['general']['analysis_name']
+    
+    run_lc = parser_namespace.run_lc
+    
+    force= force or run_lc    
+    
+    version = lc_config["container_specific"][container]["version"]    
+    # get the analysis folder information
+    
+    bidsdir_name = lc_config['general']['bidsdir_name']  
+
+    container_folder = os.path.join(basedir, bidsdir_name,'derivatives',f'{container}_{version}')
+    if not os.path.isdir(container_folder):
+        os.makedirs(container_folder)
+    
+    
+
+    Dir_analysis = os.path.join(
+        container_folder, ##########before , there is _{version}
+        f"analysis-{analysis_name}",
+                )
+    
+        
+    # define the potential exist config files
+    path_to_analysis_lc_config = os.path.join(Dir_analysis, "lc_config.yaml")
+    path_to_analysis_sub_ses_list = os.path.join(Dir_analysis, "subSesList.txt")
+    
+    if container  not in ['rtp-pipeline', 'fmriprep']:    
+        path_to_analysis_container_specific_config = [os.path.join(Dir_analysis, "config.json")] 
+    if container == 'rtp-pipeline':
+        path_to_analysis_container_specific_config = [os.path.join(Dir_analysis, "config.json"), os.path.join(Dir_analysis, "tractparams.csv")]
+    if container == 'fmriprep':
+        path_to_analysis_container_specific_config=[]
+    #TODO: heudiconv, nordic, presurfer
+    
 
-    Args:
-        lc_config (str): _description_
-        sub (str): _description_
-        ses (str): _description_
-        dir_analysis (str): _description_
-        lst_container_specific_configs (list): _description_
-        run_lc (str): _description_
 
-    Raises:
-        ValueError: Raised in presence of a faulty config.yaml file, or when the formed command is not recognized.
+    if not run_lc:
+        logger.warning(f'\nthis is PREPARE MODE, starts to  create analysis folder and copy the configs')
+        if not os.path.isdir(Dir_analysis):
+            os.makedirs(Dir_analysis)
+        
+        # backup the config info
+        
+        do.copy_file(parser_namespace.lc_config, path_to_analysis_lc_config, force) 
+        do.copy_file(parser_namespace.sub_ses_list,path_to_analysis_sub_ses_list,force)
+        for orig_config_json, copy_config_json in zip(parser_namespace.container_specific_config, path_to_analysis_container_specific_config):
+            do.copy_file(orig_config_json, copy_config_json, force)    
+        logger.debug(f'\n the analysis folder is {Dir_analysis}, all the cofigs has been copied') 
+    
+    if run_lc:
+        logger.warning(f'\n RUN MODE, this is the analysis folder that we are going to run:\n {Dir_analysis}')
+        # also copy the newest
+        do.copy_file(parser_namespace.lc_config, path_to_analysis_lc_config, force) 
+        do.copy_file(parser_namespace.sub_ses_list,path_to_analysis_sub_ses_list,force)
+        for orig_config_json, copy_config_json in zip(parser_namespace.container_specific_config,path_to_analysis_container_specific_config):
+            do.copy_file(orig_config_json, copy_config_json, force)    
+        logger.debug(f'\n the analysis folder is {Dir_analysis}, all the configs has been copied')         
+        
+        copies = [path_to_analysis_lc_config, path_to_analysis_sub_ses_list] + path_to_analysis_container_specific_config
+    
+        all_copies_present= all(os.path.isfile(copy_path) for copy_path in copies)
+
+        if all_copies_present:
+            pass
+        else:
+            logger.error(f'\n did NOT detect back up configs in the analysis folder, Please check then continue the run mode')
+    return Dir_analysis, path_to_analysis_container_specific_config
 
-    Returns:
-        _type_: _description_
+# %% prepare_input_files
+def prepare_dwi_input(parser_namespace, Dir_analysis, lc_config, df_subSes, layout, path_to_analysis_container_specific_config):
     """
 
-    # Relevant directories
-    # All other relevant directories stem from this one
-    basedir = lc_config["general"]["basedir"]
+    Parameters
+    ----------
+    lc_config : TYPE
+        DESCRIPTION.
+    df_subSes : TYPE
+        DESCRIPTION.
+
+    Returns
+    -------
+    None.
 
-    homedir = os.path.join(basedir, "singularity_home")
-    container = lc_config["general"]["container"]
-    host = lc_config["general"]["host"]
-    containerdir = lc_config["general"]["containerdir"]
-
-    # Information relevant to the host and container
-    jobqueue_config = lc_config["host_options"][host]
-    version = lc_config["container_specific"][container]["version"]
-    use_module = jobqueue_config["use_module"]
-    bind_options = jobqueue_config["bind_options"]
-
-    # Location of the Singularity Image File (.sif)
-    container_name = os.path.join(containerdir, f"{container}_{version}.sif")
-    # Define the directory and the file name to output the log of each subject
-    logdir = os.path.join(dir_analysis, "sub-" + sub, "ses-" + ses, "output", "log")
-    logfilename = f"{logdir}/t-{container}-sub-{sub}_ses-{ses}"
-
-    path_to_sub_derivatives = os.path.join(dir_analysis, f"sub-{sub}", f"ses-{ses}")
-
-    if container in ["anatrois", "rtppreproc", "rtp-pipeline"]:
-        logger.info("\n" + f"start to generate the DWI PIPELINE command")
-        config_json = lst_container_specific_configs[0]
-        logger.debug(
-            f"\n the sub is {sub} \n the ses is {ses} \n the analysis dir is {dir_analysis}"
-        )
-
-        bind_cmd = ""
-        for bind in bind_options:
-            bind_cmd += f"--bind {bind}:{bind} "
-
-        env_cmd = ""
-        if host == "local":
-            if use_module == True:
-                env_cmd = f"module load {jobqueue_config['apptainer']} &&"
-
-        cmd = (
-            f"{env_cmd} singularity run -e --no-home {bind_cmd}"
-            f"--bind {path_to_sub_derivatives}/input:/flywheel/v0/input:ro "
-            f"--bind {path_to_sub_derivatives}/output:/flywheel/v0/output "
-            f"--bind {config_json}:/flywheel/v0/config.json "
-            f"{container_name} 1>> {logfilename}.o 2>> {logfilename}.e  "
-        )
-
-    # Check which container we are using, and define the command accordingly
-    if container == "fmriprep":
-        logger.info("\n" + f"start to generate the FMRIPREP command")
-
-        nthreads = lc_config["container_specific"][container]["nthreads"]
-        mem = lc_config["container_specific"][container]["mem"]
-        fs_license = lc_config["container_specific"][container]["fs_license"]
-        containerdir = lc_config["general"]["containerdir"]
-        container_path = os.path.join(
-            containerdir,
-            f"{container}_{lc_config['container_specific'][container]['version']}.sif",
-        )
-        precommand = f"mkdir -p {homedir}; " f"unset PYTHONPATH; "
-        if "local" == host:
-            cmd = (
-                precommand + f"singularity run "
-                f"-H {homedir} "
-                f"-B {basedir}:/base -B {fs_license}:/license "
-                f"--cleanenv {container_path} "
-                f"-w {dir_analysis} "
-                f"/base/BIDS {dir_analysis} participant "
-                f"--participant-label sub-{sub} "
-                f"--skip-bids-validation "
-                f"--output-spaces func fsnative fsaverage T1w MNI152NLin2009cAsym "
-                f"--dummy-scans 0 "
-                f"--use-syn-sdc "
-                f"--fs-license-file /license/license.txt "
-                f"--nthreads {nthreads} "
-                f"--omp-nthreads {nthreads} "
-                f"--stop-on-first-crash "
-                f"--mem_mb {(mem*1000)-5000} "
-            )
-        if host in ["BCBL", "DIPC"]:
-            cmd = (
-                precommand + f"singularity run "
-                f"-H {homedir} "
-                f"-B {basedir}:/base -B {fs_license}:/license "
-                f"--cleanenv {container_path} "
-                f"-w {dir_analysis} "
-                f"/base/BIDS {dir_analysis} participant "
-                f"--participant-label sub-{sub} "
-                f"--skip-bids-validation "
-                f"--output-spaces func fsnative fsaverage T1w MNI152NLin2009cAsym "
-                f"--dummy-scans 0 "
-                f"--use-syn-sdc "
-                f"--fs-license-file /license/license.txt "
-                f"--nthreads {nthreads} "
-                f"--omp-nthreads {nthreads} "
-                f"--stop-on-first-crash "
-                f"--mem_mb {(mem*1000)-5000} "
-            )
-
-    if container in ["prfprepare", "prfreport", "prfanalyze-vista"]:
-        config_name = lc_config["container_specific"][container]["config_name"]
-        homedir = os.path.join(basedir, "singularity_home")
-        container_path = os.path.join(
-            containerdir,
-            f"{container}_{lc_config['container_specific'][container]['version']}.sif",
-        )
-        if host in ["BCBL", "DIPC"]:
-            cmd = (
-                "unset PYTHONPATH; "
-                f"singularity run "
-                f"-H {homedir} "
-                f"-B {basedir}/derivatives/fmriprep:/flywheel/v0/input "
-                f"-B {dir_analysis}:/flywheel/v0/output "
-                f"-B {basedir}/BIDS:/flywheel/v0/BIDS "
-                f"-B {dir_analysis}/{config_name}.json:/flywheel/v0/config.json "
-                f"-B {basedir}/license/license.txt:/opt/freesurfer/.license "
-                f"--cleanenv {container_path} "
-            )
-        elif host == "local":
-            cmd = (
-                "unset PYTHONPATH; "
-                f"singularity run "
-                f"-H {homedir} "
-                f"-B {basedir}/derivatives/fmriprep:/flywheel/v0/input "
-                f"-B {dir_analysis}:/flywheel/v0/output "
-                f"-B {basedir}/BIDS:/flywheel/v0/BIDS "
-                f"-B {dir_analysis}/{config_name}.json:/flywheel/v0/config.json "
-                f"-B {basedir}/license/license.txt:/opt/freesurfer/.license "
-                f"--cleanenv {container_path} "
-            )
-    # If after all configuration, we do not have command, raise an error
-    if cmd is None:
-        logger.error(
-            "\n"
-            + f"the DWI PIPELINE command is not assigned, please check your config.yaml[general][host] session\n"
-        )
-        raise ValueError("cmd is not defined, aborting")
-
-    # GLU: I don't think this is right, run is done below, I will make it work just for local but not in here,
-    #      it is good that this function just creates the cmd, I would keep it like that
-    # if run_lc:
-    #     sp.run(cmd, shell=True)
-
-    return cmd
-
-
-# %% the launchcontainer
-def launchcontainer(
-    dir_analysis,
-    lc_config,
-    sub_ses_list,
-    parser_namespace,
-    path_to_analysis_container_specific_config,
-):
-    """
-    This function launches containers generically in different Docker/Singularity HPCs
-    This function is going to assume that all files are where they need to be.
-
-    Args:
-        dir_analysis (str): _description_
-        lc_config (str): path to launchcontainer config.yaml file
-        sub_ses_list (_type_): parsed CSV containing the subject list to be analyzed, and the analysis options
-        parser_namespace (argparse.Namespace): command line arguments
     """
-    logger.info("\n" + "#####################################################\n")
-
-    # Get the host and jobqueue config info from the config.yaml file
-    host = lc_config["general"]["host"]
-    jobqueue_config = lc_config["host_options"][host]
-    if host == "local":
-        launch_mode = jobqueue_config["launch_mode"]
-    logger.debug(f"\n,, this is the job_queue config {jobqueue_config}")
-
-    force = lc_config["general"]["force"]
-    logdir = os.path.join(dir_analysis, "daskworker_log")
-
-    # Count how many jobs we need to launch from  sub_ses_list
-    n_jobs = np.sum(sub_ses_list.RUN == "True")
-
-    client, cluster = new_func(jobqueue_config, logdir, n_jobs)
-
-    logger.info(
-        "---this is the cluster and client\n" + f"{client} \n cluster: {cluster} \n"
-    )
-
-    run_lc = parser_namespace.run_lc
-
-    lc_configs = []
-    subs = []
-    sess = []
-    dir_analysiss = []
-    paths_to_analysis_config_json = []
-    run_lcs = []
+    logger.info("\n"+
+                "#####################################################\n"
+                +"---starting to prepare the input files for analysis\n")
+    
+    container = lc_config["general"]["container"]
+    force = lc_config["general"]["force"]   
+    run_lc = parser_namespace.run_lc    
+    force= force or run_lc    
+    # first thing, if the container specific config is not correct, then not doing anything
+    if len(parser_namespace.container_specific_config)==0:
+                logger.error("\n"
+                              +f"Input file error: the container specific config is not provided")
+                raise FileNotFoundError("Didn't input container_specific_config, please indicate it in your command line flag -cc")
+    else:
+        version = lc_config["container_specific"][container]["version"]
+        if "anatrois" in container or "freesurferator" in container:
+            pre_fs = lc_config["container_specific"][container]["pre_fs"]
+    
+    # If freesurferator, before copying configs, existingFS and control input fields need to be in the config.json
+    if "freesurferator" in container:
+        control_points = lc_config["container_specific"][container]["control_points"] #specific for freesurferator
+        container_specific_config_data = json.load(open(parser_namespace.container_specific_config[0]))
+        container_specific_config_data["inputs"] = {}
+        container_config_inputs = container_specific_config_data["inputs"]
+        # if pre_fs. add pre_fs in the inputs field of the container specific config.json, otherwise add T1.nii.gz
+        if pre_fs:
+            container_config_inputs["pre_fs"] = {'location': {'path': os.path.join('/flywheel/v0/input/pre_fs', 'existingFS.zip'), 'name': 'existingFS.zip'}, 'base': 'file'}
+        else:
+            container_config_inputs["anat"] = {'location': {'path': os.path.join('/flywheel/v0/input/anat', 'T1.nii.gz'), 'name': 'T1.nii.gz'}, 'base': 'file'}
+        # add control_points in the inputs field of the container specific config.json 
+        if control_points:
+            container_config_inputs["control_points"] =  {'location': {'path': '/flywheel/v0/input/control_points/control.dat', 'name': 'control.dat'}, 'base': 'file'}
+        container_specific_config_data["inputs"] = container_config_inputs
+        with open(path_to_analysis_container_specific_config[0] , "w") as outfile:
+            json.dump(container_specific_config_data, outfile, indent = 4)
 
-    # PREPARATION mode
-    if not run_lc:
-        logger.critical(
-            f"\nlaunchcontainers.py was run in PREPARATION mode (without option --run_lc)\n"
-            f"Please check that: \n"
-            f"    (1) launchcontainers.py prepared the input data properly\n"
-            f"    (2) the command created for each subject is properly formed\n"
-            f"         (you can copy the command for one subject and launch it "
-            f"on the prompt before you launch multiple subjects\n"
-            f"    (3) Once the check is done, launch the jobs by adding --run_lc to the first command you executed.\n"
-        )
-        # If the host is not local, print the job script to be launched in the cluster.
-        if host != "local":
-            logger.critical(
-                f"The cluster job script for this command is:\n"
-                f"{cluster.job_script()}"
-            )
-    # Iterate over the provided subject list
-    commands = list()
-    for row in sub_ses_list.itertuples(index=True, name="Pandas"):
+    for row in df_subSes.itertuples(index=True, name="Pandas"):
         sub = row.sub
         ses = row.ses
         RUN = row.RUN
         dwi = row.dwi
-
-        if RUN == "True":
-            # Append config, subject, session, and path info in corresponding lists
-            lc_configs.append(lc_config)
-            subs.append(sub)
-            sess.append(ses)
-            dir_analysiss.append(dir_analysis)
-            paths_to_analysis_config_json.append(
-                path_to_analysis_container_specific_config
+        
+        logger.info(f'dwi is {dwi}')
+        logger.info("\n"
+                    +"The current run is: \n"
+                    +f"{sub}_{ses}_{container}_{version}\n")
+        
+
+        if RUN == "True" and dwi == "True":
+                        
+            tmpdir = os.path.join(
+                Dir_analysis,
+                "sub-" + sub,
+                "ses-" + ses,
+                "output", "tmp"
             )
-            run_lcs.append(run_lc)
-
-            # This cmd is only for print the command
-            command = generate_cmd(
-                lc_config,
-                sub,
-                ses,
-                dir_analysis,
-                path_to_analysis_container_specific_config,
-                run_lc,
+            logdir = os.path.join(
+                Dir_analysis,
+                "sub-" + sub,
+                "ses-" + ses,
+                "output", "log"
             )
-            commands.append(command)
-            if not run_lc:
-                logger.critical(
-                    f"\nCOMMAND for subject-{sub}, and session-{ses}:\n"
-                    f"{command}\n\n"
+
+            if not os.path.isdir(tmpdir):
+                os.makedirs(tmpdir)
+            logger.info(f"\n the tmp dir is created at {tmpdir}, and it is {os.path.isdir(tmpdir)} that this file exists")
+            if not os.path.isdir(logdir):
+                os.makedirs(logdir)
+            
+            do.copy_file(parser_namespace.lc_config, os.path.join(logdir,'lc_config.yaml'), force) 
+               
+  
+
+            if "rtppreproc" in container:
+                do.copy_file(parser_namespace.container_specific_config[0], os.path.join(logdir,'config.json'), force)
+                dwipre.rtppreproc(parser_namespace, Dir_analysis, lc_config, sub, ses, layout)
+            
+            elif "rtp-pipeline" in container:
+                
+                if not len(parser_namespace.container_specific_config) == 2:
+                    logger.error("\n"
+                              +f"Input file error: the RTP-PIPELINE config is not provided completely")
+                    raise FileNotFoundError('The RTP-PIPELINE needs the config.json and tratparams.csv as container specific configs')
+                
+                output_folder_config_json=  [os.path.join(logdir, "config.json"), os.path.join(logdir, "tractparams.csv")]
+                for orig_config_json, copy_config_json in zip(parser_namespace.container_specific_config,output_folder_config_json):
+                    do.copy_file(orig_config_json, copy_config_json, force) 
+                dwipre.rtppipeline(parser_namespace, Dir_analysis,lc_config, sub, ses, layout)
+            
+            elif "anatrois" in container:
+                logger.info('we do the anatrois')
+                do.copy_file(parser_namespace.container_specific_config[0], os.path.join(logdir,'config.json'), force)
+                dwipre.anatrois(parser_namespace, Dir_analysis,lc_config,sub, ses, layout)
+            
+            elif "freesurferator" in container:
+                logger.info('we do the freesurferator')
+                do.copy_file(path_to_analysis_container_specific_config[0], os.path.join(logdir,'config.json'), force)
+                dwipre.anatrois(parser_namespace, Dir_analysis,lc_config,sub, ses, layout)
+                # in dwipre.anatrois the config.json can be modified if there are pre_fs and control.dat, so we neeed to copy the .json 
+                # after editing it 
+                
+
+            else:
+                logger.error("\n"+
+                             f"***An error occurred"
+                             +f"{container} is not created, check for typos or contact admin for singularity images\n"
                 )
 
-                if not run_lc and lc_config["general"]["container"] == "fmriprep":
-                    logger.critical(
-                        f"\n"
-                        f"fmriprep now can not deal with session specification, "
-                        f"so the analysis are running on all sessions of the "
-                        f"subject you are specifying"
-                    )
-
-    # RUN mode
-    if run_lc and host != "local":
-        # Compose the command to run in the cluster
-        futures = client.map(
-            generate_cmd,
-            lc_configs,
-            subs,
-            sess,
-            dir_analysiss,
-            paths_to_analysis_config_json,
-            run_lcs,
-        )
-        # Record the progress
-        progress(futures)
-        # Get the info and report it in the logger
-        results = client.gather(futures)
-        logger.info(results)
-        logger.info("###########")
-        # Close the connection with the client and the cluster, and inform about it
-        client.close()
-        cluster.close()
-
-        logger.critical("\n" + "launchcontainer finished, all the jobs are done")
-
-    if run_lc and host == "local":
-        if launch_mode == "parallel":
-            logger.info(
-                f"\nLocally launching {len(commands)} jobs in parallel, check "
-                f"your server's memory, some jobs might fail\n"
-            )
-            for i, cmd in enumerate(commands):
-                logger.info(f"LAUNCHING JOB {1}/{len(commands)}:\n{cmd}\n")
-                sp.run(cmd, shell=True)
-
-        if launch_mode == "serial":  # Run this with dask...
-            logger.critical(
-                f"Locally launching {len(commands)} jobs in series, this might take a lot of time"
-            )
-            serial_cmd = ""
-            for i, cmd in enumerate(commands):
-                if i == 0:
-                    serial_cmd = cmd
-                else:
-                    serial_cmd += f" && {cmd}"
-            logger.critical(
-                f"LAUNCHING SUPER SERIAL {len(commands)} JOBS:\n{serial_cmd}\n"
-            )
-            sp.run(serial_cmd, shell=True)
+        else:
+            continue
+    logger.info("\n"+
+                "#####################################################\n")
+    return  
+
+def fmriprep_intended_for(sub_ses_list, bidslayout):
+    '''
+    not implement yet, thinking how to smartly do the job
+    '''
+    layout= bidslayout
+    #number_of_topups= fmriprep_configs['number_of_topups'] # a str
+    #index_of_new_topups= fmriprep_configs['number_of_topups'] # a str about the functional run 
+    exp_TRs= [2] #fmriprep_configs['exp_TRs'] # a list
+    
+    for row in sub_ses_list.itertuples(index=True, name="Pandas"):
+        sub = row.sub
+        ses = row.ses
+        RUN = row.RUN
+        func = row.func
+        
+        if RUN == "True" and func == "True":
+
+            logger.info(f'\n working on {sub}...')
+
+        
+            # load func and fmaps
+            funcNiftis = layout.get(subject=sub, session=ses, extension='.nii.gz', datatype='func')
+            fmapNiftis = layout.get(subject=sub, session=ses, extension='.nii.gz', datatype='fmap')
+
+            funcNiftisMeta = [funcNiftis[i].get_metadata() for i in range(len(funcNiftis))]
+            fmapNiftisMeta = [fmapNiftis[i].get_metadata() for i in range(len(fmapNiftis))]
+
+            for res in exp_TRs:
+                funcN = np.array(funcNiftis)[[i['RepetitionTime'] == res for i in funcNiftisMeta]]
+                # fmapN = np.array(fmapNiftis)[[i['RepetitionTime'] == res for i in fmapNiftisMeta]]
+                fmapN = fmapNiftis
+                
+                # make list with all relative paths of func
+                funcNiftisRelPaths = [path.join(*funcN[i].relpath.split("/")[1:]) for i in range(len(funcN))]
+                funcNiftisRelPaths = [fp for fp in funcNiftisRelPaths if ((fp.endswith('_bold.nii.gz') or 
+                                                                        fp.endswith('_sbref.nii.gz')) and 
+                                                                        all([k not in fp for k in ['mag', 'phase']]))]
+
+                # add list to IntendedFor field in fmap json
+                for fmapNifti in fmapN:
+                    if not path.exists(fmapNifti.filename.replace('.nii.gz', '_orig.json')):
+                        f = fmapNifti.path.replace('.nii.gz', '.json')
+
+                        with open(f, 'r') as file:
+                            j = json.load(file)
+
+                        j['IntendedFor'] = [f.replace("\\", "/") for f in funcNiftisRelPaths]
+
+                        rename(f, f.replace('.json', '_orig.json'))
+
+                        with open(f, 'w') as file:
+                            json.dump(j, file, indent=2)
+        
+    '''add a function to check, if all the intended for is here, if so, return fmriprep'''
+    
+    return 
+
+def link_vistadisplog(basedir, sub_ses_list, bids_layout):
+    
+    
+    
+    baseP=os.path.join(basedir,'BIDS','sourcedata','vistadisplog')
+
+    
+    for row in sub_ses_list.itertuples(index=True, name='Pandas'):
+        sub  = row.sub
+        ses  = row.ses
+        RUN  = row.RUN
+        func = row.func
+        if RUN ==True and func == True:
+            taskdict=  {}
+            tasks= bids_layout.get_tasks(subject=sub, session=ses)
+            for index, item in enumerate(tasks):
+                taskdict[item]=1
+                logger.debug(taskdict)
+            matFiles = np.sort(glob(path.join(baseP, f'sub-{sub}', f'ses-{ses}', '20*.mat')))
+            logger.debug(f"\n {path.join(baseP, f'sub-{sub}', f'ses-{ses}', '20*.mat')}")
+            logger.debug(f'\n {matFiles}')
+            for matFile in matFiles:
+
+                stimName = loadmat(matFile, simplify_cells=True)['params']['loadMatrix']
+                print(stimName)
+                for key in taskdict:
+                    logger.debug(key)
+                    if key[2:] in stimName:
+                        if 'tr-2' in stimName:
+                            linkName = path.join(path.dirname(matFile), f'{sub}_{ses}_task-{key}_run-0{taskdict[key]}_params.mat')
+                            
+                            taskdict[key] += 1
+
+                    if path.islink(linkName):
+                        unlink(linkName)
+
+                    symlink(path.basename(matFile), linkName)
+
+    return True
+
+def prepare_prf_input(basedir, container, config_path, sub_ses_list, bids_layout ,run_lc):
+    # first prepare the sourcedata, the vistadisp-log
+    # then write the subject information to the config.json file
 
+    if not run_lc:
+        # if the container is prfprepare, do the preparation for vistadisplog
+        # copy the container specific information to the prfprepare.json.
+        # copy the information in subseslist to the prfprepare.json
+        # question, in this way, do we still need the config.json???
+        sub_list=[]
+        ses_list=[]
+        for row in sub_ses_list.itertuples(index=True, name='Pandas'):
+            sub  = row.sub
+            ses  = row.ses
+            RUN  = row.RUN
+            func = row.func
+            logger.debug(f'\n run is {RUN},type run is {type(RUN)} func is {func} --{sub}-{ses}' )
+            if RUN == "True" and func == "True":    # i mean yes, but there will always to better options
+                sub_list.append(sub)
+                ses_list.append(ses)
+        logger.debug(f'\nthis is sublist{sub_list}, and ses list {ses_list}\n')        
+        with open(config_path, 'r') as config_json:
+            j= json.load(config_json)
+        
+        if container == 'prfprepare':   
+            # do i need to add a check here? I don't think so
+            if link_vistadisplog(basedir,sub_ses_list, bids_layout):
+                logger.info('\n'
+                + f'the {container} prestep link vistadisplog has been done!')
+                j['subjects'] =' '.join(sub_list)
+                j['sessions'] =' '.join(ses_list)
+
+        if container =='prfresult':    
+            j['subjects'] =' '.join(sub_list)
+            j['sessions'] =' '.join(ses_list)
+        if container == 'prfanalyze-vista':
+            j['subjectName'] =' '.join(sub_list)
+            j['sessionName'] =' '.join(ses_list)
+       
+        
+        with open(config_path, 'w') as config_json:
+            json.dump(j, config_json, indent=2)
     return
-
-
-def new_func(jobqueue_config, logdir, n_jobs):
-    client, cluster = dsq.dask_scheduler(jobqueue_config, n_jobs, logdir)
-    return client, cluster
-
-
-# %% main()
-def main():
-    # Set the logging level to get the command
-    do.setup_logger()
-
-    # Get the path from command line input
-    parser_namespace = do.get_parser()
-    lc_config_path = parser_namespace.lc_config
-    lc_config = do.read_yaml(lc_config_path)
-
-    # Get general information from the config.yaml file
-    container = lc_config["general"]["container"]
-    basedir = lc_config["general"]["basedir"]
-    bidsdir_name = lc_config["general"]["bidsdir_name"]
-    sub_ses_list_path = parser_namespace.sub_ses_list
-    sub_ses_list = do.read_df(sub_ses_list_path)
-
-    # Stored value
-    verbose = parser_namespace.verbose
-    debug = parser_namespace.DEBUG
-
-    # Set the verbosity level
-    print_command_only = lc_config["general"][
-        "print_command_only"
-    ]  # TODO: this should be defined using -v and -print command only
-
-    # Set logger message level
-    # TODO: this implementation should allow changing the level of verbosity in the three levels
-    if print_command_only:
-        logger.setLevel(logging.CRITICAL)
-    if verbose:
-        logger.setLevel(logging.INFO)
-    if debug:
-        logger.setLevel(logging.DEBUG)
-    logger.critical("Reading the BIDS layout...")
-    # Prepare file and launch containers
-    # First of all prepare the analysis folder: it create you the analysis folder automatically so that you are not messing up with different analysis
-    dir_analysis, path_to_analysis_container_specific_config = (
-        prepare.prepare_analysis_folder(parser_namespace, lc_config)
-    )
-    layout = BIDSLayout(os.path.join(basedir, bidsdir_name))
-    logger.critical("                       ... finished reading the BIDS layout.")
-
-    # Prepare mode
-    if container in [
-        "anatrois",
-        "rtppreproc",
-        "rtp-pipeline",
-    ]:  # TODO: define list in another module for reusability accross modules and functions
-        prepare.prepare_dwi_input(
-            parser_namespace, dir_analysis, lc_config, sub_ses_list, layout
-        )
-
-    if container == "fmriprep":
-        prepare.fmriprep_intended_for(sub_ses_list, layout)
-
-    if container in ["prfprepare", "prfanalyze-vista", "prfreport"]:
-        logger.info(f"Container not implemented yet.")
-        pass
-
-    # Run mode
-    launchcontainer(
-        dir_analysis,
-        lc_config,
-        sub_ses_list,
-        parser_namespace,
-        path_to_analysis_container_specific_config,
-    )
-
-
-# #%%
-if __name__ == "__main__":
-    main()
```

### Comparing `launchcontainers-0.1.1/src/prepare_inputs/__init__.py` & `launchcontainers-0.2.0/src/prepare_inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.1.1/src/prepare_inputs/_version.py` & `launchcontainers-0.2.0/src/prepare_inputs/_version.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.1.1/src/prepare_inputs/check_parser.py` & `launchcontainers-0.2.0/src/prepare_inputs/check_parser.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.1.1/src/prepare_inputs/dask_scheduler_config.py` & `launchcontainers-0.2.0/src/prepare_inputs/dask_scheduler_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 MIT License
 
 Copyright (c) 2020-2023 Garikoitz Lerma-Usabiaga
 Copyright (c) 2020-2022 Mengxing Liu
-Copyright (c) 2022-2023 Leandro Lecca
+Copyright (c) 2022-2024 Leandro Lecca
 Copyright (c) 2022-2023 Yongning Lei
 Copyright (c) 2023 David Linhardt
 Copyright (c) 2023 Iñigo Tellaetxe
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 """
 import logging
+import os
 from dask import config
 from dask.distributed import Client, LocalCluster
 from dask_jobqueue import SGECluster, SLURMCluster
 
 logger = logging.getLogger("GENERAL")
 
 def initiate_cluster(jobqueue_config, n_job, logdir):
@@ -35,14 +36,18 @@
 
     '''
     config.set(distributed__comm__timeouts__tcp="90s")
     config.set(distributed__comm__timeouts__connect="90s")
     config.set(scheduler="single-threaded")
     config.set({"distributed.scheduler.allowed-failures": 50})
     config.set(admin__tick__limit="3h")
+    #config.set({"distributed.worker.use-file-locking": False})
+
+    if jobqueue_config["manager"] in ["sge","slurm"] and  not os.path.exists(logdir):
+        os.makedirs(logdir)
     
     if "sge" in jobqueue_config["manager"]:
         envextra = [f"module load {jobqueue_config['apptainer']} " 
                    #f"conda activate /export/home/tlei/tlei/conda_env/launchcontainers"
                     ]
         cluster_by_config = SGECluster(cores  = jobqueue_config["cores"], 
                                        memory = jobqueue_config["memory"],
@@ -88,15 +93,22 @@
                                          name = jobqueue_config["name"],
                                          death_timeout = 300,#jobqueue_config["death-timeout"],
                                          walltime=jobqueue_config["walltime"],
                                          job_extra_directives = ["--export=ALL"])
         cluster_by_config.scale(jobs=n_job)
     elif "local" in jobqueue_config["manager"]:
         logger.debug("defining local cluster")
-        cluster_by_config=LocalCluster()
+        cluster_by_config = LocalCluster(
+            #silence_logs = True,
+            processes = False,
+            #worker_class = "Worker",
+            n_workers = n_job,
+            threads_per_worker = jobqueue_config["threads_per_worker"],
+            memory_limit = jobqueue_config["memory_limit"],
+        )
         
     else:
         logger.warning(
             "dask configuration wasn't detected, "
             "if you are using a cluster please look at "
             "the jobqueue YAML example, modify it so it works in your cluster "
             "and add it to ~/.config/dask "
```

### Comparing `launchcontainers-0.1.1/src/prepare_inputs/prepare_dwi.py` & `launchcontainers-0.2.0/src/prepare_inputs/prepare_dwi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 MIT License
 
 Copyright (c) 2020-2023 Garikoitz Lerma-Usabiaga
 Copyright (c) 2020-2022 Mengxing Liu
-Copyright (c) 2022-2023 Leandro Lecca
+Copyright (c) 2022-2024 Leandro Lecca
 Copyright (c) 2022-2023 Yongning Lei
 Copyright (c) 2023 David Linhardt
 Copyright (c) 2023 Iñigo Tellaetxe
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -229,14 +229,22 @@
     precontainer_anat = lc_config["container_specific"][container]["precontainer_anat"]
     anat_analysis_name = lc_config["container_specific"][container]["anat_analysis_name"]
     precontainer_fmriprep = lc_config["container_specific"][container]["precontainer_fmriprep"]
     fmriprep_analysis_name = lc_config["container_specific"][container]["fmriprep_analysis_name"]
     
     srcFile_container_config_json= container_specific_config_path[0]
     new_container_specific_config_path=[]
+
+    # specific for freesurferator
+    if container == "freesurferator":
+        control_points = lc_config["container_specific"][container]["control_points"]
+        prefs_unzipname = lc_config["container_specific"][container]["prefs_unzipname"]   
+    else:
+        # if not running freesurferator control_points field is not available, then we set it False
+        control_points = False
     
     # If we ran freesurfer before:
     if pre_fs:
         logger.info("\n"
                    +f"########\n the sourceFile T1 will be pre_fs\n#########\n")
         if source_path_fszip == "anatrois":
             srcAnatPath = os.path.join(
@@ -268,14 +276,21 @@
         zips=[]
         pattern=r'^anatrois_S.*\.zip$'
         logger.debug('\n'
                      +f'the pattern is equal to prefs_zipname?  it is {pattern==prefs_zipname}')
         for filename in os.listdir(srcAnatPath):
             if filename.endswith(".zip") and re.match(prefs_zipname, filename):
                 zips.append(filename)
+            if control_points and os.path.isdir(os.path.join(srcAnatPath,filename)) and re.match(prefs_unzipname, filename):
+                srcControlPoints = os.path.join(
+                    srcAnatPath,
+                    filename,
+                    "tmp",
+                    "control.dat"
+                )
         if len(zips) == 0:
             logger.warning("\n"+
                 f"There are no files with pattern: {prefs_zipname} in {srcAnatPath}, we will listed potential zip file for you"
             )
             zips_new = sorted(glob.glob(os.path.join(srcAnatPath, "*")), key=os.path.getmtime)
             if len(zips_new) == 0:
                 logger.error("\n"+
@@ -320,17 +335,30 @@
     
     # create corresponding folder
     if not os.path.exists(dstDir_input):
         os.makedirs(dstDir_input)
     if not os.path.exists(dstDir_output):
         os.makedirs(dstDir_output)
     
+    if container == "freesurferator":
+        dstDir_work = os.path.join(
+            dir_analysis,
+            "sub-" + sub,
+            "ses-" + ses,
+            "work",
+        )
+        if not os.path.exists(dstDir_work):
+            os.makedirs(dstDir_work)
+
     if pre_fs:
         if not os.path.exists(os.path.join(dstDir_input, "pre_fs")):
             os.makedirs(os.path.join(dstDir_input, "pre_fs"))
+        if control_points:
+            if not os.path.exists(os.path.join(dstDir_input,"control_points")):
+                os.makedirs(os.path.join(dstDir_input,"control_points"))
     else:
         if not os.path.exists(os.path.join(dstDir_input, "anat")):
             os.makedirs(os.path.join(dstDir_input, "anat"))
     
     if annotfile:
         if os.path.isfile(annotfile):
             logger.info("\n"
@@ -362,14 +390,17 @@
                        +mniroizip + " does not exist")
         if not os.path.exists(os.path.join(dstDir_input, "mniroizip")):
             os.makedirs(os.path.join(dstDir_input, "mniroizip"))
 
     # Create the target files
     if pre_fs:
         dstFileT1 = os.path.join(dstDir_input, "pre_fs", "existingFS.zip")
+        if control_points:
+            dstControlPoints = os.path.join(dstDir_input, "control_points", "control.dat")
+            force_symlink(srcControlPoints,dstControlPoints,force)
     else:
         dstFileT1 = os.path.join(dstDir_input, "anat", "T1.nii.gz")
 
     dstFileAnnot = os.path.join(dstDir_input, "annotfile", "annots.zip")
     dstFileMniroizip = os.path.join(dstDir_input, "mniroizip", "mniroizip.zip")
 
     # Create the symbolic links
```

### Comparing `launchcontainers-0.1.1/src/prepare_inputs/prepare_prf.py` & `launchcontainers-0.2.0/src/prepare_inputs/prepare_prf.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.1.1/src/prepare_inputs/utils.py` & `launchcontainers-0.2.0/src/prepare_inputs/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 MIT License
 
 Copyright (c) 2020-2023 Garikoitz Lerma-Usabiaga
 Copyright (c) 2020-2022 Mengxing Liu
-Copyright (c) 2022-2023 Leandro Lecca
+Copyright (c) 2022-2024 Leandro Lecca
 Copyright (c) 2022-2023 Yongning Lei
 Copyright (c) 2023 David Linhardt
 Copyright (c) 2023 Iñigo Tellaetxe
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -138,15 +138,15 @@
         config = yaml.load(v, Loader=SafeLoader)
 
     container = config["general"]["container"]
     host = config["general"]["host"]
     host_str = f"{host}"
     if host == "local":
         launch_mode = config["host_options"]["local"]["launch_mode"]
-        valid_options = ["serial", "parallel"]
+        valid_options = ["serial", "parallel","dask_worker"]
         if launch_mode in valid_options:
             host_str = (
                 f"{host_str}, and commands will be launched in {launch_mode} mode. "
                 f"Serial is safe but it will take longer. "
                 f"If you launch in parallel be aware that some of the "
                 f"processes might be killed if the limit (usually memory) "
                 f"of the machine is reached. "
```

### Comparing `launchcontainers-0.1.1/PKG-INFO` & `launchcontainers-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchcontainers
-Version: 0.1.1
+Version: 0.2.0
 Summary: Launch Containers Package
 Home-page: https://github.com/garikoitz/launchcontainers
 License: MIT
 Keywords: HPC,MRI,RTP2,DWI,dMRI
 Author: BCBL
 Maintainer: Garikoitz Lerma-Usabiaga
 Requires-Python: >=3.10,<3.11
@@ -31,15 +31,15 @@
 1. Prepare folder structures and input files automatically
 2. Backup the input configs for data provenance
 3. Launching containers in BCBL or DIPC
 
 Currently, **launchcontainers** works along with [anatROIs](https://github.com/garikoitz/anatROIs), [RTP-preproc](https://github.com/garikoitz/rtp-preproc), and [RTP2-pipeline](https://github.com/garikoitz/rtp-pipeline).
 
 ## NEW FEATURES
-Now you can `pip install launchcontainers==0.0.6 ` and use it in the command line! check the [How to use]() for more information
+Now you can `pip install launchcontainers==0.1.1 ` and use it in the command line! check the [How to use]() for more information
 
 # Check also:
 * [Home](https://github.com/garikoitz/launchcontainers/wiki/Home)
 * [Installation](https://github.com/garikoitz/launchcontainers/wiki/Installation)
 * [Manual](https://github.com/garikoitz/launchcontainers/wiki/Manual)
     - [Edit configs](https://github.com/garikoitz/launchcontainers/wiki/Manual)
     - [Launch `prepare` mode](https://github.com/garikoitz/launchcontainers/wiki/Manual)
```

