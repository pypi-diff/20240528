# Comparing `tmp/amplify-1.1.0-cp39-cp39-win_amd64.whl.zip` & `tmp/amplify-1.1.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 5772413 bytes, number of entries: 14
+Zip file size: 5772412 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     1890 b- defN 24-Feb-20 03:48 amplify/__init__.py
--rw-rw-rw-  2.0 fat   248086 b- defN 24-May-14 13:46 amplify/__init__.pyi
+-rw-rw-rw-  2.0 fat   248092 b- defN 24-May-28 08:08 amplify/__init__.pyi
 -rw-rw-rw-  2.0 fat    16848 b- defN 24-Mar-28 08:00 amplify/_backward.py
--rw-rw-rw-  2.0 fat 18060288 b- defN 24-May-14 13:46 amplify/amplify.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat 18060288 b- defN 24-May-28 08:08 amplify/amplify.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     2564 b- defN 24-Feb-20 03:48 amplify/constraint.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-14 13:46 amplify/py.typed
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-28 08:08 amplify/py.typed
 -rw-rw-rw-  2.0 fat     4397 b- defN 24-May-09 05:53 amplify/client/__init__.py
 -rw-rw-rw-  2.0 fat      672 b- defN 24-Mar-28 08:00 amplify/client/ocean.py
--rw-rw-rw-  2.0 fat    19518 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    26624 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat    24247 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/open_source_license.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-14 13:43 amplify-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1135 b- defN 24-May-14 13:46 amplify-1.1.0.dist-info/RECORD
-14 files, 18406377 bytes uncompressed, 5770549 bytes compressed:  68.7%
+-rw-rw-rw-  2.0 fat    19518 b- defN 24-May-28 08:08 amplify-1.1.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    26624 b- defN 24-May-28 08:08 amplify-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-28 08:08 amplify-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat    24247 b- defN 24-May-28 08:08 amplify-1.1.1.dist-info/open_source_license.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-28 08:05 amplify-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1135 b- defN 24-May-28 08:08 amplify-1.1.1.dist-info/RECORD
+14 files, 18406383 bytes uncompressed, 5770548 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: amplify/client/__init__.py
 Comment: 
 
 Filename: amplify/client/ocean.py
 Comment: 
 
-Filename: amplify-1.1.0.dist-info/LICENSE.txt
+Filename: amplify-1.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: amplify-1.1.0.dist-info/METADATA
+Filename: amplify-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: amplify-1.1.0.dist-info/WHEEL
+Filename: amplify-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: amplify-1.1.0.dist-info/open_source_license.txt
+Filename: amplify-1.1.1.dist-info/open_source_license.txt
 Comment: 
 
-Filename: amplify-1.1.0.dist-info/top_level.txt
+Filename: amplify-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: amplify-1.1.0.dist-info/RECORD
+Filename: amplify-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## amplify/__init__.pyi

```diff
@@ -8048,90 +8048,90 @@
     Args:
         arg (int):
     """
 
 @overload
 def solve(
     model: Model,
-    client: AmplifyClient,
+    client: _AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: Literal[False] = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Result[_AmplifyClient]: ...
 @overload
 def solve(
     model: Model,
-    client: AmplifyClient,
+    client: _AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: Literal[True] = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Result[Literal[None]]: ...
 @overload
 def solve(
     model: Model,
-    client: AmplifyClient,
+    client: _AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: bool = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Union[Result[_AmplifyClient], Result[Literal[None]]]: ...
 @overload
 def solve(
     model: Union[Poly, Matrix, Constraint, ConstraintList],
-    client: AmplifyClient,
+    client: _AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: Literal[False] = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Result[_AmplifyClient]: ...
 @overload
 def solve(
     model: Union[Poly, Matrix, Constraint, ConstraintList],
-    client: AmplifyClient,
+    client: _AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: Literal[True] = ...,
     num_solves: int = ...,
     filter_solution: bool = ...,
     sort_solution: bool = ...,
 ) -> Result[Literal[None]]: ...
 @overload
 def solve(
     model: Union[Poly, Matrix, Constraint, ConstraintList],
-    client: AmplifyClient,
+    client: _AmplifyClient,
     integer_encoding_method: Union[Literal["Unary", "Linear", "Binary", "Default"], IntegerEncodingMethod] = ...,
     quadratization_method: Union[Literal["IshikawaKZFD", "Substitute"], QuadratizationMethod] = ...,
     substitution_multiplier: float = ...,
     embedding_method: Union[Literal["Default", "Clique", "Minor", "Parallel"], EmbeddingMethod] = ...,
     embedding_timeout: Union[float, datetime.timedelta] = ...,
     chain_strength: float = ...,
     dry_run: bool = ...,
```

## Comparing `amplify-1.1.0.dist-info/LICENSE.txt` & `amplify-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `amplify-1.1.0.dist-info/METADATA` & `amplify-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplify
-Version: 1.1.0
+Version: 1.1.1
 Summary: Amplify SDK for Quantum Annealing and Ising Machines
 Author-email: "Fixstars Amplify Corp." <y_matsuda@fixstars.com>
 Maintainer-email: Yoshiki Matsuda <y_matsuda@fixstars.com>
 License: Terms of Use
         ________________________________________
         These Terms of Use stipulate the terms and conditions for the granting of licenses by Fixstars Amplify Corporation (“we”, “us”, “our”) to the User for use of Fixstars Amplify (“Service”), which provides Users with a software development environment and computational resources for solving mathematical optimization problems. There are two types of Service plans: the “Free plan” with certain restrictions on the scope of use, and the “Paid plan” with no such restrictions. Unless otherwise specified, these Terms apply to both plan types.
         Before using the Service, the User shall carefully read and agree to the entire text of these Terms of Use. When they click on our website to the effect that they agree to these Terms of Use, or complete the other procedures specified by us, a contract for the use of the Service is established, and the User is deemed to have fully agreed to these Terms of Use.
```

## Comparing `amplify-1.1.0.dist-info/open_source_license.txt` & `amplify-1.1.1.dist-info/open_source_license.txt`

 * *Files identical despite different names*

## Comparing `amplify-1.1.0.dist-info/RECORD` & `amplify-1.1.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 amplify/__init__.py,sha256=FGKpQMKEqPuge4tlXiQx60d1hus0NoIoppooVyrU1B8,1890
-amplify/__init__.pyi,sha256=2J3MSvU2I7UohNNlbvWtKLHa1hXdfbxk1tyC3bgpBxg,248086
+amplify/__init__.pyi,sha256=MmJldjZkHeVDm6oLA3Xi6Ym5cn2jbpgGPbr3AZgHdyg,248092
 amplify/_backward.py,sha256=raEOk7NV1fBGsIIv_56gIrSzEU1-MWvMaLALU-9F_b0,16848
-amplify/amplify.cp39-win_amd64.pyd,sha256=B-PZUuIn5PqRk7S-IZc9LM5tmDjJD_Z-1d_DdRK-6yc,18060288
+amplify/amplify.cp39-win_amd64.pyd,sha256=LTe_1Uo0a---8m1BEzhSJAXN-ksj-IzJ5HDd-FL0g-8,18060288
 amplify/constraint.py,sha256=n66Ttd3rCQJIW2zMuywYZlKP-y0_n8ZkVGZSsJWEUzI,2564
 amplify/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 amplify/client/__init__.py,sha256=9Uml9Wkdo-BZBZhnh3PohHJicSwzQ8xJ1GqKf4-iJ4g,4397
 amplify/client/ocean.py,sha256=i6h9Fv4Fp6JTuz8Qi6g_uckuJwDBtmXSleT0YZBotuY,672
-amplify-1.1.0.dist-info/LICENSE.txt,sha256=Np2WJcJrsMr9Yoyt7zoNynJAiM-DNggnaK2mcz12s50,19518
-amplify-1.1.0.dist-info/METADATA,sha256=hD4KbnoiA8YZwpjBPuKTruY2q7JDmtVoNy-jRtLZjpU,26624
-amplify-1.1.0.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-amplify-1.1.0.dist-info/open_source_license.txt,sha256=SIObizROV2fUOzW5dxFeCbt3Xw61ZVJp6yLOuyDD1fQ,24247
-amplify-1.1.0.dist-info/top_level.txt,sha256=Thv8V_aiMgH7cFEe3_nYCAbxqKPCBEUNiD7m9BPPtg8,8
-amplify-1.1.0.dist-info/RECORD,,
+amplify-1.1.1.dist-info/LICENSE.txt,sha256=Np2WJcJrsMr9Yoyt7zoNynJAiM-DNggnaK2mcz12s50,19518
+amplify-1.1.1.dist-info/METADATA,sha256=sTXHu0eQDDyQCU7_iuaXc9jzOBOcT1wfZFLdOeQOmlI,26624
+amplify-1.1.1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
+amplify-1.1.1.dist-info/open_source_license.txt,sha256=SIObizROV2fUOzW5dxFeCbt3Xw61ZVJp6yLOuyDD1fQ,24247
+amplify-1.1.1.dist-info/top_level.txt,sha256=Thv8V_aiMgH7cFEe3_nYCAbxqKPCBEUNiD7m9BPPtg8,8
+amplify-1.1.1.dist-info/RECORD,,
```

