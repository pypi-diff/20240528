# Comparing `tmp/mentabotix-0.1.5.7.tar.gz` & `tmp/mentabotix-0.1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.5.7.tar", last modified: Mon May 27 10:06:53 2024, max compression
+gzip compressed data, was "mentabotix-0.1.5.8.tar", last modified: Mon May 27 12:07:42 2024, max compression
```

## Comparing `mentabotix-0.1.5.7.tar` & `mentabotix-0.1.5.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1066 2024-05-27 10:06:28.724521 mentabotix-0.1.5.7/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-27 10:06:28.724521 mentabotix-0.1.5.7/README.md
--rw-r--r--   0        0        0      613 2024-05-27 10:06:53.284565 mentabotix-0.1.5.7/pyproject.toml
--rw-r--r--   0        0        0     1301 2024-05-27 10:06:28.724521 mentabotix-0.1.5.7/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    77701 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0    20857 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0      867 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/tools/selectors.py
--rw-r--r--   0        0        0        0 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/find_tests.py
--rw-r--r--   0        0        0    15660 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_botix.py
--rw-r--r--   0        0        0     2521 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_case_registry.py
--rw-r--r--   0        0        0    11493 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_menta.py
--rw-r--r--   0        0        0    10694 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_moving_state.py
--rw-r--r--   0        0        0     7475 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-27 12:07:18.378980 mentabotix-0.1.5.8/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-27 12:07:18.378980 mentabotix-0.1.5.8/README.md
+-rw-r--r--   0        0        0      613 2024-05-27 12:07:42.530809 mentabotix-0.1.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1301 2024-05-27 12:07:18.378980 mentabotix-0.1.5.8/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    79930 2024-05-27 12:07:18.378980 mentabotix-0.1.5.8/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0    20857 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0      867 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/tools/selectors.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/find_tests.py
+-rw-r--r--   0        0        0    15660 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_botix.py
+-rw-r--r--   0        0        0     2521 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_case_registry.py
+-rw-r--r--   0        0        0    11493 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_menta.py
+-rw-r--r--   0        0        0    11921 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_moving_state.py
+-rw-r--r--   0        0        0     7475 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.8/PKG-INFO
```

### Comparing `mentabotix-0.1.5.7/LICENSE` & `mentabotix-0.1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/README.md` & `mentabotix-0.1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/pyproject.toml` & `mentabotix-0.1.5.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.5.7"
+version = "0.1.5.8"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.5.7/src/mentabotix/__init__.py` & `mentabotix-0.1.5.8/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/src/mentabotix/modules/botix.py` & `mentabotix-0.1.5.8/src/mentabotix/modules/botix.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,60 @@
             raise ValueError(f"used_context_variables can't contain duplicated item!")
         for variable in used_context_variables:
             if any(variable in str(expression) for expression in speed_expressions):
                 continue
             raise ValueError(f"Variable {variable} not found in {speed_expressions}.")
 
     @classmethod
+    def rand_move(
+        cls,
+        con: CloseLoopController,
+        speeds: Sequence[Tuple[int, int, int, int]],
+        weights: Optional[Sequence[float | int]] = None,
+        used_ctx_varname: str = "rand_move",
+    ) -> Self:
+        """
+        Registers a random movement behavior with the given CloseLoopController.
+
+        This method randomly selects a speed tuple from the provided list and updates the turn direction
+        before entering the behavior. If weights are provided, the selection is made according to them.
+
+        Args:
+            con: CloseLoopController instance to register the behavior with.
+            speeds: A sequence of speed tuples, each representing velocities for four directions.
+            weights: Optional sequence of weights corresponding to the speeds. If given, the selection is weighted.
+            used_ctx_varname: str, the name of the context variable to store the selected speed.
+
+        Returns:
+            Self: An instance of the class with the random move behavior configured.
+        """
+        if weights and len(weights) != len(speeds):
+            raise ValueError(f"weights and speeds must have the same length, got speeds: {speeds}, weights: {weights}.")
+        indexes = tuple(range(len(speeds)))
+
+        # Register a context updater to update the turn direction before entering the behavior.
+        _updater = con.register_context_updater(
+            make_weighted_selector(speeds, weights) if weights else lambda: speeds[choice(indexes)],
+            output_keys=[used_ctx_varname],
+            input_keys=[],
+        )
+
+        # Configure speed expressions and actions before entering, implementing random turning.
+        return cls(
+            speed_expressions=(
+                f"{used_ctx_varname}[0]",
+                f"{used_ctx_varname}[1]",
+                f"{used_ctx_varname}[2]",
+                f"{used_ctx_varname}[3]",
+            ),
+            used_context_variables=[used_ctx_varname],
+            before_entering=[_updater],
+        )
+
+    @classmethod
     def halt(cls) -> Self:
         """
         Create a new instance of the class with a speed of 0, effectively halting the movement.
 
         Returns:
             Self: A new instance of the class with a speed of 0.
         """
@@ -358,15 +404,16 @@
             speeds (Sequence[int]): A sequence of speeds.
             weights (Optional[Sequence[float | int]]): Weights for each speed.
             used_ctx_varname (str, optional): The name of the context variable to store the selected speed.
 
         Returns:
 
         """
-
+        if weights and len(weights) != len(speeds):
+            raise ValueError(f"weights and speeds must have the same length, got speeds: {speeds}, weights: {weights}.")
         # Register a context updater to update the turn direction before entering this behavior.
         _updater = con.register_context_updater(
             make_weighted_selector(speeds, weights) if weights else lambda: choice(speeds),
             output_keys=[used_ctx_varname],
             input_keys=[],
         )
```

### Comparing `mentabotix-0.1.5.7/src/mentabotix/modules/logger.py` & `mentabotix-0.1.5.8/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/src/mentabotix/modules/menta.py` & `mentabotix-0.1.5.8/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/src/mentabotix/tools/composers.py` & `mentabotix-0.1.5.8/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/src/mentabotix/tools/generators.py` & `mentabotix-0.1.5.8/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/src/mentabotix/tools/selectors.py` & `mentabotix-0.1.5.8/src/mentabotix/tools/selectors.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/tests/find_tests.py` & `mentabotix-0.1.5.8/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/tests/test_botix.py` & `mentabotix-0.1.5.8/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/tests/test_case_registry.py` & `mentabotix-0.1.5.8/tests/test_case_registry.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/tests/test_composer.py` & `mentabotix-0.1.5.8/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/tests/test_menta.py` & `mentabotix-0.1.5.8/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/tests/test_moving_state.py` & `mentabotix-0.1.5.8/tests/test_moving_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
         con = CloseLoopController(
             [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
         ).start_msg_sending()
         state = MovingState.rand_dir_turn(con, 500)
         print(state)
         end = MovingState(0)
-        trans = MovingTransition(1, from_states=[state], to_states={0: end})
+        trans = MovingTransition(0.2, from_states=[state], to_states={0: end})
 
         b = Botix(controller=con, token_pool=[trans])
 
         fun = b.compile()
         fun()
         con.stop_msg_sending()
         con.serial_client.close()
@@ -196,15 +196,15 @@
         state = MovingState.rand_spd_turn(
             con,
             "l",
             [500, 600, 700],
         )
         print(state)
         end = MovingState(0)
-        trans = MovingTransition(1, from_states=[state], to_states={0: end})
+        trans = MovingTransition(0.2, from_states=[state], to_states={0: end})
 
         b = Botix(controller=con, token_pool=[trans])
 
         fun = b.compile()
         for _ in range(2):
             fun()
             sleep(0.2)
@@ -216,15 +216,15 @@
 
         con = CloseLoopController(
             [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
         ).start_msg_sending()
         state = MovingState.rand_spd_turn(con, "l", [500, 600, 700], weights=[10, 80, 10])
         print(state)
         end = MovingState(0)
-        trans = MovingTransition(1, from_states=[state], to_states={0: end})
+        trans = MovingTransition(0.2, from_states=[state], to_states={0: end})
 
         b = Botix(controller=con, token_pool=[trans])
 
         fun = b.compile()
         for _ in range(2):
             fun()
             sleep(0.2)
@@ -236,15 +236,15 @@
 
         con = CloseLoopController(
             [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
         ).start_msg_sending()
         state = MovingState.rand_dir_spd_turn(con, [500, 600, -700], weights=[10, 80, 10])
         print(state)
         end = MovingState(0)
-        trans = MovingTransition(1, from_states=[state], to_states={0: end})
+        trans = MovingTransition(0.2, from_states=[state], to_states={0: end})
 
         b = Botix(controller=con, token_pool=[trans])
 
         fun = b.compile()
         for _ in range(2):
             fun()
             sleep(0.2)
@@ -256,21 +256,51 @@
 
         con = CloseLoopController(
             [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
         ).start_msg_sending()
         state = MovingState.rand_spd_straight(con, [500, 600, 700], weights=[10, 80, 10])
         print(state)
         end = MovingState(0)
-        trans = MovingTransition(1, from_states=[state], to_states={0: end})
+        trans = MovingTransition(0.2, from_states=[state], to_states={0: end})
 
         b = Botix(controller=con, token_pool=[trans])
 
         fun = b.compile()
         for _ in range(2):
             fun()
             sleep(0.2)
         con.stop_msg_sending()
         con.serial_client.close()
 
+    def test_rand_move_with_weights(self):
+        from mentabotix import MovingTransition, Botix
+
+        con = CloseLoopController(
+            [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
+        ).start_msg_sending()
+        with self.assertRaises(ValueError):
+            state = MovingState.rand_move(
+                con, [(500, 600, 700, 1100), (8000, 7000, 6000, 5000)], weights=[10, 80, 10, 10]
+            )
+        state = MovingState.rand_move(con, [(500, 600, 700, 1100), (8000, 7000, 6000, 5000)], weights=[10, 80])
+        state_no_weights = MovingState.rand_move(con, [(500, 600, 700, 1100), (8000, 7000, 6000, 5000)])
+        print(state)
+        end = MovingState(0)
+        trans = MovingTransition(0.2, from_states=[state], to_states={0: end})
+
+        b = Botix(controller=con, token_pool=[trans])
+
+        fun = b.compile()
+        for _ in range(10):
+            fun()
+        trans = MovingTransition(0.2, from_states=[state_no_weights], to_states={0: end})
+
+        b.token_pool = [trans]
+        fun_2 = b.compile()
+        for _ in range(10):
+            fun_2()
+        con.stop_msg_sending()
+        con.serial_client.close()
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.5.7/tests/test_moving_transition.py` & `mentabotix-0.1.5.8/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.7/PKG-INFO` & `mentabotix-0.1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.5.7
+Version: 0.1.5.8
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: terminaltables>=3.1.10
```

