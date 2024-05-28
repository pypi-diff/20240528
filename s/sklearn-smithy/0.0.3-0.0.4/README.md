# Comparing `tmp/sklearn_smithy-0.0.3.tar.gz` & `tmp/sklearn_smithy-0.0.4.tar.gz`

## Comparing `sklearn_smithy-0.0.3.tar` & `sklearn_smithy-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/__init__.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/__main__.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/_arguments.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/_callbacks.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/_logger.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/_models.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/_prompts.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/_utils.py
--rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/app.py
--rw-r--r--   0        0        0     6627 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/sksmithy/template.py.jinja
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/LICENSE
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/README.md
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/__init__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/__main__.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_arguments.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_callbacks.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_logger.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_models.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_prompts.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_utils.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/app.py
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/template.py.jinja
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/PKG-INFO
```

### Comparing `sklearn_smithy-0.0.3/sksmithy/__main__.py` & `sklearn_smithy-0.0.4/sksmithy/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,22 @@
     Finally, the following two questions will be prompt:
 
     * if the estimator should have tags (To know more about tags, check the dedicated
         [scikit-learn documentation](https://scikit-learn.org/dev/developers/develop.html#estimator-tags))
 
     * in which file the class should be saved (default is `f'{name.lower()}.py'`)
     """
+    required = required_params.split(",") if required_params else []
+    optional = optional_params.split(",") if optional_params else []
+
+    duplicated_params = set(required).intersection(set(optional))
+    if duplicated_params:
+        msg_duplicated_params = f"The following parameters are duplicated: {duplicated_params}"
+        raise typer.BadParameter(msg_duplicated_params)
+
     # Check if linear
     match estimator_type:
         case EstimatorType.ClassifierMixin | EstimatorType.RegressorMixin:
             linear = typer.confirm(PROMPT_LINEAR)
         case _:
             linear = False
 
@@ -77,17 +85,14 @@
             decision_function = False
 
     tags = typer.prompt(PROMPT_TAGS, default="")
     tags = parse_tags(tags)
 
     output_file = typer.prompt(PROMPT_OUTPUT, default=f"{name.lower()}.py")
 
-    required = required_params.split(",") if required_params else []
-    optional = optional_params.split(",") if optional_params else []
-
     forged_template = render_template(
         name=name,
         estimator_type=estimator_type,
         required=required,
         optional=optional,
         linear=linear,
         sample_weight=sample_weight,
```

### Comparing `sklearn_smithy-0.0.3/sksmithy/_arguments.py` & `sklearn_smithy-0.0.4/sksmithy/_arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     ),
 ]
 
 required_params_arg = Annotated[
     str,
     Option(
         prompt=PROMPT_REQUIRED,
-        help=("List of [bold green]required[/bold green] parameters (comma-separated)."),
+        help="List of [bold green]required[/bold green] parameters (comma-separated).",
         callback=args_callback,
     ),
 ]
 optional_params_arg = Annotated[
     str,
     Option(
         prompt=PROMPT_OPTIONAL,
-        help=("List of [bold green]optional[/bold green] parameters (comma-separated)."),
+        help="List of [bold green]optional[/bold green] parameters (comma-separated).",
         callback=args_callback,
     ),
 ]
 
 sample_weight_arg = Annotated[
     bool,
     Option(
```

### Comparing `sklearn_smithy-0.0.3/sksmithy/_callbacks.py` & `sklearn_smithy-0.0.4/sksmithy/_callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,32 +8,37 @@
 
 def name_callback(name: str) -> str:
     """Validate if `name` is a valid python class name."""
     valid = name.isidentifier()
     kw = iskeyword(name)
 
     if not valid:
-        msg = f"{name} is not a valid class name in python"
+        msg = f"{name} is not a valid class name in python!"
         raise BadParameter(msg)
     if kw:
-        msg = f"{name} is a valid class name, but also a python keyword"
-        console.print(msg, style="bad")
+        msg = f"Careful: {name} is a python keyword!"
+        console.print(msg, style="warning")
 
     return name
 
 
 def args_callback(params: str) -> str:
     """Validate if `params` contains valid python names."""
     if params:
         param_list = params.split(",")
         invalid = tuple(p for p in param_list if not p.isidentifier())
 
         if len(invalid) > 0:
             msg = f"The following parameters are invalid python identifiers: {invalid}"
             raise BadParameter(msg)
+
+        if len(set(param_list)) < len(param_list):
+            msg = "Found repeated parameter"
+            raise BadParameter(msg)
+
     return params
 
 
 def parse_tags(tags: str) -> list[str]:
     """Parse and validate `tags`."""
     if tags:
         list_tag = tags.split(",")
```

### Comparing `sklearn_smithy-0.0.3/sksmithy/_models.py` & `sklearn_smithy-0.0.4/sksmithy/_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class EstimatorType(str, Enum):
     """List of possible estimator types."""
 
     ClassifierMixin = "classifier"
     OutlierMixin = "outlier"
     RegressorMixin = "regressor"
     TransformerMixin = "transformer"
+    ClusterMixin = "cluster"
 
 
 class TagType(str, Enum):
     """List of extra tags.
 
     Description of each tag is available at https://scikit-learn.org/dev/developers/develop.html#estimator-tags.
     """
```

### Comparing `sklearn_smithy-0.0.3/sksmithy/_prompts.py` & `sklearn_smithy-0.0.4/sksmithy/_prompts.py`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.3/sksmithy/_utils.py` & `sklearn_smithy-0.0.4/sksmithy/_utils.py`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.3/sksmithy/template.py.jinja` & `sklearn_smithy-0.0.4/sksmithy/template.py.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         {%if linear -%}
         # For linear models, coef_ and intercept_ is all you need. `predict` is taken care of by the mixin
         self.coef_ = ...
         self.intercept_ = ...
         {%- endif %}
         {% if 'max_iter' in parameters -%}self.n_iter_ = ...{%- endif %}
         {% if estimator_type=='outlier' -%}self.offset_ = ...{%- endif %}
+        {% if estimator_type=='cluster' -%}self.labels_ = ...{%- endif %}
 
         return self
 
     {% if estimator_type == 'classifier' and decision_function == True %}
     def decision_function(self, X):
         """Confidence scores of X.
 
@@ -120,14 +121,18 @@
         -------
         Prediction array.
         """
 
         check_is_fitted(self)
         X = check_array(X, ...)  #TODO: Fill in `check_array` arguments
 
+        if X.shape[1] != self.n_features_in_:
+            msg = f"X has {X.shape[1]} features but the estimator was fitted on {self.n_features_in_} features."
+            raise ValueError(msg)
+
         y_scores = ... # TODO: Implement decision_function logic
 
         return y_scores
 
     def predict(self, X):
         """Predict X.
 
@@ -140,16 +145,16 @@
         -------
         Prediction array.
         """
 
         check_is_fitted(self)
         X = check_array(X, ...)  #TODO: Fill in `check_array` arguments
 
-        y_pred = (self.decision_function(X).ravel() > 0).astype(int)
-
+        decision = self.decision_function(X)
+        y_pred = (decision.ravel() > 0).astype(int) if self.n_classes == 2 else np.argmax(decision, axis=1)
         return y_pred
     {% endif %}
 
     {% if estimator_type == 'classifier' and predict_proba == True %}
     def predict_proba(self, X):
         """Probability estimates of X.
 
@@ -162,39 +167,47 @@
         -------
         Prediction array.
         """
 
         check_is_fitted(self)
         X = check_array(X, ...)  #TODO: Fill in `check_array` arguments
 
+        if X.shape[1] != self.n_features_in_:
+            msg = f"X has {X.shape[1]} features but the estimator was fitted on {self.n_features_in_} features."
+            raise ValueError(msg)
+
         y_proba = ... # TODO: Implement predict_proba logic
 
         return y_proba
     {% endif %}
 
     {% if estimator_type=='outlier' %}
     def score_samples(self, X):
 
         check_is_fitted(self)
         X = check_array(X, ...)  #TODO: Fill in `check_array` arguments
+        
+        if X.shape[1] != self.n_features_in_:
+            msg = f"X has {X.shape[1]} features but the estimator was fitted on {self.n_features_in_} features."
+            raise ValueError(msg)
 
         ...  # TODO: Implement scoring function, `decision_function` and `predict` will follow
 
         return ...
 
     def decision_function(self, X):
         return self.score_samples(X) - self.offset_
 
     def predict(self, X):
         preds = (self.decision_function(X) >= 0).astype(int)
         preds[preds == 0] = -1
         return preds
     {%- endif %}
 
-    {% if ((estimator_type == 'classifier' and decision_function == False) or estimator_type=='regressor') and linear == False %}
+    {% if decision_function == False and linear == False and (estimator_type in ('classifier', 'regressor', 'cluster')) %}
     def predict(self, X):
         """Predict X.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The data to predict.
@@ -202,14 +215,18 @@
         Returns
         -------
         Prediction array.
         """
 
         check_is_fitted(self)
         X = check_array(X, ...)  #TODO: Fill in `check_array` arguments
+        
+        if X.shape[1] != self.n_features_in_:
+            msg = f"X has {X.shape[1]} features but the estimator was fitted on {self.n_features_in_} features."
+            raise ValueError(msg)
 
         y_pred = ... # TODO: Implement predict logic
 
         return y_pred
     {% endif %}
 
     {% if estimator_type=='transformer' -%}
@@ -224,21 +241,32 @@
         Returns
         -------
         Transformed array.
         """
 
         check_is_fitted(self)
         X = check_array(X, ...) # TODO: Fill in `check_array` arguments
+        
+        if X.shape[1] != self.n_features_in_:
+            msg = f"X has {X.shape[1]} features but the estimator was fitted on {self.n_features_in_} features."
+            raise ValueError(msg)
 
         X_ts = ...  # TODO: Implement transform logic
 
         return X_ts
     {%- endif %}
 
     {% if tags %}
     def _more_tags(self):
         return {
             {%for tag in tags -%}
             "{{tag}}": ...,
             {% endfor -%}
             }
     {%- endif %}
+
+    {% if estimator_type == 'classifier' %}
+    @property
+    def n_classes_(self):
+        """Number of classes."""
+        return len(self.classes_)
+    {% endif %}
```

### Comparing `sklearn_smithy-0.0.3/.gitignore` & `sklearn_smithy-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.3/LICENSE` & `sklearn_smithy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.3/README.md` & `sklearn_smithy-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<img src="https://raw.githubusercontent.com/FBruzzesi/sklearn-smithy/main/docs/img/sksmith-logo.svg" width=150 height=150 align="right">
+
 # Scikit-learn Smithy
 
 A CLI to forge scikit-learn compatible estimator templates with ease.
 
 ## Why
 
 Writing a scikit-learn compatible estimators might be harder than expected.
```

### Comparing `sklearn_smithy-0.0.3/pyproject.toml` & `sklearn_smithy-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sklearn-smithy"
-version = "0.0.3"
+version = "0.0.4"
 
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{name = "Francesco Bruzzesi"}]
 
 dependencies = [
```

### Comparing `sklearn_smithy-0.0.3/PKG-INFO` & `sklearn_smithy-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sklearn-smithy
-Version: 0.0.3
+Version: 0.0.4
 Author: Francesco Bruzzesi
 License: MIT License
         
         Copyright (c) 2024 Francesco Bruzzesi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,14 +37,16 @@
 Requires-Dist: ruff>=0.4.0
 Requires-Dist: typer>=0.12.0
 Requires-Dist: typing-extensions>=4.4.0; python_version < '3.11'
 Provides-Extra: streamlit
 Requires-Dist: streamlit>=1.34.0; extra == 'streamlit'
 Description-Content-Type: text/markdown
 
+<img src="https://raw.githubusercontent.com/FBruzzesi/sklearn-smithy/main/docs/img/sksmith-logo.svg" width=150 height=150 align="right">
+
 # Scikit-learn Smithy
 
 A CLI to forge scikit-learn compatible estimator templates with ease.
 
 ## Why
 
 Writing a scikit-learn compatible estimators might be harder than expected.
```

