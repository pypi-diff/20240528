# Comparing `tmp/twinlab-2.6.1.tar.gz` & `tmp/twinlab-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-2.6.1.tar", max compression
+gzip compressed data, was "twinlab-2.7.0.tar", max compression
```

## Comparing `twinlab-2.6.1.tar` & `twinlab-2.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1031 2023-09-19 13:29:40.794269 twinlab-2.6.1/LICENSE
--rw-r--r--   0        0        0     2657 2024-04-29 12:58:08.159852 twinlab-2.6.1/README.md
--rw-r--r--   0        0        0     1759 2024-05-01 08:08:37.375772 twinlab-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     1486 2024-04-30 15:00:41.994100 twinlab-2.6.1/twinlab/__init__.py
--rw-r--r--   0        0        0      171 2023-09-19 13:29:40.807103 twinlab-2.6.1/twinlab/_version.py
--rw-r--r--   0        0        0    14702 2024-04-29 12:58:08.199408 twinlab-2.6.1/twinlab/api.py
--rw-r--r--   0        0        0    40736 2024-04-29 12:58:08.199897 twinlab-2.6.1/twinlab/client.py
--rw-r--r--   0        0        0     9549 2024-05-01 08:08:27.641140 twinlab-2.6.1/twinlab/core.py
--rw-r--r--   0        0        0     9256 2024-04-29 12:58:08.200160 twinlab-2.6.1/twinlab/dataset.py
--rw-r--r--   0        0        0      843 2024-04-29 12:58:08.200663 twinlab-2.6.1/twinlab/distributions.py
--rw-r--r--   0        0        0    66186 2024-05-01 08:08:27.641673 twinlab-2.6.1/twinlab/emulator.py
--rw-r--r--   0        0        0     4876 2024-04-15 15:01:48.559474 twinlab-2.6.1/twinlab/helper.py
--rw-r--r--   0        0        0    29618 2024-05-01 08:08:27.642016 twinlab-2.6.1/twinlab/params.py
--rw-r--r--   0        0        0     1862 2024-03-13 15:41:11.184579 twinlab-2.6.1/twinlab/plotting.py
--rw-r--r--   0        0        0      659 2024-04-29 12:58:08.201372 twinlab-2.6.1/twinlab/prior.py
--rw-r--r--   0        0        0     1926 2024-04-15 15:01:48.560048 twinlab-2.6.1/twinlab/sampling.py
--rw-r--r--   0        0        0     1637 2024-01-11 11:15:46.668160 twinlab-2.6.1/twinlab/settings.py
--rw-r--r--   0        0        0     5674 2024-05-01 08:08:27.642300 twinlab-2.6.1/twinlab/utils.py
--rw-r--r--   0        0        0     4081 1970-01-01 00:00:00.000000 twinlab-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1031 2024-03-11 09:16:22.945659 twinlab-2.7.0/LICENSE
+-rw-r--r--   0        0        0     2657 2024-04-30 11:01:34.365245 twinlab-2.7.0/README.md
+-rw-r--r--   0        0        0     1494 2024-05-28 08:13:49.871330 twinlab-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1506 2024-05-28 08:13:31.528344 twinlab-2.7.0/twinlab/__init__.py
+-rw-r--r--   0        0        0      171 2024-03-12 11:24:16.616707 twinlab-2.7.0/twinlab/_version.py
+-rw-r--r--   0        0        0    14702 2024-04-30 11:01:34.404360 twinlab-2.7.0/twinlab/api.py
+-rw-r--r--   0        0        0    40736 2024-04-29 08:14:22.327125 twinlab-2.7.0/twinlab/client.py
+-rw-r--r--   0        0        0     9549 2024-05-23 14:39:09.694729 twinlab-2.7.0/twinlab/core.py
+-rw-r--r--   0        0        0     9512 2024-05-28 08:13:31.528563 twinlab-2.7.0/twinlab/dataset.py
+-rw-r--r--   0        0        0      843 2024-04-29 08:14:22.328406 twinlab-2.7.0/twinlab/distributions.py
+-rw-r--r--   0        0        0    72358 2024-05-28 08:13:31.528920 twinlab-2.7.0/twinlab/emulator.py
+-rw-r--r--   0        0        0     4876 2024-04-24 16:37:20.503508 twinlab-2.7.0/twinlab/helper.py
+-rw-r--r--   0        0        0    38039 2024-05-28 08:13:31.529111 twinlab-2.7.0/twinlab/params.py
+-rw-r--r--   0        0        0     1862 2024-04-25 10:03:12.145327 twinlab-2.7.0/twinlab/plotting.py
+-rw-r--r--   0        0        0      659 2024-04-29 08:14:22.329240 twinlab-2.7.0/twinlab/prior.py
+-rw-r--r--   0        0        0     1926 2024-04-24 16:37:20.504073 twinlab-2.7.0/twinlab/sampling.py
+-rw-r--r--   0        0        0     1637 2024-03-12 11:24:16.626252 twinlab-2.7.0/twinlab/settings.py
+-rw-r--r--   0        0        0     5674 2024-05-23 14:39:09.695216 twinlab-2.7.0/twinlab/utils.py
+-rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 twinlab-2.7.0/PKG-INFO
```

### Comparing `twinlab-2.6.1/LICENSE` & `twinlab-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/README.md` & `twinlab-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/__init__.py` & `twinlab-2.7.0/twinlab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 from .params import (
     AcqFuncParams,
     BenchmarkParams,
     CalibrateParams,
     DesignParams,
     EstimatorParams,
     ModelSelectionParams,
+    MaximizeParams,
     OptimiserParams,
     PredictParams,
     RecommendParams,
     SampleParams,
     ScoreParams,
     TrainParams,
 )
```

### Comparing `twinlab-2.6.1/twinlab/api.py` & `twinlab-2.7.0/twinlab/api.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/client.py` & `twinlab-2.7.0/twinlab/client.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/core.py` & `twinlab-2.7.0/twinlab/core.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/dataset.py` & `twinlab-2.7.0/twinlab/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,34 +90,38 @@
         self,
         columns: List[str],
         verbose: bool = False,
     ) -> pd.DataFrame:
         """Return an analysis of the variance retained per dimension.
 
         Args:
-            columns (list[str]): List of columns to evaluate. This would usually be either the set of input or output columns.
+            columns (list[str]): List of columns to evaluate. This is typically either the set of input or output columns.
             verbose (bool, optional): Display information about the operation while running.
 
         Returns:
-            pandas.Dataframe containing the variance analysis.
+            pandas.Dataframe: A ``pandas.DataFrame`` containing the variance analysis.
 
         Example:
             .. code-block:: python
 
                 dataset = tl.Dataset("quickstart")
-                dataset.analyse_variance(columns=["x", "y"]) # Usually the columns would be either input or output
+                dataset.analyse_variance(columns=["x", "y"]) # Typically either input or output columns
 
             .. code-block:: console
 
                    Number of Dimensions  Cumulative Variance
                 0                     0             0.000000
                 1                     1             0.925741
                 2                     2             1.000000
 
         """
+        if len(columns) == 1:
+            raise ValueError(
+                "Singular value decomposition should use more than one column. Please retry with more than one input or output column."
+            )
         columns_string = ",".join(columns)
         _, response = api.analyse_dataset(
             self.id, columns=columns_string, verbose=DEBUG
         )
         if response["dataframe"] is not None:
             csv_string = utils.get_value_from_body("dataframe", response)
             csv_string = io.StringIO(csv_string)
@@ -175,15 +179,15 @@
     def view(self, verbose: bool = False) -> pd.DataFrame:
         """View (and download) a dataset that exists on the twinLab cloud.
 
         Args:
             verbose (bool, optional): Display information about the operation while running.
 
         Returns:
-            pandas.Dataframe containing the requested dataset.
+            pandas.Dataframe: A ``pandas.DataFrame`` containing the requested dataset.
 
         Example:
             .. code-block:: python
 
                 dataset = tl.Dataset("quickstart")
                 dataset.view()
 
@@ -219,15 +223,15 @@
     def summarise(self, verbose: bool = False) -> pd.DataFrame:
         """Show summary statistics for a dataset that exists on the twinLab cloud.
 
         Args:
             verbose (bool, optional): Display information about the operation while running.
 
         Returns:
-            pandas.DataFrame: DataFrame with summary statistics.
+            pandas.DataFrame: A ``pandas.DataFrame`` with summary statistics.
 
         Example:
             .. code-block:: python
 
                 dataset = tl.Dataset("my_dataset")
                 dataset.summarise()
```

### Comparing `twinlab-2.6.1/twinlab/distributions.py` & `twinlab-2.7.0/twinlab/distributions.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/emulator.py` & `twinlab-2.7.0/twinlab/emulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # Project imports
 from . import api, settings, utils
 from .dataset import Dataset
 from .params import (
     BenchmarkParams,
     CalibrateParams,
     DesignParams,
+    MaximizeParams,
     PredictParams,
     RecommendParams,
     SampleParams,
     ScoreParams,
     TrainParams,
 )
 from .plotting import DIGILAB_CMAP as digilab_cmap
@@ -55,14 +56,15 @@
 PROCESS_MAP = {
     "score": "score",
     "get_calibration_curve": "benchmark",
     "predict": "predict",
     "sample": "sample",
     "get_candidate_points": "recommend",
     "solve_inverse": "calibrate",
+    "maximize": "maximize",
 }
 
 ALLOWED_DATAFRAME_SIZE = 5.5 * int(
     1e6
 )  # 5.5MB limit to stay safely (also to allow other variables and dataframes to flow through without making a fuss) within the 6MB limit for a Lambda response payload size
 
 ### Helper functions ###
@@ -177,14 +179,17 @@
 ) -> Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]:
     if method == "predict":
         df = pd.read_csv(csv, sep=",")
         n = len(df.columns)
         df_mean, df_std = df.iloc[:, : n // 2], df.iloc[:, n // 2 :]
         df_std.columns = df_std.columns.str.removesuffix(" [std_dev]")
         return df_mean, df_std
+    elif method == "maximize":
+        df = pd.read_csv(csv, sep=",")
+        return df
     elif method == "sample":
         df_result = pd.read_csv(csv, header=[0, 1], sep=",")
         return df_result
     elif method == "get_candidate_points":
         df = pd.read_csv(csv, sep=",")
         return df
     elif method == "solve_inverse":
@@ -489,15 +494,15 @@
     def view_test_data(self, verbose: bool = False) -> pd.DataFrame:
         """View test data on which the emulator was tested in the twinLab cloud.
 
         Args:
             verbose (bool, optional): Display information about the operation while running.
 
         Returns:
-            pandas.DataFrame: Dataframe containing the training data on which the emulator was tested
+            pandas.DataFrame: Dataframe containing the training data on which the emulator was tested.
 
         Example:
 
             .. code-block:: python
 
                 emulator = tl.Emulator("quickstart")
                 emulator.view_test_data()
@@ -522,15 +527,15 @@
     def list_processes(self, verbose: bool = False) -> Dict[str, Dict]:
         """List all of the processes associated with a given emulator on the twinLab cloud.
 
         Args:
             verbose (bool, optional): Determining level of information returned to the user. Default is False.
 
         Returns:
-            dict: Dictionary containing all processes associated with the emulator
+            dict: Dictionary containing all processes associated with the emulator.
 
         Example:
 
             .. code-block:: python
 
                 emulator = tl.Emulator("quickstart")
                 emulator.list_processes()
@@ -795,22 +800,26 @@
 
     @typechecked
     def benchmark(
         self,
         params: BenchmarkParams = BenchmarkParams(),
         verbose: bool = False,
     ) -> Optional[pd.DataFrame]:
-        """Benchmark the performance of a trained emulator with a calibration curve.
+        """Benchmark the predicted uncertainty of a trained emulator.
 
-        A test dataset must have been defined in order for this to produce a meaningful result.
+        A test dataset must have been defined in order for this to produce a result (otherwise ``None`` is returned).
         This means that ``train_test_ratio`` must be less than 1 when training the emulator.
-        The calibration curve can be plotted to show how well the training data fits to the emulator,
-        and is calculated differently depending on the `params` chosen.
-        The returned dataframe contains 100 rows for each output column of the emulator.
-        These can be plotted to ascertain the performance of the emulator.
+        This method returns the calibration curve of a trained emulator, which can be used to asses the quality of the uncertainty predictions.
+        The calibration curve is a plot of the fraction of values that are predicted to be within a certain confidence interval against the actual fraction of values that are within that interval.
+
+        100 monotonically increasing values between 0 and 1 are returned for each output dimension of the emulator, in the form of a ``pandas.DataFrame``.
+        These values can be plotted as the values on a y-axis, while the x-axis is taken to be 100 equally spaced values between 0 and 1 (inclusive).
+        A well-calibrated emulator will have a curve that is close to the line ``y = x``.
+        If the shape deviates from this line, the emulator may be under- or overconfident, but the exact interpretation depends on the type of curve.
+        See the documentation for ``BenchmarkParams`` for more information on the available types.
 
         Args:
             params (BenchmarkParams, optional): A parameter-configuration object that contains optional parameters for benchmarking an emulator.
             verbose (bool, optional): Display detailed information about the operation while running.
 
         Returns:
             pandas.DataFrame, None: Either a ``pandas.DataFrame`` containing the calibration curve for an emulator, or ``None`` if there is no test data.
@@ -833,15 +842,15 @@
                 95  1.0
                 96  1.0
                 97  1.0
                 98  1.0
                 99  1.0
 
         """
-        # TODO: This needs to be understood and documented better
+        # TODO: Maybe include how to plot calibration curve in a docstring code snippet.
 
         csv = self._use_method(
             method="get_calibration_curve",
             **params.unpack_parameters(),
             verbose=verbose,
         )
 
@@ -964,16 +973,16 @@
         Rather than quantifying the uncertainty in the predictions, this method draws samples from the emulator.
         The collection of samples can be used to explore the distribution of the emulator predictions.
         Each sample is a possible prediction of the emulator, and therefore a prediction of a possible new observation from the data-generation process.
         The covariance in the emulator predictions can therefore be explored, which is particularly useful for functional Gaussian Processes.
 
         If the output of the multi-indexed DataFrame needs to be manipulated then we provide the convenience functions:
 
-            - ``tl.get_sample``: Isolate an individual sample into a new ``pandas.DataFrame``
-            - ``tl.join_samples``: Join together multiple sets of samples into a single ``pandas.DataFrame``
+        - ``tl.get_sample``: Isolate an individual sample into a new ``pandas.DataFrame``
+        - ``tl.join_samples``: Join together multiple sets of samples into a single ``pandas.DataFrame``
 
         Args:
             df (pandas.DataFrame): The ``X`` values for which to draw samples.
             num_samples (int): Number of samples to draw for each row of the evaluation data.
             params (SampleParams, optional): A `SampleParams` object with sampling parameters.
             wait (bool, optional): If ``True`` wait for the job to complete, otherwise return the process ID and exit.
             verbose (bool, optional): Display detailed information about the operation while running.
@@ -1049,22 +1058,27 @@
         wait: bool = True,
         verbose: bool = False,
     ) -> Union[Tuple[pd.DataFrame, float], str]:
         """Draw new recommended data points from a trained emulator that exists on the twinLab cloud.
 
         The recommend functionality of an emulator is used to suggest new data points to sample.
         These new data points can be chosen depending on a variety of different user objectives.
-        Currently, the user can choose between ``"optimise"`` and ``"explore"`` acquisition functions.
-        Choosing ``"optimise"`` will obtain suggested ``"X"`` values the evaluation of which (acquiring the corresponding ``"y"``) will maximise the knowledge of the emulator about the location of the maximum.
-        A classic use case for this would be a user trying to maximise the output of a model.
-        For example, the maximum strenth of a pipe given a set of design parameters.
-        Choosing ``"explore"`` will instead suggest ``"X"`` that reduce the overall uncertainty of the emulator across the entire input space.
-        A classic use case for this would be a user trying to reduce overally uncertainty.
-        For example, a user trying to reduce the uncertainty in the strength of a pipe across all design parameters.
-        The number of requested data points can be specified by the user, and if this is greater than one then then recommendations are all suggested at once, and are designed to be the optmial set, as a group, to achieve the user outcome.
+        Currently, the user can choose between ``"optimise"`` and ``"explore"`` acquisition functions:
+
+        - ``"optimise"`` will obtain suggested ``"X"`` values the evaluation of which (acquiring the corresponding ``"y"``) will maximize the knowledge of the emulator about the location of the maximum.
+          A classic use case for this would be a user trying to maximize the output of a model (e.g., the combination of metals that creates the strongest alloy).
+          This method can also be used to minimize an output, by using the ``weight`` argument of ``RecommendParams`` to multiply the output by -1.
+          If an emulator has more-than-one output, then a weighted combination of the outputs can be minimized/maximized.
+          Once again, using the ``opt_weight`` argument of ``MaximizeParams`` can control the weight assigned to each output, or can be used to focus on a single output.
+          For example, the maximum strength of a pipe given a set of design parameters.
+        - ``"explore"`` will instead suggest ``"X"`` that reduce the overall uncertainty of the emulator across the entire input space.
+          A classic use case for this would be a user trying to reduce overally uncertainty.
+          For example, a user trying to reduce the uncertainty in the strength of a pipe across all design parameters.
+
+        The number of requested data points can be specified by the user, and if this is greater than 1 then then recommendations are all suggested at once, and are designed to be the optmial set, as a group, to achieve the user outcome.
         twinLab optimises which specific acquisition function within the chosen category will be used, prioritising numerical stability based on the number of points requested.
 
         The value of the acquisition function is also returned to the user.
         While this is of limited value in isolation, the trend of the acquisition function value over multiple iterations of ``Recommend`` can be used to understand the performance of the emulator.
         The ``Emulator.learn`` method can be used to improve the performance of an emulator iteratively.
 
         Args:
@@ -1255,14 +1269,85 @@
             df = _process_csv(csv, API_METHOD)
         if verbose:
             print("Calibration summary:")
             print(df)
         return df
 
     @typechecked
+    def maximize(
+        self,
+        params: MaximizeParams = MaximizeParams(),
+        wait: bool = True,
+        verbose: bool = False,
+    ) -> Union[pd.DataFrame, str]:
+        """Finding the maximum the output of a trained emulator that exists on the twinLab cloud.
+
+        This method of an emulator is used to find the point in the input space that maximizes the output of your trained emulator.
+        This method is useful for finding the best possible input for your model, given the emulator predictions.
+        This can help provide guidance for how best to configure your experiment, for example.
+        This method can be used in a stand-alone manner to find the maximum, or at the end of a Bayesian optimization loop to find the best possible input.
+        This method can also be used to minimize an output, by using the ``opt_weight`` argument of ``MaximizeParams`` to multiply the output by -1.
+        If an emulator has more-than-one output, then a weighted combination of the outputs can be minimized/maximized.
+        Once again, using the ``opt_weight`` argument of ``MaximizeParams`` can control the weight assigned to each output, or can be used to focus on a single output.
+
+        Args:
+            params (MaximizeParams): A parameter-configuration that contains optional parameters for finding the input that produces the maximum model output.
+            wait (bool, optional): If ``True`` wait for the job to complete, otherwise return the process ID and exit.
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Returns:
+            Tuple[pandas.DataFrame], str: By default, a Dataframe containing the input that optimizes your emulator predictions.
+            Instead, if ``wait=False``, the process ID is returned.
+            The results can then be retrieved later using ``Emulator.get_process(<process_id>)``.
+            Process IDs associated with an emulator can be found using ``Emulator.list_processes()``.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                emulator.maximize()
+
+            .. code-block:: console
+
+                          X
+                0  0.845942
+
+        """
+        API_METHOD = "maximize"
+        if SYNC:
+            csv = self._use_method(
+                method=API_METHOD,
+                **params.unpack_parameters(),
+                verbose=verbose,
+            )
+        else:
+            _, response = api.use_request_model(
+                model_id=self.id,
+                method=API_METHOD,
+                **params.unpack_parameters(),
+                processor=PROCESSOR,
+                verbose=DEBUG,
+            )
+            process_id = utils.get_value_from_body("process_id", response)
+            if verbose:
+                print(f"Job {PROCESS_MAP[API_METHOD]} process ID: {process_id}")
+            if not wait:
+                return process_id
+            _, response = _wait_for_job_completion(
+                self.id, API_METHOD, process_id, verbose=verbose
+            )
+            csv = utils.get_value_from_body("dataframe", response)
+            csv = io.StringIO(csv)
+        df = _process_csv(csv, API_METHOD)
+        if verbose:
+            print("Optimal input:")
+            print(df)
+        return df
+
+    @typechecked
     def learn(
         self,
         dataset: Dataset,
         inputs: List[str],
         outputs: List[str],
         num_loops: int,
         num_points_per_loop: int,
@@ -1286,15 +1371,15 @@
             dataset (Dataset): twinLab dataset object which contains the initial training data for the emulator.
             inputs (list[str]): List of input column names in the training dataset.
             outputs (list[str]): List of output column names in the training dataset.
             num_loops (int): Number of loops to run of the learning process. This must be a positive integer. Note that in this method, the emulator is trained and then re-trained on new suggested data points, so setting ``num_loops=1`` here will mean that ``Emulator.train`` is run _twice_, and ``Emulator.recommend`` is run once.
             num_points_per_loop (int): Number of points to sample in each loop.
             acq_func (str): Specifies the acquisition function to be used when recommending new points: either ``"explore"`` or ``"optimise"``.
             simulation (Callable): A function that takes in a set of inputs and generates the outputs (for example, a simulator for the data generating process).
-            train_params (TrainParams, optional): A parameter configuration that contains optional training parameters. Note that currently we only support the case when ``"test_train_ratio=1"`` when running a learning loop.
+            train_params (TrainParams, optional): A parameter configuration that contains optional training parameters. Note that currently we only support the case when ``"test_train_ratio=1"`` when running a learning loop. Note that fixed-noise Gaussian Processes are not supported in this method and will raise an error. This includes: ``"fixed_noise_gp"``, ``"heteroskedastic_gp"``, ``"fixed_noise_multi_fidelity_gp"``.
             recommend_params (RecommendParams, optional): A parameter configuration that contains optional recommendation parameters.
             verbose (bool, optional): Display detailed information about the operation while running. If ``True``, the requested candidate points will be printed to the screen while running. If ``False`` the emulator will be updated on the cloud while the method runs silently.
 
         Examples:
             .. code-block:: python
 
                 emulator = tl.Emulator("quickstart")
@@ -1307,23 +1392,35 @@
                     num_points_per_loop=5,
                     acq_func="explore",
                     simulation=my_simulator,
                 )
 
         """
 
+        # Perform checks
+        # NOTE: We could relax the train_test_ratio requirement in the future, but only easily with shuffle=False
+        # and only by changing the train_test_ratio each iteration so that the test set is preserved
         if train_params.train_test_ratio != 1:
             raise ValueError(
                 f"The test_train_ratio must be set to 1, not {train_params.train_test_ratio}, for this method to work."
             )
-
         if num_loops <= 0:
             raise ValueError(
                 f"num_loops must be set to an integer value of 1 or more, not {num_loops}, for this method to work."
             )
+        # NOTE: We could relax this in the future if we allowed for the simulation to output an error
+        invalid_GP_estimators = [
+            "fixed_noise_gp",
+            "heteroskedastic_gp",
+            "fixed_noise_multi_fidelity_gp",
+        ]
+        if train_params.estimator_params.estimator_type in invalid_GP_estimators:
+            raise ValueError(
+                f"The specified estimator type, {train_params.estimator_params.estimator_type}, is not currently supported. Please check the ``EstimatorParams`` documentation for more available estimator types."
+            )
 
         # Train model initially
         self.train(
             dataset=dataset,
             inputs=inputs,
             outputs=outputs,
             params=train_params,
@@ -1338,38 +1435,48 @@
                 num_points=num_points_per_loop,
                 acq_func=acq_func,
                 params=recommend_params,
                 verbose=False,
             )
 
             # Evaluating the candidate points
-            candidate_points[outputs] = pd.DataFrame(
-                simulation(candidate_points[inputs].values)
-            )
+            candidate_points[outputs] = simulation(candidate_points[inputs].values)
+
+            # Download current training data, append new data, and reupload
+            df_train = self.view_train_data()
+            df_train = pd.concat([df_train, candidate_points], ignore_index=True)
+            dataset.upload(df_train)
 
             # Train model
             self.train(
                 dataset=dataset,
                 inputs=inputs,
                 outputs=outputs,
                 params=train_params,
                 verbose=False,
             )
 
-            # Download current training data, append new data, and reupload
-            df_train = self.view_train_data()
-            df_train = pd.concat([df_train, candidate_points], ignore_index=True)
-            dataset.upload(df_train)
-
+            # Write summary of the iteration if verbose
             if verbose:
-                print(f"Iteration: {i}")
+                print(f"Iteration: {i+1}")
                 print("Suggested candidate point(s):")
                 pprint(candidate_points)
                 print("Acquisition function value:")
                 print(acq_func_value)
+                print()
+
+        # Print the estimated optimal point(s) after the final iteration if optimise and verbose
+        if verbose and acq_func == "optimise":
+            params = MaximizeParams(opt_weights=recommend_params.weights)
+            df_max = self.maximize(params=params, verbose=False)
+            print("Estimated optimal point(s):")
+            print(df_max)
+            print()
+
+        # A nice final message if verbose
         if verbose:
             print(
                 f"The candidate points have been uploaded in the Dataset {dataset.id}, alongside the emulator training data, on twinLab cloud."
             )
 
     @typechecked
     def delete(self, verbose: bool = False) -> None:
```

### Comparing `twinlab-2.6.1/twinlab/helper.py` & `twinlab-2.7.0/twinlab/helper.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/params.py` & `twinlab-2.7.0/twinlab/params.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 ESTIMATORS_WITHOUT_COVAR_MODULE = [
     "heteroskedastic_gp",
     "multi_fidelity_gp",
     "fixed_noise_multi_fidelity_gp",
     "mixed_single_task_gp",
 ]
 
+DEFAULT_SEED = 42
+
 
 def _check_estimator_type(estimator_type: str):
     # NOTE: This is necessary because the library defaults to `single_task_gp` if the estimator_type is not provided or wrong!
     if estimator_type not in ALLOWED_ESTIMATORS:
         raise ValueError(
             f"Estimator type {estimator_type} not recognised. Please choose from {ALLOWED_ESTIMATORS}."
         )
@@ -136,16 +138,16 @@
     Attributes:
         seed (Union[int, None], optional): Specifies the seed for the random number generator for every trial of the model selection process.
             Setting to an integer is necessary for reproducible results.
             The default value is ``None``, which means the seed is randomly generated each time.
         evaluation_metric (str, optional): Specifies the evaluation metric used to score different configuration during the model selection process.
             Can be either:
 
-            - ``"BIC"``: Bayesian information criterion.
             - ``"MSLL"``: Mean squared log loss.
+            - ``"BIC"``: Bayesian information criterion.
 
             The default is ``"MSLL"``.
         val_ratio (float, optional): Specifies the percentage of random validation data allocated to to compute the ``"BIC"`` metric.
             The default is ``0.2``.
         base_kernels (Union[str, Set[str]], optional): Specifies the set of individual kernels to use for compositional kernel search.
             Can be:
 
@@ -233,17 +235,20 @@
             The default value is 1, which means that all of the provided data is used for training.
             This is good to make the most out of a dataset, but means that it will not be possible to score or benchmark the performance of an emulator.
         dataset_std (Union[Dataset, None], optional): A twinLab dataset object that contains the standard deviation of the training data.
             This is necessary when training a heteroskedastic or fixed noise Gaussian Process.
         model_selection (bool, optional): Whether to run Bayesian model selection, a form of automatic machine learning.
             The default value is ``False``, which simply trains the specified emulator, rather than iterating over them.
         model_selection_params (ModelSelectionParams, optional): The parameters for model selection, if it is being used.
+        shuffle (bool, optional): Whether to randomly shuffle the training data before splitting it into training and testing sets.
+            The default value is ``True``. Please be particularly careful while using this parameter with time-series data.
         seed (Union[int, None], optional): The seed used to initialise the random number generators for reproducibility.
             Setting to an integer is necessary for reproducible results.
-            The default value is ``None``, which means the seed is randomly generated each time.
+            The default value is ``42``, but it can be set to ``None`` to randomly generate the seed each time.
+            Be aware that the seed is used in the training process, so if the seed is set to ``None`` the training process will not be reproducible.
 
     """
 
     def __init__(
         self,
         estimator: str = "gaussian_process_regression",
         estimator_params: EstimatorParams = EstimatorParams(),
@@ -252,15 +257,16 @@
         output_explained_variance: Optional[float] = None,
         output_retained_dimensions: Optional[int] = None,
         fidelity: Optional[str] = None,
         dataset_std: Optional[Dataset] = None,
         train_test_ratio: float = 1.0,
         model_selection: bool = False,
         model_selection_params: ModelSelectionParams = ModelSelectionParams(),
-        seed: Optional[int] = None,
+        shuffle: bool = True,
+        seed: Optional[int] = DEFAULT_SEED,
     ):
         # Parameters that will be passed to the emulator on construction
         self.fidelity = fidelity
         self.estimator = estimator
         self.estimator_params = estimator_params
         self.input_explained_variance = input_explained_variance
         self.input_retained_dimensions = input_retained_dimensions
@@ -268,14 +274,15 @@
         self.output_retained_dimensions = output_retained_dimensions
 
         # Parameters that will be passed to the emulator.fit() method
         self.dataset_std = dataset_std
         self.train_test_ratio = train_test_ratio
         self.model_selection = model_selection
         self.model_selection_params = model_selection_params
+        self.shuffle = shuffle
         self.seed = seed
 
         # Figure out whether or not to set decompose booleans
         def decompose(
             explained_variance: Optional[float],
             retained_dimensions: Optional[int],
         ) -> bool:
@@ -309,14 +316,15 @@
             "output_retained_dimensions": self.output_retained_dimensions,
         }
         setup_params = remove_none_values(setup_params)
         train_params = {  # Pass to campaign.fit() in the library
             "train_test_ratio": self.train_test_ratio,
             "model_selection": self.model_selection,
             "model_selection_kwargs": self.model_selection_params.unpack_parameters(),
+            "shuffle": self.shuffle,
             "seed": self.seed,
         }
         train_params = remove_none_values(train_params)
         if self.dataset_std is not None:
             train_params["dataset_std_id"] = self.dataset_std.id
         params = {**setup_params, **train_params}
         return params
@@ -326,25 +334,38 @@
 class ScoreParams(Params):
     """Parameter configuration for scoring a trained emulator.
 
     Attributes:
         metric (str, optional): Metric used for scoring the performance of an emulator.
             Can be one of:
 
-            - ``"MSLL"``: Mean Squared Log Loss, which compares the distribution of the emulator prediction to that of the test data.
-              A score of zero is that of the most naive data-generating model, which predicts the mean and standard deviation of the training data.
-              Lower (more negative) scores are better, while positive scores indicate serious problems.
-            - ``"MSE"``: Mean Squared Error, which only compares the mean emulator prediction to the test data.
-
-            The default is ``"MSLL"``.
-        combined_score (bool, optional): Determining whether to combined (average) the emulator score across output dimensions.
-            If ``False`` a dataframe of scores will be returned, with the score for each output dimension, even if there is only a single emulator output dimension.
-            If ``True`` a single number will be returned, which is the average score across all output dimensions.
+            - "MSLL": The mean standardised log loss (MSLL), calculated as the mean of the log loss of the emulator minus the mean log loss of a trivial model.
+              The log loss is defined as the negative log of the probability of getting the test data value according to a predicted distribution.
+              The trivial model is taken to be a Gaussian distribution with mean and standard deviation equal to those of the training data.
+              Lower (more negative) scores are better, while positive scores indicate serious problems (a model that is less good than the extremely-trivial naive model).
+              The MSLL can be thought of as a measure of how good a model is, as opposed to just taking the average and standard deviation of the training data.
+              This is the default metric, and the only metric that accounts for the model uncertainty, which is usually necessary when training a probabilistic model.
+            - "MSE": The mean squared error (MSE) is the average of the squared differences between your predicted mean values and those of the test set.
+              The MSE quantifies deviations in the model mean predictions only, and is not affected by the model uncertainty estimates.
+              A value of zero indicates a model that fits to the data perfectly, but this is not necessarily desirable, as it may indicate overfitting.
+            - "RMSE": The root mean squared error (RMSE) is the square root of the MSE and provides a measure of the expected error in the output.
+              The RMSE may be considered more interpretable than the MSE, because it shares the same units as the output values.
+              However, like the MSE and R2, since model uncertainty is not apart of how this metric is calculated, a desirable RMSE score may belie an underlying poorly-fitting model.
+            - "R2": A dimensionless number calculated as one minus the ratio of the MSE to the variance of the test set.
+              A value of 1 indicates a perfect model, while a value of 0 indicates a model that is no better than the mean of the test set.
+              Negative values are possible but unusual, and indicate a model that is worse than simply taking the mean of the test set.
+              As with MSE and RMSE, the model uncertainty is not accounted for in this score; thus, it is possible to have a high R2 score, but a poorly-fitting model.
+
+            The default metric is "MSLL".
+
+        combined_score (bool, optional): Determine whether to combine (average) the emulator score across output dimensions.
+            If False, a dataframe of scores will be returned, with the score for each output dimension,
+            even if there is only a single emulator output dimension.
+            If True, a single number will be returned, which is the average score across all output dimensions.
             The default is ``False``.
-
     """
 
     def __init__(
         self,
         metric: str = "MSLL",
         combined_score: bool = False,
     ):
@@ -360,24 +381,35 @@
 
 
 class BenchmarkParams(Params):
     """Parameter configuration for benchmarking a trained emulator.
 
     Attributes:
         type (str, optional): Specifies the type of emulator benchmark to be performed.
-            Can be either:
+            Can be one of:
 
-            - ``"quantile"``: The calibration curve is calculated over Gaussian quantiles.
-            - ``"interval"``: The calibration curve is calculated over Gaussian confidence intervals.
+            - ``"quantile"``: The calibration curve is calculated over statistical quantiles.
+            - ``"interval"``: The calibration curve is calculated over confidence intervals.
 
             The default is ``"quantile"``.
 
-    """
+        For example, for a well calibrated emulator one would expect to have 10 percent of the unseen datapoints (from the test set) to be outside of the emulator's 90 percent confidence bound.
+        If a given confidence interval contains less than expected amount of data the model is underconfident, whereas if it contains more then it is overconfident.
+        The calibration curve is necessarily equal to ``0`` and ``1`` at the beginning and end respectively, as the fraction of data within the entire confidence interval must be between 0 and 1.
+        Curves are also necessarily monotonically increasing.
+        Convex calibration curves (those below the line ``y = x``) indicate that the model is underconfident,
+        while concave calibration curves (those above the line ``y = x``) indicate that the model is overconfident.
+        It is possible for a curve to be both above and below the line ``y = x``, indicating regions of under- and overconfidence, and possible non-Gaussianity in the data.
 
-    # TODO: This docstring needs to be massively improved.
+        If ``type = "quantile"`` then the calibration curve is calculated over statistical quantiles extending from negative infinity to positive infinity.
+
+        If ``type = "interval"`` then the calibration curve is calculated over confidence intervals,
+        starting from the mean of the distribution and extending outwards in both directions simultaneously until the entire confidence interval is covered at negative/positive infinity.
+
+    """
 
     def __init__(
         self,
         type: str = "quantile",
     ):
         self.type = type
 
@@ -387,15 +419,15 @@
 
 
 @typechecked
 class PredictParams(Params):
     """Parameter configuration for making predictions using a trained emulator.
 
     Attributes:
-        observation_noise (bool, optional): Whether or not to include the noise term in the standard deviation of the prediction.
+        observation_noise (bool): Whether or not to include the noise term in the standard deviation of the prediction.
             Setting this to ``False`` can be a good idea if the training data is noisy but the underlying trend of the trained model is smooth.
             In this case, the predictions would correspond to the underlying trend.
             Setting this to ``True`` can be a good idea to see the spread of possible predictions including the noise.
             This is useful to know the true uncertainty in the data-generation process, and to estimate the true span of values that might be observed next.
             The default value is ``True``.
 
     """
@@ -415,32 +447,45 @@
 class SampleParams(Params):
     """Parameter configuration for sampling from a trained emulator.
 
     Attributes:
         seed (Union[int, None], optional): Specifies the seed used by the random number generator to generate a set of samples.
             Setting this to an integer is useful for the reproducibility of results.
             The default value is ``None``, which means the seed is randomly generated each time.
+        observation_noise (bool): Whether or not to include the noise term in the standard deviation of the samples generated.
+            Setting this to ``False`` can be a good idea if the training data is noisy but the underlying trend of the trained model is smooth.
+            In this case, the samples would look smooth and would model the underlying trend well.
+            Setting this to ``True`` can be a good idea to visualise how noisy are the samples from the emulator, which is a consequence of the noise in the observations.
+            The default value is ``False``.
         fidelity (Union[pandas.DataFrame, None], optional): Fidelity information to be provided if the model is a multi-fidelity model (``estimator_type="multi_fidelity_gp"`` in ``EstimatorParams``).
             This must be a single column `pandas.DataFrame` with the same sample order as the dataframe of X values used to draw samples.
             The default value is ``None``, which is appropriate for most trained emulators.
 
     """
 
     # TODO: Does the fidelity parameter need to be between 0 and 1?
 
     def __init__(
         self,
         seed: Optional[int] = None,
+        observation_noise: bool = False,
         fidelity: Optional[pd.DataFrame] = None,
     ):
         self.seed = seed
+        self.observation_noise = observation_noise
         self.fidelity = fidelity
 
     def unpack_parameters(self):
-        params = {"kwargs": {"seed": self.seed, "fidelity": self.fidelity}}
+        params = {
+            "kwargs": {
+                "seed": self.seed,
+                "observation_noise": self.observation_noise,
+                "fidelity": self.fidelity,
+            }
+        }
         params = remove_none_values(params)
         if "fidelity" in params["kwargs"]:
             params["kwargs"]["fidelity"] = _convert_dataframe_to_dict(
                 params["kwargs"], "fidelity"
             )
         return params
 
@@ -465,16 +510,27 @@
 
 @typechecked
 class RecommendParams(Params):
     """Parameter configuration for recommending new points to sample using the Bayesian-optimisation routine.
 
     Attributes:
         weights (Union[list[float], None], optional):
-            A list of weighting values that are used to scalarise the objective function in the case of a multi-output model.
-            The default value is ``None``, which applies equal weight to each output dimension.
+            A list of weighting values that are used to create a scalar objective function in the case of a multi-output model.
+            The recommend functionality can only work on a single scalar function, so in the case of a multi-output model, the outputs must be combined into a single scalar value.
+            The weights create a linear combinations of the outputs, where the weights are the coefficients of the linear combination.
+            In the case of a single-output model, the weights are not used and have no impact.
+            If the output dimensions are not equally important, the weights can be used to reflect this.
+            If the output values have different units, the weights must be chosen to reflect this.
+            For example, if two outputs have units of distance and time the weights implicitly have units such that these can be combined (i.e., per metre and per second).
+            A list of values is used here, where the first value corresponds to the first output, the second value to the second output, and so on.
+            For example, ``[1, 2, 3]`` would create a linear combination of the outputs where the first output is multiplied by 1, the second output by 2, and the third output by 3.
+            In this case, the third output is considered to be three times as important as the first output.
+            If the values ``[0, 1]`` are used, the first output is ignored and the second output is used as the scalar objective function.
+            If the values ``[-1, 0]`` are used, the first output is used as the scalar objective function, and is minimized.
+            The default value, ``None``, applies equal weight to each output dimension. This is recommended for functional emulators.
         num_restarts (int, optional): The number of random restarts for optimisation.
             The default value is ``5``.
         raw_samples (int, optional): The number of samples for initialization.
             The default value is ``128``.
         bounds (Union[Tuple, None], optional): The bounds of the input space.
             If this is set to `None` then the bounds are inferred from the range of the training data.
             Otherwise, this must be a dictionary mapping column names to a tuple of lower and upper bounds.
@@ -623,7 +679,39 @@
     def __init__(
         self,
         sampling_method: Sampling = LatinHypercube(),
         seed: Optional[int] = None,
     ):
         self.seed = seed
         self.sampling_method = sampling_method
+
+
+class MaximizeParams(Params):
+    """Parameter configuration for finding the location of the maximum output of your emulator.
+
+    Attributes:
+        opt_weights (Union[List[float], None], optional): A list of weighting values that are used to create a scalar objective function in the case of a multi-output model.
+            The maximize functionality can only work on a single scalar function, so in the case of a multi-output model, the outputs must be combined into a single scalar value.
+            The weights create a linear combinations of the outputs, where the weights are the coefficients of the linear combination.
+            In the case of a single-output model, the weights are not used and have no impact.
+            If the output dimensions are not equally important, the weights can be used to reflect this.
+            If the output values have different units, the weights must be chosen to reflect this.
+            For example, if two outputs have units of distance and time the weights implicitly have units such that these can be combined (i.e., per metre and per second).
+            A list of values is used here, where the first value corresponds to the first output, the second value to the second output, and so on.
+            For example, ``[1, 2, 3]`` would create a linear combination of the outputs where the first output is multiplied by 1, the second output by 2, and the third output by 3.
+            In this case, the third output is considered to be three times as important as the first output.
+            If the values ``[0, 1]`` are used, the first output is ignored and the second output is used as the scalar objective function.
+            If the values ``[-1, 0]`` are used, the first output is used as the scalar objective function, and is minimized.
+            The default value, ``None``, applies equal weight to each output dimension. This is recommended for functional emulators.
+
+    """
+
+    def __init__(
+        self,
+        opt_weights: Optional[List[float]] = None,
+    ):
+        self.opt_weights = opt_weights
+
+    def unpack_parameters(self):
+        params = {"opt_weights": self.opt_weights}
+        params = remove_none_values(params)
+        return params
```

### Comparing `twinlab-2.6.1/twinlab/plotting.py` & `twinlab-2.7.0/twinlab/plotting.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/prior.py` & `twinlab-2.7.0/twinlab/prior.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/sampling.py` & `twinlab-2.7.0/twinlab/sampling.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/settings.py` & `twinlab-2.7.0/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/twinlab/utils.py` & `twinlab-2.7.0/twinlab/utils.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.6.1/PKG-INFO` & `twinlab-2.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 2.6.1
+Version: 2.7.0
 Summary: twinLab - Probabilistic Machine Learning for Engineers
 Home-page: https://twinlab.ai
 License: MIT
 Keywords: machine-learning,AI,cloud,twinLab,digiLab
 Author: digiLab Solutions Ltd.
-Author-email: info@digilab.co.uk
-Maintainer: Alexander Mead
-Maintainer-email: alexander@digilab.co.uk
+Author-email: twinlab@digilab.co.uk
+Maintainer: twinLab Product Team
+Maintainer-email: twinlab@digilab.co.uk
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: matplotlib (>=3.7)
 Requires-Dist: numpy (>=1.24,<2.0) ; python_version >= "3.8" and python_version < "3.9"
 Requires-Dist: numpy (>=1.26,<2.0) ; python_version >= "3.9" and python_version < "3.13"
 Requires-Dist: pandas (>=1.5.3,<2.0.0) ; python_version >= "3.8" and python_version < "3.9"
-Requires-Dist: pandas (>=2.0,<3.0) ; python_version >= "3.9" and python_version < "3.13"
+Requires-Dist: pandas (>=2.0.3,<2.1.0) ; python_version >= "3.9" and python_version < "3.13"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: setuptools (>=69.0.2,<70.0.0)
 Requires-Dist: typeguard (>=4.0.0,<5.0.0)
 Project-URL: Documentation, https://twinlab.ai
 Description-Content-Type: text/markdown
```

