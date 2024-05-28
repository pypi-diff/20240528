# Comparing `tmp/model_checker-0.4.4.tar.gz` & `tmp/model_checker-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.4.4.tar", last modified: Fri May 24 20:33:28 2024, max compression
+gzip compressed data, was "model_checker-0.4.5.tar", last modified: Tue May 28 17:34:47 2024, max compression
```

## Comparing `model_checker-0.4.4.tar` & `model_checker-0.4.5.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.075412 model_checker-0.4.4/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.4/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     9566 2024-05-24 20:33:28.075412 model_checker-0.4.4/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     8781 2024-05-23 21:42:24.000000 model_checker-0.4.4/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-24 20:33:24.000000 model_checker-0.4.4/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-24 20:33:28.075412 model_checker-0.4.4/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.074412 model_checker-0.4.4/src/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.075412 model_checker-0.4.4/src/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)      124 2024-05-24 20:33:24.000000 model_checker-0.4.4/src/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    13625 2024-05-23 17:20:26.000000 model_checker-0.4.4/src/model_checker/__main__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    22895 2024-05-24 19:48:40.000000 model_checker-0.4.4/src/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    26524 2024-05-24 17:55:48.000000 model_checker-0.4.4/src/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    28404 2024-05-24 17:38:50.000000 model_checker-0.4.4/src/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7836 2024-05-23 18:38:27.000000 model_checker-0.4.4/src/model_checker/syntax.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.075412 model_checker-0.4.4/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     9566 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      510 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.075412 model_checker-0.4.4/test/
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-23 04:07:12.000000 model_checker-0.4.4/test/test.py
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-23 04:07:12.000000 model_checker-0.4.4/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.313779 model_checker-0.4.5/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.5/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     9602 2024-05-28 17:34:47.313779 model_checker-0.4.5/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     8817 2024-05-28 16:55:37.000000 model_checker-0.4.5/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-28 17:34:42.000000 model_checker-0.4.5/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-28 17:34:47.313779 model_checker-0.4.5/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.312779 model_checker-0.4.5/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.313779 model_checker-0.4.5/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)      595 2024-05-28 17:34:42.000000 model_checker-0.4.5/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    13743 2024-05-27 19:03:37.000000 model_checker-0.4.5/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    23866 2024-05-28 17:17:04.000000 model_checker-0.4.5/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    28248 2024-05-27 19:03:37.000000 model_checker-0.4.5/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    30661 2024-05-28 17:04:14.000000 model_checker-0.4.5/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7856 2024-05-25 01:29:18.000000 model_checker-0.4.5/src/model_checker/syntax.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.313779 model_checker-0.4.5/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     9602 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      492 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.313779 model_checker-0.4.5/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)     7788 2024-05-28 17:34:02.000000 model_checker-0.4.5/test/test_sat.py
```

### Comparing `model_checker-0.4.4/LICENCE` & `model_checker-0.4.5/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.4/PKG-INFO` & `model_checker-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.4.4
+Version: 0.4.5
 Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,15 @@
 
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for finding countermodels for claims which include modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 The language currently includes the following operators:
 
   - `neg` for _negation_
-  - `not` for _exclusion_
+  <!-- - `not` for _exclusion_ -->
   - `wedge` for _conjunction_
   - `vee` for _disjunction_
   - `rightarrow` for _material conditional_
   - `leftrightarrow` for _material biconditional_
   - `Box` for _necessity_
   - `Diamond` for _possibility_
   - `boxright` for the _must counterfactual conditional_
@@ -86,17 +86,17 @@
 A _negated sentence_ is verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 A _conjunctive sentence_ is verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 A _disjunctive sentence_ is verified by the verifiers for either disjunct or fusions thereof and falsified by pairwise fusions of falsifiers for the disjuncts.
 Conjunction and disjunction are dual operators obeying the standard idempotence and De Morgan laws.
 The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
 For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
-By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_.
-In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`.
-This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison.
+<!-- By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_. -->
+<!-- In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`. -->
+<!-- This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison. -->
 
 A _necessity sentence_ `Box A` is true at a world just in case every world state includes a part that verifies `A` and a _possibility sentence_ `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
 Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include as parts both `s` and a maximal part of `w` that is compatible with `s`.
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
```

### Comparing `model_checker-0.4.4/README.md` & `model_checker-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for finding countermodels for claims which include modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 The language currently includes the following operators:
 
   - `neg` for _negation_
-  - `not` for _exclusion_
+  <!-- - `not` for _exclusion_ -->
   - `wedge` for _conjunction_
   - `vee` for _disjunction_
   - `rightarrow` for _material conditional_
   - `leftrightarrow` for _material biconditional_
   - `Box` for _necessity_
   - `Diamond` for _possibility_
   - `boxright` for the _must counterfactual conditional_
@@ -70,17 +70,17 @@
 A _negated sentence_ is verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 A _conjunctive sentence_ is verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 A _disjunctive sentence_ is verified by the verifiers for either disjunct or fusions thereof and falsified by pairwise fusions of falsifiers for the disjuncts.
 Conjunction and disjunction are dual operators obeying the standard idempotence and De Morgan laws.
 The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
 For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
-By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_.
-In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`.
-This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison.
+<!-- By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_. -->
+<!-- In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`. -->
+<!-- This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison. -->
 
 A _necessity sentence_ `Box A` is true at a world just in case every world state includes a part that verifies `A` and a _possibility sentence_ `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
 Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include as parts both `s` and a maximal part of `w` that is compatible with `s`.
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
```

### Comparing `model_checker-0.4.4/pyproject.toml` & `model_checker-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.4.4"
+version = "0.4.5"
 description = "A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators."
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
```

### Comparing `model_checker-0.4.4/src/model_checker/__main__.py` & `model_checker-0.4.5/src/model_checker/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 # import cProfile
 # import pstats
 
 # Get the directory path of the current file
 current_dir = os.path.dirname(__file__)
 # Construct the full path to your project root
 project_root = os.path.abspath(os.path.join(current_dir, ".."))
+project_root = project_root[:-4] # bandaid fix to remove "/src" from the root
 # Add the project root to the Python path
 sys.path.append(project_root)
 
-from model_checker.__init__ import __version__
-from model_checker.model_structure import ( # for packaging
+from src.model_checker.__init__ import __version__
+from src.model_checker.model_structure import ( # for packaging
     StateSpace,
     make_model_for,
     )
 
 script_template = Template("""
 '''
 Model Checker: ${name}
@@ -58,15 +59,15 @@
 ############ SYNTAX ############
 ################################
 
 ### SENTENCES ###
 
 # 'A', 'B', 'C',... can be used for sentence letters
 
-# Alternatively, 'RedBall', 'MarySings',... can be used for sentence letters.
+# Alternatively, 'RedBall', 'MarySings',... or 'red_ball', 'mary_sings',... can be used for sentence letters.
 
 # 'top' is a designated sentence for the trivial truth verified by everything and falsified by nothing.
 
 
 ### UNARY OPERATORS ###
 
 # Negation: 'neg', e.g., 'neg A'.
```

### Comparing `model_checker-0.4.4/src/model_checker/model_definitions.py` & `model_checker-0.4.5/src/model_checker/model_definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -373,40 +373,41 @@
         return True
     raise ValueError(
         prefix_modal,
         "Something has gone wrong in evaluate_cf_counterfactual. "
         f"The operator {operator} in {prefix_modal} is not a modal."
     )
 
-def evaluate_cf_expr(state_space, prefix_cf, eval_world):
+def evaluate_cf_expr(state_space, cf_sentence, eval_world):
     """evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
     used to initialize Counterfactuals
     returns a bool representing whether the counterfactual is true at the world or not
     """
-    operator, antecedent, consequent = prefix_cf[0], prefix_cf[1], prefix_cf[2]
+    operator, antecedent, consequent = cf_sentence[0], cf_sentence[1], cf_sentence[2]
     antecedent_vers = find_complex_proposition(state_space, antecedent, eval_world)[0]
-    consequent_vers = find_complex_proposition(state_space, consequent, eval_world)[0]
-    consequent_fals = find_complex_proposition(state_space, consequent, eval_world)[1]
+    consequent_vers, consequent_fals = find_complex_proposition(
+        state_space, consequent, eval_world
+    )
     antecedent_alts = state_space.find_alt_bits(antecedent_vers, eval_world)
     if 'boxright' in operator:
         for alt_world in antecedent_alts:
             for falsifier in consequent_fals:
                 if bit_part(falsifier, alt_world):
                     return False
         return True
     if 'circleright' in operator:
         for alt_world in antecedent_alts:
             for verifier in consequent_vers:
                 if bit_part(verifier, alt_world):
                     return True
         return False
     raise ValueError(
-        prefix_cf,
+        cf_sentence,
         "Something has gone wrong in evaluate_cf_counterfactual. "
-        f"The operator {operator} in {prefix_cf} is not a counterfatual."
+        f"The operator {operator} in {cf_sentence} is not a counterfatual."
     )
 
 
 # def evaluate_mainclause_cf_expr(model_structure, prefix_cf, eval_world):
 #     """evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
 #     used to initialize Counterfactuals
 #     returns a bool representing whether the counterfactual is true at the world or not
@@ -432,37 +433,56 @@
     for world in model_structure.world_bits:
         if find_complex_proposition(model_structure, cf_sentence, world)[0]:
             worlds_true_at.add(world)
             continue
         worlds_false_at.add(world)
     return (worlds_true_at, worlds_false_at)
 
+def find_precluders(verifiers, all_bits, poss_bits):
+    """simulates the set of falsifiers"""
+    # if not verifiers:
+    #     return null_singleton
+    precluders = []
+    for state in all_bits:
+        incomp_ver = set()
+        for ver in verifiers:
+            if bit_fusion(state, ver) not in poss_bits:
+                incomp_ver.add(ver)
+                break
+        comp_ver = set()
+        for ver in verifiers:
+            if bit_fusion(state, ver) in poss_bits:
+                comp_ver.add(ver)
+                break
+        if incomp_ver and not comp_ver:
+            precluders.append(state)
+    # TODO: would be nice to sort the precluders but they are bits
+    # excluders_list = sorted(excluders)
+    return precluders
+
 def find_excluders(verifiers, all_bits, poss_bits, null_singleton):
     """simulates the set of falsifiers"""
-    if not verifiers:
-        return null_singleton
+    # if not verifiers:
+    #     return null_singleton
     excluders = []
     for state in all_bits:
         comp_state_parts = set()
         for part in all_bits:
-            # print(f"TEST: part {part} is null_state {null_state}: {part in null_state}")
             if bit_part(part, state) and not part in null_singleton:
                 for ver in verifiers:
                     if bit_fusion(part, ver) in poss_bits:
                         comp_state_parts.add(part)
                         break
-                break
         incomp_ver_parts = set()
         for ver in verifiers:
             for part in all_bits:
                 if bit_part(part, state) and not part in null_singleton:
                     if bit_fusion(part, ver) not in poss_bits:
                         incomp_ver_parts.add(part)
                         break
-            break
         if not comp_state_parts and incomp_ver_parts:
             excluders.append(state)
     # TODO: would be nice to sort the excluders but they are bits
     # excluders_list = sorted(excluders)
     return excluders
 
 def find_complex_proposition(model_structure, complex_sentence, eval_world):
@@ -484,17 +504,25 @@
         Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
         return (Y_F, Y_V)
     N = model_structure.N
     null_singleton = {BitVecVal(0,N)}
     if "not" in op:
         all_bits = model_structure.all_bits
         poss_bits = model_structure.poss_bits
-        Y_V = find_complex_proposition(model_structure, Y, eval_world)[0]
-        Y_F = find_excluders(Y_V, all_bits, poss_bits, null_singleton)
-        return (Y_F, Y_V)
+        Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
+        vers = find_excluders(Y_F, all_bits, poss_bits, null_singleton)
+        fals = find_excluders(Y_V, all_bits, poss_bits, null_singleton)
+        return (vers, fals)
+    if "pre" in op:
+        all_bits = model_structure.all_bits
+        poss_bits = model_structure.poss_bits
+        Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
+        vers = find_precluders(Y_F, all_bits, poss_bits)
+        fals = find_precluders(Y_V, all_bits, poss_bits)
+        return (vers, fals)
     if 'Box' in op or 'Diamond' in op:
         if evaluate_modal_expr(model_structure, complex_sentence, eval_world):
             return (null_singleton, set())
         return (set(), null_singleton)
     Z = complex_sentence[2]
     Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
     Z_V, Z_F = find_complex_proposition(model_structure, Z, eval_world)
```

### Comparing `model_checker-0.4.4/src/model_checker/model_structure.py` & `model_checker-0.4.5/src/model_checker/model_structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 """
-file defines model structure class given a Z3 model
+file defines model structure class given a Z3 model sdffds
 """
 
 from string import Template
 import time
 import sys
+import os
 from z3 import (
     Function,
     BitVecSort,
     BoolSort,
     BitVec,
     BitVecVal
 )
 
-from model_checker.semantics import (
-    make_constraints,
+# Get the directory path of the current file
+current_dir = os.path.dirname(__file__)
+# Construct the full path to your project root
+project_root = os.path.abspath(os.path.join(current_dir, ".."))
+project_root = project_root[:-4] # bandaid fix to remove "/src" from the root
+# Add the project root to the Python path
+sys.path.append(project_root)
+
+from src.model_checker.semantics import ( # imports issue fixed with above code
+    define_N_semantics,
     solve_constraints,
     all_sentence_letters,
 )
-from model_checker.model_definitions import (
+from src.model_checker.model_definitions import (
     find_compatible_parts,
     atomic_propositions_dict_maker,
     find_all_bits,
     find_max_comp_ver_parts,
     find_poss_bits,
     find_subsentences,
     find_world_bits,
     pretty_set_print,
     bit_part,
     bitvec_to_substates,
     int_to_binary,
     true_and_false_worlds_for_cf,
     find_complex_proposition,
 )
-from model_checker.syntax import (
+from src.model_checker.syntax import (
     AtomSort,
     infix,
     prefix,
     add_backslashes_to_infix,
 )
 
 inputs_template = Template(
@@ -100,15 +109,15 @@
         self.verify = Function("verify", BitVecSort(N), AtomSort, BoolSort())
         self.falsify = Function("falsify", BitVecSort(N), AtomSort, BoolSort())
         self.assign = Function("assign", BitVecSort(N), AtomSort, BitVecSort(N))
         self.w = BitVec("w", N) # what will be the main world
         self.prefix_premises = [prefix(prem) for prem in infix_premises]
         # M: I think below is a problem
         self.prefix_conclusions = [prefix(con) for con in infix_conclusions]
-        find_constraints_func = make_constraints(
+        find_constraints_func = define_N_semantics(
             self.verify,
             self.falsify,
             self.possible,
             self.assign,
             self.N,
             self.w
         )
@@ -133,26 +142,29 @@
         self.model_runtime is the runtime of the model as a float
         self.all_bits is a list of all bits (each of sort BitVecVal)
         self.poss_bits is a list of all possible bits
         self.world_bits is a lsit of all world bits
         self.main_world is the eval world (as a BitVecVal)
         self.atomic_props_dict is a dictionary with keys AtomSorts and keys (V,F)
         """
-        model_start = time.time()  # start benchmark timer
         constraints = (
             self.frame_constraints +
             self.prop_constraints +
             self.premise_constraints +
             self.conclusion_constraints
         )
+        model_start = time.time()  # start benchmark timer
         z3_model_status, z3_model = solve_constraints(constraints)
         model_end = time.time()
         model_runtime = round(model_end - model_start, 4)
         return (z3_model_status, z3_model, model_runtime)
 
+    def __str__(self):
+        return f'ModelSetup object with premises {self.infix_premises} and conclusions {self.infix_conclusions}'
+
 
 class ModelStructure:
     """self.premises is a list of prefix sentences
     self.conclusions is a list of prefix sentences
     self.input_sentences is the combination of self.premises and self.conclusions with the
     conclusions negated
     self.sentence letters is a list of atomic sentence letters (each of sort AtomSort)
@@ -225,14 +237,27 @@
         if self.model_status:
             print(f"Satisfiable {name} constraints:\n", file=output)
         else:
             print("Unsatisfiable core constraints:\n", file=output)
         for index, con in enumerate(consts, start=1):
             print(f"{index}. {con}\n", file=output)
             # print(f"Constraints time: {time}\n")
+    
+    def __str__(self):
+        '''useful for people who want to use model_checker in a python file (like we use z3 or numpy, if that makes sense)
+        feel free to change/remove'''
+        return f'{"" if self.model_status else "un"}sat ModelStructure for premises {self.infix_premises} and conclusions {self.infix_conclusions} with status {self.model_status}'
+
+    def __bool__(self):
+        '''returns the value of self.model_status (ie, whether the z3 model was solved)
+        reasoning: say ms is a ModelStructure object. Now we can check its model_status by doing:
+        if ms: # as opposed to if ms.model_status
+            (do_something)
+        '''
+        return self.model_status
 
 
 class StateSpace:
     """class for all states and their attributes"""
 
     def __init__(self, model_setup, model_structure):
         self.model_setup = model_setup
@@ -282,14 +307,15 @@
                 for max_ver in max_comp_ver_parts:
                     if bit_part(max_ver, world):
                         alt_bits.add(world)
                         break  # to return to the second for loop over world_bits
         return alt_bits
 
     # Useful to user now that can search an infix expression
+    # NOTE: I think this option is no longer available
     def find_proposition_object(self, expression):
         """given a sentence, finds the Proposition object in the model that corresponds
         to it. Can optionally search through only the extensional sentences
         Also defaults to searching an infix sentence, though internally it always searches
         prefix.
         If search infix, make sure you put double backslashes always!!
         returns a Proposition object"""
@@ -377,14 +403,15 @@
         if cons_include:
             print("# Satisfiable constraints", file=output)
             # TODO: print constraint objects, not constraint strings
             print(f"all_constraints = {constraints}", file=output)
 
     def print_states(self, print_impossible, output=sys.__stdout__):
         """print all fusions of atomic states in the model
+        print_impossible is a boolean for whether to print impossible states or not
         first print function in print.py"""
         N = self.model_setup.N
         print("\nState Space:", file=output)  # Print states
         YELLOW = '\033[33m'
         BLUE = '\033[34m'
         MAGENTA = '\033[35m'
         CYAN = '\033[36m'
@@ -417,15 +444,15 @@
         prop_obj.print_verifiers_and_falsifiers(world_bit, print_impossible, indent, output)
         if str(prop_obj) in [str(atom) for atom in sentence_letters]:
             return
         prefix_expr = prop_obj["prefix expression"]
         op = prefix_expr[0]
         first_subprop = self.find_proposition_object(prefix_expr[1])
         indent += 1 # begin subcases, so indent
-        if "neg" in op or "not" in op:
+        if "neg" in op or "not" in op or "pre" in op:
             self.rec_print(first_subprop, world_bit, print_impossible, output, indent)
             return
         if 'Diamond' in op or 'Box' in op:
             for u in self.world_bits:
                 self.rec_print(first_subprop, u, print_impossible, output, indent)
             return
         left_subprop = first_subprop
@@ -615,7 +642,11 @@
     returns a function that will solve the premises and conclusions"""
     backslash_premises = [add_backslashes_to_infix(prem) for prem in premises]
     backslash_conclusions = [add_backslashes_to_infix(concl) for concl in conclusions]
     model_setup = ModelSetup(N, backslash_premises, backslash_conclusions)
     z3_model_status, z3_model, model_runtime = model_setup.solve()
     model_structure = ModelStructure(z3_model_status, model_setup, z3_model, model_runtime)
     return model_setup, model_structure
+    # NOTE: since you save the ModelSetup object as an attribute of the ModelStructure object,
+    # there's really no need to return it as well. I'm not going to remove it in case it adds
+    # some bugs down the road since it's been a while since I've touched things, but just thought
+    # I'd say to consider
```

### Comparing `model_checker-0.4.4/src/model_checker/semantics.py` & `model_checker-0.4.5/src/model_checker/semantics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """
+BEDABEDEEBDABEDAO
 contains all semantic functions
 this file defines the functions needed to generate Z3 constraints from
 input_sentences in infix form.
 """
 
 from z3 import (
     sat,
@@ -30,27 +31,30 @@
         return [prefix_input_sentence[0]] # redundant but conceptually clear
     return_list = []
     for part in prefix_input_sentence[1:]:
         return_list.extend(sentence_letters_in_compound(part))
     return return_list
 
 def all_sentence_letters(prefix_sentences):
-    """finds all the sentence letters in a list of input sentences.
-    returns as a list with no repeats (sorted for consistency)
-    used in find_all_constraints and StateSpace __init__"""
+    """finds all the sentence letters in a list of input sentences, in prefix form.
+    returns as a list with no repeats (sorted for consistency) of AtomSorts
+    used in find_all_constraints (to feed into find_prop_constraints) and StateSpace __init__"""
     sentence_letters = set()
     for prefix_input in prefix_sentences:
         sentence_letters_in_input = sentence_letters_in_compound(prefix_input)
         for sentence_letter in sentence_letters_in_input:
             sentence_letters.add(sentence_letter)
     return list(sentence_letters)
     # sort just to make every output the same, given sets aren't hashable
 
 
-def make_constraints(verify, falsify, possible, assign, N, w):
+def define_N_semantics(verify, falsify, possible, assign, N, w):
+    # NOTE: just thought of this—we could make the options to do non_null or non_triv optional.
+    # Like it coulld be an optional argument put into the model at the top level, just like
+    # unsat_core is. Let me below know if you think that's a good idea or if it wouln't be useful.
     '''function that makes the function to make the constraints (and list of sentence letters
     and prefix sentences) This has to be done in order to define N in an input file—you'll see
     here that N is passed in as a variable to the function, after which these 'make' a semantics
     with that N (and the other inputs to this function also depend on N)
     returns a function find_all_constraints that is used to find the constraints, the sentence letters,
     and prefix sentences.. 
     '''
@@ -80,14 +84,19 @@
         return bit_s | bit_t
 
     def is_part_of(bit_s, bit_t):
         """the fusion of bit_s and bit_t is identical to bit_t
         returns a Z3 constraint"""
         return fusion(bit_s, bit_t) == bit_t
 
+    def non_null_part_of(bit_s, bit_t):
+        """bit_s verifies atom and is not the null state
+        returns a Z3 constraint"""
+        return And(Not(bit_s == 0), is_part_of(bit_s, bit_t))
+
     def compatible(bit_x, bit_y):
         """the fusion of bit_x and bit_y is possible
         returns a Z3 constraint"""
         return possible(fusion(bit_x, bit_y))
 
     def maximal(bit_w):
         """bit_w includes all compatible states as parts.
@@ -139,61 +148,84 @@
         return And(
             is_world(bit_u),
             is_part_of(bit_y, bit_u),
             Exists(z, And(is_part_of(z, bit_u), max_compatible_part(z, bit_w, bit_y))),
         )
 
     def preclude(state, sentence, eval_world):
-        """to simulate bilateral semantics"""
+        """to simulate bilateral semantics
+        returns a Z3 constraint"""
         x = BitVec("preclude_x", N)
-        y = BitVec("preclude_y", N)
+        # return And(
+        #     Exists(
+        #         x,
+        #         And(
+        #             extended_verify(x, sentence, eval_world),
+        #             Not(compatible(x, state))
+        #         )
+        #     ),
         return ForAll(
             x,
             Implies(
                 extended_verify(x, sentence, eval_world),
                 Not(compatible(x, state))
             )
         )
+    # ),
+
+    # def precluder_fusion(state, sentence, eval_world):
+    #     x = BitVec("exclude_x", N)
+    #     y = BitVec("exclude_y", N)
+    #     return Or(
+    #         preclude(state, sentence, eval_world),
+    #         Exists(
+    #             [x, y],
+    #             And(
+    #                 non_null_part_of(x, state),
+    #                 preclude(x, sentence, eval_world),
+    #                 precluder_fusion(y, sentence, eval_world),
+    #                 state == fusion(x, y)
+    #             )
+    #         )
+    #     )
 
     def exclude(state, sentence, eval_world):
-        """to simulate bilateral semantics"""
+        """to simulate bilateral semantics
+        returns a Z3 constraint"""
         x = BitVec("exclude_x", N)
         y = BitVec("exclude_y", N)
         return And(
             ForAll(
                 x,
                 Implies(
-                    is_part_of(x, state),
+                    # is_part_of(x, state),
+                    non_null_part_of(x, state),
                     Exists(
                         y,
                         And(
-                            # possible(y),
                             extended_verify(y, sentence, eval_world),
                             Not(compatible(x, y))
                         )
                     )
                 )
             ),
             ForAll(
                 x,
                 Implies(
-                    And(
-                        # possible(x),
-                        extended_verify(x, sentence, eval_world),
-                    ),
+                    extended_verify(x, sentence, eval_world),
                     Exists(
                         y,
                         And(
-                            is_part_of(y, state),
+                            # is_part_of(y, state),
+                            non_null_part_of(y, state),
                             Not(compatible(x, y))
                         )
                     )
                 )
             )
-
         )
 
     def extended_verify(state, sentence, eval_world):
         """ext_sent is in prefix form. The state is the state that verifies ext_sent. 
         evaluate is an optional bool to evaluate something (now unused).
         returns a Z3 constraint"""
         if len(sentence) == 1:
@@ -204,19 +236,17 @@
         for choice in hyper_ops:
             if choice in operator:
                 return true_at(sentence, eval_world)
         Y = sentence[1]
         if "neg" in operator:
             return extended_falsify(state, Y, eval_world)
         if "not" in operator:
-            # print(f"TEST: op = {op}; arg = {Y}")
-            # TEST = exclude(state, Y, eval_world)
-            # print(TEST)
             return exclude(state, Y, eval_world)
-            # return preclude(state, Y, eval_world)
+        if "pre" in operator:
+            return preclude(state, Y, eval_world)
         Z = sentence[2]
         if "wedge" in operator:
             y = BitVec("ex_ver_y", N)
             z = BitVec("ex_ver_z", N)
             return Exists(
                 [y, z],
                 And(
@@ -236,20 +266,20 @@
                 extended_verify(state, ["wedge", Y, Z], eval_world),
                 extended_falsify(state, ["vee", Y, Z], eval_world),
             )
         if "rightarrow" in operator:
             return Or(
                 extended_falsify(state, Y, eval_world),
                 extended_verify(state, Z, eval_world),
-                extended_verify(state, ["wedge", ["neg", Y], Z], eval_world),
+                extended_verify(state, ["wedge", ["neg", Y], Z], eval_world), # M: out of curiosity, what's this for?
             )
         raise ValueError(
             sentence,
             "Something has gone wrong in extended_falsify. "
-            f"The operator {operator} in {sentence} is not a recognized."
+            f"The operator {operator} in {sentence} is not a recognized operator."
         )
 
     def extended_falsify(state, sentence, eval_world):
         """ext_sent is in prefix form. The state is the state that falsifies ext_sent. 
         returns a Z3 constraint"""
         if len(sentence) == 1:
             return falsify(state, sentence[0])
@@ -259,15 +289,16 @@
             if choice in operator:
                 return false_at(sentence, eval_world)
         Y = sentence[1]
         if "neg" in operator:
             return extended_verify(state, Y, eval_world)
         if "not" in operator:
             return exclude(state, Y, eval_world)
-            # return preclude(state, Y, eval_world)
+        if "pre" in operator:
+            return preclude(state, Y, eval_world)
         Z = sentence[2]
         if "wedge" in operator:
             return Or(
                 extended_falsify(state, Y, eval_world),
                 extended_falsify(state, Z, eval_world),
                 extended_falsify(state, ["vee", Y, Z], eval_world),
             )
@@ -313,39 +344,38 @@
         y = BitVec("t_y", N)
         u = BitVec("t_u", N)
         if len(sentence) == 1:
             sent = sentence[0]
             if 'top' not in str(sent)[0]: # top const alr in model, see find_model_constraints
                 return Exists(x, And(is_part_of(x, eval_world), verify(x, sent)))
         if len(sentence) == 2:
-            op = sentence[0]
+            operator = sentence[0]
             Y = sentence[1]
-            if "neg" in op or "not" in op:
-                # print(f"TEST: neg operator = {op}")
+            if "neg" in operator or "not" in operator or "pre" in operator:
                 return false_at(sentence[1], eval_world)
-            if 'Box' in op:
+            if 'Box' in operator:
                 return ForAll(u, Implies(is_world(u), true_at(sentence[1], u)))
-            if 'Diamond' in op:
+            if 'Diamond' in operator:
                 return Exists(u, And(is_world(u), true_at(sentence[1], u)))
         if len(sentence) == 3:
-            op = sentence[0]
+            operator = sentence[0]
             Y = sentence[1]
             Z = sentence[2]
-            if "wedge" in op:
+            if "wedge" in operator:
                 return And(true_at(Y, eval_world), true_at(Z, eval_world))
-            if "vee" in op:
+            if "vee" in operator:
                 return Or(true_at(Y, eval_world), true_at(Z, eval_world))
-            if "leftrightarrow" in op:
+            if "leftrightarrow" in operator:
                 return Or(
                     And(true_at(Y, eval_world), true_at(Z, eval_world)),
                     And(false_at(Y, eval_world), false_at(Z, eval_world)),
                 )
-            if "rightarrow" in op:
+            if "rightarrow" in operator:
                 return Or(false_at(Y, eval_world), true_at(Z, eval_world))
-            if "leq" in op:
+            if "leq" in operator:
                 return ForAll(
                     [x, y],
                     And(
                         Implies(
                             extended_verify(x, Y, eval_world),
                             extended_verify(x, Z, eval_world)
                         ),
@@ -364,15 +394,15 @@
                                     is_part_of(u, y),
                                     extended_falsify(u, Y, eval_world)
                                 )
                             )
                         )
                     )
                 )
-            if "sqsubseteq" in op:
+            if "sqsubseteq" in operator:
                 return ForAll(
                     [x, y],
                     And(
                         Implies(
                             And(
                                 extended_verify(x, Y, eval_world),
                                 extended_verify(y, Z, eval_world)
@@ -391,15 +421,15 @@
                         ),
                         Implies(
                             extended_falsify(x, Y, eval_world),
                             extended_falsify(x, Z, eval_world)
                         )
                     )
                 )
-            if "equiv" in op:
+            if "equiv" in operator:
                 return ForAll(
                     x,
                     And(
                         Implies(
                             extended_verify(x, Y, eval_world),
                             extended_verify(x, Z, eval_world)
                         ),
@@ -413,27 +443,27 @@
                         ),
                         Implies(
                             extended_falsify(x, Z, eval_world),
                             extended_falsify(x, Y, eval_world)
                         ),
                     )
                 )
-            if "boxright" in op:
+            if "boxright" in operator:
                 # print(f"TEST: cf operator = {op}, ant = {Y}, con = {Z}")
                 return ForAll(
                     [x, u],
                     Implies(
                         And(
                             extended_verify(x, Y, eval_world),
                             is_alternative(u, x, eval_world)
                         ),
                         true_at(Z, u),
                     ),
                 )
-            if "circleright" in op:
+            if "circleright" in operator:
                 return Exists(
                     [x, u],
                     And(
                         extended_verify(x, Y, eval_world),
                         is_alternative(u, x, eval_world),
                         true_at(Z, u),
                     ),
@@ -449,39 +479,39 @@
         x = BitVec("f_x", N)
         y = BitVec("f_y", N)
         u = BitVec("f_u", N)
         if len(sentence) == 1:
             sent = sentence[0]
             return Exists(x, And(is_part_of(x, eval_world), falsify(x, sent)))
         if len(sentence) == 2:
-            op = sentence[0]
+            operator = sentence[0]
             Y = sentence[1]
-            if "neg" in op or "not" in op:
+            if "neg" in operator or "not" in operator or "pre" in operator:
                 # print(f"TEST: neg operator = {op}")
                 return true_at(sentence[1], eval_world)
-            if 'Box' in op:
+            if 'Box' in operator:
                 return Exists(u, And(is_world(u), false_at(sentence[1], u)))
-            if 'Diamond' in op:
+            if 'Diamond' in operator:
                 return ForAll(u, Implies(is_world(u), false_at(sentence[1], u)))
         if len(sentence) == 3:
-            op = sentence[0]
+            operator = sentence[0]
             Y = sentence[1]
             Z = sentence[2]
-            if "wedge" in op:
+            if "wedge" in operator:
                 return Or(false_at(Y, eval_world), false_at(Z, eval_world))
-            if "vee" in op:
+            if "vee" in operator:
                 return And(false_at(Y, eval_world), false_at(Z, eval_world))
-            if "leftrightarrow" in op:
+            if "leftrightarrow" in operator:
                 return Or(
                     And(true_at(Y, eval_world), false_at(Z, eval_world)),
                     And(false_at(Y, eval_world), true_at(Z, eval_world)),
                 )
-            if "rightarrow" in op:
+            if "rightarrow" in operator:
                 return And(true_at(Y, eval_world), false_at(Z, eval_world))
-            if "leq" in op:
+            if "leq" in operator:
                 return Exists(
                     [x, y],
                     Or(
                         And(
                             extended_verify(x, Y, eval_world),
                             Not(extended_verify(x, Z, eval_world))
                         ),
@@ -498,15 +528,15 @@
                                     is_part_of(u, y),
                                     Not(extended_falsify(u, Y, eval_world))
                                 )
                             )
                         )
                     )
                 )
-            if "sqsubseteq" in op:
+            if "sqsubseteq" in operator:
                 return Exists(
                     [x, y],
                     Or(
                         And(
                             extended_verify(x, Y, eval_world),
                             extended_verify(y, Z, eval_world),
                             Not(extended_verify(fusion(x, y), Z, eval_world))
@@ -523,15 +553,15 @@
                         ),
                         And(
                             extended_falsify(x, Y, eval_world),
                             Not(extended_falsify(x, Z, eval_world))
                         )
                     )
                 )
-            if "equiv" in op:
+            if "equiv" in operator:
                 return Exists(
                     x,
                     Or(
                         And(
                             extended_verify(x, Y, eval_world),
                             Not(extended_verify(x, Z, eval_world))
                         ),
@@ -545,40 +575,41 @@
                         ),
                         And(
                             extended_falsify(x, Z, eval_world),
                             Not(extended_falsify(x, Y, eval_world))
                         ),
                     )
                 )
-            if "boxright" in op:
+            if "boxright" in operator:
                 # print(f"TEST: cf operator = {op}, ant = {Y}, con = {Z}")
                 return Exists(
                     [x, u],
                     And(
                         extended_verify(x, Y, eval_world),
                         is_alternative(u, x, eval_world),
                         false_at(Z, u)),
                 )
-            if "circleright" in op:
+            if "circleright" in operator:
                 return ForAll(
                     [x, u],
                     Implies(
                         And(
                             extended_verify(x, Y, eval_world),
                             is_alternative(u, x, eval_world)
                         ),
                         false_at(Z, u),
                     ),
                 )
         raise ValueError(
             f'No if statements triggered in false_at for {sentence} at world {eval_world}'
         )
 
-    def prop_const(atom):
+    def make_atom_prop_constraint(atom):
         """
+        Input: an atomic proposition as an AtomSort (ie, NOT in prefix notation)
         atom is a proposition since its verifiers and falsifiers are closed under
         fusion respectively, and the verifiers and falsifiers for atom are
         incompatible (exclusivity). NOTE: exhaustivity crashes Z3 so left off.
         returns a Z3 constraint for the proposition atom
         """
         x = BitVec("prop_x", N)
         y = BitVec("prop_y", N)
@@ -622,32 +653,40 @@
         returns a list of Z3 constraints"""
         x = BitVec("frame_x", N)
         y = BitVec("frame_y", N)
         z = BitVec("frame_z", N)
         frame_constraints = [
             ForAll([x, y], Implies(And(possible(y), is_part_of(x, y)), possible(x))),
             ForAll([x, y], Exists(z, fusion(x, y) == z)),
-            is_world(w), # w is passed in from the big outer function
+            is_world(w), # w is passed in from the big outer function define_N_semantics
         ]
         return frame_constraints
 
     def find_prop_constraints(sentence_letters):
+        """Input: a list of all sentence letters in the premises and conclusions, as returned
+        by the function all_sentence_letters (i.e., a list of AtomSorts).
+        Returns the a list of the Z3 constraints that each atomic proposition gets, which is
+        the one defined by make_atom_prop_constraint.
+        Note that all atomic propositions all get the same one, except if the atomic proposition
+        is \\top, in which case it gets its own constraint that every state verifies it and none
+        falsify it.
+        """
         prop_constraints = []
         for sent_letter in sentence_letters:
             if 'top' in str(sent_letter):
                 x = BitVec("top_x", N)
                 top_constraint = ForAll(x,
                     And(
                         verify(x,sent_letter),
                         Not(falsify(x,sent_letter))
                     )
                 )
                 prop_constraints.append(top_constraint)
-                continue # ie, prop_const should never be called on '\\top'
-            for constraint in prop_const(sent_letter):
+                continue # ie, make_atom_prop_constraint should never be called on '\\top'
+            for constraint in make_atom_prop_constraint(sent_letter):
                 prop_constraints.append(constraint)
         return prop_constraints
 
     def find_premise_const(prefix_premises):
         """find constraints corresponding to the input sentences
         takes in sentences in prefix form and the input sentence letters (a list of AtomSorts)
         returns a list of Z3 constraints
@@ -661,15 +700,15 @@
     def find_conclusion_const(prefix_conclusions):
         """find constraints corresponding to the input sentences
         takes in sentences in prefix form and the input sentence letters (a list of AtomSorts)
         returns a list of Z3 constraints
         used in find_all_constraints"""
         conclusion_constraints = []
         for conclusion in prefix_conclusions:
-            conclusion_constraint = false_at(conclusion, w)
+            conclusion_constraint = false_at(conclusion, w) # M: is there a reason you chose to do it like this?
             conclusion_constraints.append(conclusion_constraint)
         return conclusion_constraints
 
     # def find_sent_constraints(prefix_premises,prefix_conclusions):
     #     """find constraints corresponding to the input sentences
     #     takes in sentences in prefix form and the input sentence letters (a list of AtomSorts)
     #     returns a list of Z3 constraints
@@ -699,15 +738,15 @@
         premise_constraints = find_premise_const(prefix_premises)
         conclusion_constraints = find_conclusion_const(prefix_conclusions)
         return frame_constraints, prop_constraints, premise_constraints, conclusion_constraints
 
     return find_all_constraints
 
 
-def solve_constraints(all_constraints): # all_constraints is a list
+def solve_constraints(all_constraints): # all_constraints is a list of constraints
     """find model for the input constraints if there is any
     returns a tuple with a boolean representing if the constraints were solved or not
     and, if True, the model, if False the unsatisfiable core of the constraints"""
     solver = Solver()
     solver.add(all_constraints)
     result = solver.check(*[all_constraints])
     if result == sat:
```

### Comparing `model_checker-0.4.4/src/model_checker/syntax.py` & `model_checker-0.4.5/src/model_checker/syntax.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 AtomSort = DeclareSort("AtomSort")
 capital_alphabet = {"A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M",
                     "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z",}
 unary_operators = {
     "\\neg", "neg",
     "\\not", "not",
+    "\\pre", "pre",
     "Box", "\\Box",
     "Diamond", "\\Diamond"
 }
 binary_operators = {
     "\\wedge", "wedge",
     "\\vee", "vee",
     "\\rightarrow", "rightarrow",
```

### Comparing `model_checker-0.4.4/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.4.5/src/model_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.4.4
+Version: 0.4.5
 Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,15 @@
 
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for finding countermodels for claims which include modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 The language currently includes the following operators:
 
   - `neg` for _negation_
-  - `not` for _exclusion_
+  <!-- - `not` for _exclusion_ -->
   - `wedge` for _conjunction_
   - `vee` for _disjunction_
   - `rightarrow` for _material conditional_
   - `leftrightarrow` for _material biconditional_
   - `Box` for _necessity_
   - `Diamond` for _possibility_
   - `boxright` for the _must counterfactual conditional_
@@ -86,17 +86,17 @@
 A _negated sentence_ is verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 A _conjunctive sentence_ is verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 A _disjunctive sentence_ is verified by the verifiers for either disjunct or fusions thereof and falsified by pairwise fusions of falsifiers for the disjuncts.
 Conjunction and disjunction are dual operators obeying the standard idempotence and De Morgan laws.
 The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
 For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
-By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_.
-In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`.
-This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison.
+<!-- By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_. -->
+<!-- In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`. -->
+<!-- This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison. -->
 
 A _necessity sentence_ `Box A` is true at a world just in case every world state includes a part that verifies `A` and a _possibility sentence_ `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
 Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include as parts both `s` and a maximal part of `w` that is compatible with `s`.
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
```

