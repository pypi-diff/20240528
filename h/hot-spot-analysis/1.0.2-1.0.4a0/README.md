# Comparing `tmp/hot_spot_analysis-1.0.2.tar.gz` & `tmp/hot_spot_analysis-1.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hot_spot_analysis-1.0.2.tar", max compression
+gzip compressed data, was "hot_spot_analysis-1.0.4a0.tar", last modified: Tue May 28 05:15:46 2024, max compression
```

## Comparing `hot_spot_analysis-1.0.2.tar` & `hot_spot_analysis-1.0.4a0.tar`

### file list

```diff
@@ -1,13 +1,33 @@
--rw-r--r--   0        0        0     1068 2023-04-08 19:09:05.390182 hot_spot_analysis-1.0.2/LICENSE
--rw-r--r--   0        0        0     5164 2023-04-08 19:09:05.390418 hot_spot_analysis-1.0.2/README.md
--rw-r--r--   0        0        0      512 2024-05-19 23:16:33.144203 hot_spot_analysis-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 21:29:20.208895 hot_spot_analysis-1.0.2/src/hot_spot_analysis/__init__.py
--rw-r--r--   0        0        0    16706 2024-05-19 23:15:25.854133 hot_spot_analysis-1.0.2/src/hot_spot_analysis/hot_spot_analysis.py
--rw-r--r--   0        0        0        0 2024-05-15 21:29:20.211324 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/__init__.py
--rw-r--r--   0        0        0       66 2024-05-15 21:29:20.211724 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/analyze.py
--rw-r--r--   0        0        0     1230 2024-05-15 21:29:20.212762 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/combos.py
--rw-r--r--   0        0        0      454 2024-05-15 21:29:20.213727 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/demo.py
--rw-r--r--   0        0        0      717 2024-05-15 21:29:20.214515 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/general.py
--rw-r--r--   0        0        0     1654 2024-05-15 21:29:20.215885 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/grouped_df.py
--rw-r--r--   0        0        0     3032 2024-05-15 21:29:20.216918 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/lists.py
--rw-r--r--   0        0        0     5909 1970-01-01 00:00:00.000000 hot_spot_analysis-1.0.2/PKG-INFO
+drwxr-xr-x   0 philipgundy   (501) staff       (20)        0 2024-05-28 05:15:46.092060 hot_spot_analysis-1.0.4a0/
+-rw-r--r--   0 philipgundy   (501) staff       (20)     1068 2024-05-25 22:50:01.000000 hot_spot_analysis-1.0.4a0/LICENSE
+-rw-r--r--   0 philipgundy   (501) staff       (20)     3039 2024-05-28 05:15:46.091837 hot_spot_analysis-1.0.4a0/PKG-INFO
+-rw-r--r--   0 philipgundy   (501) staff       (20)     2316 2024-05-27 23:05:14.000000 hot_spot_analysis-1.0.4a0/README.md
+-rw-r--r--   0 philipgundy   (501) staff       (20)     1016 2024-05-28 05:15:33.000000 hot_spot_analysis-1.0.4a0/pyproject.toml
+-rw-r--r--   0 philipgundy   (501) staff       (20)       38 2024-05-28 05:15:46.092095 hot_spot_analysis-1.0.4a0/setup.cfg
+drwxr-xr-x   0 philipgundy   (501) staff       (20)        0 2024-05-28 05:15:46.088075 hot_spot_analysis-1.0.4a0/src/
+drwxr-xr-x   0 philipgundy   (501) staff       (20)        0 2024-05-28 05:15:46.088955 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/
+-rw-r--r--   0 philipgundy   (501) staff       (20)        0 2024-05-27 07:39:38.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/__init__.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)    15382 2024-05-27 16:34:43.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/hot_spot_analysis.py
+drwxr-xr-x   0 philipgundy   (501) staff       (20)        0 2024-05-28 05:15:46.090538 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/
+-rw-r--r--   0 philipgundy   (501) staff       (20)        0 2024-05-27 07:39:38.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/__init__.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)       66 2024-05-27 07:39:38.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/analyze.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)     1028 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/combos.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)      840 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/demo.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)     1064 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/general.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)     1901 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/grouped_df.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)     3473 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/lists.py
+drwxr-xr-x   0 philipgundy   (501) staff       (20)        0 2024-05-28 05:15:46.091628 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis.egg-info/
+-rw-r--r--   0 philipgundy   (501) staff       (20)     3039 2024-05-28 05:15:46.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 philipgundy   (501) staff       (20)      813 2024-05-28 05:15:46.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 philipgundy   (501) staff       (20)        1 2024-05-28 05:15:46.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 philipgundy   (501) staff       (20)       90 2024-05-28 05:15:46.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 philipgundy   (501) staff       (20)       26 2024-05-28 05:15:46.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis.egg-info/requires.txt
+-rw-r--r--   0 philipgundy   (501) staff       (20)       18 2024-05-28 05:15:46.000000 hot_spot_analysis-1.0.4a0/src/hot_spot_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 philipgundy   (501) staff       (20)        0 2024-05-28 05:15:46.091468 hot_spot_analysis-1.0.4a0/tests/
+-rw-r--r--   0 philipgundy   (501) staff       (20)        0 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/tests/test_analyze.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)      966 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/tests/test_combos.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)      787 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/tests/test_demo.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)      892 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/tests/test_general.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)     2611 2024-05-27 23:45:57.000000 hot_spot_analysis-1.0.4a0/tests/test_grouped_df.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)     2604 2024-05-27 23:42:51.000000 hot_spot_analysis-1.0.4a0/tests/test_hot_spot_analysis.py
+-rw-r--r--   0 philipgundy   (501) staff       (20)     1411 2024-05-27 07:40:08.000000 hot_spot_analysis-1.0.4a0/tests/test_lists.py
```

### Comparing `hot_spot_analysis-1.0.2/LICENSE` & `hot_spot_analysis-1.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `hot_spot_analysis-1.0.2/src/hot_spot_analysis/hot_spot_analysis.py` & `hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/hot_spot_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-# %%
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional
+from typing import Callable
 
 import numpy as np
 import pandas as pd
-import seaborn as sns
-from utils import combos, demo, general, grouped_df, lists
+
+from hot_spot_analysis.utils import combos, general, grouped_df, lists
 
 
-# %%
 @dataclass
 class HotSpotAnalysis:
     """
     _summary_ TODO
     fdsfsd
     """
 
-    # data: pd.DataFrame
-    # target_cols: list[str]
-    # interaction_limit: int
-    # objective_function: Callable
+    data: pd.DataFrame
+    target_cols: list[str]
+    interaction_limit: int
+    objective_function: Callable
 
     def __init__(
         self,  # Default values
-        objective_function: Callable,
         data: pd.DataFrame = pd.DataFrame(None),  # HSA.data.empty -> True
-        target_cols: List[Any] = [None],  # []
-        interaction_limit: int = 3,
-        time_period: List[Any] = [None],  # []
+        target_cols: list = [None],  # []
+        time_period: list = [None],  # []
+        interaction_limit: int = 3,  # 3
+        objective_function: Callable = None,
     ):
-        self.objective_function = objective_function
         self.data_input = data
         self.target_cols = lists.unique(target_cols, drop_none=True)
-        self.interaction_limit = interaction_limit
         self.time_period = lists.unique(time_period, drop_none=True)
+        self.interaction_limit = interaction_limit
+        self.objective_function = objective_function
 
         # Set defaults for variables set via functions
-        self.grouped_by: List[Any] = []
+        self.grouped_by: list[str] = None
         self.data_prep: pd.DataFrame = pd.DataFrame(None)
-        self.combinations: List[List[Any]] = []
+        self.combinations: list[list[str]] = None
         self.obj_func_tested: bool = False
-        self.hsa_raw_output_dicts: List[Dict] = []
+        self.hsa_raw_output_dicts: list[dict] = None
         self.hsa_output_df: pd.DataFrame = pd.DataFrame(None)
 
     def prep_class(self):
         """Extract any groups & the dataframe from the init"""
         self.data_prep = grouped_df.return_data(self.data_input)
 
         if grouped_df.is_grouped(self.data_input):
@@ -58,15 +56,15 @@
         elif validate == "time_period":
             if not self.time_period:
                 return
             input_to_validate = self.time_period
         else:
             raise ValueError("validate must be either: 'target_cols' or 'time_period")
 
-        valid_inputs = list(self.data_prep.columns)
+        valid_inputs = self.data_prep.columns
 
         valid_columns_bools = lists.find_items(
             input_to_validate,
             valid_inputs,
             return_bools=True,
         )
 
@@ -92,15 +90,15 @@
         combinations = combos.create_combos(
             target_cols=self.target_cols,
             interaction_max=self.interaction_limit,
         )
 
         combinations = [["Overall"]] + combinations
 
-        if not self.grouped_by:
+        if self.grouped_by is not None:
             # If the input data is grouped we add the groups!
             combinations = grouped_df.add_groups_to_combos(
                 group_vars=self.grouped_by,
                 combos=combinations,
             )
 
         if self.time_period:
@@ -140,15 +138,15 @@
                 f"Using random sample of {row_limit} rows. Note that rows will be recycled to meet row_limit if data has insufficient rows."
             )
 
         test_df = self.data_prep.sample(row_limit, replace=True)
 
         try:
             output = self.objective_function(test_df.groupby("Overall"))
-        except Exception:
+        except:
             raise ValueError(
                 "The function supplied to 'objective_function' is not compatible\n\nThe function must be able to run on a grouped data frame."
             )
 
         self.obj_func_tested = True
         if verbose:
             return output
@@ -159,47 +157,48 @@
         self._build_combos()
         if not self.obj_func_tested:
             self.test_objective_function(verbose=False)
 
     def run_obj_func_iterations(self):
         self.prep_analysis()
 
-        print("\n")
+        if self.hsa_raw_output_dicts is not None:
+            print("The objective function has already been run.")
+
         combination_outputs = []
+        print("\n")
         for step_i, combo in enumerate(self.combinations):
             print(f"\tstep: {step_i} group by {combo}")
             df_grp_by_combo = self.data_prep.groupby(combo, observed=True)
             df_combo_output = self.objective_function(df_grp_by_combo)
 
-            df_grp_nrows = grouped_df.group_sizes(df_grp_by_combo)
+            df_grp_nrows = df_grp_by_combo.size().reset_index(name="n_rows")
 
             combination_output_df = df_grp_nrows.merge(df_combo_output, on=combo)
 
             if "Overall" in combo:
                 interaction_count = len(combo) - 1
             else:
                 interaction_count = len(combo)
 
             combination_output = {
                 "combination": combo,
                 "interaction_count": interaction_count,
                 "df": combination_output_df.reset_index(drop=True),
             }
             combination_outputs.append(combination_output)
-            if step_i == len(self.combinations):
-                print("\nAll combinations have been run.")
-
+        print("\n")
         self.hsa_raw_output_dicts = combination_outputs
 
     def process_hsa_raw_output_dicts(self):
         if not self.hsa_output_df.empty:
             print("The HSA data output already exsists.")
             return
 
-        if not self.hsa_raw_output_dicts:
+        if self.hsa_raw_output_dicts is None:
             self.run_obj_func_iterations()
 
         combo_dfs = []
         for row_i, _ in enumerate(self.hsa_raw_output_dicts):
             combo_i_dict = self.hsa_raw_output_dicts[row_i]
 
             combo_i_combination = combo_i_dict["combination"]
@@ -209,20 +208,19 @@
             combo_i_df_obj_func_calcs = lists.find_items(
                 combo_i_df.columns,
                 combo_i_combination,
                 return_matching=False,
             )
 
             #! Xform keys & values into a dict, and drop keys & values
-            combo_i_df["combo_keys"] = pd.Series(
-                [combo_i_combination] * len(combo_i_df)
-            )
+            combo_i_df["combo_keys"] = pd.Series([combo_i_combination] * len(combo_i_df))
             combo_i_df["combo_values"] = combo_i_df[combo_i_combination].apply(
                 lambda row: list(row.values.astype(str)),
                 axis=1,
+                # ??lambda row: list(row.values), axis=1
             )
             combo_i_df["combo_dict"] = lists.lists_to_dict(
                 combo_i_df["combo_keys"],
                 combo_i_df["combo_values"],
             )
 
             combo_i_df.drop(
@@ -249,27 +247,25 @@
         self.hsa_output_df = hsa_df
 
     def pop_key_off_combo_dict(self, pop_type=None):
         #!! move into process_hsa_raw_output_dicts() at end
         # TODO: once moved add a condition that the following var is not None
 
         if pop_type == "grouped_by":
-            if not self.grouped_by:
+            if self.grouped_by is None:
                 return
             pop_key = self.grouped_by
             pop_dict = "grouped_by_dict"
         elif pop_type == "time_period":
             if not self.time_period:
                 return
             pop_key = self.time_period
             pop_dict = "time_period_dict"
         else:
-            raise ValueError(
-                "Invalid pop_type. Must be either: 'grouped_by' or 'time_period'"
-            )
+            raise ValueError("Invalid pop_type. Must be either: 'grouped_by' or 'time_period'")
 
         popped_dicts = []
         for _, combo_dict_i in enumerate(self.hsa_output_df["combo_dict"]):
             popped_dict = general.pop_keys(combo_dict_i, pop_key)
             popped_dicts.append(popped_dict)
 
         self.hsa_output_df[pop_dict] = popped_dicts
@@ -299,26 +295,24 @@
 
         df = self.hsa_output_df.copy()
 
         lag_across = ", ".join(self.time_period)
         print(f"Attempting to lag data across: {lag_across}")
 
         dict_columns = ["combo_dict"]
-        if not self.grouped_by:
+        if self.grouped_by is not None:
             dict_columns = ["grouped_by_dict"] + dict_columns
         for dict_column in dict_columns:
             df[dict_column] = general.dict_to_json(df[dict_column])
 
         # Loop through the lags & merge them back into df.
         df_baseline = df.copy()  # copy() is required to keep the objects separate
         for lag_i in lag_iterations:
             print(f"Running lag: {lag_i}")
-            df_lag_i = df_baseline.groupby(["combo_dict", "interaction_count"]).shift(
-                lag_i
-            )
+            df_lag_i = df_baseline.groupby(["combo_dict", "interaction_count"]).shift(lag_i)
 
             df = df.merge(
                 df_lag_i,
                 how="left",
                 left_index=True,
                 right_index=True,
                 suffixes=("", f"_lag{lag_i}"),
@@ -327,58 +321,48 @@
         for dict_column in dict_columns:
             df[dict_column] = general.json_to_dict(df[dict_column])
 
         return df
 
     def export_hsa_output_df(self):
         if self.hsa_output_df.empty:
-            raise ValueError(
-                "hsa_output_df is not defined. Try: running run_hsa() then use this command."
-            )
+            raise ValueError("hsa_output_df is not defined. Try: running run_hsa() then use this command.")
         return self.hsa_output_df
 
     def search_hsa_output(
         self,
         hsa_df: pd.DataFrame = pd.DataFrame(None),
         search_terms: str | list[str] = None,
         search_across: str = "keys",
         search_type: str = "any",
         interactions: int | list[int] = [0],  # default defined below
         n_row_minimum: int = 0,
     ):
-        # TODO: add check to see if 'self.hsa_output_df' is defined.
         if hsa_df.empty:
-            if HSA.hsa_output_df.empty:
+            if self.hsa_output_df.empty:
                 raise UserWarning("You must first run: run_hsa()")
             hsa_df = self.hsa_output_df.copy()
 
         if isinstance(interactions, int):
             interactions = [interactions]
         if interactions == [0]:
             # default to all possible interactions
             interactions = list(np.arange(self.interaction_limit) + 1)
 
-        df = hsa_df[
-            (hsa_df["interaction_count"].isin(interactions))
-            & (hsa_df["n_rows"] >= n_row_minimum)
-        ].copy()
+        df = hsa_df[(hsa_df["interaction_count"].isin(interactions)) & (hsa_df["n_rows"] >= n_row_minimum)].copy()
         df.reset_index(inplace=True, drop=True)
 
         has_grouped_by_dict = "grouped_by_dict" in df.columns
         has_time_period_dict = "time_period_dict" in df.columns
 
         df["hsa_dict"] = df["combo_dict"]
         if has_grouped_by_dict:
-            df["hsa_dict"] = lists.zip_lists_of_dicts(
-                df["grouped_by_dict"], df["hsa_dict"]
-            )
+            df["hsa_dict"] = lists.zip_lists_of_dicts(df["grouped_by_dict"], df["hsa_dict"])
         if has_time_period_dict:
-            df["hsa_dict"] = lists.zip_lists_of_dicts(
-                df["time_period_dict"], df["hsa_dict"]
-            )
+            df["hsa_dict"] = lists.zip_lists_of_dicts(df["time_period_dict"], df["hsa_dict"])
 
         if isinstance(search_terms, str):
             search_terms = [search_terms]
         search_terms = sorted(search_terms)
 
         #! START - TODO: migrate the following into a util func
         search_types = ["any", "all"]
@@ -396,18 +380,15 @@
             search_vector = [list(x.values()) for x in df["hsa_dict"]]
         else:
             raise ValueError("search_across must be either: 'keys' or 'values'")
 
         if search_type == "all":
             search_results_bool = [search_terms == sorted(x) for x in search_vector]
         else:
-            search_results_interim = [
-                lists.find_items(search_terms, x, return_bools=True)
-                for x in search_vector
-            ]
+            search_results_interim = [lists.find_items(search_terms, x, return_bools=True) for x in search_vector]
             search_results_bool = [any(x) for x in search_results_interim]
 
         search_results = df[search_results_bool]
 
         # If we have valid results return them else
         if len(search_results) > 0:
             return search_results.drop(columns="hsa_dict")
@@ -433,50 +414,7 @@
                 + f"search_type: '{search_type}' of the search_terms"
                 + "\n\t"
                 + f"interactions: {msg_interactions}"
                 + "\n\t"
                 + f"n_row_minimum: {n_row_minimum}"
             )
             raise ValueError(search_failed_helper)
-
-
-# %%
-
-if __name__ == "__main__":
-
-    df_tips = demo.data_stacker(
-        # Here we artificially create more rows
-        df=sns.load_dataset("tips"),
-        stack_count=50,
-    )
-
-    df_tips.info()
-
-    #! Feature construction + aggregation function!
-    df_tips["tip_perc"] = df_tips["tip"] / df_tips["total_bill"]
-
-    def tip_stats(data: pd.DataFrame) -> pd.DataFrame:
-        """fake"""
-        tmp = data.agg(
-            #!count_tips=pd.NamedAgg("tip", "count"),
-            avg_tips=pd.NamedAgg("tip", "mean"),
-            avg_tip_perc=pd.NamedAgg("tip_perc", "mean"),
-        ).round(2)
-
-        return tmp
-
-    HSA = HotSpotAnalysis(
-        objective_function=tip_stats,
-        data=df_tips,
-        # data=df_tips.groupby("sex", observed=True),
-        target_cols=["day", "smoker", "size"],
-        # time_period=["timestamp"],
-        interaction_limit=3,
-    )
-
-    # HSA.prep_analysis()
-    # HSA.test_objective_function(verbose=False)
-    HSA.run_hsa()
-    hsa_data = HSA.export_hsa_output_df()
-    print(hsa_data.tail(25))
-
-# %%
```

### Comparing `hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/combos.py` & `hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/combos.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,25 @@
-"""
-functions that handle the combinations to reduce code complexity elsewhere
-"""
-
 import itertools
-from typing import Any, List
-
-import numpy as np
+from typing import List
 
 
-def create_combos(target_cols: List[str], interaction_max: int = 3) -> List[List[Any]]:
-    """Build the combinations of target_cols for 0->interaction_max
+def create_combos(target_cols: List[str], interaction_max: int = 3) -> List[List[str]]:
+    """Build combinations of target_cols for interactions from 0 to interaction_max.
 
     Args:
-        target_cols: _description_
-        interaction_max: limits interactions. Defaults to 3.
+        target_cols (List[str]): List of column names to combine.
+        interaction_max (int, optional): Maximum number of interactions. Defaults to 3.
 
     Returns:
-        list[str]: target_cols for combination lengths 0->interaction_max
+        List[List[str]]: List of combinations of target_cols for interaction lengths from 0 to interaction_max.
     """
-    combos_nested = []  # 1 layer more nested than combos_final
-    combos_final: list[list[str]] = []
-
-    def combo_interaction_i(interactions: int):
-        """
-        Build combos with 1->X interactions
-        """
-        combo_interim = []
-        for combo in itertools.combinations(target_cols, interactions):
-            combo_interim.append(list(combo))
-        return combo_interim
-
-    for interaction_i in np.arange(interaction_max) + 1:
-        # Build combinations up through the interaction max
-        combos = combo_interaction_i(interaction_i)
-        combos_nested.append(combos)
+    combos_final: List[List[str]] = []
 
-    # Now convert the
+    # Helper function to generate combinations with a specified number of interactions
+    def generate_combinations(interactions: int) -> List[List[str]]:
+        return [list(combo) for combo in itertools.combinations(target_cols, interactions)]
+
+    # Generate combinations for each interaction level up to interaction_max
+    for interaction_i in range(1, interaction_max + 1):
+        combos_final.extend(generate_combinations(interaction_i))
 
-    combos_final = list(itertools.chain.from_iterable(combos_nested))
     return combos_final
```

### Comparing `hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/general.py` & `hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/general.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,43 @@
-"""Below are functions that don't fit into one of the other util themes"""
-
 import json
 
 
-def pop_keys(dictionary, keys):
+def pop_keys(dictionary: dict, keys: list) -> dict:
     """
-    Removes the specified keys from the dictionary and returns a tuple
-    with the updated dictionary and a new dictionary containing the popped items.
+    Removes the specified keys from the dictionary and returns a dictionary
+    containing the popped items.
 
     Parameters:
-    - dictionary: The input dictionary.
-    - keys: A list of keys to be popped.
+    - dictionary (dict): The input dictionary.
+    - keys (list): A list of keys to be popped.
 
     Returns:
-    - A new dictionary with the popped items.
+    - dict: A dictionary containing the popped items.
     """
     popped_items = {key: dictionary.pop(key, None) for key in keys}
     return popped_items
 
 
-def dict_to_json(series_of_dicts):
+def dict_to_json(series_of_dicts: list) -> list:
+    """
+    Convert a list of dictionaries to a list of JSON strings.
+
+    Parameters:
+    - series_of_dicts (list): A list of dictionaries.
+
+    Returns:
+    - list: A list of JSON strings.
+    """
     return [json.dumps(d) for d in series_of_dicts]
 
 
-def json_to_dict(series_of_json):
+def json_to_dict(series_of_json: list) -> list:
+    """
+    Convert a list of JSON strings to a list of dictionaries.
+
+    Parameters:
+    - series_of_json (list): A list of JSON strings.
+
+    Returns:
+    - list: A list of dictionaries.
+    """
     return [json.loads(s) for s in series_of_json]
```

### Comparing `hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/grouped_df.py` & `hot_spot_analysis-1.0.4a0/src/hot_spot_analysis/utils/grouped_df.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,65 @@
-from typing import Any, List
-
 import pandas as pd
-from pandas.core.groupby import DataFrameGroupBy
 
 """
 Functions meant to check the content, values or attributes of a data object.
 """
 
 
 def is_grouped(dataframe: pd.DataFrame) -> bool:
-    """Check if the data argument is grouped."""
-    return isinstance(dataframe, DataFrameGroupBy)
+    # TODO: remove the need for this function, and just take groupby as arg in HSA
+    """
+    Check if the DataFrame is grouped.
+
+    Parameters:
+    - dataframe (pd.DataFrame): Input DataFrame.
+
+    Returns:
+    - bool: True if the DataFrame is grouped, False otherwise.
+    """
+    return hasattr(dataframe, "groups")
 
 
-def get_groups(dataframe: pd.DataFrame) -> List[Any]:
+def get_groups(dataframe: pd.DataFrame) -> list:
+    # TODO: remove the need for this function, and just take groupby as arg in HSA
     """
-    If grouped, then return [column_name(s)] ELSE [None].
-    Returns list(str).
+    If the DataFrame is grouped, return the group variable(s).
+    Otherwise, return [None].
+
+    Parameters:
+    - dataframe (pd.DataFrame): Input DataFrame.
+
+    Returns:
+    - list: List of group variable(s) if the DataFrame is grouped, otherwise [None].
     """
     if is_grouped(dataframe):
-        group_vars = dataframe.keys
-        if isinstance(group_vars, str):
-            group_vars = [group_vars]
+        group_vars = list(dataframe.keys)  # type: ignore
         return group_vars
     else:
         return [None]
 
 
-def return_data(
-    dataframe: pd.DataFrame = pd.DataFrame(None),
-) -> pd.DataFrame:
-    """return dataframe from grouped or standard DataFrame"""
+def return_data(dataframe: pd.DataFrame = pd.DataFrame(None)) -> pd.DataFrame:
+    # TODO: remove the need for this function, and just take groupby as arg in HSA
+    """Return the original DataFrame from a grouped DataFrame if it's grouped."""
     if is_grouped(dataframe):
-        return dataframe.obj.reset_index()
+        return dataframe.obj  # type: ignore
     else:
         return dataframe
 
 
-def add_groups_to_combos(
-    group_vars: list[str], combos: list[list[str]]
-) -> List[List[Any]]:
-    """adds a fixed list to a list of lists"""
-    combos_plus = []
-    for combo in combos:
-        combo_plus = group_vars + combo
-        combos_plus.append(combo_plus)
-    return combos_plus
-
-
-def group_sizes(grouped_df: DataFrameGroupBy) -> pd.DataFrame:
+def add_groups_to_combos(group_vars: list, combos: list[list]) -> list[list]:
     """
-    Get the size of each group from a grouped Pandas DataFrame.
+    Adds group variables to each combination in a list of combinations.
 
     Parameters:
-    - grouped_df: The grouped Pandas DataFrame.
+    - group_vars (list): List of group variables.
+    - combos (list[list]): List of combinations.
 
     Returns:
-    - A DataFrame containing the size of each group.
+    - list[list]: List of combinations with group variables added.
     """
-    temp = pd.DataFrame(grouped_df.size()).reset_index()
-    results_df = temp.rename(columns={0: "n_rows"})
-
-    return results_df
+    combos_plus = []
+    for combo in combos:
+        combo_plus = group_vars + combo
+        combos_plus.append(combo_plus)
+    return combos_plus
```

