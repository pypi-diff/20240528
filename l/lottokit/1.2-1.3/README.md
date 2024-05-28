# Comparing `tmp/lottokit-1.2.tar.gz` & `tmp/lottokit-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lottokit-1.2.tar", last modified: Fri May 24 07:28:08 2024, max compression
+gzip compressed data, was "lottokit-1.3.tar", last modified: Tue May 28 07:32:39 2024, max compression
```

## Comparing `lottokit-1.2.tar` & `lottokit-1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-24 07:28:08.372195 lottokit-1.2/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-1.2/LICENSE
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-24 07:28:08.372089 lottokit-1.2/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-04-15 06:05:32.000000 lottokit-1.2/README.md
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-24 07:28:08.370642 lottokit-1.2/lottokit/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-1.2/lottokit/__init__.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    73989 2024-05-24 07:16:45.000000 lottokit-1.2/lottokit/daletou.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    85918 2024-05-05 05:42:52.000000 lottokit-1.2/lottokit/util.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-24 07:28:08.371667 lottokit-1.2/lottokit.egg-info/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/requires.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/top_level.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-1.2/pyproject.toml
--rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-05-24 07:28:08.372234 lottokit-1.2/setup.cfg
--rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-05-24 07:26:55.000000 lottokit-1.2/setup.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-24 07:28:08.371792 lottokit-1.2/tests/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-1.2/tests/test.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-28 07:32:39.424133 lottokit-1.3/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-1.3/LICENSE
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-28 07:32:39.424016 lottokit-1.3/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-04-15 06:05:32.000000 lottokit-1.3/README.md
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-28 07:32:39.423183 lottokit-1.3/lottokit/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-1.3/lottokit/__init__.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    88683 2024-05-28 07:30:05.000000 lottokit-1.3/lottokit/daletou.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    93793 2024-05-28 07:29:46.000000 lottokit-1.3/lottokit/util.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-28 07:32:39.423758 lottokit-1.3/lottokit.egg-info/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-28 07:32:39.000000 lottokit-1.3/lottokit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-05-28 07:32:39.000000 lottokit-1.3/lottokit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-05-28 07:32:39.000000 lottokit-1.3/lottokit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      173 2024-05-28 07:32:39.000000 lottokit-1.3/lottokit.egg-info/requires.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-05-28 07:32:39.000000 lottokit-1.3/lottokit.egg-info/top_level.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-1.3/pyproject.toml
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-05-28 07:32:39.424170 lottokit-1.3/setup.cfg
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)     1211 2024-05-28 07:32:03.000000 lottokit-1.3/setup.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-28 07:32:39.423864 lottokit-1.3/tests/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-1.3/tests/test.py
```

### Comparing `lottokit-1.2/LICENSE` & `lottokit-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lottokit-1.2/PKG-INFO` & `lottokit-1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 1.2
+Version: 1.3
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.9
```

### Comparing `lottokit-1.2/lottokit/daletou.py` & `lottokit-1.3/lottokit/daletou.py`

 * *Files 12% similar despite different names*

```diff
@@ -657,190 +657,324 @@
         for i in range(delta.days % 7 + 1):
             if (first_day_of_year + timedelta(days=i)).weekday() in [0, 2, 5]:
                 next_period += 1
 
         # Return the draw number of the next t for the current year
         return next_period
 
-    def get_kill_numbers(self, data: List[Any], next_period: int = None, next_weekday: int = None) -> Tuple[
+    def get_kill_numbers(
+            self,
+            data: List[Any],
+            next_period: int = None,
+            next_weekday: int = None,
+            show_details: str = None
+    ) -> Tuple[
         Set[int], Set[int]]:
         """
         Calculate and return sets of 'kill numbers' for both front and back sequences based on provided data.
 
         Parameters:
             data (List[Any]): The data to process.
             next_period (int, optional): The next period number. If None, it's calculated.
             next_weekday (int, optional): The next weekday number. If None, it's calculated.
+            show_details: ['en' | 'zh'] str flag to output details about the prediction, default is None
 
         Returns:
             Tuple[Set[int], Set[int]]: A tuple containing two sets of kill numbers for front and back sequences.
         """
         front_sequences = [self.calculate_front(d) for d in data]
         back_sequences = [self.calculate_back(d) for d in data]
 
         next_weekday = next_weekday or self.get_next_weekday()
         next_period = next_period or self.get_next_period()
 
-        front_kill_numbers = self.calculate_front_kills(front_sequences, next_period, next_weekday)
-        back_kill_numbers = self.calculate_back_kills(back_sequences, next_weekday)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"last award front data: {sorted(front_sequences[-1])}",
+        #                 zh=f"最近一期中奖前区: {sorted(front_sequences[-1])}")
+        front_kill_numbers = self.calculate_front_kills(front_sequences, next_period, next_weekday,
+                                                        show_details=show_details)
+        front_kill_numbers = {num for num in front_kill_numbers if 1 <= num <= self.front_vocab_size}
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"front kill numbers: {sorted(front_kill_numbers)}, size: {len(front_kill_numbers)}",
+        #                 zh=f"前区杀码: {sorted(front_kill_numbers)}, 数量: {len(front_kill_numbers)}")
 
         # Ensure numbers are within the valid range
-        front_kill_numbers = {num for num in front_kill_numbers if 1 <= num <= self.front_vocab_size}
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"last award back data: {sorted(back_sequences[-1])}",
+        #                 zh=f"最近一期中奖后区: {sorted(back_sequences[-1])}")
+        back_kill_numbers = self.calculate_back_kills(back_sequences, next_weekday, show_details=show_details)
         back_kill_numbers = {num for num in back_kill_numbers if 1 <= num <= self.back_vocab_size}
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"back kill numbers: {sorted(back_kill_numbers)}, size: {len(back_kill_numbers)}",
+        #                 zh=f"后区杀码: {sorted(back_kill_numbers)}, 数量: {len(back_kill_numbers)}")
 
         return front_kill_numbers, back_kill_numbers
 
-    @staticmethod
-    def get_same_number_index(pre_data, cur_data):
-        same_number_index = []
-        for ind, num in enumerate(pre_data):
-            if num in cur_data:
-                same_number_index.append(ind + 1)
-        return same_number_index
-
-    @staticmethod
-    def get_edge_number_index(pre_data, cur_data):
-        edge_info = []
-        for ind, num in enumerate(pre_data):
-            edge_nums = set(num + i for i in [-1, 1])
-            plead_edge = set(cur_data).intersection(edge_nums)
-            if len(plead_edge) > 0:
-                edge_info.append(ind + 1)
-        return edge_info
-
-    def calculate_front_kills(self, sequences: List[List[int]], next_period: int, next_weekday: int) -> Set[int]:
+    def calculate_front_kills(
+            self,
+            sequences: List[List[int]],
+            next_period: int,
+            next_weekday: int,
+            show_details: str = None
+    ) -> Set[int]:
         """Helper function to calculate front kill numbers based on the last sequence."""
-
         def train_predict(chunk, func_name, chunk_size=1):
             train_data = [result
                           for c, n in self.get_chunks_with_next(chunk, chunk_size)
                           for result in func_name(c[-1], n)]
             return (
-                {self.exponential_moving_average_next_value(train_data),
-                 self.linear_regression_next_value_by_index(train_data),
-                 self.harmonic_regression_next_value_by_index(train_data)}
+                {
+                    self.exponential_moving_average_next_value(train_data),
+                    self.linear_regression_next_value_by_index(train_data),
+                    self.harmonic_regression_next_value_by_index(train_data)
+                }
                 if len(train_data) > 2 else {}
             )
 
+        kills = set()
         last_sequence = sequences[-1]
-        a1, a2, a3, a4, a5 = last_sequence
-        fb = abs(a5 - a3 - a1)
-        fc = a4 - a2
-        average = sum(last_sequence) // self.front_size
-
-        kills = {fb + t for t in [0, 1, 3, 6] if abs(t) != next_weekday}
-        if fb == 0:
-            kills.update({a1, a3, a5})
-        kills.update({fc, (fc + next_period) % self.front_vocab_size, abs(fc - next_period) % self.front_vocab_size})
-        kills.update({average, sum([a1, a2, a3]) // 3})
-        kills.update({(a1 + a2) - (a3 + a4) - a5, a1 + a2 + a3 + a4 - a5})
-
-        # odd_even_ratio = [n - 1 if n != 0 else n for n in set(self.calculate_odd_even_ratio(sequences[-1]))]
-        zone_ratio = [n - 1 if n != 0 else n for n in set(self.calculate_zone_ratio(sequences[-1],
-                                                                                    self.front_zone_ranges))]
-        span = self.calculate_span(sequences[-1])
-        edge_index = train_predict(sequences, self.get_edge_number_index)
-        same_index = train_predict(sequences, self.get_edge_number_index)
-        kills.update({
-            abs(sequences[-1][zone_ratio[0]] - sequences[-1][zone_ratio[-1]]),
-            (sequences[-1][zone_ratio[0]] + sequences[-1][zone_ratio[-1]]) % 35,
-            abs(sequences[-1][-zone_ratio[0]] - sequences[-1][-zone_ratio[-1]]),
-            (sequences[-1][-zone_ratio[0]] + sequences[-1][-zone_ratio[-1]]) % 35,
-            abs(sequences[-1][0] - span),
-            (sequences[-1][-1] + span) % 35,
-            span
-        })
-        if edge_index:
-            kills.update(sequences[-1][edge - 1] + i for edge in edge_index if edge - 1 in range(5) for i in [-1, 1])
-
-        if same_index:
-            kills.update(sequences[-1][same - 1] for same in same_index if same - 1 in range(5))
+        odd_even_ratio = self.calculate_odd_even_ratio(last_sequence)
+        zone_ratio = self.calculate_zone_ratio(last_sequence, self.front_zone_ranges)
+        zone_ratio_index = [min((n - 1 if n != 0 else n) for n in zone_ratio),
+                            max((n - 1 if n != 0 else n) for n in zone_ratio)]
+        euclidean_distance = self.calculate_euclidean_distance((zone_ratio[0], zone_ratio[-1]),
+                                                               (odd_even_ratio[0], odd_even_ratio[-1]))
+        indices = [zone_ratio_index[0], zone_ratio_index[-1]]
+        reverse_indices = [-(zone_ratio_index[0] + 1), -(zone_ratio_index[-1] + 1)]
+        zone_ratio_index_num_set = {
+            abs(last_sequence[indices[0]] - last_sequence[indices[1]]) + euclidean_distance,
+            (abs(last_sequence[indices[0]] + last_sequence[indices[1]]) + euclidean_distance) % self.front_vocab_size,
+            abs(last_sequence[reverse_indices[0]] - last_sequence[reverse_indices[1]]) + euclidean_distance,
+            (abs(last_sequence[reverse_indices[0]] + last_sequence[reverse_indices[1]]) + euclidean_distance) % self.front_vocab_size,
+        }
+        kills.update(zone_ratio_index_num_set)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"The difference between the sum of the filter zone ratio "
+        #                    f"and the corresponding subscript: {sorted(zone_ratio_index_num_set)}, size: {len(zone_ratio_index_num_set)}",
+        #                 zh=f"过滤区间比对应下标的和差值: {sorted(zone_ratio_index_num_set)}, 数量: {len(zone_ratio_index_num_set)}")
+
+        zone_average_set = set()
+        for zone in self.front_zone_ranges:
+            tmp = [n for n in last_sequence if n in range(zone[0], zone[1] + 1)]
+            if len(tmp) == 1:
+                unique_index = last_sequence.index(tmp[0])
+                tmp = [last_sequence[unique_index - 1], last_sequence[(unique_index + 1) % len(last_sequence)]]
+            zone_average_set.add(self.real_round(sum(tmp) / len(tmp))) if len(tmp) > 0 else None
+        kills.update(zone_average_set)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"zone average add: {sorted(zone_average_set)}, size: {len(zone_average_set)}",
+        #                 zh=f"过滤区间平均值: {sorted(zone_average_set)}, 数量: {len(zone_average_set)}")
+
+        sum_total = self.calculate_sum_total(last_sequence)
+        sum_total_average_set = {
+            self.real_round(sum_total / self.front_size),
+            self.real_round((min(last_sequence) + max(last_sequence)) / 2)
+        }
+        kills.update(sum_total_average_set)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"sum total average add: {sorted(sum_total_average_set)}, size: {len(sum_total_average_set)}",
+        #                 zh=f"过滤和值平均值: {sorted(sum_total_average_set)}, 数量: {len(sum_total_average_set)}")
+
+        span = self.calculate_span(last_sequence)
+        span_set = {abs(last_sequence[0] - span), (last_sequence[-1] + span) % 35, span - next_weekday}
+        kills.update(span_set)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"span about add: {sorted(span_set)}, size: {len(span_set)}",
+        #                 zh=f"过滤跨度相关值: {sorted(span_set)}, 数量: {len(span_set)}")
+
+        edge_indexs = train_predict(sequences, self.calculate_edge_number_index)
+        previous_edge_index = self.calculate_edge_number_index(sequences[-2], last_sequence)
+        edge_indexs.update(set(previous_edge_index))
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"predict maybe edge indexs: {edge_indexs}",
+        #                 zh=f"预测可能的边号下标: {edge_indexs}")
+        if edge_indexs:
+            for edge in range(self.front_size):
+                if edge + 1 not in edge_indexs:
+                    kills.update(last_sequence[edge] + i for i in [-1, 1])
+
+        same_indexs = train_predict(sequences, self.calculate_same_number_index)
+        previous_same_index = self.calculate_same_number_index(sequences[-2], last_sequence)
+        same_indexs.update(set(previous_same_index))
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"predict maybe same index: {same_indexs}",
+        #                 zh=f"预测可能的同号下标: {same_indexs}")
+        if same_indexs:
+            for same in range(self.front_size):
+                if same + 1 not in same_indexs:
+                    kills.update({last_sequence[same]})
 
         return kills
 
-    def calculate_back_kills(self, sequences: List[List[int]], next_weekday: int) -> Set[int]:
+    def calculate_back_kills(self, sequences: List[List[int]], next_weekday: int, show_details: str = None) -> Set[int]:
         """Helper function to calculate back kill numbers based on the last sequence."""
-
         def train_predict(chunk, func_name, chunk_size=1):
             train_data = [result
                           for c, n in self.get_chunks_with_next(chunk, chunk_size)
                           for result in func_name(c[-1], n)]
             return (
-                {self.exponential_moving_average_next_value(train_data),
-                 self.linear_regression_next_value_by_index(train_data),
-                 self.harmonic_regression_next_value_by_index(train_data)}
+                {
+                    self.exponential_moving_average_next_value(train_data),
+                    self.linear_regression_next_value_by_index(train_data),
+                    self.harmonic_regression_next_value_by_index(train_data)
+                }
                 if len(train_data) > 2 else {}
             )
 
+        kills = set()
         last_sequence = sequences[-1]
-        b1, b2 = last_sequence
-        bb = abs(b1 - b2)
-        kills = {bb + t for t in [0, 1, 3, 6] if abs(t) != next_weekday}
-        kills.update(sequences[-2])
-        if bb == 0:
-            kills.update({b1, b2})
-        kills.update({sum(last_sequence) // self.back_size})
-
-        # odd_even_ratio = [n - 1 if n != 0 else n for n in set(self.calculate_odd_even_ratio(sequences[-1]))]
-        zone_ratio = [n - 1 if n != 0 else n for n in set(self.calculate_zone_ratio(sequences[-1],
-                                                                                    self.back_zone_ranges))]
-        span = self.calculate_span(sequences[-1])
-        edge_index = train_predict(sequences, self.get_edge_number_index)
-        same_index = train_predict(sequences, self.get_edge_number_index)
-        kills.update({
-            abs(sequences[-1][zone_ratio[0]] - sequences[-1][zone_ratio[-1]]),
-            (sequences[-1][zone_ratio[0]] + sequences[-1][zone_ratio[-1]]) % 35,
-            abs(sequences[-1][-zone_ratio[0]] - sequences[-1][-zone_ratio[-1]]),
-            (sequences[-1][-zone_ratio[0]] + sequences[-1][-zone_ratio[-1]]) % 35,
-            abs(sequences[-1][0] - span),
-            (sequences[-1][-1] + span) % 35,
-            span
-        })
-        if edge_index:
-            kills.update(sequences[-1][edge - 1] + i for edge in edge_index if edge - 1 in range(5) for i in [-1, 1])
+        odd_even_ratio = self.calculate_odd_even_ratio(last_sequence)
+        zone_ratio = self.calculate_zone_ratio(last_sequence, self.back_zone_ranges)
+        zone_ratio_index = [min((n - 1 if n != 0 else n) for n in zone_ratio),
+                            max((n - 1 if n != 0 else n) for n in zone_ratio)]
+        euclidean_distance = self.calculate_euclidean_distance((zone_ratio[0], zone_ratio[-1]),
+                                                               (odd_even_ratio[0], odd_even_ratio[-1]))
+        indices = [zone_ratio_index[0], zone_ratio_index[-1]]
+        reverse_indices = [-(zone_ratio_index[0] + 1), -(zone_ratio_index[-1] + 1)]
+        zone_ratio_index_num_set = {
+            abs(last_sequence[indices[0]] - last_sequence[indices[1]]) + euclidean_distance,
+            # (abs(last_sequence[indices[0]] + last_sequence[indices[1]]) + euclidean_distance) % self.back_vocab_size,
+            abs(last_sequence[reverse_indices[0]] - last_sequence[reverse_indices[1]]) + euclidean_distance,
+            # (abs(last_sequence[reverse_indices[0]] + last_sequence[reverse_indices[1]]) + euclidean_distance) % self.back_vocab_size,
+        }
+        kills.update(zone_ratio_index_num_set)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"The difference between the sum of the filter zone ratio "
+        #                    f"and the corresponding subscript: {sorted(zone_ratio_index_num_set)}, size: {len(zone_ratio_index_num_set)}",
+        #                 zh=f"过滤区间比对应下标的和差值: {sorted(zone_ratio_index_num_set)}, 数量: {len(zone_ratio_index_num_set)}")
+
+        zone_average_set = set()
+        for zone in self.back_zone_ranges:
+            tmp = [n for n in last_sequence if n in range(zone[0], zone[1] + 1)]
+            if len(tmp) == 1:
+                unique_index = last_sequence.index(tmp[0])
+                tmp = [last_sequence[unique_index - 1], last_sequence[(unique_index + 1) % len(last_sequence)]]
+            zone_average_set.add(self.real_round(sum(tmp) / len(tmp))) if len(tmp) > 0 else None
+        kills.update(zone_average_set)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"zone average add: {sorted(zone_average_set)}, size: {len(zone_average_set)}",
+        #                 zh=f"过滤区间平均值: {sorted(zone_average_set)}, 数量: {len(zone_average_set)}")
+
+        sum_total = self.calculate_sum_total(last_sequence)
+        sum_total_average_set = {
+            self.real_round(sum_total / self.back_size),
+            self.real_round((min(last_sequence) + max(last_sequence)) / 2)
+        }
+        kills.update(sum_total_average_set)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"sum total average add: {sorted(sum_total_average_set)}, size: {len(sum_total_average_set)}",
+        #                 zh=f"过滤和值平均值: {sorted(sum_total_average_set)}, 数量: {len(sum_total_average_set)}")
+
+        span = self.calculate_span(last_sequence)
+        span_set = {abs(last_sequence[0] - span), (last_sequence[-1] + span) % 35, span - next_weekday}
+        kills.update(span_set)
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"span about add: {sorted(span_set)}, size: {len(span_set)}",
+        #                 zh=f"过滤跨度相关值: {sorted(span_set)}, 数量: {len(span_set)}")
+
+        edge_indexs = train_predict(sequences, self.calculate_edge_number_index)
+        # previous_edge_index = self.calculate_edge_number_index(sequences[-2], last_sequence)
+        # edge_indexs.update(set(previous_edge_index))
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"predict maybe edge indexs: {edge_indexs}",
+        #                 zh=f"预测可能的边号下标: {edge_indexs}")
+        if edge_indexs:
+            for edge in range(self.back_size):
+                if edge + 1 not in edge_indexs:
+                    kills.update(last_sequence[edge] + i for i in [-1, 1])
+
+        same_indexs = train_predict(sequences, self.calculate_same_number_index)
+        # previous_same_index = self.calculate_same_number_index(sequences[-2], last_sequence)
+        # same_indexs.update(set(previous_same_index))
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"predict maybe same index: {same_indexs}",
+        #                 zh=f"预测可能的同号下标: {same_indexs}")
+        if same_indexs:
+            for same in range(self.back_size):
+                if same + 1 not in same_indexs:
+                    kills.update({last_sequence[same]})
 
-        if same_index:
-            kills.update(sequences[-1][same - 1] for same in same_index if same - 1 in range(5))
         return kills
 
-    def get_banker_numbers(self, data: List[Any], next_period: int = None, next_weekday: int = None) -> Tuple[
+    def get_banker_numbers(
+            self,
+            data: List[Any],
+            next_period: int = None,
+            next_weekday: int = None,
+            show_details: str = None
+    ) -> Tuple[
         Set[int], Set[int]]:
         """
         Calculate and return sets of 'banker numbers' for both front and back sequences based on provided data.
 
         Parameters:
             data (List[Any]): The data to process.
             next_period (int, optional): The next period number. If None, it's calculated.
             next_weekday (int, optional): The next weekday number. If None, it's calculated.
+            show_details: ['en' | 'zh'] str flag to output details about the prediction, default is None
 
         Returns:
             Tuple[Set[int], Set[int]]: A tuple containing two sets of banker numbers for front and back sequences.
         """
         front_sequences = [self.calculate_front(d) for d in data]
         back_sequences = [self.calculate_back(d) for d in data]
         next_weekday = next_weekday or self.get_next_weekday()
         next_period = next_period or self.get_next_period()
 
+        # Ensure front numbers are within the valid range
         front_banker_numbers = self.calculate_front_bankers(front_sequences, next_period, next_weekday)
-        back_backer_numbers = self.calculate_back_bankers(back_sequences, next_weekday)
-
-        # Ensure numbers are within the valid range
         front_banker_numbers = {num for num in front_banker_numbers if 1 <= num <= self.front_vocab_size}
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"back banker numbers: {sorted(front_banker_numbers)}, size: {len(front_banker_numbers)}",
+        #                 zh=f"前区胆码: {sorted(front_banker_numbers)}, 数量: {len(front_banker_numbers)}")
+
+        # Ensure back numbers are within the valid range
+        back_backer_numbers = self.calculate_back_bankers(back_sequences, next_weekday)
         back_banker_numbers = {num for num in back_backer_numbers if 1 <= num <= self.back_vocab_size}
+        # self.detail_log(app_log=self.app_log, show_details=show_details,
+        #                 en=f"back banker numbers: {sorted(back_banker_numbers)}, size: {len(back_banker_numbers)}",
+        #                 zh=f"后区胆码: {sorted(back_banker_numbers)}, 数量: {len(back_banker_numbers)}")
 
         return front_banker_numbers, back_banker_numbers
 
-    @staticmethod
-    def calculate_front_bankers(sequences: List[List[int]], next_period: int, next_weekday: int) -> Set[int]:
+    def calculate_front_bankers(
+            self,
+            sequences: List[List[int]],
+            next_period: int,
+            next_weekday: int,
+            show_details: str = None
+    ) -> Set[int]:
         """Helper function to calculate front banker numbers based on the last sequence."""
-        last_sequence = sequences[-1]
-        a1, a2, a3, a4, a5 = last_sequence
-        bankers = {a1, a2, a3, a4, a5}
-        for i in last_sequence:
-            bankers.update({i - 1, i + 1})
+
+        def train_predict(chunk, func_name, chunk_size=1):
+            train_data = [result
+                          for c, n in self.get_chunks_with_next(chunk, chunk_size)
+                          for result in func_name(c[-1], n)]
+            return (
+                {self.exponential_moving_average_next_value(train_data),
+                 self.linear_regression_next_value_by_index(train_data),
+                 self.harmonic_regression_next_value_by_index(train_data)}
+                if len(train_data) > 2 else {}
+            )
+
+        bankers = set()
+        edge_index = train_predict(sequences, self.calculate_edge_number_index)
+        self.detail_log(app_log=self.app_log, show_details=show_details,
+                        en=f"predict maybe edge index: {edge_index}",
+                        zh=f"预测可能的边号下标: {edge_index}")
+        if edge_index:
+            bankers.update(sequences[-1][edge - 1] + i for edge in edge_index if edge - 1 in range(self.front_size) for i in [-1, 1])
+        previous_edge_index = self.calculate_edge_number_index(sequences[-2], sequences[-1])
+        bankers.update(sequences[-1][edge - 1] + i for edge in previous_edge_index if edge - 1 in range(5) for i in [-1, 1])
+
+        same_index = train_predict(sequences, self.calculate_same_number_index)
+        if same_index:
+            bankers.update(sequences[-1][same - 1] for same in same_index if same - 1 in range(self.front_size))
+        previous_same_index = self.calculate_same_number_index(sequences[-2], sequences[-1])
+        bankers.update(sequences[-1][same - 1] for same in previous_same_index if same - 1 in range(5))
         return bankers
 
     @staticmethod
     def calculate_back_bankers(sequences: List[List[int]], next_weekday: int) -> Set[int]:
         """Helper function to calculate back banker numbers based on the last sequence."""
         last_sequence = sequences[-1]
         b1, b2 = last_sequence
@@ -928,15 +1062,15 @@
         # If data length is equal to the back size, return an empty list.
         elif length == self.back_size:
             return []
 
         # If none of the above conditions are met, raise an IndexError.
         raise IndexError(f'length:{length} does not match any expected size')
 
-    def calculate_back(self, data: Iterable[int]) -> List[int]:
+    def calculate_back(self, data: Iterable[Any]) -> List[int]:
         """
         Calculate the 'back' portion of the data based on predefined size settings.
 
         :param data: The input data list whose 'back' part is to be calculated.
         :return: A list representing the 'back' portion of the data.
         :raises IndexError: If the length of data does not match any expected size.
         """
@@ -1167,136 +1301,152 @@
             self.Lottery('', '', '', self.calculate_front(d), self.calculate_back(d))
             for d in predictions
         ]
 
     def predict_by_last_period(
             self,
             next_period: int = None,
-            show_details: bool = False,
+            show_details: str = None,
             window_size: int = 15
     ) -> List[List[int]]:
         """
         Predicts features by the last period window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_period: int eg: 24001
-        :param show_details: boolean flag to output details about the prediction
+        :param show_details: ['en' | 'zh'] str flag to output details about the prediction, default is None
         :param window_size: int, default is 15
         """
         history_data = self.get_previous_history_data(next_period=next_period)
 
         maybe_combinations = self.predict_by_last_window_data(history_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
-        self.app_log.info(predict_data) if show_details is True else None
+        self.detail_log(app_log=self.app_log, show_details=show_details, en=predict_data, zh=predict_data)
 
         handle_result = self.handle_last_window_data(data=history_data, window=window_size)
-        self.app_log.info(handle_result) if show_details is True else None
+        self.detail_log(app_log=self.app_log, show_details=show_details, en=handle_result, zh=handle_result)
 
         return predict_data
 
     def predict_by_same_period(
             self,
             next_period: int = None,
-            show_details: bool = False,
+            show_details: str = None,
             window_size: int = 15
     ) -> List[List[int]]:
         """
         Predicts features by the last period window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_period: int eg: 24001
-        :param show_details: boolean flag to output details about the prediction
+        :param show_details: ['en' | 'zh'] str flag to output details about the prediction, default is None
         :param window_size: int, default is 15
         """
         period_data = self.get_previous_period_data(next_period=next_period)
 
         maybe_combinations = self.predict_by_last_window_data(period_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
-        self.app_log.info(predict_data) if show_details is True else None
+        self.detail_log(app_log=self.app_log, show_details=show_details, en=predict_data, zh=predict_data)
 
         handle_result = self.handle_last_window_data(data=period_data, window=window_size)
-        self.app_log.info(handle_result) if show_details is True else None
+        self.detail_log(app_log=self.app_log, show_details=show_details, en=handle_result, zh=handle_result)
 
         return predict_data
 
     def predict_by_last_weekday(
             self,
             next_weekday: int = None,
             next_period: int = None,
-            show_details: bool = False,
+            show_details: str = None,
             window_size: int = 15
     ) -> List[List[int]]:
         """
         Predicts features by the last weekday window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_weekday: int eg: [1 | 3 | 6]
         :param next_period: int eg: 24001
-        :param show_details: boolean flag to output details about the prediction
+        :param show_details: ['en' | 'zh'] flag to output details about the prediction, default is None
         :param window_size: int, default is 15
         """
         weekday_data = self.get_previous_weekday_data(next_weekday=next_weekday, next_period=next_period)
 
         maybe_combinations = self.predict_by_last_window_data(weekday_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
-        self.app_log.info(predict_data) if show_details is True else None
+        self.detail_log(app_log=self.app_log, show_details=show_details, en=predict_data, zh=predict_data)
 
         handle_result = self.handle_last_window_data(data=weekday_data, window=window_size)
-        self.app_log.info(handle_result) if show_details is True else None
+        self.detail_log(app_log=self.app_log, show_details=show_details, en=handle_result, zh=handle_result)
 
         return predict_data
 
     def model_predict(
             self,
             next_period: int = None,
             next_weekday: int = None,
-            show_details: bool = False,
+            show_details: str = None,
             window_size: int = 15
     ) -> List[List[int]]:
         """
         :param next_period: int eg: 24001
         :param next_weekday: int eg: [1 | 3 | 6]
-        :param show_details: boolean flag to output details about the prediction
+        :param show_details: ['en' | 'zh'] str flag to output details about the prediction, default is None
         :param window_size: int, the default is 15
         """
         predictions = []
         predictions.extend(self.predict_by_last_period(next_period=next_period,
                                                        show_details=show_details,
                                                        window_size=window_size))
         predictions.extend(self.predict_by_same_period(next_period=next_period,
                                                        show_details=show_details,
                                                        window_size=window_size))
         predictions.extend(self.predict_by_last_weekday(next_weekday=next_weekday,
                                                         next_period=next_period,
                                                         show_details=show_details,
                                                         window_size=window_size))
 
-        if show_details is True:
-            self.app_log.info("The following is a preliminary forecast of the data analysis : ")
+        if show_details:
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en="The following is a preliminary forecast of the data analysis : ",
+                            zh='以下是对数据分析的初步预测:')
             # Splitting the data into first 5 and last 2 numbers
             front_zone = [num for row in predictions for num in row[:5]]
             back_zone = [num for row in predictions for num in row[5:]]
 
             # Counting occurrences
             front_zone_frequency = Counter(front_zone)
             back_zone_frequency = Counter(back_zone)
 
             # Sorting the counts
             sorted_front_zone_frequency = sorted(front_zone_frequency.items(), key=lambda x: x[1], reverse=True)
             sorted_back_zone_frequency = sorted(back_zone_frequency.items(), key=lambda x: x[1], reverse=True)
 
             # Printing the results
-            self.app_log.info("Counts of the front zone numbers in each row sorted by frequency:")
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en="Counts of the front zone numbers in each row sorted by frequency:",
+                            zh='按频次排序的前区号计数:')
             for number, count in sorted_front_zone_frequency:
-                self.app_log.info(f"Number {number}: {count} times")
-            self.app_log.info(f"Total count of the front zone numbers in each row: {len(sorted_front_zone_frequency)}")
-
-            self.app_log.info("\nCounts of the back zone numbers in each row sorted by frequency:")
+                self.detail_log(app_log=self.app_log, show_details=show_details,
+                                en=f"Number {number}: {count} times",
+                                zh=f"数字 {number}: {count} 次")
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"Total count of the front zone numbers in each row: {len(sorted_front_zone_frequency)}",
+                            zh=f"前区号码总数: {len(sorted_front_zone_frequency)}")
+
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en="\nCounts of the back zone numbers in each row sorted by frequency:",
+                            zh="\n按频率排序的后区编号计数:")
             for number, count in sorted_back_zone_frequency:
-                self.app_log.info(f"Number {number}: {count} times")
-            self.app_log.info(f"Total count of the back zone numbers in each row: {len(sorted_back_zone_frequency)}")
-
-            self.app_log.info("\nHere are the preliminary predictions: ")
+                self.detail_log(app_log=self.app_log, show_details=show_details,
+                                en=f"Number {number}: {count} times",
+                                zh=f"数字 {number}: {count} 次")
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"Total count of the front zone numbers in each row: {len(sorted_back_zone_frequency)}",
+                            zh=f"后区号码总数: {len(sorted_back_zone_frequency)}")
+
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en="\nHere are the preliminary predictions: ",
+                            zh="\n以下是初步预测:")
             for data in predictions:
                 self.app_log.info(', '.join(map(str, data)))
         return predictions
 
     def calculate_predictions_and_intervals(
             self,
             data: List[Union[float, int]],
@@ -1357,137 +1507,181 @@
 
         return pred, min_val, max_val
 
     def analyze_predict(
             self,
             next_period: int = None,
             next_weekday: int = None,
-            show_details: bool = False,
+            show_details: str = None,
             window_size: int = 15
     ) -> List[List[int]]:
         """
         :param next_period: int eg: 24001
         :param next_weekday: int eg: [1 | 3 | 6]
-        :param show_details: boolean flag to output details about the prediction
+        :param show_details: ['en' | 'zh'] str flag to output details about the prediction, default is None
         :param window_size: int, the default is 15
         """
-        # use model predict combinations and handle number set
+        # use analyze predict combinations and handle number set
+        self.detail_log(app_log=self.app_log, show_details=show_details,
+                        en="Make initial predictions using model predictions",
+                        zh="使用模型预测进行初步预测")
         predict_data = self.model_predict(next_period=next_period, next_weekday=next_weekday,
-                                          show_details=False, window_size=window_size)
-        predict_front_set, predict_back_set = set(), set()
+                                          show_details=None, window_size=window_size)
         for data in predict_data:
-            predict_front_set.update(self.calculate_front(data))
-            predict_back_set.update(self.calculate_back(data))
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=', '.join(f'{num:>2}' for num in data),
+                            zh=', '.join(f'{num:>2}' for num in data))
+        predict_data_front = [self.calculate_front(data) for data in predict_data]
+        predict_front_set = {num for data in predict_data_front for num in data}
+        self.detail_log(app_log=self.app_log, show_details=show_details,
+                        en=f"model predict front: {sorted(predict_front_set)}, size: {len(predict_front_set)}",
+                        zh=f"模型预测前区数字: {sorted(predict_front_set)}, 数量: {len(predict_front_set)}")
+
+        predict_data_back = [self.calculate_back(data) for data in predict_data]
+        predict_back_set = {num for data in predict_data_back for num in data}
+        self.detail_log(app_log=self.app_log, show_details=show_details,
+                        en=f"model predict back: {sorted(predict_back_set)}, size: {len(predict_back_set)}",
+                        zh=f"模型预测后区数字: {sorted(predict_back_set)}, 数量: {len(predict_back_set)}")
+
         exclude_front_set = set(range(1, self.front_vocab_size + 1)).difference(predict_front_set)
+        self.detail_log(app_log=self.app_log, show_details=show_details,
+                        en=f"model predict exclude front: {sorted(exclude_front_set)}, size: {len(exclude_front_set)}",
+                        zh=f"模型预测前区排除数字: {sorted(exclude_front_set)}, 数量: {len(exclude_front_set)}")
+
         exclude_back_set = set(range(1, self.back_vocab_size + 1)).difference(predict_back_set)
+        self.detail_log(app_log=self.app_log, show_details=show_details,
+                        en=f"model predict exclude front: {sorted(exclude_back_set)}, size: {len(exclude_back_set)}",
+                        zh=f"模型预测后区排除数字: {sorted(exclude_back_set)}, 数量: {len(exclude_back_set)}")
 
-        # generate kill and banker numbers
+        # ready data
         history_data = self.get_previous_history_data(next_period=next_period)
-        period_data = self.get_previous_period_data(next_period=next_period)
-        weekday_data = self.get_previous_weekday_data(next_period=next_period, next_weekday=next_weekday)
-        front_kill_numbers, back_kill_numbers = self.get_kill_numbers(history_data, next_period=next_period,
-                                                                      next_weekday=next_weekday)
-        front_banker_numbers, back_banker_numbers = self.get_banker_numbers(history_data, next_period=next_period,
-                                                                            next_weekday=next_weekday)
+        period_data = [self.convert_lottery_data(d) for d in self.get_previous_period_data(next_period=next_period)]
+        weekday_data = [self.convert_lottery_data(d) for d in self.get_previous_weekday_data(next_period=next_period,
+                                                                                             next_weekday=next_weekday)]
+        data_map = {
+            'history': history_data,
+            'period': period_data,
+            'weekday': weekday_data
+        }
 
-        self.app_log.info("Now, Will analyze the predictions..., Then adjust data")
+        # generate kill numbers
+        front_kill_numbers, back_kill_numbers = set(), set()
+        for key, val in data_map.items():
+            # self.detail_log(app_log=self.app_log, show_details=show_details,
+            #                 en=f"analyze last {window_size} {key} get kill data:",
+            #                 zh=f"分析最近 {window_size} {key} 获得杀码数据:")
+            kill_numbers = self.get_kill_numbers(val[-window_size:], next_period=next_period,
+                                                 next_weekday=next_weekday, show_details=show_details)
+            front_kill_numbers.update(kill_numbers[0])
+            back_kill_numbers.update(kill_numbers[1])
+
+        # generate banker numbers
+        front_banker_numbers, back_banker_numbers = set(), set()
+        for key, val in data_map.items():
+            # self.detail_log(app_log=self.app_log, show_details=show_details,
+            #                 en=f"analyze last {window_size} {key} get banker data:",
+            #                 zh=f"分析最近 {window_size} {key} 获得胆码数据:")
+            banker_numbers = self.get_banker_numbers(val[-window_size:], next_period=next_period,
+                                                     next_weekday=next_weekday, show_details=show_details)
+            front_banker_numbers.update(banker_numbers[0])
+            back_banker_numbers.update(banker_numbers[1])
+
+        self.detail_log(app_log=self.app_log, show_details=show_details,
+                        en="Now, Will analyze the predictions..., Then adjust data",
+                        zh="现在，将会分析这些预测…，然后调整数据")
         # Calculate available numbers avoiding both kill and banker numbers for the front
-        available_front_numbers = set(range(1, self.front_vocab_size + 1)) - front_kill_numbers - front_banker_numbers
-        # Calculate intersection of kill and banker numbers for the back
-        available_back_numbers = back_kill_numbers & back_banker_numbers
-
-        # Convert sets to lists for sampling
-        available_front_numbers = list(available_front_numbers)
-        available_back_numbers = list(available_back_numbers)
-
         predictions = []
         random.seed(self.calculate_sum_total(self.calculate_front(history_data[-1])))
-        # Generate a prediction if there are enough numbers to sample from
-        if len(available_front_numbers) >= 5 and len(available_back_numbers) >= 2:
-            fd = sorted(available_front_numbers) if len(available_front_numbers) == 5 else sorted(
-                random.sample(list(available_front_numbers), 5))
-            bd = sorted(available_back_numbers) if len(available_back_numbers) == 2 else sorted(
-                random.sample(list(available_back_numbers), 2))
-            predictions.append(fd + bd)
-
-        # Generate prediction from kill numbers if there are enough
-        if len(front_kill_numbers) >= 5 and len(available_back_numbers) >= 2:
-            fd = sorted(front_kill_numbers) if len(front_kill_numbers) == 5 else sorted(
-                random.sample(list(front_kill_numbers), 5))
-            bd = sorted(available_back_numbers) if len(available_back_numbers) == 2 else sorted(
-                random.sample(list(available_back_numbers), 2))
-            predictions.append(fd + bd)
-
-        # Generate prediction from banker numbers if there are enough
-        if len(front_banker_numbers) >= 5 and len(available_back_numbers) >= 2:
-            fd = sorted(front_banker_numbers) if len(front_banker_numbers) == 5 else sorted(
-                random.sample(list(front_banker_numbers), 5))
-            bd = sorted(available_back_numbers) if len(available_back_numbers) == 2 else sorted(
-                random.sample(list(available_back_numbers), 2))
-            predictions.append(fd + bd)
 
         # Combine front and back combinations
-        if show_details is True:
-            self.app_log.info("The following is a preliminary forecast of the data analysis : ")
-            self.app_log.info(f"available front numbers: {available_front_numbers}")
-            self.app_log.info(f"available back numbers: {available_back_numbers}")
-            self.app_log.info(f"front kill numbers: {front_kill_numbers}")
-            self.app_log.info(f"back kill numbers: {back_kill_numbers}")
-            self.app_log.info(f"front banker numbers: {front_banker_numbers}")
-            self.app_log.info(f"back banker numbers: {back_banker_numbers}")
-
-            self.app_log.info(f"last combination: {history_data[-1]}")
-            self.app_log.info(f"model predict front: {sorted(predict_front_set)}")
-            self.app_log.info(f"model predict back: {sorted(predict_back_set)}")
-            self.app_log.info(f"exclude model predict front: {sorted(exclude_front_set)}")
-            self.app_log.info(f"exclude model predict back: {sorted(exclude_back_set)}")
+        if show_details:
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en="The following is a preliminary forecast of the data analysis : ",
+                            zh="以下是对数据分析的初步预测:")
+            # kill
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"front kill numbers: {front_kill_numbers}, size: {len(front_kill_numbers)}",
+                            zh=f"前区杀码: {front_kill_numbers}, 数量: {len(front_kill_numbers)}")
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"back kill numbers: {back_kill_numbers}, size: {len(back_kill_numbers)}",
+                            zh=f"后区杀码: {back_kill_numbers}, 数量: {len(back_kill_numbers)}")
+            # banker
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"front banker numbers: {front_banker_numbers}, size: {len(front_banker_numbers)}",
+                            zh=f"前区胆码: {front_banker_numbers}, 数量: {len(front_banker_numbers)}")
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"back banker numbers: {back_banker_numbers}, size: {len(back_banker_numbers)}",
+                            zh=f"后区胆码: {back_banker_numbers}, 数量: {len(back_banker_numbers)}")
+
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"last combination: {history_data[-1]}",
+                            zh=f"最近一期中奖数据: {history_data[-1]}")
 
             # Splitting the data into first 5 and last 2 numbers
             front_zone = [num for row in predictions for num in row[:5]]
             back_zone = [num for row in predictions for num in row[5:]]
 
             # Counting occurrences
             front_zone_frequency = Counter(front_zone)
             back_zone_frequency = Counter(back_zone)
 
             # Sorting the counts
             sorted_front_zone_frequency = sorted(front_zone_frequency.items(), key=lambda x: x[1], reverse=True)
             sorted_back_zone_frequency = sorted(back_zone_frequency.items(), key=lambda x: x[1], reverse=True)
 
             # Printing the results
-            self.app_log.info("Counts of the front zone numbers in each row sorted by frequency:")
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en="Counts of the front zone numbers in each row sorted by frequency:",
+                            zh='按频次排序的前区号计数:')
             for number, count in sorted_front_zone_frequency:
-                self.app_log.info(f"Number {number}: {count} times")
-            self.app_log.info(f"Total count of the front zone numbers in each row: {len(sorted_front_zone_frequency)}")
-
-            self.app_log.info("\nCounts of the back zone numbers in each row sorted by frequency:")
+                self.detail_log(app_log=self.app_log, show_details=show_details,
+                                en=f"Number {number}: {count} times",
+                                zh=f"数字 {number}: {count} 次")
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"Total count of the front zone numbers in each row: {len(sorted_front_zone_frequency)}",
+                            zh=f"前区号码总数: {len(sorted_front_zone_frequency)}")
+
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en="\nCounts of the back zone numbers in each row sorted by frequency:",
+                            zh="\n按频率排序的后区编号计数:")
             for number, count in sorted_back_zone_frequency:
-                self.app_log.info(f"Number {number}: {count} times")
-            self.app_log.info(f"Total count of the back zone numbers in each row: {len(sorted_back_zone_frequency)}")
-
-            self.app_log.info("\nHere are the preliminary predictions: ")
-            for data in predictions:
-                self.app_log.info(', '.join(map(str, data)))
-        return predictions
+                self.detail_log(app_log=self.app_log, show_details=show_details,
+                                en=f"Number {number}: {count} times",
+                                zh=f"数字 {number}: {count} 次")
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en=f"Total count of the front zone numbers in each row: {len(sorted_back_zone_frequency)}",
+                            zh=f"后区号码总数: {len(sorted_back_zone_frequency)}")
+
+            self.detail_log(app_log=self.app_log, show_details=show_details,
+                            en="\nHere are the preliminary predictions: ",
+                            zh="\n以下是初步预测:")
+
+            # for data in predictions:
+            #     self.app_log.info(', '.join(map(str, data)))
+            self.print_matrix([self.calculate_front(history_data[-1])] + [list(front_kill_numbers)] + predict_data_front,
+                              self.front_vocab_size)
+            self.print_matrix([self.calculate_back(history_data[-1])] + [list(back_kill_numbers)] + predict_data_back,
+                              self.back_vocab_size)
+        return []
 
     def predict(
             self,
             next_period: int = None,
             next_weekday: int = None,
-            show_details: bool = False,
+            show_details: str = None,
             window_size: int = 15,
             predict_type: str = 'model'
     ) -> List[List[int]]:
         """
         Generates predictions based on the specified prediction type.
 
         Parameters:
         next_period (int, optional): The next period to predict, defaults to None.
         next_weekday (int, optional): The next weekday to predict, defaults to None.
-        show_details (bool): Whether to show detailed predictions, defaults to False.
+        show_details (str): ['en' | 'zh'] Whether to show detailed predictions, defaults is None.
         window_size (int): The window size used for predictions, defaults to 15.
         predict_type (str): The type of prediction, can be 'model', 'analyze', or 'train', defaults to 'model'.
 
         Returns:
         List[List[int]]: A list of prediction results based on the prediction type.
 
         Raises:
```

### Comparing `lottokit-1.2/lottokit/util.py` & `lottokit-1.3/lottokit/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,5362 +9,5855 @@
 00000080: 7469 6c2e 7079 0a40 4461 7465 5469 6d65  til.py.@DateTime
 00000090: 3a20 3230 3233 2f38 2f32 3320 3233 3a31  : 2023/8/23 23:1
 000000a0: 330a 4053 6f66 7457 6172 653a 200a 2222  3.@SoftWare: .""
 000000b0: 220a 0a69 6d70 6f72 7420 7265 0a69 6d70  "..import re.imp
 000000c0: 6f72 7420 7379 730a 696d 706f 7274 2063  ort sys.import c
 000000d0: 7376 0a69 6d70 6f72 7420 6d61 7468 0a69  sv.import math.i
 000000e0: 6d70 6f72 7420 7469 6d65 0a69 6d70 6f72  mport time.impor
-000000f0: 7420 6a73 6f6e 0a69 6d70 6f72 7420 6461  t json.import da
-00000100: 7465 7469 6d65 0a69 6d70 6f72 7420 6c6f  tetime.import lo
-00000110: 6767 696e 670a 696d 706f 7274 206c 6f67  gging.import log
-00000120: 6769 6e67 2e68 616e 646c 6572 730a 6672  ging.handlers.fr
-00000130: 6f6d 2061 6263 2069 6d70 6f72 7420 4142  om abc import AB
-00000140: 432c 2061 6273 7472 6163 746d 6574 686f  C, abstractmetho
-00000150: 640a 6672 6f6d 2074 7970 696e 6720 696d  d.from typing im
-00000160: 706f 7274 2049 7465 7261 626c 652c 204c  port Iterable, L
-00000170: 6973 742c 2054 7570 6c65 2c20 416e 792c  ist, Tuple, Any,
-00000180: 204f 7074 696f 6e61 6c2c 2055 6e69 6f6e   Optional, Union
-00000190: 2c20 5365 742c 2044 6963 740a 696d 706f  , Set, Dict.impo
-000001a0: 7274 2072 616e 646f 6d0a 696d 706f 7274  rt random.import
-000001b0: 206e 756d 7079 2061 7320 6e70 0a69 6d70   numpy as np.imp
-000001c0: 6f72 7420 7061 6e64 6173 2061 7320 7064  ort pandas as pd
-000001d0: 0a66 726f 6d20 706d 6461 7269 6d61 2069  .from pmdarima i
-000001e0: 6d70 6f72 7420 6175 746f 5f61 7269 6d61  mport auto_arima
-000001f0: 0a66 726f 6d20 7365 6c65 6e69 756d 2069  .from selenium i
-00000200: 6d70 6f72 7420 7765 6264 7269 7665 720a  mport webdriver.
-00000210: 6672 6f6d 2073 6b6c 6561 726e 2e70 6970  from sklearn.pip
-00000220: 656c 696e 6520 696d 706f 7274 2050 6970  eline import Pip
-00000230: 656c 696e 650a 6672 6f6d 2073 6b6c 6561  eline.from sklea
-00000240: 726e 2e62 6173 6520 696d 706f 7274 2042  rn.base import B
-00000250: 6173 6545 7374 696d 6174 6f72 2c20 5472  aseEstimator, Tr
-00000260: 616e 7366 6f72 6d65 724d 6978 696e 0a66  ansformerMixin.f
-00000270: 726f 6d20 736b 6c65 6172 6e2e 7069 7065  rom sklearn.pipe
-00000280: 6c69 6e65 2069 6d70 6f72 7420 6d61 6b65  line import make
-00000290: 5f70 6970 656c 696e 650a 6672 6f6d 2073  _pipeline.from s
-000002a0: 6b6c 6561 726e 2e70 7265 7072 6f63 6573  klearn.preproces
-000002b0: 7369 6e67 2069 6d70 6f72 7420 5374 616e  sing import Stan
-000002c0: 6461 7264 5363 616c 6572 0a66 726f 6d20  dardScaler.from 
-000002d0: 736b 6c65 6172 6e2e 656e 7365 6d62 6c65  sklearn.ensemble
-000002e0: 2069 6d70 6f72 7420 5261 6e64 6f6d 466f   import RandomFo
-000002f0: 7265 7374 5265 6772 6573 736f 720a 6672  restRegressor.fr
-00000300: 6f6d 2073 6b6c 6561 726e 2e6c 696e 6561  om sklearn.linea
-00000310: 725f 6d6f 6465 6c20 696d 706f 7274 204c  r_model import L
-00000320: 696e 6561 7252 6567 7265 7373 696f 6e0a  inearRegression.
-00000330: 6672 6f6d 2073 6b6c 6561 726e 2e70 7265  from sklearn.pre
-00000340: 7072 6f63 6573 7369 6e67 2069 6d70 6f72  processing impor
-00000350: 7420 506f 6c79 6e6f 6d69 616c 4665 6174  t PolynomialFeat
-00000360: 7572 6573 0a66 726f 6d20 736b 6c65 6172  ures.from sklear
-00000370: 6e2e 6d6f 6465 6c5f 7365 6c65 6374 696f  n.model_selectio
-00000380: 6e20 696d 706f 7274 2052 616e 646f 6d69  n import Randomi
-00000390: 7a65 6453 6561 7263 6843 560a 6672 6f6d  zedSearchCV.from
-000003a0: 2073 656c 656e 6975 6d2e 7765 6264 7269   selenium.webdri
-000003b0: 7665 722e 636f 6d6d 6f6e 2e62 7920 696d  ver.common.by im
-000003c0: 706f 7274 2042 790a 6672 6f6d 2073 656c  port By.from sel
-000003d0: 656e 6975 6d2e 7765 6264 7269 7665 722e  enium.webdriver.
-000003e0: 7375 7070 6f72 742e 7569 2069 6d70 6f72  support.ui impor
-000003f0: 7420 5765 6244 7269 7665 7257 6169 740a  t WebDriverWait.
-00000400: 6672 6f6d 2073 656c 656e 6975 6d2e 7765  from selenium.we
-00000410: 6264 7269 7665 722e 7375 7070 6f72 7420  bdriver.support 
-00000420: 696d 706f 7274 2065 7870 6563 7465 645f  import expected_
-00000430: 636f 6e64 6974 696f 6e73 2061 7320 4543  conditions as EC
-00000440: 0a0a 0a63 6c61 7373 2049 4f55 7469 6c3a  ...class IOUtil:
-00000450: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00000460: 640a 2020 2020 6465 6620 6765 745f 6c6f  d.    def get_lo
-00000470: 6767 6572 280a 2020 2020 2020 2020 2020  gger(.          
-00000480: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
-00000490: 2020 206c 6f67 5f66 696c 653a 2073 7472     log_file: str
-000004a0: 203d 204e 6f6e 650a 2020 2020 2920 2d3e   = None.    ) ->
-000004b0: 206c 6f67 6769 6e67 2e4c 6f67 6765 723a   logging.Logger:
-000004c0: 0a20 2020 2020 2020 2023 2043 686f 6f73  .        # Choos
-000004d0: 6520 6120 756e 6971 7565 206c 6f67 6765  e a unique logge
-000004e0: 7220 6e61 6d65 2062 6173 6564 206f 6e20  r name based on 
-000004f0: 7468 6520 6c6f 675f 6669 6c65 2061 7267  the log_file arg
-00000500: 756d 656e 740a 2020 2020 2020 2020 6c6f  ument.        lo
-00000510: 6767 6572 5f6e 616d 6520 3d20 6c6f 675f  gger_name = log_
-00000520: 6669 6c65 2069 6620 6c6f 675f 6669 6c65  file if log_file
-00000530: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-00000540: 6520 2764 6566 6175 6c74 5f6c 6f67 6765  e 'default_logge
-00000550: 7227 0a20 2020 2020 2020 2023 2047 6574  r'.        # Get
-00000560: 2074 6865 206c 6f67 6765 7220 696e 7374   the logger inst
-00000570: 616e 6365 2062 7920 6e61 6d65 0a20 2020  ance by name.   
-00000580: 2020 2020 206c 6f67 6765 7220 3d20 6c6f       logger = lo
-00000590: 6767 696e 672e 6765 744c 6f67 6765 7228  gging.getLogger(
-000005a0: 6c6f 6767 6572 5f6e 616d 6529 0a0a 2020  logger_name)..  
-000005b0: 2020 2020 2020 2320 4368 6563 6b20 6966        # Check if
-000005c0: 2074 6865 206c 6f67 6765 7220 616c 7265   the logger alre
-000005d0: 6164 7920 6861 7320 6861 6e64 6c65 7273  ady has handlers
-000005e0: 2074 6f20 7072 6576 656e 7420 6164 6469   to prevent addi
-000005f0: 6e67 2074 6865 6d20 6167 6169 6e0a 2020  ng them again.  
-00000600: 2020 2020 2020 6966 206e 6f74 206c 6f67        if not log
-00000610: 6765 722e 6861 6e64 6c65 7273 3a0a 2020  ger.handlers:.  
-00000620: 2020 2020 2020 2020 2020 6966 206c 6f67            if log
-00000630: 5f66 696c 6520 6973 204e 6f6e 653a 0a20  _file is None:. 
-00000640: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00000650: 2043 6f6e 6669 6775 7261 7469 6f6e 2066   Configuration f
-00000660: 6f72 206c 6f67 6769 6e67 2074 6f20 7468  or logging to th
-00000670: 6520 7465 726d 696e 616c 0a20 2020 2020  e terminal.     
-00000680: 2020 2020 2020 2020 2020 2023 206c 6f67             # log
-00000690: 5f66 6f72 6d61 7420 3d20 2725 2861 7363  _format = '%(asc
-000006a0: 7469 6d65 2973 205b 2528 6c65 7665 6c6e  time)s [%(leveln
-000006b0: 616d 6529 735d 203c 2528 6c69 6e65 6e6f  ame)s] <%(lineno
-000006c0: 2964 3e20 2528 6675 6e63 4e61 6d65 2973  )d> %(funcName)s
-000006d0: 3a20 2528 6d65 7373 6167 6529 7327 0a20  : %(message)s'. 
-000006e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000006f0: 6f67 5f66 6f72 6d61 7420 3d20 2725 286d  og_format = '%(m
-00000700: 6573 7361 6765 2973 270a 2020 2020 2020  essage)s'.      
-00000710: 2020 2020 2020 2020 2020 6861 6e64 6c65            handle
-00000720: 7220 3d20 6c6f 6767 696e 672e 5374 7265  r = logging.Stre
-00000730: 616d 4861 6e64 6c65 7228 7379 732e 7374  amHandler(sys.st
-00000740: 646f 7574 290a 2020 2020 2020 2020 2020  dout).          
-00000750: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00000760: 2020 2020 2020 2020 2320 436f 6e66 6967          # Config
-00000770: 7572 6174 696f 6e20 666f 7220 6c6f 6767  uration for logg
-00000780: 696e 6720 746f 2061 2066 696c 6520 7769  ing to a file wi
-00000790: 7468 2072 6f74 6174 696f 6e20 6174 206d  th rotation at m
-000007a0: 6964 6e69 6768 740a 2020 2020 2020 2020  idnight.        
-000007b0: 2020 2020 2020 2020 6c6f 675f 666f 726d          log_form
-000007c0: 6174 203d 2028 2725 2861 7363 7469 6d65  at = ('%(asctime
-000007d0: 2973 205b 2528 6c65 7665 6c6e 616d 6529  )s [%(levelname)
-000007e0: 735d 2025 2870 726f 6365 7373 2964 2025  s] %(process)d %
-000007f0: 2874 6872 6561 6429 6420 270a 2020 2020  (thread)d '.    
-00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000810: 2020 2020 2020 2020 2020 2725 2866 696c            '%(fil
-00000820: 656e 616d 6529 7320 3c25 286c 696e 656e  ename)s <%(linen
-00000830: 6f29 643e 2025 2866 756e 634e 616d 6529  o)d> %(funcName)
-00000840: 733a 2025 286d 6573 7361 6765 2973 2729  s: %(message)s')
-00000850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000860: 2068 616e 646c 6572 203d 206c 6f67 6769   handler = loggi
-00000870: 6e67 2e68 616e 646c 6572 732e 5469 6d65  ng.handlers.Time
-00000880: 6452 6f74 6174 696e 6746 696c 6548 616e  dRotatingFileHan
-00000890: 646c 6572 286c 6f67 5f66 696c 652c 2077  dler(log_file, w
-000008a0: 6865 6e3d 276d 6964 6e69 6768 7427 2c20  hen='midnight', 
-000008b0: 6261 636b 7570 436f 756e 743d 3729 0a0a  backupCount=7)..
-000008c0: 2020 2020 2020 2020 2020 2020 2320 5365              # Se
-000008d0: 7420 7468 6520 666f 726d 6174 7465 7220  t the formatter 
-000008e0: 666f 7220 7468 6520 6861 6e64 6c65 720a  for the handler.
-000008f0: 2020 2020 2020 2020 2020 2020 666f 726d              form
-00000900: 6174 7465 7220 3d20 6c6f 6767 696e 672e  atter = logging.
-00000910: 466f 726d 6174 7465 7228 6c6f 675f 666f  Formatter(log_fo
-00000920: 726d 6174 290a 2020 2020 2020 2020 2020  rmat).          
-00000930: 2020 6861 6e64 6c65 722e 7365 7446 6f72    handler.setFor
-00000940: 6d61 7474 6572 2866 6f72 6d61 7474 6572  matter(formatter
-00000950: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00000960: 204f 7074 696f 6e61 6c6c 7920 7365 7420   Optionally set 
-00000970: 6120 6469 6666 6572 656e 7420 6c6f 6720  a different log 
-00000980: 6c65 7665 6c20 666f 7220 7468 6520 6861  level for the ha
-00000990: 6e64 6c65 720a 2020 2020 2020 2020 2020  ndler.          
-000009a0: 2020 6861 6e64 6c65 722e 7365 744c 6576    handler.setLev
-000009b0: 656c 286c 6f67 6769 6e67 2e49 4e46 4f29  el(logging.INFO)
-000009c0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000009d0: 4164 6420 7468 6520 6861 6e64 6c65 7220  Add the handler 
-000009e0: 746f 2074 6865 206c 6f67 6765 720a 2020  to the logger.  
-000009f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00000a00: 2e61 6464 4861 6e64 6c65 7228 6861 6e64  .addHandler(hand
-00000a10: 6c65 7229 0a20 2020 2020 2020 2020 2020  ler).           
-00000a20: 2023 2053 6574 2074 6865 206c 6f67 206c   # Set the log l
-00000a30: 6576 656c 2066 6f72 2074 6865 206c 6f67  evel for the log
-00000a40: 6765 720a 2020 2020 2020 2020 2020 2020  ger.            
-00000a50: 6c6f 6767 6572 2e73 6574 4c65 7665 6c28  logger.setLevel(
-00000a60: 6c6f 6767 696e 672e 494e 464f 290a 0a20  logging.INFO).. 
-00000a70: 2020 2020 2020 2023 2052 6574 7572 6e20         # Return 
-00000a80: 7468 6520 636f 6e66 6967 7572 6564 206c  the configured l
-00000a90: 6f67 6765 720a 2020 2020 2020 2020 7265  ogger.        re
-00000aa0: 7475 726e 206c 6f67 6765 720a 0a20 2020  turn logger..   
-00000ab0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00000ac0: 2020 6465 6620 6c69 7374 5f74 6f5f 696e    def list_to_in
-00000ad0: 7428 0a20 2020 2020 2020 2020 2020 2063  t(.            c
-00000ae0: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-00000af0: 6e75 6d62 6572 733a 204c 6973 745b 696e  numbers: List[in
-00000b00: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
-00000b10: 7a65 726f 5f72 6570 6c61 6365 6d65 6e74  zero_replacement
-00000b20: 3a20 7374 7220 3d20 2727 2c0a 2020 2020  : str = '',.    
-00000b30: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00000b40: 3a20 416e 790a 2020 2020 2920 2d3e 2069  : Any.    ) -> i
-00000b50: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-00000b60: 2020 2020 2020 2020 436f 6e76 6572 7420          Convert 
-00000b70: 6120 6c69 7374 206f 6620 696e 7465 6765  a list of intege
-00000b80: 7273 2074 6f20 6120 7369 6e67 6c65 2069  rs to a single i
-00000b90: 6e74 6567 6572 2c20 7769 7468 2061 6e20  nteger, with an 
-00000ba0: 6f70 7469 6f6e 616c 2072 6570 6c61 6365  optional replace
-00000bb0: 6d65 6e74 2066 6f72 207a 6572 6f73 2e0a  ment for zeros..
-00000bc0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000bd0: 6e75 6d62 6572 733a 206c 6973 7420 6f66  numbers: list of
-00000be0: 2069 6e74 6567 6572 730a 2020 2020 2020   integers.      
-00000bf0: 2020 3a70 6172 616d 207a 6572 6f5f 7265    :param zero_re
-00000c00: 706c 6163 656d 656e 743a 2073 7472 696e  placement: strin
-00000c10: 6720 746f 2072 6570 6c61 6365 207a 6572  g to replace zer
-00000c20: 6f73 2077 6974 682c 2064 6566 6175 6c74  os with, default
-00000c30: 7320 746f 2061 6e20 656d 7074 7920 7374  s to an empty st
-00000c40: 7269 6e67 0a20 2020 2020 2020 203a 7265  ring.        :re
-00000c50: 7475 726e 3a20 7369 6e67 6c65 2069 6e74  turn: single int
-00000c60: 6567 6572 2066 6f72 6d65 6420 6279 2063  eger formed by c
-00000c70: 6f6e 6361 7465 6e61 7469 6e67 2074 6865  oncatenating the
-00000c80: 206c 6973 7420 656c 656d 656e 7473 0a20   list elements. 
-00000c90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00000ca0: 2020 2023 2056 616c 6964 6174 6520 696e     # Validate in
-00000cb0: 7075 7420 6461 7461 2069 7320 6120 6c69  put data is a li
-00000cc0: 7374 0a20 2020 2020 2020 2069 6620 6e6f  st.        if no
-00000cd0: 7420 6973 696e 7374 616e 6365 286e 756d  t isinstance(num
-00000ce0: 6265 7273 2c20 4c69 7374 293a 0a20 2020  bers, List):.   
-00000cf0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00000d00: 616c 7565 4572 726f 7228 2249 6e70 7574  alueError("Input
-00000d10: 2027 6e75 6d62 6572 7327 206d 7573 7420   'numbers' must 
-00000d20: 6265 2061 206c 6973 742e 2229 0a0a 2020  be a list.")..  
-00000d30: 2020 2020 2020 2320 5661 6c69 6461 7465        # Validate
-00000d40: 2061 6c6c 2065 6c65 6d65 6e74 7320 696e   all elements in
-00000d50: 2074 6865 206c 6973 7420 6172 6520 696e   the list are in
-00000d60: 7465 6765 7273 0a20 2020 2020 2020 2069  tegers.        i
-00000d70: 6620 6e6f 7420 616c 6c28 6973 696e 7374  f not all(isinst
-00000d80: 616e 6365 2878 2c20 696e 7429 2066 6f72  ance(x, int) for
-00000d90: 2078 2069 6e20 6e75 6d62 6572 7329 3a0a   x in numbers):.
-00000da0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00000db0: 6520 5661 6c75 6545 7272 6f72 2822 416c  e ValueError("Al
-00000dc0: 6c20 656c 656d 656e 7473 2069 6e20 7468  l elements in th
-00000dd0: 6520 276e 756d 6265 7273 2720 6c69 7374  e 'numbers' list
-00000de0: 206d 7573 7420 6265 2069 6e74 6567 6572   must be integer
-00000df0: 732e 2229 0a0a 2020 2020 2020 2020 2320  s.")..        # 
-00000e00: 436f 6e76 6572 7420 6c69 7374 2065 6c65  Convert list ele
-00000e10: 6d65 6e74 7320 746f 2073 7472 696e 6773  ments to strings
-00000e20: 2c20 7265 706c 6163 696e 6720 7a65 726f  , replacing zero
-00000e30: 7320 7769 7468 207a 6572 6f5f 7265 706c  s with zero_repl
-00000e40: 6163 656d 656e 740a 2020 2020 2020 2020  acement.        
-00000e50: 7061 7274 7320 3d20 5b7a 6572 6f5f 7265  parts = [zero_re
-00000e60: 706c 6163 656d 656e 7420 6966 2078 203d  placement if x =
-00000e70: 3d20 3020 656c 7365 2073 7472 2878 2920  = 0 else str(x) 
-00000e80: 666f 7220 7820 696e 206e 756d 6265 7273  for x in numbers
-00000e90: 5d0a 0a20 2020 2020 2020 2023 204a 6f69  ]..        # Joi
-00000ea0: 6e20 7468 6520 7061 7274 7320 616e 6420  n the parts and 
-00000eb0: 636f 6e76 6572 7420 746f 2061 6e20 696e  convert to an in
-00000ec0: 7465 6765 720a 2020 2020 2020 2020 7265  teger.        re
-00000ed0: 7475 726e 2069 6e74 2827 272e 6a6f 696e  turn int(''.join
-00000ee0: 2870 6172 7473 2929 0a0a 2020 2020 4063  (parts))..    @c
-00000ef0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00000f00: 6566 2069 6e74 5f74 6f5f 6c69 7374 280a  ef int_to_list(.
-00000f10: 2020 2020 2020 2020 2020 2020 636c 732c              cls,
-00000f20: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-00000f30: 6265 723a 2069 6e74 2c0a 2020 2020 2020  ber: int,.      
-00000f40: 2020 2020 2020 6d6f 6475 6c75 733a 2069        modulus: i
-00000f50: 6e74 203d 2031 302c 0a20 2020 2020 2020  nt = 10,.       
-00000f60: 2020 2020 202a 2a6b 7761 7267 733a 2041       **kwargs: A
-00000f70: 6e79 0a20 2020 2029 202d 3e20 4c69 7374  ny.    ) -> List
-00000f80: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
-00000f90: 2222 0a20 2020 2020 2020 2043 6f6e 7665  "".        Conve
-00000fa0: 7274 2061 6e20 696e 7465 6765 7220 746f  rt an integer to
-00000fb0: 2061 206c 6973 7420 6f66 2064 6967 6974   a list of digit
-00000fc0: 732c 2065 6163 6820 6469 6769 7420 6973  s, each digit is
-00000fd0: 2074 6865 2072 656d 6169 6e64 6572 206f   the remainder o
-00000fe0: 6620 6469 7669 7369 6f6e 2062 7920 6120  f division by a 
-00000ff0: 6d6f 6475 6c75 732e 0a0a 2020 2020 2020  modulus...      
-00001000: 2020 3a70 6172 616d 206e 756d 6265 723a    :param number:
-00001010: 2054 6865 2069 6e74 6567 6572 2074 6f20   The integer to 
-00001020: 6265 2063 6f6e 7665 7274 6564 2069 6e74  be converted int
-00001030: 6f20 6120 6c69 7374 206f 6620 6469 6769  o a list of digi
-00001040: 7473 2e0a 2020 2020 2020 2020 3a70 6172  ts..        :par
-00001050: 616d 206d 6f64 756c 7573 3a20 5468 6520  am modulus: The 
-00001060: 6469 7669 736f 7220 7573 6564 2066 6f72  divisor used for
-00001070: 2074 6865 206d 6f64 756c 6f20 6f70 6572   the modulo oper
-00001080: 6174 696f 6e20 6f6e 2065 6163 6820 6469  ation on each di
-00001090: 6769 742c 2064 6566 6175 6c74 7320 746f  git, defaults to
-000010a0: 2031 302e 0a20 2020 2020 2020 203a 7265   10..        :re
-000010b0: 7475 726e 3a20 4120 6c69 7374 206f 6620  turn: A list of 
-000010c0: 696e 7465 6765 7273 2c20 7768 6572 6520  integers, where 
-000010d0: 6561 6368 2069 6e74 6567 6572 2069 7320  each integer is 
-000010e0: 6120 6469 6769 7420 6f66 2074 6865 206f  a digit of the o
-000010f0: 7269 6769 6e61 6c20 6e75 6d62 6572 2061  riginal number a
-00001100: 6674 6572 2074 6865 206d 6f64 756c 6f20  fter the modulo 
-00001110: 6f70 6572 6174 696f 6e2e 0a20 2020 2020  operation..     
-00001120: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00001130: 2056 616c 6964 6174 6520 696e 7075 7420   Validate input 
-00001140: 6461 7461 2069 7320 616e 2069 6e74 6567  data is an integ
-00001150: 6572 0a20 2020 2020 2020 2069 6620 6e6f  er.        if no
-00001160: 7420 6973 696e 7374 616e 6365 286e 756d  t isinstance(num
-00001170: 6265 722c 2069 6e74 293a 0a20 2020 2020  ber, int):.     
-00001180: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00001190: 7565 4572 726f 7228 2249 6e70 7574 2027  ueError("Input '
-000011a0: 6e75 6d62 6572 2720 6d75 7374 2062 6520  number' must be 
-000011b0: 616e 2069 6e74 6567 6572 2e22 290a 0a20  an integer.").. 
-000011c0: 2020 2020 2020 2023 2056 616c 6964 6174         # Validat
-000011d0: 6520 6d6f 6475 6c75 7320 6973 2061 2070  e modulus is a p
-000011e0: 6f73 6974 6976 6520 696e 7465 6765 720a  ositive integer.
-000011f0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00001200: 7369 6e73 7461 6e63 6528 6d6f 6475 6c75  sinstance(modulu
-00001210: 732c 2069 6e74 2920 6f72 206d 6f64 756c  s, int) or modul
-00001220: 7573 203c 3d20 303a 0a20 2020 2020 2020  us <= 0:.       
-00001230: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00001240: 4572 726f 7228 2249 6e70 7574 2027 6d6f  Error("Input 'mo
-00001250: 6475 6c75 7327 206d 7573 7420 6265 2061  dulus' must be a
-00001260: 2070 6f73 6974 6976 6520 696e 7465 6765   positive intege
-00001270: 722e 2229 0a0a 2020 2020 2020 2020 2320  r.")..        # 
-00001280: 436f 6e76 6572 7420 7468 6520 696e 7465  Convert the inte
-00001290: 6765 7220 746f 2061 206c 6973 7420 6f66  ger to a list of
-000012a0: 2064 6967 6974 7320 7573 696e 6720 7468   digits using th
-000012b0: 6520 6d6f 6475 6c75 730a 2020 2020 2020  e modulus.      
-000012c0: 2020 6469 6769 745f 6c69 7374 203d 205b    digit_list = [
-000012d0: 696e 7428 6429 2025 206d 6f64 756c 7573  int(d) % modulus
-000012e0: 2066 6f72 2064 2069 6e20 7374 7228 6162   for d in str(ab
-000012f0: 7328 6e75 6d62 6572 2929 5d0a 0a20 2020  s(number))]..   
-00001300: 2020 2020 2023 2052 6574 7572 6e20 7468       # Return th
-00001310: 6520 6c69 7374 206f 6620 6469 6769 7473  e list of digits
-00001320: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001330: 6469 6769 745f 6c69 7374 0a0a 2020 2020  digit_list..    
-00001340: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00001350: 2064 6566 2077 7269 7465 5f64 6174 615f   def write_data_
-00001360: 746f 5f66 696c 6528 0a20 2020 2020 2020  to_file(.       
-00001370: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
-00001380: 2020 2020 2020 6669 6c65 5f70 6174 683a        file_path:
-00001390: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-000013a0: 2020 6461 7461 3a20 4c69 7374 5b73 7472    data: List[str
-000013b0: 5d2c 0a20 2020 2020 2020 2020 2020 2061  ],.            a
-000013c0: 7070 5f6c 6f67 3a20 4f70 7469 6f6e 616c  pp_log: Optional
-000013d0: 5b6c 6f67 6769 6e67 2e4c 6f67 6765 725d  [logging.Logger]
-000013e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000013f0: 2020 2020 206d 6f64 653a 2073 7472 203d       mode: str =
-00001400: 2027 612b 272c 0a20 2020 2020 2020 2020   'a+',.         
-00001410: 2020 202a 2a6b 7761 7267 733a 2041 6e79     **kwargs: Any
-00001420: 0a20 2020 2029 202d 3e20 626f 6f6c 3a0a  .    ) -> bool:.
-00001430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00001440: 2020 2020 5772 6974 6520 6461 7461 2074      Write data t
-00001450: 6f20 6120 6669 6c65 2e0a 0a20 2020 2020  o a file...     
-00001460: 2020 203a 7061 7261 6d20 6669 6c65 5f70     :param file_p
-00001470: 6174 683a 2050 6174 6820 746f 2074 6865  ath: Path to the
-00001480: 2066 696c 6520 7768 6572 6520 6461 7461   file where data
-00001490: 2077 696c 6c20 6265 2077 7269 7474 656e   will be written
-000014a0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000014b0: 2064 6174 613a 204c 6973 7420 6f66 2064   data: List of d
-000014c0: 6174 6120 746f 2077 7269 7465 2074 6f20  ata to write to 
-000014d0: 7468 6520 6669 6c65 2e0a 2020 2020 2020  the file..      
-000014e0: 2020 3a70 6172 616d 2061 7070 5f6c 6f67    :param app_log
-000014f0: 3a20 4f70 7469 6f6e 616c 206c 6f67 6765  : Optional logge
-00001500: 7220 666f 7220 6c6f 6767 696e 6720 696e  r for logging in
-00001510: 666f 726d 6174 696f 6e2c 2064 6566 6175  formation, defau
-00001520: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
-00001530: 2020 2020 203a 7061 7261 6d20 6d6f 6465       :param mode
-00001540: 3a20 4d6f 6465 2069 6e20 7768 6963 6820  : Mode in which 
-00001550: 7468 6520 6669 6c65 2073 686f 756c 6420  the file should 
-00001560: 6265 206f 7065 6e65 642c 2064 6566 6175  be opened, defau
-00001570: 6c74 7320 746f 2027 612b 2720 666f 7220  lts to 'a+' for 
-00001580: 6170 7065 6e64 2e0a 2020 2020 2020 2020  append..        
-00001590: 3a72 6574 7572 6e3a 2062 6f6f 6c20 7765  :return: bool we
-000015a0: 6174 6865 7220 7375 6363 6573 7320 6f72  ather success or
-000015b0: 2066 6169 6c65 640a 2020 2020 2020 2020   failed.        
-000015c0: 2222 220a 2020 2020 2020 2020 6966 2061  """.        if a
-000015d0: 7070 5f6c 6f67 2069 7320 4e6f 6e65 3a0a  pp_log is None:.
-000015e0: 2020 2020 2020 2020 2020 2020 6170 705f              app_
-000015f0: 6c6f 6720 3d20 636c 732e 6765 745f 6c6f  log = cls.get_lo
-00001600: 6767 6572 2829 0a0a 2020 2020 2020 2020  gger()..        
-00001610: 6966 206e 6f74 2064 6174 613a 0a20 2020  if not data:.   
-00001620: 2020 2020 2020 2020 2061 7070 5f6c 6f67           app_log
-00001630: 2e77 6172 6e69 6e67 2822 4e6f 2064 6174  .warning("No dat
-00001640: 6120 7072 6f76 6964 6564 2074 6f20 7772  a provided to wr
-00001650: 6974 6520 746f 2074 6865 2066 696c 652e  ite to the file.
-00001660: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-00001670: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-00001680: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00001690: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-000016a0: 6669 6c65 5f70 6174 682c 206d 6f64 6529  file_path, mode)
-000016b0: 2061 7320 6670 3a0a 2020 2020 2020 2020   as fp:.        
-000016c0: 2020 2020 2020 2020 6170 705f 6c6f 672e          app_log.
-000016d0: 696e 666f 2866 2757 7269 7469 6e67 2074  info(f'Writing t
-000016e0: 6f20 6669 6c65 3a20 7b66 702e 6e61 6d65  o file: {fp.name
-000016f0: 7d27 290a 2020 2020 2020 2020 2020 2020  }').            
-00001700: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-00001710: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-00001720: 2020 2020 2020 2020 2020 6966 206c 696e            if lin
-00001730: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001750: 2020 2020 2020 2066 702e 7772 6974 6528         fp.write(
-00001760: 6627 7b6c 696e 657d 5c6e 2729 0a20 2020  f'{line}\n').   
-00001770: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00001780: 7074 696f 6e20 6173 2065 783a 0a20 2020  ption as ex:.   
-00001790: 2020 2020 2020 2020 2061 7070 5f6c 6f67           app_log
-000017a0: 2e65 7863 6570 7469 6f6e 2866 2241 6e20  .exception(f"An 
-000017b0: 6572 726f 7220 6f63 6375 7272 6564 2077  error occurred w
-000017c0: 6869 6c65 2077 7269 7469 6e67 2074 6f20  hile writing to 
-000017d0: 7468 6520 6669 6c65 3a20 7b65 787d 2229  the file: {ex}")
-000017e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000017f0: 7572 6e20 4661 6c73 650a 0a20 2020 2020  urn False..     
-00001800: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00001810: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00001820: 0a20 2020 2064 6566 2072 6561 645f 6461  .    def read_da
-00001830: 7461 5f66 726f 6d5f 6669 6c65 280a 2020  ta_from_file(.  
-00001840: 2020 2020 2020 2020 2020 636c 732c 0a20            cls,. 
-00001850: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-00001860: 7061 7468 3a20 7374 722c 0a20 2020 2020  path: str,.     
-00001870: 2020 2020 2020 2061 7070 5f6c 6f67 3a20         app_log: 
-00001880: 4f70 7469 6f6e 616c 5b6c 6f67 6769 6e67  Optional[logging
-00001890: 2e4c 6f67 6765 725d 203d 204e 6f6e 652c  .Logger] = None,
-000018a0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-000018b0: 653a 2073 7472 203d 2027 7227 0a20 2020  e: str = 'r'.   
-000018c0: 2029 202d 3e20 4f70 7469 6f6e 616c 5b4c   ) -> Optional[L
-000018d0: 6973 745b 7374 725d 5d3a 0a20 2020 2020  ist[str]]:.     
-000018e0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-000018f0: 6561 6420 6461 7461 2066 726f 6d20 6120  ead data from a 
-00001900: 6669 6c65 2061 6e64 2072 6574 7572 6e20  file and return 
-00001910: 6120 6c69 7374 206f 6620 6e6f 6e2d 656d  a list of non-em
-00001920: 7074 7920 6c69 6e65 732e 0a0a 2020 2020  pty lines...    
-00001930: 2020 2020 3a70 6172 616d 2066 696c 655f      :param file_
-00001940: 7061 7468 3a20 5061 7468 2074 6f20 7468  path: Path to th
-00001950: 6520 6669 6c65 2074 6f20 6265 2072 6561  e file to be rea
-00001960: 642e 0a20 2020 2020 2020 203a 7061 7261  d..        :para
-00001970: 6d20 6170 705f 6c6f 673a 204f 7074 696f  m app_log: Optio
-00001980: 6e61 6c20 6c6f 6767 6572 2066 6f72 206c  nal logger for l
-00001990: 6f67 6769 6e67 2069 6e66 6f72 6d61 7469  ogging informati
-000019a0: 6f6e 2c20 6465 6661 756c 7473 2074 6f20  on, defaults to 
-000019b0: 4e6f 6e65 2e0a 2020 2020 2020 2020 3a70  None..        :p
-000019c0: 6172 616d 206d 6f64 653a 204d 6f64 6520  aram mode: Mode 
-000019d0: 696e 2077 6869 6368 2074 6865 2066 696c  in which the fil
-000019e0: 6520 7368 6f75 6c64 2062 6520 6f70 656e  e should be open
-000019f0: 6564 2c20 6465 6661 756c 7473 2074 6f20  ed, defaults to 
-00001a00: 2772 2720 666f 7220 7265 6164 206f 6e6c  'r' for read onl
-00001a10: 792e 0a20 2020 2020 2020 203a 7265 7475  y..        :retu
-00001a20: 726e 3a20 4c69 7374 206f 6620 6e6f 6e2d  rn: List of non-
-00001a30: 656d 7074 7920 6c69 6e65 7320 6672 6f6d  empty lines from
-00001a40: 2074 6865 2066 696c 6520 6f72 204e 6f6e   the file or Non
-00001a50: 6520 6966 2061 6e20 6578 6365 7074 696f  e if an exceptio
-00001a60: 6e20 6f63 6375 7273 2e0a 2020 2020 2020  n occurs..      
-00001a70: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00001a80: 2061 7070 5f6c 6f67 2069 7320 4e6f 6e65   app_log is None
-00001a90: 3a0a 2020 2020 2020 2020 2020 2020 6170  :.            ap
-00001aa0: 705f 6c6f 6720 3d20 636c 732e 6765 745f  p_log = cls.get_
-00001ab0: 6c6f 6767 6572 2829 0a0a 2020 2020 2020  logger()..      
-00001ac0: 2020 6461 7461 203d 205b 5d0a 2020 2020    data = [].    
-00001ad0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00001ae0: 2020 2020 2077 6974 6820 6f70 656e 2866       with open(f
-00001af0: 696c 655f 7061 7468 2c20 6d6f 6465 2920  ile_path, mode) 
-00001b00: 6173 2066 703a 0a20 2020 2020 2020 2020  as fp:.         
-00001b10: 2020 2020 2020 2061 7070 5f6c 6f67 2e69         app_log.i
-00001b20: 6e66 6f28 6627 4f70 656e 696e 6720 6669  nfo(f'Opening fi
-00001b30: 6c65 3a20 7b66 702e 6e61 6d65 7d27 290a  le: {fp.name}').
-00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 6461 7461 203d 205b 6c69 6e65 2e73 7472  data = [line.str
-00001b60: 6970 2829 2066 6f72 206c 696e 6520 696e  ip() for line in
-00001b70: 2066 7020 6966 206c 696e 652e 7374 7269   fp if line.stri
-00001b80: 7028 295d 0a20 2020 2020 2020 2065 7863  p()].        exc
-00001b90: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00001ba0: 2065 783a 0a20 2020 2020 2020 2020 2020   ex:.           
-00001bb0: 2061 7070 5f6c 6f67 2e65 7863 6570 7469   app_log.excepti
-00001bc0: 6f6e 2866 2241 6e20 6572 726f 7220 6f63  on(f"An error oc
-00001bd0: 6375 7272 6564 2077 6869 6c65 2072 6561  curred while rea
-00001be0: 6469 6e67 2074 6865 2066 696c 653a 207b  ding the file: {
-00001bf0: 6578 7d22 290a 2020 2020 2020 2020 2020  ex}").          
-00001c00: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-00001c10: 2020 2020 2020 2061 7070 5f6c 6f67 2e69         app_log.i
-00001c20: 6e66 6f28 6627 4e75 6d62 6572 206f 6620  nfo(f'Number of 
-00001c30: 6e6f 6e2d 656d 7074 7920 6c69 6e65 7320  non-empty lines 
-00001c40: 7265 6164 3a20 7b6c 656e 2864 6174 6129  read: {len(data)
-00001c50: 7d27 290a 2020 2020 2020 2020 7265 7475  }').        retu
-00001c60: 726e 2064 6174 610a 0a20 2020 2040 636c  rn data..    @cl
-00001c70: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00001c80: 6620 7772 6974 655f 6373 765f 6461 7461  f write_csv_data
-00001c90: 5f74 6f5f 6669 6c65 280a 2020 2020 2020  _to_file(.      
-00001ca0: 2020 2020 2020 636c 732c 0a20 2020 2020        cls,.     
-00001cb0: 2020 2020 2020 2066 696c 655f 7061 7468         file_path
-00001cc0: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
-00001cd0: 2020 2064 6174 613a 204c 6973 745b 4c69     data: List[Li
-00001ce0: 7374 5b41 6e79 5d5d 2c0a 2020 2020 2020  st[Any]],.      
-00001cf0: 2020 2020 2020 6170 705f 6c6f 673a 204f        app_log: O
-00001d00: 7074 696f 6e61 6c5b 6c6f 6767 696e 672e  ptional[logging.
-00001d10: 4c6f 6767 6572 5d20 3d20 4e6f 6e65 2c0a  Logger] = None,.
-00001d20: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00001d30: 3a20 7374 7220 3d20 2761 2b27 2c0a 2020  : str = 'a+',.  
-00001d40: 2020 2020 2020 2020 2020 6e65 776c 696e            newlin
-00001d50: 653a 2073 7472 203d 2027 272c 0a20 2020  e: str = '',.   
-00001d60: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-00001d70: 733a 2041 6e79 0a20 2020 2029 202d 3e20  s: Any.    ) -> 
-00001d80: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00001d90: 220a 2020 2020 2020 2020 5772 6974 6520  ".        Write 
-00001da0: 6461 7461 2074 6f20 6120 4353 5620 6669  data to a CSV fi
-00001db0: 6c65 2e0a 0a20 2020 2020 2020 203a 7061  le...        :pa
-00001dc0: 7261 6d20 6669 6c65 5f70 6174 683a 2050  ram file_path: P
-00001dd0: 6174 6820 746f 2074 6865 2066 696c 6520  ath to the file 
-00001de0: 7768 6572 6520 4353 5620 6461 7461 2077  where CSV data w
-00001df0: 696c 6c20 6265 2077 7269 7474 656e 2e0a  ill be written..
-00001e00: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00001e10: 6174 613a 204c 6973 7420 6f66 2072 6f77  ata: List of row
-00001e20: 7320 2877 6865 7265 2065 6163 6820 726f  s (where each ro
-00001e30: 7720 6973 2061 206c 6973 7429 2074 6f20  w is a list) to 
-00001e40: 7772 6974 6520 746f 2074 6865 2043 5356  write to the CSV
-00001e50: 2066 696c 652e 0a20 2020 2020 2020 203a   file..        :
-00001e60: 7061 7261 6d20 6170 705f 6c6f 673a 204f  param app_log: O
-00001e70: 7074 696f 6e61 6c20 6c6f 6767 6572 2066  ptional logger f
-00001e80: 6f72 206c 6f67 6769 6e67 2069 6e66 6f72  or logging infor
-00001e90: 6d61 7469 6f6e 2c20 6465 6661 756c 7473  mation, defaults
-00001ea0: 2074 6f20 4e6f 6e65 2077 6869 6368 2077   to None which w
-00001eb0: 696c 6c20 6372 6561 7465 2061 206e 6577  ill create a new
-00001ec0: 206c 6f67 6765 722e 0a20 2020 2020 2020   logger..       
-00001ed0: 203a 7061 7261 6d20 6d6f 6465 3a20 4d6f   :param mode: Mo
-00001ee0: 6465 2069 6e20 7768 6963 6820 7468 6520  de in which the 
-00001ef0: 6669 6c65 2073 686f 756c 6420 6265 206f  file should be o
-00001f00: 7065 6e65 642c 2064 6566 6175 6c74 7320  pened, defaults 
-00001f10: 746f 2027 612b 2720 666f 7220 6170 7065  to 'a+' for appe
-00001f20: 6e64 2e0a 2020 2020 2020 2020 3a70 6172  nd..        :par
-00001f30: 616d 206e 6577 6c69 6e65 3a20 436f 6e74  am newline: Cont
-00001f40: 726f 6c73 2068 6f77 2075 6e69 7665 7273  rols how univers
-00001f50: 616c 206e 6577 6c69 6e65 7320 776f 726b  al newlines work
-00001f60: 7320 2869 7420 6f6e 6c79 2061 7070 6c69  s (it only appli
-00001f70: 6573 2074 6f20 7465 7874 206d 6f64 6529  es to text mode)
-00001f80: 2e20 4974 2064 6566 6175 6c74 7320 746f  . It defaults to
-00001f90: 2027 272e 0a20 2020 2020 2020 203a 7265   ''..        :re
-00001fa0: 7475 726e 3a20 626f 6f6c 2077 6561 7468  turn: bool weath
-00001fb0: 6572 2073 7563 6365 7373 206f 7220 6661  er success or fa
-00001fc0: 696c 6564 0a20 2020 2020 2020 2022 2222  iled.        """
-00001fd0: 0a20 2020 2020 2020 2069 6620 6170 705f  .        if app_
-00001fe0: 6c6f 6720 6973 204e 6f6e 653a 0a20 2020  log is None:.   
-00001ff0: 2020 2020 2020 2020 2061 7070 5f6c 6f67           app_log
-00002000: 203d 2063 6c73 2e67 6574 5f6c 6f67 6765   = cls.get_logge
-00002010: 7228 290a 0a20 2020 2020 2020 2069 6620  r()..        if 
-00002020: 6e6f 7420 6461 7461 3a0a 2020 2020 2020  not data:.      
-00002030: 2020 2020 2020 6170 705f 6c6f 672e 7761        app_log.wa
-00002040: 726e 696e 6728 224e 6f20 6461 7461 2070  rning("No data p
-00002050: 726f 7669 6465 6420 746f 2077 7269 7465  rovided to write
-00002060: 2074 6f20 7468 6520 6669 6c65 2e22 290a   to the file.").
-00002070: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002080: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
-00002090: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-000020a0: 2020 2077 6974 6820 6f70 656e 2866 696c     with open(fil
-000020b0: 655f 7061 7468 2c20 6d6f 6465 3d6d 6f64  e_path, mode=mod
-000020c0: 652c 206e 6577 6c69 6e65 3d6e 6577 6c69  e, newline=newli
-000020d0: 6e65 2920 6173 2066 703a 0a20 2020 2020  ne) as fp:.     
-000020e0: 2020 2020 2020 2020 2020 2061 7070 5f6c             app_l
-000020f0: 6f67 2e69 6e66 6f28 6627 5772 6974 696e  og.info(f'Writin
-00002100: 6720 746f 2043 5356 2066 696c 653a 207b  g to CSV file: {
-00002110: 6670 2e6e 616d 657d 2729 0a20 2020 2020  fp.name}').     
-00002120: 2020 2020 2020 2020 2020 2077 7269 7465             write
-00002130: 7220 3d20 6373 762e 7772 6974 6572 2866  r = csv.writer(f
-00002140: 702c 202a 2a6b 7761 7267 7329 0a20 2020  p, **kwargs).   
-00002150: 2020 2020 2020 2020 2020 2020 2077 7269               wri
-00002160: 7465 722e 7772 6974 6572 6f77 7328 6461  ter.writerows(da
-00002170: 7461 290a 2020 2020 2020 2020 6578 6365  ta).        exce
-00002180: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00002190: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-000021a0: 6170 705f 6c6f 672e 6578 6365 7074 696f  app_log.exceptio
-000021b0: 6e28 6622 416e 2065 7272 6f72 206f 6363  n(f"An error occ
-000021c0: 7572 7265 6420 7768 696c 6520 7772 6974  urred while writ
-000021d0: 696e 6720 746f 2074 6865 2043 5356 2066  ing to the CSV f
-000021e0: 696c 653a 207b 6578 7d22 290a 2020 2020  ile: {ex}").    
-000021f0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00002200: 616c 7365 0a0a 2020 2020 2020 2020 7265  alse..        re
-00002210: 7475 726e 2054 7275 650a 0a20 2020 2040  turn True..    @
-00002220: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00002230: 6465 6620 7265 6164 5f63 7376 5f64 6174  def read_csv_dat
-00002240: 615f 6672 6f6d 5f66 696c 6528 0a20 2020  a_from_file(.   
-00002250: 2020 2020 2020 2020 2063 6c73 2c0a 2020           cls,.  
-00002260: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
-00002270: 6174 683a 2073 7472 2c0a 2020 2020 2020  ath: str,.      
-00002280: 2020 2020 2020 6170 705f 6c6f 673a 204f        app_log: O
-00002290: 7074 696f 6e61 6c5b 6c6f 6767 696e 672e  ptional[logging.
-000022a0: 4c6f 6767 6572 5d20 3d20 4e6f 6e65 2c0a  Logger] = None,.
-000022b0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-000022c0: 3a20 7374 7220 3d20 2772 272c 0a20 2020  : str = 'r',.   
-000022d0: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-000022e0: 733a 2041 6e79 0a20 2020 2029 202d 3e20  s: Any.    ) -> 
-000022f0: 4f70 7469 6f6e 616c 5b4c 6973 745b 4c69  Optional[List[Li
-00002300: 7374 5b73 7472 5d5d 5d3a 0a20 2020 2020  st[str]]]:.     
-00002310: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00002320: 6561 6420 4353 5620 6461 7461 2066 726f  ead CSV data fro
-00002330: 6d20 6120 6669 6c65 2061 6e64 2072 6574  m a file and ret
-00002340: 7572 6e20 6120 6c69 7374 206f 6620 726f  urn a list of ro
-00002350: 7773 2e0a 0a20 2020 2020 2020 203a 7061  ws...        :pa
-00002360: 7261 6d20 6669 6c65 5f70 6174 683a 2050  ram file_path: P
-00002370: 6174 6820 746f 2074 6865 2043 5356 2066  ath to the CSV f
-00002380: 696c 6520 746f 2062 6520 7265 6164 2e0a  ile to be read..
-00002390: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
-000023a0: 7070 5f6c 6f67 3a20 4f70 7469 6f6e 616c  pp_log: Optional
-000023b0: 206c 6f67 6765 7220 666f 7220 6c6f 6767   logger for logg
-000023c0: 696e 6720 696e 666f 726d 6174 696f 6e2c  ing information,
-000023d0: 2064 6566 6175 6c74 7320 746f 2061 206e   defaults to a n
-000023e0: 6577 206c 6f67 6765 7220 6966 204e 6f6e  ew logger if Non
-000023f0: 652e 0a20 2020 2020 2020 203a 7061 7261  e..        :para
-00002400: 6d20 6d6f 6465 3a20 4d6f 6465 2069 6e20  m mode: Mode in 
-00002410: 7768 6963 6820 7468 6520 6669 6c65 2073  which the file s
-00002420: 686f 756c 6420 6265 206f 7065 6e65 642c  hould be opened,
-00002430: 2064 6566 6175 6c74 7320 746f 2027 7227   defaults to 'r'
-00002440: 2066 6f72 2072 6561 6420 6f6e 6c79 2e0a   for read only..
-00002450: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00002460: 204c 6973 7420 6f66 2072 6f77 7320 6672   List of rows fr
-00002470: 6f6d 2074 6865 2043 5356 2066 696c 6520  om the CSV file 
-00002480: 6f72 204e 6f6e 6520 6966 2061 6e20 6578  or None if an ex
-00002490: 6365 7074 696f 6e20 6f63 6375 7273 2e0a  ception occurs..
-000024a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000024b0: 2020 2020 6966 2061 7070 5f6c 6f67 2069      if app_log i
-000024c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000024d0: 2020 2020 6170 705f 6c6f 6720 3d20 636c      app_log = cl
-000024e0: 732e 6765 745f 6c6f 6767 6572 2829 0a0a  s.get_logger()..
-000024f0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00002500: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-00002510: 656e 2866 696c 655f 7061 7468 2c20 6d6f  en(file_path, mo
-00002520: 6465 3d6d 6f64 652c 202a 2a6b 7761 7267  de=mode, **kwarg
-00002530: 7329 2061 7320 6670 3a0a 2020 2020 2020  s) as fp:.      
-00002540: 2020 2020 2020 2020 2020 6170 705f 6c6f            app_lo
-00002550: 672e 696e 666f 2866 2752 6561 6469 6e67  g.info(f'Reading
-00002560: 2043 5356 2066 696c 653a 207b 6670 2e6e   CSV file: {fp.n
-00002570: 616d 657d 2729 0a20 2020 2020 2020 2020  ame}').         
-00002580: 2020 2020 2020 2072 6561 6465 7220 3d20         reader = 
-00002590: 6373 762e 7265 6164 6572 2866 702c 202a  csv.reader(fp, *
-000025a0: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
-000025b0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-000025c0: 5b72 6f77 2066 6f72 2072 6f77 2069 6e20  [row for row in 
-000025d0: 7265 6164 6572 5d0a 2020 2020 2020 2020  reader].        
-000025e0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-000025f0: 2061 7320 6578 3a0a 2020 2020 2020 2020   as ex:.        
-00002600: 2020 2020 6170 705f 6c6f 672e 6578 6365      app_log.exce
-00002610: 7074 696f 6e28 6622 416e 2065 7272 6f72  ption(f"An error
-00002620: 206f 6363 7572 7265 6420 7768 696c 6520   occurred while 
-00002630: 7265 6164 696e 6720 7468 6520 4353 5620  reading the CSV 
-00002640: 6669 6c65 3a20 7b65 787d 2229 0a20 2020  file: {ex}").   
-00002650: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002660: 4e6f 6e65 0a0a 2020 2020 2020 2020 7265  None..        re
-00002670: 7475 726e 2064 6174 610a 0a20 2020 2040  turn data..    @
-00002680: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00002690: 6465 6620 7772 6974 655f 6a73 6f6e 5f64  def write_json_d
-000026a0: 6174 615f 746f 5f66 696c 6528 0a20 2020  ata_to_file(.   
-000026b0: 2020 2020 2020 2020 2063 6c73 2c0a 2020           cls,.  
-000026c0: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
-000026d0: 6174 683a 2073 7472 2c0a 2020 2020 2020  ath: str,.      
-000026e0: 2020 2020 2020 6461 7461 3a20 416e 792c        data: Any,
-000026f0: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
-00002700: 5f6c 6f67 3a20 4f70 7469 6f6e 616c 5b6c  _log: Optional[l
-00002710: 6f67 6769 6e67 2e4c 6f67 6765 725d 203d  ogging.Logger] =
-00002720: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00002730: 2020 206d 6f64 653a 2073 7472 203d 2027     mode: str = '
-00002740: 7727 2c0a 2020 2020 2020 2020 2020 2020  w',.            
-00002750: 2a2a 6b77 6172 6773 3a20 416e 790a 2020  **kwargs: Any.  
-00002760: 2020 2920 2d3e 2062 6f6f 6c3a 0a20 2020    ) -> bool:.   
-00002770: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00002780: 2057 7269 7465 2064 6174 6120 746f 2061   Write data to a
-00002790: 204a 534f 4e20 6669 6c65 2e0a 0a20 2020   JSON file...   
-000027a0: 2020 2020 203a 7061 7261 6d20 6669 6c65       :param file
-000027b0: 5f70 6174 683a 204e 616d 6520 6f66 2074  _path: Name of t
-000027c0: 6865 204a 534f 4e20 6669 6c65 2e0a 2020  he JSON file..  
-000027d0: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
-000027e0: 613a 2044 6174 6120 746f 2077 7269 7465  a: Data to write
-000027f0: 2028 7573 7561 6c6c 7920 6120 6469 6374   (usually a dict
-00002800: 206f 7220 6120 6c69 7374 292e 0a20 2020   or a list)..   
-00002810: 2020 2020 203a 7061 7261 6d20 6170 705f       :param app_
-00002820: 6c6f 673a 204f 7074 696f 6e61 6c20 6c6f  log: Optional lo
-00002830: 6767 6572 2066 6f72 206c 6f67 6769 6e67  gger for logging
-00002840: 2069 6e66 6f72 6d61 7469 6f6e 2c20 6465   information, de
-00002850: 6661 756c 7473 2074 6f20 6120 6e65 7720  faults to a new 
-00002860: 6c6f 6767 6572 2069 6620 4e6f 6e65 2e0a  logger if None..
-00002870: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
-00002880: 6f64 653a 204d 6f64 6520 696e 2077 6869  ode: Mode in whi
-00002890: 6368 2074 6865 2066 696c 6520 7368 6f75  ch the file shou
-000028a0: 6c64 2062 6520 6f70 656e 6564 2c20 6465  ld be opened, de
-000028b0: 6661 756c 7473 2074 6f20 2777 2720 666f  faults to 'w' fo
-000028c0: 7220 7772 6974 6520 286f 7665 7277 7269  r write (overwri
-000028d0: 7469 6e67 292e 0a20 2020 2020 2020 203a  ting)..        :
-000028e0: 7265 7475 726e 3a20 626f 6f6c 2077 6561  return: bool wea
-000028f0: 7468 6572 2073 7563 6365 7373 206f 7220  ther success or 
-00002900: 6661 696c 6564 0a20 2020 2020 2020 2022  failed.        "
-00002910: 2222 0a20 2020 2020 2020 2069 6620 6170  "".        if ap
-00002920: 705f 6c6f 6720 6973 204e 6f6e 653a 0a20  p_log is None:. 
-00002930: 2020 2020 2020 2020 2020 2061 7070 5f6c             app_l
-00002940: 6f67 203d 2063 6c73 2e67 6574 5f6c 6f67  og = cls.get_log
-00002950: 6765 7228 290a 0a20 2020 2020 2020 2061  ger()..        a
-00002960: 7070 5f6c 6f67 2e69 6e66 6f28 6627 5772  pp_log.info(f'Wr
-00002970: 6974 696e 6720 746f 204a 534f 4e20 6669  iting to JSON fi
-00002980: 6c65 3a20 7b66 696c 655f 7061 7468 7d27  le: {file_path}'
-00002990: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
-000029a0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-000029b0: 6f70 656e 2866 696c 655f 7061 7468 2c20  open(file_path, 
-000029c0: 6d6f 6465 2c20 656e 636f 6469 6e67 3d27  mode, encoding='
-000029d0: 7574 662d 3827 2920 6173 2066 703a 0a20  utf-8') as fp:. 
-000029e0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-000029f0: 736f 6e2e 6475 6d70 2864 6174 612c 2066  son.dump(data, f
-00002a00: 702c 2065 6e73 7572 655f 6173 6369 693d  p, ensure_ascii=
-00002a10: 4661 6c73 652c 2069 6e64 656e 743d 342c  False, indent=4,
-00002a20: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-00002a30: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00002a40: 696f 6e20 6173 2065 783a 0a20 2020 2020  ion as ex:.     
-00002a50: 2020 2020 2020 2061 7070 5f6c 6f67 2e65         app_log.e
-00002a60: 7863 6570 7469 6f6e 2866 2241 6e20 6572  xception(f"An er
-00002a70: 726f 7220 6f63 6375 7272 6564 2077 6869  ror occurred whi
-00002a80: 6c65 2077 7269 7469 6e67 2074 6f20 7468  le writing to th
-00002a90: 6520 4a53 4f4e 2066 696c 653a 207b 6578  e JSON file: {ex
-00002aa0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00002ab0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-00002ac0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00002ad0: 650a 0a20 2020 2040 636c 6173 736d 6574  e..    @classmet
-00002ae0: 686f 640a 2020 2020 6465 6620 7265 6164  hod.    def read
-00002af0: 5f6a 736f 6e5f 6461 7461 5f66 726f 6d5f  _json_data_from_
-00002b00: 6669 6c65 280a 2020 2020 2020 2020 2020  file(.          
-00002b10: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
-00002b20: 2020 2066 696c 655f 7061 7468 3a20 7374     file_path: st
-00002b30: 722c 0a20 2020 2020 2020 2020 2020 2061  r,.            a
-00002b40: 7070 5f6c 6f67 3a20 4f70 7469 6f6e 616c  pp_log: Optional
-00002b50: 5b6c 6f67 6769 6e67 2e4c 6f67 6765 725d  [logging.Logger]
-00002b60: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00002b70: 2020 2020 206d 6f64 653a 2073 7472 203d       mode: str =
-00002b80: 2027 7227 2c0a 2020 2020 2020 2020 2020   'r',.          
-00002b90: 2020 2a2a 6b77 6172 6773 3a20 416e 790a    **kwargs: Any.
-00002ba0: 2020 2020 2920 2d3e 204f 7074 696f 6e61      ) -> Optiona
-00002bb0: 6c5b 416e 795d 3a0a 2020 2020 2020 2020  l[Any]:.        
-00002bc0: 2222 220a 2020 2020 2020 2020 5265 6164  """.        Read
-00002bd0: 2064 6174 6120 6672 6f6d 2061 204a 534f   data from a JSO
-00002be0: 4e20 6669 6c65 2e0a 0a20 2020 2020 2020  N file...       
-00002bf0: 203a 7061 7261 6d20 6669 6c65 5f70 6174   :param file_pat
-00002c00: 683a 204e 616d 6520 6f66 2074 6865 204a  h: Name of the J
-00002c10: 534f 4e20 6669 6c65 2e0a 2020 2020 2020  SON file..      
-00002c20: 2020 3a70 6172 616d 2061 7070 5f6c 6f67    :param app_log
-00002c30: 3a20 4f70 7469 6f6e 616c 206c 6f67 6765  : Optional logge
-00002c40: 7220 666f 7220 6c6f 6767 696e 6720 696e  r for logging in
-00002c50: 666f 726d 6174 696f 6e2c 2064 6566 6175  formation, defau
-00002c60: 6c74 7320 746f 2061 206e 6577 206c 6f67  lts to a new log
-00002c70: 6765 7220 6966 204e 6f6e 652e 0a20 2020  ger if None..   
-00002c80: 2020 2020 203a 7061 7261 6d20 6d6f 6465       :param mode
-00002c90: 3a20 4d6f 6465 2069 6e20 7768 6963 6820  : Mode in which 
-00002ca0: 7468 6520 6669 6c65 2073 686f 756c 6420  the file should 
-00002cb0: 6265 206f 7065 6e65 642c 2064 6566 6175  be opened, defau
-00002cc0: 6c74 7320 746f 2027 7227 2066 6f72 2072  lts to 'r' for r
-00002cd0: 6561 642e 0a20 2020 2020 2020 203a 7265  ead..        :re
-00002ce0: 7475 726e 3a20 4461 7461 2072 6561 6420  turn: Data read 
-00002cf0: 6672 6f6d 2074 6865 204a 534f 4e20 6669  from the JSON fi
-00002d00: 6c65 206f 7220 4e6f 6e65 2069 6620 616e  le or None if an
-00002d10: 2065 7863 6570 7469 6f6e 206f 6363 7572   exception occur
-00002d20: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00002d30: 2020 2020 2020 2069 6620 6170 705f 6c6f         if app_lo
-00002d40: 6720 6973 204e 6f6e 653a 0a20 2020 2020  g is None:.     
-00002d50: 2020 2020 2020 2061 7070 5f6c 6f67 203d         app_log =
-00002d60: 2063 6c73 2e67 6574 5f6c 6f67 6765 7228   cls.get_logger(
-00002d70: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
-00002d80: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00002d90: 206f 7065 6e28 6669 6c65 5f70 6174 682c   open(file_path,
-00002da0: 206d 6f64 652c 2065 6e63 6f64 696e 673d   mode, encoding=
-00002db0: 2775 7466 2d38 272c 202a 2a6b 7761 7267  'utf-8', **kwarg
-00002dc0: 7329 2061 7320 6670 3a0a 2020 2020 2020  s) as fp:.      
-00002dd0: 2020 2020 2020 2020 2020 6170 705f 6c6f            app_lo
-00002de0: 672e 696e 666f 2866 2752 6561 6469 6e67  g.info(f'Reading
-00002df0: 2066 726f 6d20 4a53 4f4e 2066 696c 653a   from JSON file:
-00002e00: 207b 6669 6c65 5f70 6174 687d 2729 0a20   {file_path}'). 
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002e20: 6574 7572 6e20 6a73 6f6e 2e6c 6f61 6428  eturn json.load(
-00002e30: 6670 290a 2020 2020 2020 2020 6578 6365  fp).        exce
-00002e40: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00002e50: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-00002e60: 6170 705f 6c6f 672e 6578 6365 7074 696f  app_log.exceptio
-00002e70: 6e28 6622 416e 2065 7272 6f72 206f 6363  n(f"An error occ
-00002e80: 7572 7265 6420 7768 696c 6520 7265 6164  urred while read
-00002e90: 696e 6720 7468 6520 4a53 4f4e 2066 696c  ing the JSON fil
-00002ea0: 653a 207b 6578 7d22 290a 2020 2020 2020  e: {ex}").      
-00002eb0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00002ec0: 650a 0a0a 636c 6173 7320 4d6f 6465 6c55  e...class ModelU
-00002ed0: 7469 6c3a 0a20 2020 2040 7374 6174 6963  til:.    @static
-00002ee0: 6d65 7468 6f64 0a20 2020 2064 6566 2065  method.    def e
-00002ef0: 7870 6f6e 656e 7469 616c 5f6d 6f76 696e  xponential_movin
-00002f00: 675f 6176 6572 6167 655f 6e65 7874 5f76  g_average_next_v
-00002f10: 616c 7565 280a 2020 2020 2020 2020 2020  alue(.          
-00002f20: 2020 6e75 6d65 7269 635f 7365 7175 656e    numeric_sequen
-00002f30: 6365 3a20 4c69 7374 5b69 6e74 5d2c 0a20  ce: List[int],. 
-00002f40: 2020 2020 2020 2020 2020 2073 7061 6e3a             span:
-00002f50: 2069 6e74 203d 2035 2c0a 2020 2020 2020   int = 5,.      
-00002f60: 2020 2020 2020 656e 6162 6c65 5f72 6f6c        enable_rol
-00002f70: 6c69 6e67 5f64 6966 6665 7265 6e63 653a  ling_difference:
-00002f80: 2062 6f6f 6c20 3d20 4661 6c73 650a 2020   bool = False.  
-00002f90: 2020 2920 2d3e 2069 6e74 3a0a 2020 2020    ) -> int:.    
-00002fa0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002fb0: 4361 6c63 756c 6174 6520 7468 6520 4578  Calculate the Ex
-00002fc0: 706f 6e65 6e74 6961 6c20 4d6f 7669 6e67  ponential Moving
-00002fd0: 2041 7665 7261 6765 2028 454d 4129 2061   Average (EMA) a
-00002fe0: 6e64 2075 7365 2072 6f6c 6c69 6e67 2064  nd use rolling d
-00002ff0: 6966 6665 7265 6e63 6520 746f 2070 7265  ifference to pre
-00003000: 6469 6374 2074 6865 206e 6578 7420 7661  dict the next va
-00003010: 6c75 6520 6f66 2061 2073 6571 7565 6e63  lue of a sequenc
-00003020: 652e 0a0a 2020 2020 2020 2020 454d 4120  e...        EMA 
-00003030: 6973 2061 2074 7970 6520 6f66 206d 6f76  is a type of mov
-00003040: 696e 6720 6176 6572 6167 6520 7468 6174  ing average that
-00003050: 2070 6c61 6365 7320 6120 6772 6561 7465   places a greate
-00003060: 7220 7765 6967 6874 2061 6e64 2073 6967  r weight and sig
-00003070: 6e69 6669 6361 6e63 650a 2020 2020 2020  nificance.      
-00003080: 2020 6f6e 2074 6865 206d 6f73 7420 7265    on the most re
-00003090: 6365 6e74 2064 6174 6120 706f 696e 7473  cent data points
-000030a0: 2e20 4974 2773 206d 6f72 6520 7265 7370  . It's more resp
-000030b0: 6f6e 7369 7665 2074 6f20 6e65 7720 696e  onsive to new in
-000030c0: 666f 726d 6174 696f 6e20 636f 6d70 6172  formation compar
-000030d0: 6564 0a20 2020 2020 2020 2074 6f20 6120  ed.        to a 
-000030e0: 7369 6d70 6c65 206d 6f76 696e 6720 6176  simple moving av
-000030f0: 6572 6167 6520 2853 4d41 292e 0a0a 2020  erage (SMA)...  
-00003100: 2020 2020 2020 3a70 6172 616d 206e 756d        :param num
-00003110: 6572 6963 5f73 6571 7565 6e63 653a 2041  eric_sequence: A
-00003120: 206c 6973 7420 6f72 2073 6571 7565 6e63   list or sequenc
-00003130: 6520 6f66 206e 756d 6265 7273 2066 6f72  e of numbers for
-00003140: 2077 6869 6368 2074 6865 2045 4d41 2069   which the EMA i
-00003150: 7320 746f 2062 6520 6361 6c63 756c 6174  s to be calculat
-00003160: 6564 2e0a 2020 2020 2020 2020 3a70 6172  ed..        :par
-00003170: 616d 2073 7061 6e3a 2054 6865 206e 756d  am span: The num
-00003180: 6265 7220 6f66 2070 6572 696f 6473 206f  ber of periods o
-00003190: 7665 7220 7768 6963 6820 746f 2063 616c  ver which to cal
-000031a0: 6375 6c61 7465 2074 6865 2045 4d41 2e20  culate the EMA. 
-000031b0: 4465 6661 756c 7420 6973 2035 2e0a 2020  Default is 5..  
-000031c0: 2020 2020 2020 3a70 6172 616d 2065 6e61        :param ena
-000031d0: 626c 655f 726f 6c6c 696e 675f 6469 6666  ble_rolling_diff
-000031e0: 6572 656e 6365 3a20 7765 6174 6865 7220  erence: weather 
-000031f0: 746f 2065 6e61 626c 6520 726f 6c6c 696e  to enable rollin
-00003200: 672e 2064 6566 6175 6c74 2069 7320 4661  g. default is Fa
-00003210: 6c73 650a 2020 2020 2020 2020 3a72 6574  lse.        :ret
-00003220: 7572 6e3a 2050 7265 6469 6374 6564 206e  urn: Predicted n
-00003230: 6578 7420 7661 6c75 6520 6f66 2074 6865  ext value of the
-00003240: 2073 6571 7565 6e63 6520 6261 7365 6420   sequence based 
-00003250: 6f6e 2045 4d41 2061 6e64 2072 6f6c 6c69  on EMA and rolli
-00003260: 6e67 2064 6966 6665 7265 6e63 652e 0a20  ng difference.. 
-00003270: 2020 2020 2020 203a 7261 6973 6573 2056         :raises V
-00003280: 616c 7565 4572 726f 723a 2049 6620 7468  alueError: If th
-00003290: 6520 696e 7075 7420 6c69 7374 2069 7320  e input list is 
-000032a0: 656d 7074 7920 6f72 2063 6f6e 7461 696e  empty or contain
-000032b0: 7320 6e6f 6e2d 6e75 6d65 7269 6320 7661  s non-numeric va
-000032c0: 6c75 6573 2e0a 2020 2020 2020 2020 2222  lues..        ""
-000032d0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-000032e0: 206e 756d 6572 6963 5f73 6571 7565 6e63   numeric_sequenc
-000032f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00003300: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00003310: 2254 6865 206e 756d 6572 6963 2073 6571  "The numeric seq
-00003320: 7565 6e63 6520 6361 6e6e 6f74 2062 6520  uence cannot be 
-00003330: 656d 7074 792e 2229 0a20 2020 2020 2020  empty.").       
-00003340: 2069 6620 6e6f 7420 616c 6c28 6973 696e   if not all(isin
-00003350: 7374 616e 6365 2878 2c20 2869 6e74 2c20  stance(x, (int, 
-00003360: 666c 6f61 7429 2920 666f 7220 7820 696e  float)) for x in
-00003370: 206e 756d 6572 6963 5f73 6571 7565 6e63   numeric_sequenc
-00003380: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00003390: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-000033a0: 2822 416c 6c20 656c 656d 656e 7473 2069  ("All elements i
-000033b0: 6e20 7468 6520 6e75 6d65 7269 6320 7365  n the numeric se
-000033c0: 7175 656e 6365 206d 7573 7420 6265 206e  quence must be n
-000033d0: 756d 6265 7273 2e22 290a 0a20 2020 2020  umbers.")..     
-000033e0: 2020 2023 2043 6f6e 7665 7274 2074 6865     # Convert the
-000033f0: 206e 756d 6572 6963 2073 6571 7565 6e63   numeric sequenc
-00003400: 6520 696e 746f 2061 2070 616e 6461 7320  e into a pandas 
-00003410: 5365 7269 6573 206f 626a 6563 740a 2020  Series object.  
-00003420: 2020 2020 2020 7365 7269 6573 203d 2070        series = p
-00003430: 642e 5365 7269 6573 286e 756d 6572 6963  d.Series(numeric
-00003440: 5f73 6571 7565 6e63 6529 0a0a 2020 2020  _sequence)..    
-00003450: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
-00003460: 7468 6520 454d 4120 7573 696e 6720 7061  the EMA using pa
-00003470: 6e64 6173 2720 6577 6d20 6d65 7468 6f64  ndas' ewm method
-00003480: 0a20 2020 2020 2020 2023 2041 646a 7573  .        # Adjus
-00003490: 7420 276d 696e 5f70 6572 696f 6473 2720  t 'min_periods' 
-000034a0: 746f 2068 616e 646c 6520 7368 6f72 7465  to handle shorte
-000034b0: 7220 7365 7175 656e 6365 7320 6772 6163  r sequences grac
-000034c0: 6566 756c 6c79 0a20 2020 2020 2020 2065  efully.        e
-000034d0: 6d61 203d 2073 6572 6965 732e 6577 6d28  ma = series.ewm(
-000034e0: 7370 616e 3d73 7061 6e2c 206d 696e 5f70  span=span, min_p
-000034f0: 6572 696f 6473 3d6d 696e 2873 7061 6e2c  eriods=min(span,
-00003500: 206c 656e 286e 756d 6572 6963 5f73 6571   len(numeric_seq
-00003510: 7565 6e63 6529 292c 2061 646a 7573 743d  uence)), adjust=
-00003520: 4661 6c73 6529 2e6d 6561 6e28 290a 0a20  False).mean().. 
-00003530: 2020 2020 2020 2023 2043 616c 6375 6c61         # Calcula
-00003540: 7465 2072 6f6c 6c69 6e67 2064 6966 6665  te rolling diffe
-00003550: 7265 6e63 650a 2020 2020 2020 2020 726f  rence.        ro
-00003560: 6c6c 696e 675f 6469 6666 6572 656e 6365  lling_difference
-00003570: 203d 2073 6572 6965 732e 6469 6666 2829   = series.diff()
-00003580: 0a0a 2020 2020 2020 2020 2320 5072 6564  ..        # Pred
-00003590: 6963 7420 7468 6520 6e65 7874 2076 616c  ict the next val
-000035a0: 7565 2062 7920 6578 7472 6170 6f6c 6174  ue by extrapolat
-000035b0: 696e 6720 7468 6520 6c61 7374 2072 6f6c  ing the last rol
-000035c0: 6c69 6e67 2064 6966 6665 7265 6e63 6520  ling difference 
-000035d0: 616e 6420 7468 6520 6c61 7374 2045 4d41  and the last EMA
-000035e0: 2076 616c 7565 0a20 2020 2020 2020 2069   value.        i
-000035f0: 6620 6c65 6e28 726f 6c6c 696e 675f 6469  f len(rolling_di
-00003600: 6666 6572 656e 6365 2920 3e20 3120 616e  fference) > 1 an
-00003610: 6420 656e 6162 6c65 5f72 6f6c 6c69 6e67  d enable_rolling
-00003620: 5f64 6966 6665 7265 6e63 6520 6973 2054  _difference is T
-00003630: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
-00003640: 2070 7265 6469 6374 6564 5f6e 6578 745f   predicted_next_
-00003650: 7661 6c75 6520 3d20 656d 612e 696c 6f63  value = ema.iloc
-00003660: 5b2d 315d 202b 2072 6f6c 6c69 6e67 5f64  [-1] + rolling_d
-00003670: 6966 6665 7265 6e63 652e 696c 6f63 5b2d  ifference.iloc[-
-00003680: 315d 0a20 2020 2020 2020 2065 6c73 653a  1].        else:
-00003690: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
-000036a0: 6620 7468 6572 6527 7320 6e6f 2065 6e6f  f there's no eno
-000036b0: 7567 6820 6461 7461 2074 6f20 6361 6c63  ugh data to calc
-000036c0: 756c 6174 6520 6469 6666 6572 656e 6365  ulate difference
-000036d0: 2c20 7573 6520 7468 6520 6c61 7374 2045  , use the last E
-000036e0: 4d41 2061 7320 7468 6520 7072 6564 6963  MA as the predic
-000036f0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00003700: 2070 7265 6469 6374 6564 5f6e 6578 745f   predicted_next_
-00003710: 7661 6c75 6520 3d20 656d 612e 696c 6f63  value = ema.iloc
-00003720: 5b2d 315d 0a0a 2020 2020 2020 2020 2320  [-1]..        # 
-00003730: 5265 7475 726e 2074 6865 2070 7265 6469  Return the predi
-00003740: 6374 6564 206e 6578 7420 7661 6c75 6520  cted next value 
-00003750: 726f 756e 6465 6420 746f 2074 6865 206e  rounded to the n
-00003760: 6561 7265 7374 2069 6e74 6567 6572 0a20  earest integer. 
-00003770: 2020 2020 2020 2072 6574 7572 6e20 726f         return ro
-00003780: 756e 6428 7072 6564 6963 7465 645f 6e65  und(predicted_ne
-00003790: 7874 5f76 616c 7565 290a 0a20 2020 2040  xt_value)..    @
-000037a0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-000037b0: 2064 6566 206c 696e 6561 725f 7265 6772   def linear_regr
-000037c0: 6573 7369 6f6e 5f6e 6578 745f 7661 6c75  ession_next_valu
-000037d0: 655f 6279 5f69 6e64 6578 286e 756d 6572  e_by_index(numer
-000037e0: 6963 5f73 6571 7565 6e63 653a 204c 6973  ic_sequence: Lis
-000037f0: 745b 696e 745d 2920 2d3e 2069 6e74 3a0a  t[int]) -> int:.
-00003800: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003810: 2020 2020 5072 6564 6963 7473 2074 6865      Predicts the
-00003820: 206e 6578 7420 7661 6c75 6520 696e 2061   next value in a
-00003830: 2073 6571 7565 6e63 6520 7573 696e 6720   sequence using 
-00003840: 6c69 6e65 6172 2072 6567 7265 7373 696f  linear regressio
-00003850: 6e2e 0a0a 2020 2020 2020 2020 4c69 6e65  n...        Line
-00003860: 6172 2072 6567 7265 7373 696f 6e20 696e  ar regression in
-00003870: 766f 6c76 6573 2066 6974 7469 6e67 2061  volves fitting a
-00003880: 206c 696e 6520 746f 2074 6865 2064 6174   line to the dat
-00003890: 6120 706f 696e 7473 2069 6e20 7375 6368  a points in such
-000038a0: 2061 2077 6179 0a20 2020 2020 2020 2074   a way.        t
-000038b0: 6861 7420 7468 6520 6469 7374 616e 6365  hat the distance
-000038c0: 2062 6574 7765 656e 2074 6865 2064 6174   between the dat
-000038d0: 6120 706f 696e 7473 2061 6e64 2074 6865  a points and the
-000038e0: 206c 696e 6520 6973 206d 696e 696d 697a   line is minimiz
-000038f0: 6564 2e20 5468 6973 2066 756e 6374 696f  ed. This functio
-00003900: 6e0a 2020 2020 2020 2020 7573 6573 2074  n.        uses t
-00003910: 6865 206d 6574 686f 6420 746f 2070 7265  he method to pre
-00003920: 6469 6374 2074 6865 206e 6578 7420 7661  dict the next va
-00003930: 6c75 6520 696e 2061 2067 6976 656e 2073  lue in a given s
-00003940: 6571 7565 6e63 6520 6f66 206e 756d 6265  equence of numbe
-00003950: 7273 2062 7920 6669 7474 696e 670a 2020  rs by fitting.  
-00003960: 2020 2020 2020 6120 6d6f 6465 6c20 746f        a model to
-00003970: 2074 6865 2073 6571 7565 6e63 6520 616e   the sequence an
-00003980: 6420 6578 616d 696e 696e 6720 7468 6520  d examining the 
-00003990: 736c 6f70 6520 6f66 2074 6865 206c 696e  slope of the lin
-000039a0: 652e 0a0a 2020 2020 2020 2020 3a70 6172  e...        :par
-000039b0: 616d 206e 756d 6572 6963 5f73 6571 7565  am numeric_seque
-000039c0: 6e63 653a 2041 206c 6973 7420 6f72 2073  nce: A list or s
-000039d0: 6571 7565 6e63 6520 6f66 206e 756d 6265  equence of numbe
-000039e0: 7273 2074 6f20 6d6f 6465 6c2e 0a20 2020  rs to model..   
-000039f0: 2020 2020 203a 7265 7475 726e 3a20 5468       :return: Th
-00003a00: 6520 7072 6564 6963 7465 6420 6e65 7874  e predicted next
-00003a10: 2076 616c 7565 2069 6e20 7468 6520 7365   value in the se
-00003a20: 7175 656e 6365 2061 7320 616e 2069 6e74  quence as an int
-00003a30: 6567 6572 2e0a 2020 2020 2020 2020 3a72  eger..        :r
-00003a40: 6169 7365 7320 5661 6c75 6545 7272 6f72  aises ValueError
-00003a50: 3a20 4966 2074 6865 2069 6e70 7574 2073  : If the input s
-00003a60: 6571 7565 6e63 6520 6973 2065 6d70 7479  equence is empty
-00003a70: 206f 7220 746f 6f20 7368 6f72 7420 666f   or too short fo
-00003a80: 7220 7265 6772 6573 7369 6f6e 2061 6e61  r regression ana
-00003a90: 6c79 7369 732e 0a20 2020 2020 2020 2022  lysis..        "
-00003aa0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-00003ab0: 7420 6e75 6d65 7269 635f 7365 7175 656e  t numeric_sequen
-00003ac0: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-00003ad0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00003ae0: 2822 5468 6520 6e75 6d65 7269 6320 7365  ("The numeric se
-00003af0: 7175 656e 6365 2063 616e 6e6f 7420 6265  quence cannot be
-00003b00: 2065 6d70 7479 2e22 290a 2020 2020 2020   empty.").      
-00003b10: 2020 6966 206c 656e 286e 756d 6572 6963    if len(numeric
-00003b20: 5f73 6571 7565 6e63 6529 203c 2032 3a0a  _sequence) < 2:.
-00003b30: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00003b40: 6520 5661 6c75 6545 7272 6f72 2822 5468  e ValueError("Th
-00003b50: 6520 6e75 6d65 7269 6320 7365 7175 656e  e numeric sequen
-00003b60: 6365 206d 7573 7420 636f 6e74 6169 6e20  ce must contain 
-00003b70: 6174 206c 6561 7374 2074 776f 2065 6c65  at least two ele
-00003b80: 6d65 6e74 7320 666f 7220 6c69 6e65 6172  ments for linear
-00003b90: 2072 6567 7265 7373 696f 6e2e 2229 0a0a   regression.")..
-00003ba0: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-00003bb0: 7420 7468 6520 6e75 6d65 7269 6320 7365  t the numeric se
-00003bc0: 7175 656e 6365 2069 6e74 6f20 6120 6e75  quence into a nu
-00003bd0: 6d70 7920 6172 7261 7920 616e 6420 7265  mpy array and re
-00003be0: 7368 6170 6520 666f 7220 736b 6c65 6172  shape for sklear
-00003bf0: 6e0a 2020 2020 2020 2020 6461 7461 203d  n.        data =
-00003c00: 206e 702e 6172 7261 7928 6e75 6d65 7269   np.array(numeri
-00003c10: 635f 7365 7175 656e 6365 292e 7265 7368  c_sequence).resh
-00003c20: 6170 6528 2d31 2c20 3129 0a0a 2020 2020  ape(-1, 1)..    
-00003c30: 2020 2020 2320 4372 6561 7465 2061 6e20      # Create an 
-00003c40: 6172 7261 7920 7265 7072 6573 656e 7469  array representi
-00003c50: 6e67 2074 696d 6520 6f72 2074 6865 2069  ng time or the i
-00003c60: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
-00003c70: 626c 652c 2072 6573 6861 7065 6420 6173  ble, reshaped as
-00003c80: 2061 2063 6f6c 756d 6e0a 2020 2020 2020   a column.      
-00003c90: 2020 696e 6465 7820 3d20 6e70 2e61 7272    index = np.arr
-00003ca0: 6179 2872 616e 6765 286c 656e 2864 6174  ay(range(len(dat
-00003cb0: 6129 2929 2e72 6573 6861 7065 282d 312c  a))).reshape(-1,
-00003cc0: 2031 290a 0a20 2020 2020 2020 2023 2043   1)..        # C
-00003cd0: 7265 6174 6520 6120 4c69 6e65 6172 5265  reate a LinearRe
-00003ce0: 6772 6573 7369 6f6e 206d 6f64 656c 2061  gression model a
-00003cf0: 6e64 2066 6974 2069 7420 746f 2074 6865  nd fit it to the
-00003d00: 2064 6174 610a 2020 2020 2020 2020 6d6f   data.        mo
-00003d10: 6465 6c20 3d20 4c69 6e65 6172 5265 6772  del = LinearRegr
-00003d20: 6573 7369 6f6e 2829 0a20 2020 2020 2020  ession().       
-00003d30: 206d 6f64 656c 2e66 6974 2869 6e64 6578   model.fit(index
-00003d40: 2c20 6461 7461 290a 0a20 2020 2020 2020  , data)..       
-00003d50: 2023 2050 7265 6469 6374 2074 6865 206e   # Predict the n
-00003d60: 6578 7420 7661 6c75 6520 696e 2074 6865  ext value in the
-00003d70: 2073 6571 7565 6e63 6520 7573 696e 6720   sequence using 
-00003d80: 7468 6520 6669 7474 6564 206d 6f64 656c  the fitted model
-00003d90: 0a20 2020 2020 2020 2070 7265 6469 6374  .        predict
-00003da0: 696f 6e20 3d20 6d6f 6465 6c2e 7072 6564  ion = model.pred
-00003db0: 6963 7428 5b5b 6c65 6e28 6461 7461 295d  ict([[len(data)]
-00003dc0: 5d29 5b30 5d5b 305d 0a0a 2020 2020 2020  ])[0][0]..      
-00003dd0: 2020 2320 5265 7475 726e 2074 6865 2070    # Return the p
-00003de0: 7265 6469 6374 6564 2076 616c 7565 2061  redicted value a
-00003df0: 7320 616e 2069 6e74 6567 6572 0a20 2020  s an integer.   
-00003e00: 2020 2020 2072 6574 7572 6e20 726f 756e       return roun
-00003e10: 6428 7072 6564 6963 7469 6f6e 290a 0a20  d(prediction).. 
-00003e20: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00003e30: 0a20 2020 2064 6566 206d 756c 7469 7661  .    def multiva
-00003e40: 7269 6174 655f 706f 6c79 6e6f 6d69 616c  riate_polynomial
-00003e50: 5f72 6567 7265 7373 696f 6e5f 6e65 7874  _regression_next
-00003e60: 5f76 616c 7565 280a 2020 2020 2020 2020  _value(.        
-00003e70: 2020 2020 6e75 6d65 7269 635f 7365 7175      numeric_sequ
-00003e80: 656e 6365 3a20 4c69 7374 5b69 6e74 5d2c  ence: List[int],
-00003e90: 0a20 2020 2020 2020 2020 2020 2072 6f6c  .            rol
-00003ea0: 6c69 6e67 5f73 697a 653a 2069 6e74 2c0a  ling_size: int,.
-00003eb0: 2020 2020 2020 2020 2020 2020 6465 6772              degr
-00003ec0: 6565 733a 2069 6e74 203d 2033 2c0a 2020  ees: int = 3,.  
-00003ed0: 2020 2920 2d3e 2066 6c6f 6174 3a0a 2020    ) -> float:.  
-00003ee0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00003ef0: 2020 5072 6564 6963 7473 2074 6865 206e    Predicts the n
-00003f00: 6578 7420 7661 6c75 6520 696e 2061 206e  ext value in a n
-00003f10: 756d 6572 6963 2073 6571 7565 6e63 6520  umeric sequence 
-00003f20: 7573 696e 6720 6d75 6c74 6976 6172 6961  using multivaria
-00003f30: 7465 2070 6f6c 796e 6f6d 6961 6c20 7265  te polynomial re
-00003f40: 6772 6573 7369 6f6e 2e0a 0a20 2020 2020  gression...     
-00003f50: 2020 2054 6869 7320 6d65 7468 6f64 2061     This method a
-00003f60: 7070 6c69 6573 2061 2070 6f6c 796e 6f6d  pplies a polynom
-00003f70: 6961 6c20 7265 6772 6573 7369 6f6e 206d  ial regression m
-00003f80: 6f64 656c 2074 6f20 6120 6e75 6d65 7269  odel to a numeri
-00003f90: 6320 7365 7175 656e 6365 2074 6f20 7072  c sequence to pr
-00003fa0: 6564 6963 7420 7468 6520 6e65 7874 2076  edict the next v
-00003fb0: 616c 7565 2e0a 2020 2020 2020 2020 4974  alue..        It
-00003fc0: 2075 7469 6c69 7a65 7320 6120 726f 6c6c   utilizes a roll
-00003fd0: 696e 6720 7769 6e64 6f77 2061 7070 726f  ing window appro
-00003fe0: 6163 6820 746f 2063 7265 6174 6520 6461  ach to create da
-00003ff0: 7461 7365 7473 2c20 7363 616c 6573 2074  tasets, scales t
-00004000: 6865 2066 6561 7475 7265 732c 2061 6e64  he features, and
-00004010: 2066 6974 7320 6120 706f 6c79 6e6f 6d69   fits a polynomi
-00004020: 616c 0a20 2020 2020 2020 2072 6567 7265  al.        regre
-00004030: 7373 696f 6e20 6d6f 6465 6c20 746f 206d  ssion model to m
-00004040: 616b 6520 7468 6520 7072 6564 6963 7469  ake the predicti
-00004050: 6f6e 2e0a 0a20 2020 2020 2020 2041 7267  on...        Arg
-00004060: 733a 0a20 2020 2020 2020 2020 2020 206e  s:.            n
-00004070: 756d 6572 6963 5f73 6571 7565 6e63 6520  umeric_sequence 
-00004080: 284c 6973 745b 696e 745d 293a 2054 6865  (List[int]): The
-00004090: 206c 6973 7420 6f66 2069 6e74 6567 6572   list of integer
-000040a0: 7320 7265 7072 6573 656e 7469 6e67 2074  s representing t
-000040b0: 6865 2073 6571 7565 6e63 652e 0a20 2020  he sequence..   
-000040c0: 2020 2020 2020 2020 2072 6f6c 6c69 6e67           rolling
-000040d0: 5f73 697a 6520 2869 6e74 293a 2054 6865  _size (int): The
-000040e0: 206e 756d 6265 7220 6f66 2065 6c65 6d65   number of eleme
-000040f0: 6e74 7320 696e 2065 6163 6820 726f 6c6c  nts in each roll
-00004100: 696e 6720 7769 6e64 6f77 2e0a 2020 2020  ing window..    
-00004110: 2020 2020 2020 2020 6465 6772 6565 7320          degrees 
-00004120: 2869 6e74 293a 2054 6865 2064 6567 7265  (int): The degre
-00004130: 6520 6f66 2074 6865 2070 6f6c 796e 6f6d  e of the polynom
-00004140: 6961 6c20 7265 6772 6573 7369 6f6e 2e20  ial regression. 
-00004150: 4465 6661 756c 7473 2074 6f20 332e 0a0a  Defaults to 3...
-00004160: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00004170: 0a20 2020 2020 2020 2020 2020 2066 6c6f  .            flo
-00004180: 6174 3a20 5468 6520 7072 6564 6963 7465  at: The predicte
-00004190: 6420 6e65 7874 2076 616c 7565 2069 6e20  d next value in 
-000041a0: 7468 6520 7365 7175 656e 6365 2e0a 0a20  the sequence... 
-000041b0: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-000041c0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-000041d0: 4572 726f 723a 2049 6620 7468 6520 726f  Error: If the ro
-000041e0: 6c6c 696e 675f 7369 7a65 2069 7320 6c61  lling_size is la
-000041f0: 7267 6572 2074 6861 6e20 7468 6520 7369  rger than the si
-00004200: 7a65 206f 6620 6e75 6d65 7269 635f 7365  ze of numeric_se
-00004210: 7175 656e 6365 2e0a 2020 2020 2020 2020  quence..        
-00004220: 2222 220a 2020 2020 2020 2020 6966 2072  """.        if r
-00004230: 6f6c 6c69 6e67 5f73 697a 6520 3e20 6c65  olling_size > le
-00004240: 6e28 6e75 6d65 7269 635f 7365 7175 656e  n(numeric_sequen
-00004250: 6365 293a 0a20 2020 2020 2020 2020 2020  ce):.           
-00004260: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00004270: 7228 2272 6f6c 6c69 6e67 5f73 697a 6520  r("rolling_size 
-00004280: 6361 6e6e 6f74 2062 6520 6c61 7267 6572  cannot be larger
-00004290: 2074 6861 6e20 7468 6520 7369 7a65 206f   than the size o
-000042a0: 6620 6e75 6d65 7269 635f 7365 7175 656e  f numeric_sequen
-000042b0: 6365 2229 0a0a 2020 2020 2020 2020 2320  ce")..        # 
-000042c0: 4765 6e65 7261 7465 2064 6174 6173 6574  Generate dataset
-000042d0: 7320 7769 7468 2074 6865 2073 7065 6369  s with the speci
-000042e0: 6669 6564 2072 6f6c 6c69 6e67 2073 697a  fied rolling siz
-000042f0: 650a 2020 2020 2020 2020 7472 6169 6e5f  e.        train_
-00004300: 782c 2074 7261 696e 5f79 203d 2043 616c  x, train_y = Cal
-00004310: 6375 6c61 7465 5574 696c 2e67 656e 6572  culateUtil.gener
-00004320: 6174 655f 6461 7461 7365 7473 5f77 6974  ate_datasets_wit
-00004330: 685f 726f 6c6c 696e 675f 7369 7a65 280a  h_rolling_size(.
-00004340: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00004350: 3d6e 756d 6572 6963 5f73 6571 7565 6e63  =numeric_sequenc
-00004360: 652c 2072 6f6c 6c69 6e67 5f73 697a 653d  e, rolling_size=
-00004370: 726f 6c6c 696e 675f 7369 7a65 0a20 2020  rolling_size.   
-00004380: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00004390: 2320 5072 6570 6172 696e 6720 696e 7075  # Preparing inpu
-000043a0: 7420 6461 7461 2066 6f72 206d 6f64 656c  t data for model
-000043b0: 2074 7261 696e 696e 670a 2020 2020 2020   training.      
-000043c0: 2020 696e 7075 745f 7820 3d20 6e70 2e61    input_x = np.a
-000043d0: 7272 6179 2874 7261 696e 5f78 290a 2020  rray(train_x).  
-000043e0: 2020 2020 2020 6f75 7470 7574 5f79 203d        output_y =
-000043f0: 206e 702e 6172 7261 7928 7472 6169 6e5f   np.array(train_
-00004400: 7929 0a0a 2020 2020 2020 2020 2320 5363  y)..        # Sc
-00004410: 616c 696e 6720 7468 6520 6665 6174 7572  aling the featur
-00004420: 6573 0a20 2020 2020 2020 2073 6361 6c65  es.        scale
-00004430: 7220 3d20 5374 616e 6461 7264 5363 616c  r = StandardScal
-00004440: 6572 2829 0a20 2020 2020 2020 2069 6e70  er().        inp
-00004450: 7574 5f78 5f73 6361 6c65 6420 3d20 7363  ut_x_scaled = sc
-00004460: 616c 6572 2e66 6974 5f74 7261 6e73 666f  aler.fit_transfo
-00004470: 726d 2869 6e70 7574 5f78 290a 0a20 2020  rm(input_x)..   
-00004480: 2020 2020 2023 2043 7265 6174 696e 6720       # Creating 
-00004490: 616e 6420 7472 6169 6e69 6e67 2074 6865  and training the
-000044a0: 2070 6f6c 796e 6f6d 6961 6c20 7265 6772   polynomial regr
-000044b0: 6573 7369 6f6e 206d 6f64 656c 0a20 2020  ession model.   
-000044c0: 2020 2020 206d 6f64 656c 203d 206d 616b       model = mak
-000044d0: 655f 7069 7065 6c69 6e65 2850 6f6c 796e  e_pipeline(Polyn
-000044e0: 6f6d 6961 6c46 6561 7475 7265 7328 6465  omialFeatures(de
-000044f0: 6772 6565 7329 2c20 4c69 6e65 6172 5265  grees), LinearRe
-00004500: 6772 6573 7369 6f6e 2829 290a 2020 2020  gression()).    
-00004510: 2020 2020 6d6f 6465 6c2e 6669 7428 696e      model.fit(in
-00004520: 7075 745f 785f 7363 616c 6564 2c20 6f75  put_x_scaled, ou
-00004530: 7470 7574 5f79 290a 0a20 2020 2020 2020  tput_y)..       
-00004540: 2023 2050 7265 7061 7269 6e67 2074 6865   # Preparing the
-00004550: 206c 6173 7420 726f 6c6c 696e 6720 7769   last rolling wi
-00004560: 6e64 6f77 206f 6620 6461 7461 2066 6f72  ndow of data for
-00004570: 2070 7265 6469 6374 696f 6e0a 2020 2020   prediction.    
-00004580: 2020 2020 7465 7374 5f78 203d 206e 702e      test_x = np.
-00004590: 6172 7261 7928 5b6e 756d 6572 6963 5f73  array([numeric_s
-000045a0: 6571 7565 6e63 655b 2d72 6f6c 6c69 6e67  equence[-rolling
-000045b0: 5f73 697a 653a 5d5d 290a 2020 2020 2020  _size:]]).      
-000045c0: 2020 7465 7374 5f78 5f73 6361 6c65 6420    test_x_scaled 
-000045d0: 3d20 7363 616c 6572 2e74 7261 6e73 666f  = scaler.transfo
-000045e0: 726d 2874 6573 745f 7829 0a0a 2020 2020  rm(test_x)..    
-000045f0: 2020 2020 2320 5072 6564 6963 7469 6e67      # Predicting
-00004600: 2074 6865 206e 6578 7420 7661 6c75 650a   the next value.
-00004610: 2020 2020 2020 2020 7072 6564 5f79 203d          pred_y =
-00004620: 206d 6f64 656c 2e70 7265 6469 6374 2874   model.predict(t
-00004630: 6573 745f 785f 7363 616c 6564 290a 2020  est_x_scaled).  
-00004640: 2020 2020 2020 7265 7475 726e 2070 7265        return pre
-00004650: 645f 795b 305d 0a0a 2020 2020 4073 7461  d_y[0]..    @sta
-00004660: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-00004670: 6620 6861 726d 6f6e 6963 5f72 6567 7265  f harmonic_regre
-00004680: 7373 696f 6e5f 6e65 7874 5f76 616c 7565  ssion_next_value
-00004690: 5f62 795f 696e 6465 7828 6e75 6d65 7269  _by_index(numeri
-000046a0: 635f 7365 7175 656e 6365 3a20 4c69 7374  c_sequence: List
-000046b0: 5b69 6e74 5d2c 2066 7265 7175 656e 6379  [int], frequency
-000046c0: 3a20 666c 6f61 7420 3d20 312e 3029 202d  : float = 1.0) -
-000046d0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-000046e0: 2222 0a20 2020 2020 2020 2050 7265 6469  "".        Predi
-000046f0: 6374 7320 7468 6520 6e65 7874 2076 616c  cts the next val
-00004700: 7565 2069 6e20 6120 7365 7175 656e 6365  ue in a sequence
-00004710: 2075 7369 6e67 2068 6172 6d6f 6e69 6320   using harmonic 
-00004720: 7265 6772 6573 7369 6f6e 2e0a 0a20 2020  regression...   
-00004730: 2020 2020 2048 6172 6d6f 6e69 6320 7265       Harmonic re
-00004740: 6772 6573 7369 6f6e 2069 6e76 6f6c 7665  gression involve
-00004750: 7320 6669 7474 696e 6720 6120 6d6f 6465  s fitting a mode
-00004760: 6c20 7769 7468 2073 696e 6520 616e 6420  l with sine and 
-00004770: 636f 7369 6e65 2063 6f6d 706f 6e65 6e74  cosine component
-00004780: 7320 746f 2063 6170 7475 7265 0a20 2020  s to capture.   
-00004790: 2020 2020 2070 6572 696f 6469 6320 7061       periodic pa
-000047a0: 7474 6572 6e73 2069 6e20 7468 6520 6461  tterns in the da
-000047b0: 7461 2e20 5468 6973 2066 756e 6374 696f  ta. This functio
-000047c0: 6e20 7072 6564 6963 7473 2074 6865 206e  n predicts the n
-000047d0: 6578 7420 7661 6c75 6520 696e 2061 2067  ext value in a g
-000047e0: 6976 656e 2073 6571 7565 6e63 650a 2020  iven sequence.  
-000047f0: 2020 2020 2020 6f66 206e 756d 6265 7273        of numbers
-00004800: 2062 7920 6669 7474 696e 6720 6120 6861   by fitting a ha
-00004810: 726d 6f6e 6963 206d 6f64 656c 2074 6f20  rmonic model to 
-00004820: 7468 6520 7365 7175 656e 6365 2e0a 0a20  the sequence... 
-00004830: 2020 2020 2020 203a 7061 7261 6d20 6e75         :param nu
-00004840: 6d65 7269 635f 7365 7175 656e 6365 3a20  meric_sequence: 
-00004850: 4120 6c69 7374 206f 7220 7365 7175 656e  A list or sequen
-00004860: 6365 206f 6620 6e75 6d62 6572 7320 746f  ce of numbers to
-00004870: 206d 6f64 656c 2e0a 2020 2020 2020 2020   model..        
-00004880: 3a70 6172 616d 2066 7265 7175 656e 6379  :param frequency
-00004890: 3a20 5468 6520 6672 6571 7565 6e63 7920  : The frequency 
-000048a0: 6f66 2074 6865 2070 6572 696f 6469 6320  of the periodic 
-000048b0: 636f 6d70 6f6e 656e 7420 746f 206d 6f64  component to mod
-000048c0: 656c 2e0a 2020 2020 2020 2020 3a72 6574  el..        :ret
-000048d0: 7572 6e3a 2054 6865 2070 7265 6469 6374  urn: The predict
-000048e0: 6564 206e 6578 7420 7661 6c75 6520 696e  ed next value in
-000048f0: 2074 6865 2073 6571 7565 6e63 6520 6173   the sequence as
-00004900: 2061 6e20 696e 7465 6765 722e 0a20 2020   an integer..   
-00004910: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00004920: 2023 2043 6f6e 7665 7274 2074 6865 206e   # Convert the n
-00004930: 756d 6572 6963 2073 6571 7565 6e63 6520  umeric sequence 
-00004940: 696e 746f 2061 206e 756d 7079 2061 7272  into a numpy arr
-00004950: 6179 0a20 2020 2020 2020 2064 6174 6120  ay.        data 
-00004960: 3d20 6e70 2e61 7272 6179 286e 756d 6572  = np.array(numer
-00004970: 6963 5f73 6571 7565 6e63 6529 2e72 6573  ic_sequence).res
-00004980: 6861 7065 282d 312c 2031 290a 0a20 2020  hape(-1, 1)..   
-00004990: 2020 2020 2023 2043 7265 6174 6520 616e       # Create an
-000049a0: 2061 7272 6179 2072 6570 7265 7365 6e74   array represent
-000049b0: 696e 6720 7469 6d65 206f 7220 7468 6520  ing time or the 
-000049c0: 696e 6465 7065 6e64 656e 7420 7661 7269  independent vari
-000049d0: 6162 6c65 0a20 2020 2020 2020 2069 6e64  able.        ind
-000049e0: 6578 203d 206e 702e 6172 7261 7928 7261  ex = np.array(ra
-000049f0: 6e67 6528 6c65 6e28 6461 7461 2929 292e  nge(len(data))).
-00004a00: 7265 7368 6170 6528 2d31 2c20 3129 0a0a  reshape(-1, 1)..
-00004a10: 2020 2020 2020 2020 2320 4765 6e65 7261          # Genera
-00004a20: 7465 2073 696e 6520 616e 6420 636f 7369  te sine and cosi
-00004a30: 6e65 2066 6561 7475 7265 7320 6261 7365  ne features base
-00004a40: 6420 6f6e 2074 6865 2074 696d 6520 6172  d on the time ar
-00004a50: 7261 7920 616e 6420 6769 7665 6e20 6672  ray and given fr
-00004a60: 6571 7565 6e63 790a 2020 2020 2020 2020  equency.        
-00004a70: 7369 6e65 5f66 6561 7475 7265 203d 206e  sine_feature = n
-00004a80: 702e 7369 6e28 3220 2a20 6e70 2e70 6920  p.sin(2 * np.pi 
-00004a90: 2a20 6672 6571 7565 6e63 7920 2a20 696e  * frequency * in
-00004aa0: 6465 7829 0a20 2020 2020 2020 2063 6f73  dex).        cos
-00004ab0: 696e 655f 6665 6174 7572 6520 3d20 6e70  ine_feature = np
-00004ac0: 2e63 6f73 2832 202a 206e 702e 7069 202a  .cos(2 * np.pi *
-00004ad0: 2066 7265 7175 656e 6379 202a 2069 6e64   frequency * ind
-00004ae0: 6578 290a 0a20 2020 2020 2020 2023 2043  ex)..        # C
-00004af0: 6f6d 6269 6e65 2073 696e 6520 616e 6420  ombine sine and 
-00004b00: 636f 7369 6e65 2066 6561 7475 7265 7320  cosine features 
-00004b10: 696e 746f 2061 2073 696e 676c 6520 6665  into a single fe
-00004b20: 6174 7572 6520 6d61 7472 6978 0a20 2020  ature matrix.   
-00004b30: 2020 2020 2066 6561 7475 7265 7320 3d20       features = 
-00004b40: 6e70 2e68 7374 6163 6b28 2873 696e 655f  np.hstack((sine_
-00004b50: 6665 6174 7572 652c 2063 6f73 696e 655f  feature, cosine_
-00004b60: 6665 6174 7572 6529 290a 0a20 2020 2020  feature))..     
-00004b70: 2020 2023 2043 7265 6174 6520 6120 4c69     # Create a Li
-00004b80: 6e65 6172 5265 6772 6573 7369 6f6e 206d  nearRegression m
-00004b90: 6f64 656c 2061 6e64 2066 6974 2069 7420  odel and fit it 
-00004ba0: 746f 2074 6865 2064 6174 6120 7769 7468  to the data with
-00004bb0: 2068 6172 6d6f 6e69 6320 6665 6174 7572   harmonic featur
-00004bc0: 6573 0a20 2020 2020 2020 206d 6f64 656c  es.        model
-00004bd0: 203d 204c 696e 6561 7252 6567 7265 7373   = LinearRegress
-00004be0: 696f 6e28 290a 2020 2020 2020 2020 6d6f  ion().        mo
-00004bf0: 6465 6c2e 6669 7428 6665 6174 7572 6573  del.fit(features
-00004c00: 2c20 6461 7461 290a 0a20 2020 2020 2020  , data)..       
-00004c10: 2023 2050 7265 6469 6374 2074 6865 206e   # Predict the n
-00004c20: 6578 7420 7661 6c75 6520 696e 2074 6865  ext value in the
-00004c30: 2073 6571 7565 6e63 6520 7573 696e 6720   sequence using 
-00004c40: 7468 6520 6669 7474 6564 206d 6f64 656c  the fitted model
-00004c50: 0a20 2020 2020 2020 206e 6578 745f 7469  .        next_ti
-00004c60: 6d65 5f70 6f69 6e74 203d 206e 702e 6172  me_point = np.ar
-00004c70: 7261 7928 5b5b 6c65 6e28 6461 7461 295d  ray([[len(data)]
-00004c80: 5d29 0a20 2020 2020 2020 206e 6578 745f  ]).        next_
-00004c90: 7369 6e65 5f66 6561 7475 7265 203d 206e  sine_feature = n
-00004ca0: 702e 7369 6e28 3220 2a20 6e70 2e70 6920  p.sin(2 * np.pi 
-00004cb0: 2a20 6672 6571 7565 6e63 7920 2a20 6e65  * frequency * ne
-00004cc0: 7874 5f74 696d 655f 706f 696e 7429 0a20  xt_time_point). 
-00004cd0: 2020 2020 2020 206e 6578 745f 636f 7369         next_cosi
-00004ce0: 6e65 5f66 6561 7475 7265 203d 206e 702e  ne_feature = np.
-00004cf0: 636f 7328 3220 2a20 6e70 2e70 6920 2a20  cos(2 * np.pi * 
-00004d00: 6672 6571 7565 6e63 7920 2a20 6e65 7874  frequency * next
-00004d10: 5f74 696d 655f 706f 696e 7429 0a20 2020  _time_point).   
-00004d20: 2020 2020 206e 6578 745f 6665 6174 7572       next_featur
-00004d30: 6573 203d 206e 702e 6873 7461 636b 2828  es = np.hstack((
-00004d40: 6e65 7874 5f73 696e 655f 6665 6174 7572  next_sine_featur
-00004d50: 652c 206e 6578 745f 636f 7369 6e65 5f66  e, next_cosine_f
-00004d60: 6561 7475 7265 2929 0a0a 2020 2020 2020  eature))..      
-00004d70: 2020 7072 6564 6963 7469 6f6e 203d 206d    prediction = m
-00004d80: 6f64 656c 2e70 7265 6469 6374 286e 6578  odel.predict(nex
-00004d90: 745f 6665 6174 7572 6573 295b 305d 5b30  t_features)[0][0
-00004da0: 5d0a 0a20 2020 2020 2020 2023 2052 6574  ]..        # Ret
-00004db0: 7572 6e20 7468 6520 7072 6564 6963 7465  urn the predicte
-00004dc0: 6420 7661 6c75 6520 6173 2061 6e20 696e  d value as an in
-00004dd0: 7465 6765 720a 2020 2020 2020 2020 7265  teger.        re
-00004de0: 7475 726e 2072 6f75 6e64 2870 7265 6469  turn round(predi
-00004df0: 6374 696f 6e29 0a0a 2020 2020 4073 7461  ction)..    @sta
-00004e00: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-00004e10: 6620 7261 6e64 6f6d 5f66 6f72 6573 745f  f random_forest_
-00004e20: 7265 6772 6573 736f 725f 7472 616e 7366  regressor_transf
-00004e30: 6f72 6d65 7228 0a20 2020 2020 2020 2020  ormer(.         
-00004e40: 2020 206e 756d 6572 6963 5f73 6571 7565     numeric_seque
-00004e50: 6e63 653a 204c 6973 745b 696e 745d 2c0a  nce: List[int],.
-00004e60: 2020 2020 2020 2020 2020 2020 726f 6c6c              roll
-00004e70: 696e 675f 7369 7a65 3a20 696e 742c 0a20  ing_size: int,. 
-00004e80: 2020 2020 2020 2020 2020 2077 6172 6d5f             warm_
-00004e90: 7374 6172 743a 2062 6f6f 6c20 3d20 4661  start: bool = Fa
-00004ea0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00004eb0: 2072 616e 646f 6d5f 7374 6174 653a 2069   random_state: i
-00004ec0: 6e74 203d 2031 322c 0a20 2020 2020 2020  nt = 12,.       
-00004ed0: 2020 2020 2070 6172 616d 5f64 6973 7472       param_distr
-00004ee0: 6962 7574 696f 6e73 3a20 4f70 7469 6f6e  ibutions: Option
-00004ef0: 616c 5b44 6963 745d 203d 204e 6f6e 652c  al[Dict] = None,
-00004f00: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00004f10: 616d 5f6f 7665 7272 6964 6573 3a20 4f70  am_overrides: Op
-00004f20: 7469 6f6e 616c 5b44 6963 745d 203d 204e  tional[Dict] = N
-00004f30: 6f6e 650a 2020 2020 2920 2d3e 2066 6c6f  one.    ) -> flo
-00004f40: 6174 3a0a 2020 2020 2020 2020 7472 6169  at:.        trai
-00004f50: 6e5f 782c 2074 7261 696e 5f79 203d 2043  n_x, train_y = C
-00004f60: 616c 6375 6c61 7465 5574 696c 2e67 656e  alculateUtil.gen
-00004f70: 6572 6174 655f 6461 7461 7365 7473 5f77  erate_datasets_w
-00004f80: 6974 685f 726f 6c6c 696e 675f 7369 7a65  ith_rolling_size
-00004f90: 280a 2020 2020 2020 2020 2020 2020 6461  (.            da
-00004fa0: 7461 3d6e 756d 6572 6963 5f73 6571 7565  ta=numeric_seque
-00004fb0: 6e63 652c 2072 6f6c 6c69 6e67 5f73 697a  nce, rolling_siz
-00004fc0: 653d 726f 6c6c 696e 675f 7369 7a65 0a20  e=rolling_size. 
-00004fd0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00004fe0: 2020 2320 436f 6e76 6572 7420 6c69 7374    # Convert list
-00004ff0: 7320 746f 206e 756d 7079 2061 7272 6179  s to numpy array
-00005000: 7320 666f 7220 636f 6d70 6174 6962 696c  s for compatibil
-00005010: 6974 7920 7769 7468 2073 6369 6b69 742d  ity with scikit-
-00005020: 6c65 6172 6e0a 2020 2020 2020 2020 696e  learn.        in
-00005030: 7075 745f 7820 3d20 6e70 2e61 7272 6179  put_x = np.array
-00005040: 2874 7261 696e 5f78 290a 2020 2020 2020  (train_x).      
-00005050: 2020 6f75 7470 7574 5f79 203d 206e 702e    output_y = np.
-00005060: 6172 7261 7928 7472 6169 6e5f 7929 0a0a  array(train_y)..
-00005070: 2020 2020 2020 2020 2320 5363 616c 6520          # Scale 
-00005080: 7468 6520 6665 6174 7572 6573 2074 6f20  the features to 
-00005090: 6e6f 726d 616c 697a 6520 6461 7461 0a20  normalize data. 
-000050a0: 2020 2020 2020 2073 6361 6c65 7220 3d20         scaler = 
-000050b0: 5374 616e 6461 7264 5363 616c 6572 2829  StandardScaler()
-000050c0: 0a20 2020 2020 2020 2069 6e70 7574 5f78  .        input_x
-000050d0: 5f73 6361 6c65 6420 3d20 7363 616c 6572  _scaled = scaler
-000050e0: 2e66 6974 5f74 7261 6e73 666f 726d 2869  .fit_transform(i
-000050f0: 6e70 7574 5f78 290a 0a20 2020 2020 2020  nput_x)..       
-00005100: 2023 2049 6e69 7469 616c 697a 6520 616e   # Initialize an
-00005110: 6420 7472 6169 6e20 7468 6520 5261 6e64  d train the Rand
-00005120: 6f6d 2046 6f72 6573 7420 5265 6772 6573  om Forest Regres
-00005130: 736f 720a 2020 2020 2020 2020 6d6f 6465  sor.        mode
-00005140: 6c20 3d20 5261 6e64 6f6d 466f 7265 7374  l = RandomForest
-00005150: 5265 6772 6573 736f 7228 7761 726d 5f73  Regressor(warm_s
-00005160: 7461 7274 3d77 6172 6d5f 7374 6172 742c  tart=warm_start,
-00005170: 2072 616e 646f 6d5f 7374 6174 653d 7261   random_state=ra
-00005180: 6e64 6f6d 5f73 7461 7465 290a 2020 2020  ndom_state).    
-00005190: 2020 2020 6966 2070 6172 616d 5f64 6973      if param_dis
-000051a0: 7472 6962 7574 696f 6e73 3a0a 2020 2020  tributions:.    
-000051b0: 2020 2020 2020 2020 7061 7261 6d5f 6f76          param_ov
-000051c0: 6572 7269 6465 7320 3d20 7061 7261 6d5f  errides = param_
-000051d0: 6f76 6572 7269 6465 7320 6f72 207b 7d0a  overrides or {}.
-000051e0: 2020 2020 2020 2020 2020 2020 7261 6e64              rand
-000051f0: 6f6d 5f73 6561 7263 6820 3d20 5261 6e64  om_search = Rand
-00005200: 6f6d 697a 6564 5365 6172 6368 4356 2865  omizedSearchCV(e
-00005210: 7374 696d 6174 6f72 3d6d 6f64 656c 2c20  stimator=model, 
-00005220: 7061 7261 6d5f 6469 7374 7269 6275 7469  param_distributi
-00005230: 6f6e 733d 7061 7261 6d5f 6469 7374 7269  ons=param_distri
-00005240: 6275 7469 6f6e 732c 0a20 2020 2020 2020  butions,.       
-00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005270: 2020 2020 2020 2020 2a2a 7061 7261 6d5f          **param_
-00005280: 6f76 6572 7269 6465 7329 0a20 2020 2020  overrides).     
-00005290: 2020 2020 2020 2072 616e 646f 6d5f 7365         random_se
-000052a0: 6172 6368 2e66 6974 2869 6e70 7574 5f78  arch.fit(input_x
-000052b0: 5f73 6361 6c65 642c 206f 7574 7075 745f  _scaled, output_
-000052c0: 7929 0a20 2020 2020 2020 2020 2020 206d  y).            m
-000052d0: 6f64 656c 203d 2052 616e 646f 6d46 6f72  odel = RandomFor
-000052e0: 6573 7452 6567 7265 7373 6f72 2877 6172  estRegressor(war
-000052f0: 6d5f 7374 6172 743d 7761 726d 5f73 7461  m_start=warm_sta
-00005300: 7274 2c20 7261 6e64 6f6d 5f73 7461 7465  rt, random_state
-00005310: 3d72 616e 646f 6d5f 7374 6174 652c 0a20  =random_state,. 
-00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 2020 2020 202a 2a72 616e 646f           **rando
-00005350: 6d5f 7365 6172 6368 2e62 6573 745f 7061  m_search.best_pa
-00005360: 7261 6d73 5f29 0a0a 2020 2020 2020 2020  rams_)..        
-00005370: 6d6f 6465 6c5f 7069 706c 696e 6520 3d20  model_pipline = 
-00005380: 5069 7065 6c69 6e65 285b 0a20 2020 2020  Pipeline([.     
-00005390: 2020 2020 2020 2028 2770 7265 6469 6374         ('predict
-000053a0: 696f 6e5f 7472 616e 7366 6f72 6d65 7227  ion_transformer'
-000053b0: 2c20 5261 6e64 6f6d 466f 7265 7374 5265  , RandomForestRe
-000053c0: 6772 6573 736f 7254 7261 6e73 666f 726d  gressorTransform
-000053d0: 6572 286d 6f64 656c 2929 2c0a 2020 2020  er(model)),.    
-000053e0: 2020 2020 2020 2020 2827 7072 6564 6963          ('predic
-000053f0: 7469 6f6e 5f74 7261 6e73 666f 726d 6572  tion_transformer
-00005400: 5f74 776f 272c 2052 616e 646f 6d46 6f72  _two', RandomFor
-00005410: 6573 7452 6567 7265 7373 6f72 2877 6172  estRegressor(war
-00005420: 6d5f 7374 6172 743d 7761 726d 5f73 7461  m_start=warm_sta
-00005430: 7274 2c20 7261 6e64 6f6d 5f73 7461 7465  rt, random_state
-00005440: 3d72 616e 646f 6d5f 7374 6174 6529 292c  =random_state)),
-00005450: 0a20 2020 2020 2020 2020 2020 2023 2028  .            # (
-00005460: 2770 6f6c 795f 6665 6174 7572 6573 272c  'poly_features',
-00005470: 2050 6f6c 796e 6f6d 6961 6c46 6561 7475   PolynomialFeatu
-00005480: 7265 7328 6465 6772 6565 3d32 2929 2c0a  res(degree=2)),.
-00005490: 2020 2020 2020 2020 2020 2020 2320 2827              # ('
-000054a0: 6c69 6e65 6172 5f72 6567 7265 7373 696f  linear_regressio
-000054b0: 6e27 2c20 4c69 6e65 6172 5265 6772 6573  n', LinearRegres
-000054c0: 7369 6f6e 2829 290a 2020 2020 2020 2020  sion()).        
-000054d0: 5d29 0a20 2020 2020 2020 206d 6f64 656c  ]).        model
-000054e0: 5f70 6970 6c69 6e65 2e66 6974 2869 6e70  _pipline.fit(inp
-000054f0: 7574 5f78 5f73 6361 6c65 642c 206f 7574  ut_x_scaled, out
-00005500: 7075 745f 7929 0a0a 2020 2020 2020 2020  put_y)..        
-00005510: 2320 5072 6570 6172 6520 7468 6520 6c61  # Prepare the la
-00005520: 7374 2072 6f6c 6c69 6e67 2077 696e 646f  st rolling windo
-00005530: 7720 6f66 2064 6174 6120 666f 7220 7072  w of data for pr
-00005540: 6564 6963 7469 6f6e 0a20 2020 2020 2020  ediction.       
-00005550: 2074 6573 745f 7820 3d20 6e70 2e61 7272   test_x = np.arr
-00005560: 6179 285b 6e75 6d65 7269 635f 7365 7175  ay([numeric_sequ
-00005570: 656e 6365 5b2d 726f 6c6c 696e 675f 7369  ence[-rolling_si
-00005580: 7a65 3a5d 5d29 0a20 2020 2020 2020 2074  ze:]]).        t
-00005590: 6573 745f 785f 7363 616c 6564 203d 2073  est_x_scaled = s
-000055a0: 6361 6c65 722e 7472 616e 7366 6f72 6d28  caler.transform(
-000055b0: 7465 7374 5f78 290a 0a20 2020 2020 2020  test_x)..       
-000055c0: 2023 2050 7265 6469 6374 696e 6720 7468   # Predicting th
-000055d0: 6520 6e65 7874 2076 616c 7565 0a20 2020  e next value.   
-000055e0: 2020 2020 2070 7265 645f 7920 3d20 6d6f       pred_y = mo
-000055f0: 6465 6c5f 7069 706c 696e 652e 7072 6564  del_pipline.pred
-00005600: 6963 7428 7465 7374 5f78 5f73 6361 6c65  ict(test_x_scale
-00005610: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
-00005620: 6e20 7072 6564 5f79 0a0a 2020 2020 4073  n pred_y..    @s
-00005630: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00005640: 6465 6620 7261 6e64 6f6d 5f66 6f72 6573  def random_fores
-00005650: 745f 7265 6772 6573 736f 725f 6e65 7874  t_regressor_next
-00005660: 5f76 616c 7565 280a 2020 2020 2020 2020  _value(.        
-00005670: 2020 2020 6e75 6d65 7269 635f 7365 7175      numeric_sequ
-00005680: 656e 6365 3a20 4c69 7374 5b69 6e74 5d2c  ence: List[int],
-00005690: 0a20 2020 2020 2020 2020 2020 2072 6f6c  .            rol
-000056a0: 6c69 6e67 5f73 697a 653a 2069 6e74 2c0a  ling_size: int,.
-000056b0: 2020 2020 2020 2020 2020 2020 7761 726d              warm
-000056c0: 5f73 7461 7274 3a20 626f 6f6c 203d 2046  _start: bool = F
-000056d0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-000056e0: 2020 7261 6e64 6f6d 5f73 7461 7465 3a20    random_state: 
-000056f0: 696e 7420 3d20 3132 2c0a 2020 2020 2020  int = 12,.      
-00005700: 2020 2020 2020 7061 7261 6d5f 6469 7374        param_dist
-00005710: 7269 6275 7469 6f6e 733a 204f 7074 696f  ributions: Optio
-00005720: 6e61 6c5b 4469 6374 5d20 3d20 4e6f 6e65  nal[Dict] = None
-00005730: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
-00005740: 7261 6d5f 6f76 6572 7269 6465 733a 204f  ram_overrides: O
-00005750: 7074 696f 6e61 6c5b 4469 6374 5d20 3d20  ptional[Dict] = 
-00005760: 4e6f 6e65 0a20 2020 2029 202d 3e20 666c  None.    ) -> fl
-00005770: 6f61 743a 0a20 2020 2020 2020 2022 2222  oat:.        """
-00005780: 0a20 2020 2020 2020 2050 7265 6469 6374  .        Predict
-00005790: 7320 7468 6520 6e65 7874 2076 616c 7565  s the next value
-000057a0: 2069 6e20 6120 6e75 6d65 7269 6320 7365   in a numeric se
-000057b0: 7175 656e 6365 2075 7369 6e67 2061 2052  quence using a R
-000057c0: 616e 646f 6d20 466f 7265 7374 2052 6567  andom Forest Reg
-000057d0: 7265 7373 6f72 206d 6f64 656c 2e0a 0a20  ressor model... 
-000057e0: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-000057f0: 6f64 2075 7365 7320 6120 5261 6e64 6f6d  od uses a Random
-00005800: 2046 6f72 6573 7420 5265 6772 6573 736f   Forest Regresso
-00005810: 7220 746f 2070 7265 6469 6374 2074 6865  r to predict the
-00005820: 206e 6578 7420 7661 6c75 6520 696e 2061   next value in a
-00005830: 2073 6571 7565 6e63 6520 6261 7365 6420   sequence based 
-00005840: 6f6e 0a20 2020 2020 2020 2074 6865 2076  on.        the v
-00005850: 616c 7565 7320 696e 2061 2072 6f6c 6c69  alues in a rolli
-00005860: 6e67 2077 696e 646f 772e 2054 6865 2073  ng window. The s
-00005870: 6571 7565 6e63 6520 6973 2066 6972 7374  equence is first
-00005880: 2074 7261 6e73 666f 726d 6564 2069 6e74   transformed int
-00005890: 6f20 6120 6461 7461 7365 7420 7375 6974  o a dataset suit
-000058a0: 6162 6c65 2066 6f72 0a20 2020 2020 2020  able for.       
-000058b0: 2072 6567 7265 7373 696f 6e20 6279 2063   regression by c
-000058c0: 7265 6174 696e 6720 6f76 6572 6c61 7070  reating overlapp
-000058d0: 696e 6720 7769 6e64 6f77 7320 6f66 2073  ing windows of s
-000058e0: 7065 6369 6669 6564 2073 697a 652e 0a0a  pecified size...
-000058f0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00005900: 2020 2020 2020 2020 2020 6e75 6d65 7269            numeri
-00005910: 635f 7365 7175 656e 6365 2028 4c69 7374  c_sequence (List
-00005920: 5b69 6e74 5d29 3a20 5468 6520 6c69 7374  [int]): The list
-00005930: 206f 6620 696e 7465 6765 7273 2072 6570   of integers rep
-00005940: 7265 7365 6e74 696e 6720 7468 6520 7365  resenting the se
-00005950: 7175 656e 6365 2e0a 2020 2020 2020 2020  quence..        
+000000f0: 7420 6a73 6f6e 0a69 6d70 6f72 7420 7079  t json.import py
+00000100: 7774 0a69 6d70 6f72 7420 6461 7465 7469  wt.import dateti
+00000110: 6d65 0a69 6d70 6f72 7420 6c6f 6767 696e  me.import loggin
+00000120: 670a 696d 706f 7274 206c 6f67 6769 6e67  g.import logging
+00000130: 2e68 616e 646c 6572 730a 6672 6f6d 2061  .handlers.from a
+00000140: 6263 2069 6d70 6f72 7420 4142 432c 2061  bc import ABC, a
+00000150: 6273 7472 6163 746d 6574 686f 640a 6672  bstractmethod.fr
+00000160: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000170: 2049 7465 7261 626c 652c 204c 6973 742c   Iterable, List,
+00000180: 2054 7570 6c65 2c20 416e 792c 204f 7074   Tuple, Any, Opt
+00000190: 696f 6e61 6c2c 2055 6e69 6f6e 2c20 5365  ional, Union, Se
+000001a0: 742c 2044 6963 740a 696d 706f 7274 2072  t, Dict.import r
+000001b0: 616e 646f 6d0a 696d 706f 7274 206e 756d  andom.import num
+000001c0: 7079 2061 7320 6e70 0a69 6d70 6f72 7420  py as np.import 
+000001d0: 7061 6e64 6173 2061 7320 7064 0a66 726f  pandas as pd.fro
+000001e0: 6d20 706d 6461 7269 6d61 2069 6d70 6f72  m pmdarima impor
+000001f0: 7420 6175 746f 5f61 7269 6d61 0a66 726f  t auto_arima.fro
+00000200: 6d20 7365 6c65 6e69 756d 2069 6d70 6f72  m selenium impor
+00000210: 7420 7765 6264 7269 7665 720a 6672 6f6d  t webdriver.from
+00000220: 2073 6b6c 6561 726e 2e70 6970 656c 696e   sklearn.pipelin
+00000230: 6520 696d 706f 7274 2050 6970 656c 696e  e import Pipelin
+00000240: 650a 6672 6f6d 2073 6b6c 6561 726e 2e62  e.from sklearn.b
+00000250: 6173 6520 696d 706f 7274 2042 6173 6545  ase import BaseE
+00000260: 7374 696d 6174 6f72 2c20 5472 616e 7366  stimator, Transf
+00000270: 6f72 6d65 724d 6978 696e 0a66 726f 6d20  ormerMixin.from 
+00000280: 736b 6c65 6172 6e2e 7069 7065 6c69 6e65  sklearn.pipeline
+00000290: 2069 6d70 6f72 7420 6d61 6b65 5f70 6970   import make_pip
+000002a0: 656c 696e 650a 6672 6f6d 2073 6b6c 6561  eline.from sklea
+000002b0: 726e 2e70 7265 7072 6f63 6573 7369 6e67  rn.preprocessing
+000002c0: 2069 6d70 6f72 7420 5374 616e 6461 7264   import Standard
+000002d0: 5363 616c 6572 0a66 726f 6d20 736b 6c65  Scaler.from skle
+000002e0: 6172 6e2e 656e 7365 6d62 6c65 2069 6d70  arn.ensemble imp
+000002f0: 6f72 7420 5261 6e64 6f6d 466f 7265 7374  ort RandomForest
+00000300: 5265 6772 6573 736f 720a 6672 6f6d 2073  Regressor.from s
+00000310: 6b6c 6561 726e 2e6c 696e 6561 725f 6d6f  klearn.linear_mo
+00000320: 6465 6c20 696d 706f 7274 204c 696e 6561  del import Linea
+00000330: 7252 6567 7265 7373 696f 6e0a 6672 6f6d  rRegression.from
+00000340: 2073 6b6c 6561 726e 2e70 7265 7072 6f63   sklearn.preproc
+00000350: 6573 7369 6e67 2069 6d70 6f72 7420 506f  essing import Po
+00000360: 6c79 6e6f 6d69 616c 4665 6174 7572 6573  lynomialFeatures
+00000370: 0a66 726f 6d20 736b 6c65 6172 6e2e 6d6f  .from sklearn.mo
+00000380: 6465 6c5f 7365 6c65 6374 696f 6e20 696d  del_selection im
+00000390: 706f 7274 2052 616e 646f 6d69 7a65 6453  port RandomizedS
+000003a0: 6561 7263 6843 560a 6672 6f6d 2073 656c  earchCV.from sel
+000003b0: 656e 6975 6d2e 7765 6264 7269 7665 722e  enium.webdriver.
+000003c0: 636f 6d6d 6f6e 2e62 7920 696d 706f 7274  common.by import
+000003d0: 2042 790a 6672 6f6d 2073 656c 656e 6975   By.from seleniu
+000003e0: 6d2e 7765 6264 7269 7665 722e 7375 7070  m.webdriver.supp
+000003f0: 6f72 742e 7569 2069 6d70 6f72 7420 5765  ort.ui import We
+00000400: 6244 7269 7665 7257 6169 740a 6672 6f6d  bDriverWait.from
+00000410: 2073 656c 656e 6975 6d2e 7765 6264 7269   selenium.webdri
+00000420: 7665 722e 7375 7070 6f72 7420 696d 706f  ver.support impo
+00000430: 7274 2065 7870 6563 7465 645f 636f 6e64  rt expected_cond
+00000440: 6974 696f 6e73 2061 7320 4543 0a0a 0a63  itions as EC...c
+00000450: 6c61 7373 2049 4f55 7469 6c3a 0a20 2020  lass IOUtil:.   
+00000460: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00000470: 2020 6465 6620 6765 745f 6c6f 6767 6572    def get_logger
+00000480: 280a 2020 2020 2020 2020 2020 2020 636c  (.            cl
+00000490: 732c 0a20 2020 2020 2020 2020 2020 206c  s,.            l
+000004a0: 6f67 5f66 696c 653a 2073 7472 203d 204e  og_file: str = N
+000004b0: 6f6e 650a 2020 2020 2920 2d3e 206c 6f67  one.    ) -> log
+000004c0: 6769 6e67 2e4c 6f67 6765 723a 0a20 2020  ging.Logger:.   
+000004d0: 2020 2020 2023 2043 686f 6f73 6520 6120       # Choose a 
+000004e0: 756e 6971 7565 206c 6f67 6765 7220 6e61  unique logger na
+000004f0: 6d65 2062 6173 6564 206f 6e20 7468 6520  me based on the 
+00000500: 6c6f 675f 6669 6c65 2061 7267 756d 656e  log_file argumen
+00000510: 740a 2020 2020 2020 2020 6c6f 6767 6572  t.        logger
+00000520: 5f6e 616d 6520 3d20 6c6f 675f 6669 6c65  _name = log_file
+00000530: 2069 6620 6c6f 675f 6669 6c65 2069 7320   if log_file is 
+00000540: 6e6f 7420 4e6f 6e65 2065 6c73 6520 2764  not None else 'd
+00000550: 6566 6175 6c74 5f6c 6f67 6765 7227 0a20  efault_logger'. 
+00000560: 2020 2020 2020 2023 2047 6574 2074 6865         # Get the
+00000570: 206c 6f67 6765 7220 696e 7374 616e 6365   logger instance
+00000580: 2062 7920 6e61 6d65 0a20 2020 2020 2020   by name.       
+00000590: 206c 6f67 6765 7220 3d20 6c6f 6767 696e   logger = loggin
+000005a0: 672e 6765 744c 6f67 6765 7228 6c6f 6767  g.getLogger(logg
+000005b0: 6572 5f6e 616d 6529 0a0a 2020 2020 2020  er_name)..      
+000005c0: 2020 2320 4368 6563 6b20 6966 2074 6865    # Check if the
+000005d0: 206c 6f67 6765 7220 616c 7265 6164 7920   logger already 
+000005e0: 6861 7320 6861 6e64 6c65 7273 2074 6f20  has handlers to 
+000005f0: 7072 6576 656e 7420 6164 6469 6e67 2074  prevent adding t
+00000600: 6865 6d20 6167 6169 6e0a 2020 2020 2020  hem again.      
+00000610: 2020 6966 206e 6f74 206c 6f67 6765 722e    if not logger.
+00000620: 6861 6e64 6c65 7273 3a0a 2020 2020 2020  handlers:.      
+00000630: 2020 2020 2020 6966 206c 6f67 5f66 696c        if log_fil
+00000640: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+00000650: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
+00000660: 6669 6775 7261 7469 6f6e 2066 6f72 206c  figuration for l
+00000670: 6f67 6769 6e67 2074 6f20 7468 6520 7465  ogging to the te
+00000680: 726d 696e 616c 0a20 2020 2020 2020 2020  rminal.         
+00000690: 2020 2020 2020 2023 206c 6f67 5f66 6f72         # log_for
+000006a0: 6d61 7420 3d20 2725 2861 7363 7469 6d65  mat = '%(asctime
+000006b0: 2973 205b 2528 6c65 7665 6c6e 616d 6529  )s [%(levelname)
+000006c0: 735d 203c 2528 6c69 6e65 6e6f 2964 3e20  s] <%(lineno)d> 
+000006d0: 2528 6675 6e63 4e61 6d65 2973 3a20 2528  %(funcName)s: %(
+000006e0: 6d65 7373 6167 6529 7327 0a20 2020 2020  message)s'.     
+000006f0: 2020 2020 2020 2020 2020 206c 6f67 5f66             log_f
+00000700: 6f72 6d61 7420 3d20 2725 286d 6573 7361  ormat = '%(messa
+00000710: 6765 2973 270a 2020 2020 2020 2020 2020  ge)s'.          
+00000720: 2020 2020 2020 6861 6e64 6c65 7220 3d20        handler = 
+00000730: 6c6f 6767 696e 672e 5374 7265 616d 4861  logging.StreamHa
+00000740: 6e64 6c65 7228 7379 732e 7374 646f 7574  ndler(sys.stdout
+00000750: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00000760: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00000770: 2020 2020 2320 436f 6e66 6967 7572 6174      # Configurat
+00000780: 696f 6e20 666f 7220 6c6f 6767 696e 6720  ion for logging 
+00000790: 746f 2061 2066 696c 6520 7769 7468 2072  to a file with r
+000007a0: 6f74 6174 696f 6e20 6174 206d 6964 6e69  otation at midni
+000007b0: 6768 740a 2020 2020 2020 2020 2020 2020  ght.            
+000007c0: 2020 2020 6c6f 675f 666f 726d 6174 203d      log_format =
+000007d0: 2028 2725 2861 7363 7469 6d65 2973 205b   ('%(asctime)s [
+000007e0: 2528 6c65 7665 6c6e 616d 6529 735d 2025  %(levelname)s] %
+000007f0: 2870 726f 6365 7373 2964 2025 2874 6872  (process)d %(thr
+00000800: 6561 6429 6420 270a 2020 2020 2020 2020  ead)d '.        
+00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000820: 2020 2020 2020 2725 2866 696c 656e 616d        '%(filenam
+00000830: 6529 7320 3c25 286c 696e 656e 6f29 643e  e)s <%(lineno)d>
+00000840: 2025 2866 756e 634e 616d 6529 733a 2025   %(funcName)s: %
+00000850: 286d 6573 7361 6765 2973 2729 0a20 2020  (message)s').   
+00000860: 2020 2020 2020 2020 2020 2020 2068 616e               han
+00000870: 646c 6572 203d 206c 6f67 6769 6e67 2e68  dler = logging.h
+00000880: 616e 646c 6572 732e 5469 6d65 6452 6f74  andlers.TimedRot
+00000890: 6174 696e 6746 696c 6548 616e 646c 6572  atingFileHandler
+000008a0: 286c 6f67 5f66 696c 652c 2077 6865 6e3d  (log_file, when=
+000008b0: 276d 6964 6e69 6768 7427 2c20 6261 636b  'midnight', back
+000008c0: 7570 436f 756e 743d 3729 0a0a 2020 2020  upCount=7)..    
+000008d0: 2020 2020 2020 2020 2320 5365 7420 7468          # Set th
+000008e0: 6520 666f 726d 6174 7465 7220 666f 7220  e formatter for 
+000008f0: 7468 6520 6861 6e64 6c65 720a 2020 2020  the handler.    
+00000900: 2020 2020 2020 2020 666f 726d 6174 7465          formatte
+00000910: 7220 3d20 6c6f 6767 696e 672e 466f 726d  r = logging.Form
+00000920: 6174 7465 7228 6c6f 675f 666f 726d 6174  atter(log_format
+00000930: 290a 2020 2020 2020 2020 2020 2020 6861  ).            ha
+00000940: 6e64 6c65 722e 7365 7446 6f72 6d61 7474  ndler.setFormatt
+00000950: 6572 2866 6f72 6d61 7474 6572 290a 0a20  er(formatter).. 
+00000960: 2020 2020 2020 2020 2020 2023 204f 7074             # Opt
+00000970: 696f 6e61 6c6c 7920 7365 7420 6120 6469  ionally set a di
+00000980: 6666 6572 656e 7420 6c6f 6720 6c65 7665  fferent log leve
+00000990: 6c20 666f 7220 7468 6520 6861 6e64 6c65  l for the handle
+000009a0: 720a 2020 2020 2020 2020 2020 2020 6861  r.            ha
+000009b0: 6e64 6c65 722e 7365 744c 6576 656c 286c  ndler.setLevel(l
+000009c0: 6f67 6769 6e67 2e49 4e46 4f29 0a0a 2020  ogging.INFO)..  
+000009d0: 2020 2020 2020 2020 2020 2320 4164 6420            # Add 
+000009e0: 7468 6520 6861 6e64 6c65 7220 746f 2074  the handler to t
+000009f0: 6865 206c 6f67 6765 720a 2020 2020 2020  he logger.      
+00000a00: 2020 2020 2020 6c6f 6767 6572 2e61 6464        logger.add
+00000a10: 4861 6e64 6c65 7228 6861 6e64 6c65 7229  Handler(handler)
+00000a20: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
+00000a30: 6574 2074 6865 206c 6f67 206c 6576 656c  et the log level
+00000a40: 2066 6f72 2074 6865 206c 6f67 6765 720a   for the logger.
+00000a50: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00000a60: 6572 2e73 6574 4c65 7665 6c28 6c6f 6767  er.setLevel(logg
+00000a70: 696e 672e 494e 464f 290a 0a20 2020 2020  ing.INFO)..     
+00000a80: 2020 2023 2052 6574 7572 6e20 7468 6520     # Return the 
+00000a90: 636f 6e66 6967 7572 6564 206c 6f67 6765  configured logge
+00000aa0: 720a 2020 2020 2020 2020 7265 7475 726e  r.        return
+00000ab0: 206c 6f67 6765 720a 0a20 2020 2040 636c   logger..    @cl
+00000ac0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00000ad0: 6620 6465 7461 696c 5f6c 6f67 2863 6c73  f detail_log(cls
+00000ae0: 3a20 416e 792c 2061 7070 5f6c 6f67 3a20  : Any, app_log: 
+00000af0: 416e 792c 2073 686f 775f 6465 7461 696c  Any, show_detail
+00000b00: 733a 204f 7074 696f 6e61 6c5b 7374 725d  s: Optional[str]
+00000b10: 203d 204e 6f6e 652c 202a 2a6b 7761 7267   = None, **kwarg
+00000b20: 733a 2041 6e79 2920 2d3e 204e 6f6e 653a  s: Any) -> None:
+00000b30: 0a20 2020 2020 2020 2069 6620 7368 6f77  .        if show
+00000b40: 5f64 6574 6169 6c73 2069 7320 6e6f 7420  _details is not 
+00000b50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00000b60: 2020 6465 7461 696c 5f6d 6573 7361 6765    detail_message
+00000b70: 203d 206b 7761 7267 732e 6765 7428 7368   = kwargs.get(sh
+00000b80: 6f77 5f64 6574 6169 6c73 2c20 2727 290a  ow_details, '').
+00000b90: 2020 2020 2020 2020 2020 2020 6170 705f              app_
+00000ba0: 6c6f 672e 696e 666f 2864 6574 6169 6c5f  log.info(detail_
+00000bb0: 6d65 7373 6167 6529 0a0a 2020 2020 4063  message)..    @c
+00000bc0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00000bd0: 6566 2070 7269 6e74 5f6d 6174 7269 7828  ef print_matrix(
+00000be0: 636c 733a 2041 6e79 2c20 6170 7065 6172  cls: Any, appear
+00000bf0: 6564 5f73 6571 7565 6e63 6573 3a20 4c69  ed_sequences: Li
+00000c00: 7374 5b4c 6973 745b 696e 745d 5d2c 206d  st[List[int]], m
+00000c10: 6174 7269 785f 7369 7a65 3a20 696e 7429  atrix_size: int)
+00000c20: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00000c30: 2020 666f 7220 7365 7175 656e 6365 2069    for sequence i
+00000c40: 6e20 6170 7065 6172 6564 5f73 6571 7565  n appeared_seque
+00000c50: 6e63 6573 3a0a 2020 2020 2020 2020 2020  nces:.          
+00000c60: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00000c70: 2831 2c20 6d61 7472 6978 5f73 697a 6520  (1, matrix_size 
+00000c80: 2b20 3129 3a0a 2020 2020 2020 2020 2020  + 1):.          
+00000c90: 2020 2020 2020 6966 2069 2069 6e20 7365        if i in se
+00000ca0: 7175 656e 6365 3a0a 2020 2020 2020 2020  quence:.        
+00000cb0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000cc0: 7428 6622 7b69 3a3e 347d 222c 2065 6e64  t(f"{i:>4}", end
+00000cd0: 3d22 2022 290a 2020 2020 2020 2020 2020  =" ").          
+00000ce0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d00: 7072 696e 7428 6622 7b27 2d27 3a3e 347d  print(f"{'-':>4}
+00000d10: 222c 2065 6e64 3d22 2022 290a 2020 2020  ", end=" ").    
+00000d20: 2020 2020 2020 2020 7072 696e 7428 290a          print().
+00000d30: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00000d40: 640a 2020 2020 6465 6620 6c69 7374 5f74  d.    def list_t
+00000d50: 6f5f 696e 7428 0a20 2020 2020 2020 2020  o_int(.         
+00000d60: 2020 2063 6c73 2c0a 2020 2020 2020 2020     cls,.        
+00000d70: 2020 2020 6e75 6d62 6572 733a 204c 6973      numbers: Lis
+00000d80: 745b 696e 745d 2c0a 2020 2020 2020 2020  t[int],.        
+00000d90: 2020 2020 7a65 726f 5f72 6570 6c61 6365      zero_replace
+00000da0: 6d65 6e74 3a20 7374 7220 3d20 2727 2c0a  ment: str = '',.
+00000db0: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+00000dc0: 6172 6773 3a20 416e 790a 2020 2020 2920  args: Any.    ) 
+00000dd0: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00000de0: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
+00000df0: 6572 7420 6120 6c69 7374 206f 6620 696e  ert a list of in
+00000e00: 7465 6765 7273 2074 6f20 6120 7369 6e67  tegers to a sing
+00000e10: 6c65 2069 6e74 6567 6572 2c20 7769 7468  le integer, with
+00000e20: 2061 6e20 6f70 7469 6f6e 616c 2072 6570   an optional rep
+00000e30: 6c61 6365 6d65 6e74 2066 6f72 207a 6572  lacement for zer
+00000e40: 6f73 2e0a 0a20 2020 2020 2020 203a 7061  os...        :pa
+00000e50: 7261 6d20 6e75 6d62 6572 733a 206c 6973  ram numbers: lis
+00000e60: 7420 6f66 2069 6e74 6567 6572 730a 2020  t of integers.  
+00000e70: 2020 2020 2020 3a70 6172 616d 207a 6572        :param zer
+00000e80: 6f5f 7265 706c 6163 656d 656e 743a 2073  o_replacement: s
+00000e90: 7472 696e 6720 746f 2072 6570 6c61 6365  tring to replace
+00000ea0: 207a 6572 6f73 2077 6974 682c 2064 6566   zeros with, def
+00000eb0: 6175 6c74 7320 746f 2061 6e20 656d 7074  aults to an empt
+00000ec0: 7920 7374 7269 6e67 0a20 2020 2020 2020  y string.       
+00000ed0: 203a 7265 7475 726e 3a20 7369 6e67 6c65   :return: single
+00000ee0: 2069 6e74 6567 6572 2066 6f72 6d65 6420   integer formed 
+00000ef0: 6279 2063 6f6e 6361 7465 6e61 7469 6e67  by concatenating
+00000f00: 2074 6865 206c 6973 7420 656c 656d 656e   the list elemen
+00000f10: 7473 0a20 2020 2020 2020 2022 2222 0a20  ts.        """. 
+00000f20: 2020 2020 2020 2023 2056 616c 6964 6174         # Validat
+00000f30: 6520 696e 7075 7420 6461 7461 2069 7320  e input data is 
+00000f40: 6120 6c69 7374 0a20 2020 2020 2020 2069  a list.        i
+00000f50: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00000f60: 286e 756d 6265 7273 2c20 4c69 7374 293a  (numbers, List):
+00000f70: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00000f80: 7365 2056 616c 7565 4572 726f 7228 2249  se ValueError("I
+00000f90: 6e70 7574 2027 6e75 6d62 6572 7327 206d  nput 'numbers' m
+00000fa0: 7573 7420 6265 2061 206c 6973 742e 2229  ust be a list.")
+00000fb0: 0a0a 2020 2020 2020 2020 2320 5661 6c69  ..        # Vali
+00000fc0: 6461 7465 2061 6c6c 2065 6c65 6d65 6e74  date all element
+00000fd0: 7320 696e 2074 6865 206c 6973 7420 6172  s in the list ar
+00000fe0: 6520 696e 7465 6765 7273 0a20 2020 2020  e integers.     
+00000ff0: 2020 2069 6620 6e6f 7420 616c 6c28 6973     if not all(is
+00001000: 696e 7374 616e 6365 2878 2c20 696e 7429  instance(x, int)
+00001010: 2066 6f72 2078 2069 6e20 6e75 6d62 6572   for x in number
+00001020: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00001030: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00001040: 2822 416c 6c20 656c 656d 656e 7473 2069  ("All elements i
+00001050: 6e20 7468 6520 276e 756d 6265 7273 2720  n the 'numbers' 
+00001060: 6c69 7374 206d 7573 7420 6265 2069 6e74  list must be int
+00001070: 6567 6572 732e 2229 0a0a 2020 2020 2020  egers.")..      
+00001080: 2020 2320 436f 6e76 6572 7420 6c69 7374    # Convert list
+00001090: 2065 6c65 6d65 6e74 7320 746f 2073 7472   elements to str
+000010a0: 696e 6773 2c20 7265 706c 6163 696e 6720  ings, replacing 
+000010b0: 7a65 726f 7320 7769 7468 207a 6572 6f5f  zeros with zero_
+000010c0: 7265 706c 6163 656d 656e 740a 2020 2020  replacement.    
+000010d0: 2020 2020 7061 7274 7320 3d20 5b7a 6572      parts = [zer
+000010e0: 6f5f 7265 706c 6163 656d 656e 7420 6966  o_replacement if
+000010f0: 2078 203d 3d20 3020 656c 7365 2073 7472   x == 0 else str
+00001100: 2878 2920 666f 7220 7820 696e 206e 756d  (x) for x in num
+00001110: 6265 7273 5d0a 0a20 2020 2020 2020 2023  bers]..        #
+00001120: 204a 6f69 6e20 7468 6520 7061 7274 7320   Join the parts 
+00001130: 616e 6420 636f 6e76 6572 7420 746f 2061  and convert to a
+00001140: 6e20 696e 7465 6765 720a 2020 2020 2020  n integer.      
+00001150: 2020 7265 7475 726e 2069 6e74 2827 272e    return int(''.
+00001160: 6a6f 696e 2870 6172 7473 2929 0a0a 2020  join(parts))..  
+00001170: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00001180: 2020 2064 6566 2069 6e74 5f74 6f5f 6c69     def int_to_li
+00001190: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+000011a0: 636c 732c 0a20 2020 2020 2020 2020 2020  cls,.           
+000011b0: 206e 756d 6265 723a 2069 6e74 2c0a 2020   number: int,.  
+000011c0: 2020 2020 2020 2020 2020 6d6f 6475 6c75            modulu
+000011d0: 733a 2069 6e74 203d 2031 302c 0a20 2020  s: int = 10,.   
+000011e0: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+000011f0: 733a 2041 6e79 0a20 2020 2029 202d 3e20  s: Any.    ) -> 
+00001200: 4c69 7374 5b69 6e74 5d3a 0a20 2020 2020  List[int]:.     
+00001210: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00001220: 6f6e 7665 7274 2061 6e20 696e 7465 6765  onvert an intege
+00001230: 7220 746f 2061 206c 6973 7420 6f66 2064  r to a list of d
+00001240: 6967 6974 732c 2065 6163 6820 6469 6769  igits, each digi
+00001250: 7420 6973 2074 6865 2072 656d 6169 6e64  t is the remaind
+00001260: 6572 206f 6620 6469 7669 7369 6f6e 2062  er of division b
+00001270: 7920 6120 6d6f 6475 6c75 732e 0a0a 2020  y a modulus...  
+00001280: 2020 2020 2020 3a70 6172 616d 206e 756d        :param num
+00001290: 6265 723a 2054 6865 2069 6e74 6567 6572  ber: The integer
+000012a0: 2074 6f20 6265 2063 6f6e 7665 7274 6564   to be converted
+000012b0: 2069 6e74 6f20 6120 6c69 7374 206f 6620   into a list of 
+000012c0: 6469 6769 7473 2e0a 2020 2020 2020 2020  digits..        
+000012d0: 3a70 6172 616d 206d 6f64 756c 7573 3a20  :param modulus: 
+000012e0: 5468 6520 6469 7669 736f 7220 7573 6564  The divisor used
+000012f0: 2066 6f72 2074 6865 206d 6f64 756c 6f20   for the modulo 
+00001300: 6f70 6572 6174 696f 6e20 6f6e 2065 6163  operation on eac
+00001310: 6820 6469 6769 742c 2064 6566 6175 6c74  h digit, default
+00001320: 7320 746f 2031 302e 0a20 2020 2020 2020  s to 10..       
+00001330: 203a 7265 7475 726e 3a20 4120 6c69 7374   :return: A list
+00001340: 206f 6620 696e 7465 6765 7273 2c20 7768   of integers, wh
+00001350: 6572 6520 6561 6368 2069 6e74 6567 6572  ere each integer
+00001360: 2069 7320 6120 6469 6769 7420 6f66 2074   is a digit of t
+00001370: 6865 206f 7269 6769 6e61 6c20 6e75 6d62  he original numb
+00001380: 6572 2061 6674 6572 2074 6865 206d 6f64  er after the mod
+00001390: 756c 6f20 6f70 6572 6174 696f 6e2e 0a20  ulo operation.. 
+000013a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000013b0: 2020 2023 2056 616c 6964 6174 6520 696e     # Validate in
+000013c0: 7075 7420 6461 7461 2069 7320 616e 2069  put data is an i
+000013d0: 6e74 6567 6572 0a20 2020 2020 2020 2069  nteger.        i
+000013e0: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+000013f0: 286e 756d 6265 722c 2069 6e74 293a 0a20  (number, int):. 
+00001400: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00001410: 2056 616c 7565 4572 726f 7228 2249 6e70   ValueError("Inp
+00001420: 7574 2027 6e75 6d62 6572 2720 6d75 7374  ut 'number' must
+00001430: 2062 6520 616e 2069 6e74 6567 6572 2e22   be an integer."
+00001440: 290a 0a20 2020 2020 2020 2023 2056 616c  )..        # Val
+00001450: 6964 6174 6520 6d6f 6475 6c75 7320 6973  idate modulus is
+00001460: 2061 2070 6f73 6974 6976 6520 696e 7465   a positive inte
+00001470: 6765 720a 2020 2020 2020 2020 6966 206e  ger.        if n
+00001480: 6f74 2069 7369 6e73 7461 6e63 6528 6d6f  ot isinstance(mo
+00001490: 6475 6c75 732c 2069 6e74 2920 6f72 206d  dulus, int) or m
+000014a0: 6f64 756c 7573 203c 3d20 303a 0a20 2020  odulus <= 0:.   
+000014b0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000014c0: 616c 7565 4572 726f 7228 2249 6e70 7574  alueError("Input
+000014d0: 2027 6d6f 6475 6c75 7327 206d 7573 7420   'modulus' must 
+000014e0: 6265 2061 2070 6f73 6974 6976 6520 696e  be a positive in
+000014f0: 7465 6765 722e 2229 0a0a 2020 2020 2020  teger.")..      
+00001500: 2020 2320 436f 6e76 6572 7420 7468 6520    # Convert the 
+00001510: 696e 7465 6765 7220 746f 2061 206c 6973  integer to a lis
+00001520: 7420 6f66 2064 6967 6974 7320 7573 696e  t of digits usin
+00001530: 6720 7468 6520 6d6f 6475 6c75 730a 2020  g the modulus.  
+00001540: 2020 2020 2020 6469 6769 745f 6c69 7374        digit_list
+00001550: 203d 205b 696e 7428 6429 2025 206d 6f64   = [int(d) % mod
+00001560: 756c 7573 2066 6f72 2064 2069 6e20 7374  ulus for d in st
+00001570: 7228 6162 7328 6e75 6d62 6572 2929 5d0a  r(abs(number))].
+00001580: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+00001590: 6e20 7468 6520 6c69 7374 206f 6620 6469  n the list of di
+000015a0: 6769 7473 0a20 2020 2020 2020 2072 6574  gits.        ret
+000015b0: 7572 6e20 6469 6769 745f 6c69 7374 0a0a  urn digit_list..
+000015c0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+000015d0: 0a20 2020 2064 6566 2077 7269 7465 5f64  .    def write_d
+000015e0: 6174 615f 746f 5f66 696c 6528 0a20 2020  ata_to_file(.   
+000015f0: 2020 2020 2020 2020 2063 6c73 2c0a 2020           cls,.  
+00001600: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
+00001610: 6174 683a 2073 7472 2c0a 2020 2020 2020  ath: str,.      
+00001620: 2020 2020 2020 6461 7461 3a20 4c69 7374        data: List
+00001630: 5b73 7472 5d2c 0a20 2020 2020 2020 2020  [str],.         
+00001640: 2020 2061 7070 5f6c 6f67 3a20 4f70 7469     app_log: Opti
+00001650: 6f6e 616c 5b6c 6f67 6769 6e67 2e4c 6f67  onal[logging.Log
+00001660: 6765 725d 203d 204e 6f6e 652c 0a20 2020  ger] = None,.   
+00001670: 2020 2020 2020 2020 206d 6f64 653a 2073           mode: s
+00001680: 7472 203d 2027 612b 272c 0a20 2020 2020  tr = 'a+',.     
+00001690: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
+000016a0: 2041 6e79 0a20 2020 2029 202d 3e20 626f   Any.    ) -> bo
+000016b0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
+000016c0: 2020 2020 2020 2020 5772 6974 6520 6461          Write da
+000016d0: 7461 2074 6f20 6120 6669 6c65 2e0a 0a20  ta to a file... 
+000016e0: 2020 2020 2020 203a 7061 7261 6d20 6669         :param fi
+000016f0: 6c65 5f70 6174 683a 2050 6174 6820 746f  le_path: Path to
+00001700: 2074 6865 2066 696c 6520 7768 6572 6520   the file where 
+00001710: 6461 7461 2077 696c 6c20 6265 2077 7269  data will be wri
+00001720: 7474 656e 2e0a 2020 2020 2020 2020 3a70  tten..        :p
+00001730: 6172 616d 2064 6174 613a 204c 6973 7420  aram data: List 
+00001740: 6f66 2064 6174 6120 746f 2077 7269 7465  of data to write
+00001750: 2074 6f20 7468 6520 6669 6c65 2e0a 2020   to the file..  
+00001760: 2020 2020 2020 3a70 6172 616d 2061 7070        :param app
+00001770: 5f6c 6f67 3a20 4f70 7469 6f6e 616c 206c  _log: Optional l
+00001780: 6f67 6765 7220 666f 7220 6c6f 6767 696e  ogger for loggin
+00001790: 6720 696e 666f 726d 6174 696f 6e2c 2064  g information, d
+000017a0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+000017b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000017c0: 6d6f 6465 3a20 4d6f 6465 2069 6e20 7768  mode: Mode in wh
+000017d0: 6963 6820 7468 6520 6669 6c65 2073 686f  ich the file sho
+000017e0: 756c 6420 6265 206f 7065 6e65 642c 2064  uld be opened, d
+000017f0: 6566 6175 6c74 7320 746f 2027 612b 2720  efaults to 'a+' 
+00001800: 666f 7220 6170 7065 6e64 2e0a 2020 2020  for append..    
+00001810: 2020 2020 3a72 6574 7572 6e3a 2062 6f6f      :return: boo
+00001820: 6c20 7765 6174 6865 7220 7375 6363 6573  l weather succes
+00001830: 7320 6f72 2066 6169 6c65 640a 2020 2020  s or failed.    
+00001840: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00001850: 6966 2061 7070 5f6c 6f67 2069 7320 4e6f  if app_log is No
+00001860: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00001870: 6170 705f 6c6f 6720 3d20 636c 732e 6765  app_log = cls.ge
+00001880: 745f 6c6f 6767 6572 2829 0a0a 2020 2020  t_logger()..    
+00001890: 2020 2020 6966 206e 6f74 2064 6174 613a      if not data:
+000018a0: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+000018b0: 5f6c 6f67 2e77 6172 6e69 6e67 2822 4e6f  _log.warning("No
+000018c0: 2064 6174 6120 7072 6f76 6964 6564 2074   data provided t
+000018d0: 6f20 7772 6974 6520 746f 2074 6865 2066  o write to the f
+000018e0: 696c 652e 2229 0a20 2020 2020 2020 2020  ile.").         
+000018f0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00001900: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00001910: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+00001920: 7065 6e28 6669 6c65 5f70 6174 682c 206d  pen(file_path, m
+00001930: 6f64 6529 2061 7320 6670 3a0a 2020 2020  ode) as fp:.    
+00001940: 2020 2020 2020 2020 2020 2020 6170 705f              app_
+00001950: 6c6f 672e 6465 6275 6728 6627 5772 6974  log.debug(f'Writ
+00001960: 696e 6720 746f 2066 696c 653a 207b 6670  ing to file: {fp
+00001970: 2e6e 616d 657d 2729 0a20 2020 2020 2020  .name}').       
+00001980: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
+00001990: 6520 696e 2064 6174 613a 0a20 2020 2020  e in data:.     
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000019b0: 6620 6c69 6e65 2069 7320 6e6f 7420 4e6f  f line is not No
+000019c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000019d0: 2020 2020 2020 2020 2020 2020 6670 2e77              fp.w
+000019e0: 7269 7465 2866 277b 6c69 6e65 7d5c 6e27  rite(f'{line}\n'
+000019f0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00001a00: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
+00001a10: 3a0a 2020 2020 2020 2020 2020 2020 6170  :.            ap
+00001a20: 705f 6c6f 672e 6578 6365 7074 696f 6e28  p_log.exception(
+00001a30: 6622 416e 2065 7272 6f72 206f 6363 7572  f"An error occur
+00001a40: 7265 6420 7768 696c 6520 7772 6974 696e  red while writin
+00001a50: 6720 746f 2074 6865 2066 696c 653a 207b  g to the file: {
+00001a60: 6578 7d22 290a 2020 2020 2020 2020 2020  ex}").          
+00001a70: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00001a80: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00001a90: 7275 650a 0a20 2020 2040 636c 6173 736d  rue..    @classm
+00001aa0: 6574 686f 640a 2020 2020 6465 6620 7265  ethod.    def re
+00001ab0: 6164 5f64 6174 615f 6672 6f6d 5f66 696c  ad_data_from_fil
+00001ac0: 6528 0a20 2020 2020 2020 2020 2020 2063  e(.            c
+00001ad0: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+00001ae0: 6669 6c65 5f70 6174 683a 2073 7472 2c0a  file_path: str,.
+00001af0: 2020 2020 2020 2020 2020 2020 6170 705f              app_
+00001b00: 6c6f 673a 204f 7074 696f 6e61 6c5b 6c6f  log: Optional[lo
+00001b10: 6767 696e 672e 4c6f 6767 6572 5d20 3d20  gging.Logger] = 
+00001b20: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001b30: 2020 6d6f 6465 3a20 7374 7220 3d20 2772    mode: str = 'r
+00001b40: 270a 2020 2020 2920 2d3e 204f 7074 696f  '.    ) -> Optio
+00001b50: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 3a0a  nal[List[str]]:.
+00001b60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00001b70: 2020 2020 5265 6164 2064 6174 6120 6672      Read data fr
+00001b80: 6f6d 2061 2066 696c 6520 616e 6420 7265  om a file and re
+00001b90: 7475 726e 2061 206c 6973 7420 6f66 206e  turn a list of n
+00001ba0: 6f6e 2d65 6d70 7479 206c 696e 6573 2e0a  on-empty lines..
+00001bb0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001bc0: 6669 6c65 5f70 6174 683a 2050 6174 6820  file_path: Path 
+00001bd0: 746f 2074 6865 2066 696c 6520 746f 2062  to the file to b
+00001be0: 6520 7265 6164 2e0a 2020 2020 2020 2020  e read..        
+00001bf0: 3a70 6172 616d 2061 7070 5f6c 6f67 3a20  :param app_log: 
+00001c00: 4f70 7469 6f6e 616c 206c 6f67 6765 7220  Optional logger 
+00001c10: 666f 7220 6c6f 6767 696e 6720 696e 666f  for logging info
+00001c20: 726d 6174 696f 6e2c 2064 6566 6175 6c74  rmation, default
+00001c30: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
+00001c40: 2020 203a 7061 7261 6d20 6d6f 6465 3a20     :param mode: 
+00001c50: 4d6f 6465 2069 6e20 7768 6963 6820 7468  Mode in which th
+00001c60: 6520 6669 6c65 2073 686f 756c 6420 6265  e file should be
+00001c70: 206f 7065 6e65 642c 2064 6566 6175 6c74   opened, default
+00001c80: 7320 746f 2027 7227 2066 6f72 2072 6561  s to 'r' for rea
+00001c90: 6420 6f6e 6c79 2e0a 2020 2020 2020 2020  d only..        
+00001ca0: 3a72 6574 7572 6e3a 204c 6973 7420 6f66  :return: List of
+00001cb0: 206e 6f6e 2d65 6d70 7479 206c 696e 6573   non-empty lines
+00001cc0: 2066 726f 6d20 7468 6520 6669 6c65 206f   from the file o
+00001cd0: 7220 4e6f 6e65 2069 6620 616e 2065 7863  r None if an exc
+00001ce0: 6570 7469 6f6e 206f 6363 7572 732e 0a20  eption occurs.. 
+00001cf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00001d00: 2020 2069 6620 6170 705f 6c6f 6720 6973     if app_log is
+00001d10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00001d20: 2020 2061 7070 5f6c 6f67 203d 2063 6c73     app_log = cls
+00001d30: 2e67 6574 5f6c 6f67 6765 7228 290a 0a20  .get_logger().. 
+00001d40: 2020 2020 2020 2064 6174 6120 3d20 5b5d         data = []
+00001d50: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00001d60: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+00001d70: 7065 6e28 6669 6c65 5f70 6174 682c 206d  pen(file_path, m
+00001d80: 6f64 6529 2061 7320 6670 3a0a 2020 2020  ode) as fp:.    
+00001d90: 2020 2020 2020 2020 2020 2020 6170 705f              app_
+00001da0: 6c6f 672e 6465 6275 6728 6627 4f70 656e  log.debug(f'Open
+00001db0: 696e 6720 6669 6c65 3a20 7b66 702e 6e61  ing file: {fp.na
+00001dc0: 6d65 7d27 290a 2020 2020 2020 2020 2020  me}').          
+00001dd0: 2020 2020 2020 6461 7461 203d 205b 6c69        data = [li
+00001de0: 6e65 2e73 7472 6970 2829 2066 6f72 206c  ne.strip() for l
+00001df0: 696e 6520 696e 2066 7020 6966 206c 696e  ine in fp if lin
+00001e00: 652e 7374 7269 7028 295d 0a20 2020 2020  e.strip()].     
+00001e10: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00001e20: 696f 6e20 6173 2065 783a 0a20 2020 2020  ion as ex:.     
+00001e30: 2020 2020 2020 2061 7070 5f6c 6f67 2e65         app_log.e
+00001e40: 7863 6570 7469 6f6e 2866 2241 6e20 6572  xception(f"An er
+00001e50: 726f 7220 6f63 6375 7272 6564 2077 6869  ror occurred whi
+00001e60: 6c65 2072 6561 6469 6e67 2074 6865 2066  le reading the f
+00001e70: 696c 653a 207b 6578 7d22 290a 2020 2020  ile: {ex}").    
+00001e80: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00001e90: 6f6e 650a 0a20 2020 2020 2020 2061 7070  one..        app
+00001ea0: 5f6c 6f67 2e69 6e66 6f28 6627 4e75 6d62  _log.info(f'Numb
+00001eb0: 6572 206f 6620 6e6f 6e2d 656d 7074 7920  er of non-empty 
+00001ec0: 6c69 6e65 7320 7265 6164 3a20 7b6c 656e  lines read: {len
+00001ed0: 2864 6174 6129 7d27 290a 2020 2020 2020  (data)}').      
+00001ee0: 2020 7265 7475 726e 2064 6174 610a 0a20    return data.. 
+00001ef0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00001f00: 2020 2020 6465 6620 7772 6974 655f 6373      def write_cs
+00001f10: 765f 6461 7461 5f74 6f5f 6669 6c65 280a  v_data_to_file(.
+00001f20: 2020 2020 2020 2020 2020 2020 636c 732c              cls,
+00001f30: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00001f40: 655f 7061 7468 3a20 7374 722c 0a20 2020  e_path: str,.   
+00001f50: 2020 2020 2020 2020 2064 6174 613a 204c           data: L
+00001f60: 6973 745b 4c69 7374 5b41 6e79 5d5d 2c0a  ist[List[Any]],.
+00001f70: 2020 2020 2020 2020 2020 2020 6170 705f              app_
+00001f80: 6c6f 673a 204f 7074 696f 6e61 6c5b 6c6f  log: Optional[lo
+00001f90: 6767 696e 672e 4c6f 6767 6572 5d20 3d20  gging.Logger] = 
+00001fa0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001fb0: 2020 6d6f 6465 3a20 7374 7220 3d20 2761    mode: str = 'a
+00001fc0: 2b27 2c0a 2020 2020 2020 2020 2020 2020  +',.            
+00001fd0: 6e65 776c 696e 653a 2073 7472 203d 2027  newline: str = '
+00001fe0: 272c 0a20 2020 2020 2020 2020 2020 202a  ',.            *
+00001ff0: 2a6b 7761 7267 733a 2041 6e79 0a20 2020  *kwargs: Any.   
+00002000: 2029 202d 3e20 626f 6f6c 3a0a 2020 2020   ) -> bool:.    
+00002010: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00002020: 5772 6974 6520 6461 7461 2074 6f20 6120  Write data to a 
+00002030: 4353 5620 6669 6c65 2e0a 0a20 2020 2020  CSV file...     
+00002040: 2020 203a 7061 7261 6d20 6669 6c65 5f70     :param file_p
+00002050: 6174 683a 2050 6174 6820 746f 2074 6865  ath: Path to the
+00002060: 2066 696c 6520 7768 6572 6520 4353 5620   file where CSV 
+00002070: 6461 7461 2077 696c 6c20 6265 2077 7269  data will be wri
+00002080: 7474 656e 2e0a 2020 2020 2020 2020 3a70  tten..        :p
+00002090: 6172 616d 2064 6174 613a 204c 6973 7420  aram data: List 
+000020a0: 6f66 2072 6f77 7320 2877 6865 7265 2065  of rows (where e
+000020b0: 6163 6820 726f 7720 6973 2061 206c 6973  ach row is a lis
+000020c0: 7429 2074 6f20 7772 6974 6520 746f 2074  t) to write to t
+000020d0: 6865 2043 5356 2066 696c 652e 0a20 2020  he CSV file..   
+000020e0: 2020 2020 203a 7061 7261 6d20 6170 705f       :param app_
+000020f0: 6c6f 673a 204f 7074 696f 6e61 6c20 6c6f  log: Optional lo
+00002100: 6767 6572 2066 6f72 206c 6f67 6769 6e67  gger for logging
+00002110: 2069 6e66 6f72 6d61 7469 6f6e 2c20 6465   information, de
+00002120: 6661 756c 7473 2074 6f20 4e6f 6e65 2077  faults to None w
+00002130: 6869 6368 2077 696c 6c20 6372 6561 7465  hich will create
+00002140: 2061 206e 6577 206c 6f67 6765 722e 0a20   a new logger.. 
+00002150: 2020 2020 2020 203a 7061 7261 6d20 6d6f         :param mo
+00002160: 6465 3a20 4d6f 6465 2069 6e20 7768 6963  de: Mode in whic
+00002170: 6820 7468 6520 6669 6c65 2073 686f 756c  h the file shoul
+00002180: 6420 6265 206f 7065 6e65 642c 2064 6566  d be opened, def
+00002190: 6175 6c74 7320 746f 2027 612b 2720 666f  aults to 'a+' fo
+000021a0: 7220 6170 7065 6e64 2e0a 2020 2020 2020  r append..      
+000021b0: 2020 3a70 6172 616d 206e 6577 6c69 6e65    :param newline
+000021c0: 3a20 436f 6e74 726f 6c73 2068 6f77 2075  : Controls how u
+000021d0: 6e69 7665 7273 616c 206e 6577 6c69 6e65  niversal newline
+000021e0: 7320 776f 726b 7320 2869 7420 6f6e 6c79  s works (it only
+000021f0: 2061 7070 6c69 6573 2074 6f20 7465 7874   applies to text
+00002200: 206d 6f64 6529 2e20 4974 2064 6566 6175   mode). It defau
+00002210: 6c74 7320 746f 2027 272e 0a20 2020 2020  lts to ''..     
+00002220: 2020 203a 7265 7475 726e 3a20 626f 6f6c     :return: bool
+00002230: 2077 6561 7468 6572 2073 7563 6365 7373   weather success
+00002240: 206f 7220 6661 696c 6564 0a20 2020 2020   or failed.     
+00002250: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00002260: 6620 6170 705f 6c6f 6720 6973 204e 6f6e  f app_log is Non
+00002270: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+00002280: 7070 5f6c 6f67 203d 2063 6c73 2e67 6574  pp_log = cls.get
+00002290: 5f6c 6f67 6765 7228 290a 0a20 2020 2020  _logger()..     
+000022a0: 2020 2069 6620 6e6f 7420 6461 7461 3a0a     if not data:.
+000022b0: 2020 2020 2020 2020 2020 2020 6170 705f              app_
+000022c0: 6c6f 672e 7761 726e 696e 6728 224e 6f20  log.warning("No 
+000022d0: 6461 7461 2070 726f 7669 6465 6420 746f  data provided to
+000022e0: 2077 7269 7465 2074 6f20 7468 6520 6669   write to the fi
+000022f0: 6c65 2e22 290a 2020 2020 2020 2020 2020  le.").          
+00002300: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00002310: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00002320: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+00002330: 656e 2866 696c 655f 7061 7468 2c20 6d6f  en(file_path, mo
+00002340: 6465 3d6d 6f64 652c 206e 6577 6c69 6e65  de=mode, newline
+00002350: 3d6e 6577 6c69 6e65 2920 6173 2066 703a  =newline) as fp:
+00002360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002370: 2061 7070 5f6c 6f67 2e64 6562 7567 2866   app_log.debug(f
+00002380: 2757 7269 7469 6e67 2074 6f20 4353 5620  'Writing to CSV 
+00002390: 6669 6c65 3a20 7b66 702e 6e61 6d65 7d27  file: {fp.name}'
+000023a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000023b0: 2020 7772 6974 6572 203d 2063 7376 2e77    writer = csv.w
+000023c0: 7269 7465 7228 6670 2c20 2a2a 6b77 6172  riter(fp, **kwar
+000023d0: 6773 290a 2020 2020 2020 2020 2020 2020  gs).            
+000023e0: 2020 2020 7772 6974 6572 2e77 7269 7465      writer.write
+000023f0: 726f 7773 2864 6174 6129 0a20 2020 2020  rows(data).     
+00002400: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00002410: 696f 6e20 6173 2065 783a 0a20 2020 2020  ion as ex:.     
+00002420: 2020 2020 2020 2061 7070 5f6c 6f67 2e65         app_log.e
+00002430: 7863 6570 7469 6f6e 2866 2241 6e20 6572  xception(f"An er
+00002440: 726f 7220 6f63 6375 7272 6564 2077 6869  ror occurred whi
+00002450: 6c65 2077 7269 7469 6e67 2074 6f20 7468  le writing to th
+00002460: 6520 4353 5620 6669 6c65 3a20 7b65 787d  e CSV file: {ex}
+00002470: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00002480: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00002490: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+000024a0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+000024b0: 6f64 0a20 2020 2064 6566 2072 6561 645f  od.    def read_
+000024c0: 6373 765f 6461 7461 5f66 726f 6d5f 6669  csv_data_from_fi
+000024d0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+000024e0: 636c 732c 0a20 2020 2020 2020 2020 2020  cls,.           
+000024f0: 2066 696c 655f 7061 7468 3a20 7374 722c   file_path: str,
+00002500: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+00002510: 5f6c 6f67 3a20 4f70 7469 6f6e 616c 5b6c  _log: Optional[l
+00002520: 6f67 6769 6e67 2e4c 6f67 6765 725d 203d  ogging.Logger] =
+00002530: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00002540: 2020 206d 6f64 653a 2073 7472 203d 2027     mode: str = '
+00002550: 7227 2c0a 2020 2020 2020 2020 2020 2020  r',.            
+00002560: 2a2a 6b77 6172 6773 3a20 416e 790a 2020  **kwargs: Any.  
+00002570: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+00002580: 4c69 7374 5b4c 6973 745b 7374 725d 5d5d  List[List[str]]]
+00002590: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000025a0: 2020 2020 2020 5265 6164 2043 5356 2064        Read CSV d
+000025b0: 6174 6120 6672 6f6d 2061 2066 696c 6520  ata from a file 
+000025c0: 616e 6420 7265 7475 726e 2061 206c 6973  and return a lis
+000025d0: 7420 6f66 2072 6f77 732e 0a0a 2020 2020  t of rows...    
+000025e0: 2020 2020 3a70 6172 616d 2066 696c 655f      :param file_
+000025f0: 7061 7468 3a20 5061 7468 2074 6f20 7468  path: Path to th
+00002600: 6520 4353 5620 6669 6c65 2074 6f20 6265  e CSV file to be
+00002610: 2072 6561 642e 0a20 2020 2020 2020 203a   read..        :
+00002620: 7061 7261 6d20 6170 705f 6c6f 673a 204f  param app_log: O
+00002630: 7074 696f 6e61 6c20 6c6f 6767 6572 2066  ptional logger f
+00002640: 6f72 206c 6f67 6769 6e67 2069 6e66 6f72  or logging infor
+00002650: 6d61 7469 6f6e 2c20 6465 6661 756c 7473  mation, defaults
+00002660: 2074 6f20 6120 6e65 7720 6c6f 6767 6572   to a new logger
+00002670: 2069 6620 4e6f 6e65 2e0a 2020 2020 2020   if None..      
+00002680: 2020 3a70 6172 616d 206d 6f64 653a 204d    :param mode: M
+00002690: 6f64 6520 696e 2077 6869 6368 2074 6865  ode in which the
+000026a0: 2066 696c 6520 7368 6f75 6c64 2062 6520   file should be 
+000026b0: 6f70 656e 6564 2c20 6465 6661 756c 7473  opened, defaults
+000026c0: 2074 6f20 2772 2720 666f 7220 7265 6164   to 'r' for read
+000026d0: 206f 6e6c 792e 0a20 2020 2020 2020 203a   only..        :
+000026e0: 7265 7475 726e 3a20 4c69 7374 206f 6620  return: List of 
+000026f0: 726f 7773 2066 726f 6d20 7468 6520 4353  rows from the CS
+00002700: 5620 6669 6c65 206f 7220 4e6f 6e65 2069  V file or None i
+00002710: 6620 616e 2065 7863 6570 7469 6f6e 206f  f an exception o
+00002720: 6363 7572 732e 0a20 2020 2020 2020 2022  ccurs..        "
+00002730: 2222 0a20 2020 2020 2020 2069 6620 6170  "".        if ap
+00002740: 705f 6c6f 6720 6973 204e 6f6e 653a 0a20  p_log is None:. 
+00002750: 2020 2020 2020 2020 2020 2061 7070 5f6c             app_l
+00002760: 6f67 203d 2063 6c73 2e67 6574 5f6c 6f67  og = cls.get_log
+00002770: 6765 7228 290a 0a20 2020 2020 2020 2074  ger()..        t
+00002780: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00002790: 7769 7468 206f 7065 6e28 6669 6c65 5f70  with open(file_p
+000027a0: 6174 682c 206d 6f64 653d 6d6f 6465 2c20  ath, mode=mode, 
+000027b0: 2a2a 6b77 6172 6773 2920 6173 2066 703a  **kwargs) as fp:
+000027c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027d0: 2061 7070 5f6c 6f67 2e64 6562 7567 2866   app_log.debug(f
+000027e0: 2752 6561 6469 6e67 2043 5356 2066 696c  'Reading CSV fil
+000027f0: 653a 207b 6670 2e6e 616d 657d 2729 0a20  e: {fp.name}'). 
+00002800: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002810: 6561 6465 7220 3d20 6373 762e 7265 6164  eader = csv.read
+00002820: 6572 2866 702c 202a 2a6b 7761 7267 7329  er(fp, **kwargs)
+00002830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002840: 2064 6174 6120 3d20 5b72 6f77 2066 6f72   data = [row for
+00002850: 2072 6f77 2069 6e20 7265 6164 6572 5d0a   row in reader].
+00002860: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00002870: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
+00002880: 2020 2020 2020 2020 2020 2020 6170 705f              app_
+00002890: 6c6f 672e 6578 6365 7074 696f 6e28 6622  log.exception(f"
+000028a0: 416e 2065 7272 6f72 206f 6363 7572 7265  An error occurre
+000028b0: 6420 7768 696c 6520 7265 6164 696e 6720  d while reading 
+000028c0: 7468 6520 4353 5620 6669 6c65 3a20 7b65  the CSV file: {e
+000028d0: 787d 2229 0a20 2020 2020 2020 2020 2020  x}").           
+000028e0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+000028f0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+00002900: 610a 0a20 2020 2040 636c 6173 736d 6574  a..    @classmet
+00002910: 686f 640a 2020 2020 6465 6620 7772 6974  hod.    def writ
+00002920: 655f 6a73 6f6e 5f64 6174 615f 746f 5f66  e_json_data_to_f
+00002930: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+00002940: 2063 6c73 2c0a 2020 2020 2020 2020 2020   cls,.          
+00002950: 2020 6669 6c65 5f70 6174 683a 2073 7472    file_path: str
+00002960: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00002970: 7461 3a20 416e 792c 0a20 2020 2020 2020  ta: Any,.       
+00002980: 2020 2020 2061 7070 5f6c 6f67 3a20 4f70       app_log: Op
+00002990: 7469 6f6e 616c 5b6c 6f67 6769 6e67 2e4c  tional[logging.L
+000029a0: 6f67 6765 725d 203d 204e 6f6e 652c 0a20  ogger] = None,. 
+000029b0: 2020 2020 2020 2020 2020 206d 6f64 653a             mode:
+000029c0: 2073 7472 203d 2027 7727 2c0a 2020 2020   str = 'w',.    
+000029d0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+000029e0: 3a20 416e 790a 2020 2020 2920 2d3e 2062  : Any.    ) -> b
+000029f0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00002a00: 0a20 2020 2020 2020 2057 7269 7465 2064  .        Write d
+00002a10: 6174 6120 746f 2061 204a 534f 4e20 6669  ata to a JSON fi
+00002a20: 6c65 2e0a 0a20 2020 2020 2020 203a 7061  le...        :pa
+00002a30: 7261 6d20 6669 6c65 5f70 6174 683a 204e  ram file_path: N
+00002a40: 616d 6520 6f66 2074 6865 204a 534f 4e20  ame of the JSON 
+00002a50: 6669 6c65 2e0a 2020 2020 2020 2020 3a70  file..        :p
+00002a60: 6172 616d 2064 6174 613a 2044 6174 6120  aram data: Data 
+00002a70: 746f 2077 7269 7465 2028 7573 7561 6c6c  to write (usuall
+00002a80: 7920 6120 6469 6374 206f 7220 6120 6c69  y a dict or a li
+00002a90: 7374 292e 0a20 2020 2020 2020 203a 7061  st)..        :pa
+00002aa0: 7261 6d20 6170 705f 6c6f 673a 204f 7074  ram app_log: Opt
+00002ab0: 696f 6e61 6c20 6c6f 6767 6572 2066 6f72  ional logger for
+00002ac0: 206c 6f67 6769 6e67 2069 6e66 6f72 6d61   logging informa
+00002ad0: 7469 6f6e 2c20 6465 6661 756c 7473 2074  tion, defaults t
+00002ae0: 6f20 6120 6e65 7720 6c6f 6767 6572 2069  o a new logger i
+00002af0: 6620 4e6f 6e65 2e0a 2020 2020 2020 2020  f None..        
+00002b00: 3a70 6172 616d 206d 6f64 653a 204d 6f64  :param mode: Mod
+00002b10: 6520 696e 2077 6869 6368 2074 6865 2066  e in which the f
+00002b20: 696c 6520 7368 6f75 6c64 2062 6520 6f70  ile should be op
+00002b30: 656e 6564 2c20 6465 6661 756c 7473 2074  ened, defaults t
+00002b40: 6f20 2777 2720 666f 7220 7772 6974 6520  o 'w' for write 
+00002b50: 286f 7665 7277 7269 7469 6e67 292e 0a20  (overwriting).. 
+00002b60: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00002b70: 626f 6f6c 2077 6561 7468 6572 2073 7563  bool weather suc
+00002b80: 6365 7373 206f 7220 6661 696c 6564 0a20  cess or failed. 
+00002b90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00002ba0: 2020 2069 6620 6170 705f 6c6f 6720 6973     if app_log is
+00002bb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00002bc0: 2020 2061 7070 5f6c 6f67 203d 2063 6c73     app_log = cls
+00002bd0: 2e67 6574 5f6c 6f67 6765 7228 290a 0a20  .get_logger().. 
+00002be0: 2020 2020 2020 2061 7070 5f6c 6f67 2e64         app_log.d
+00002bf0: 6562 7567 2866 2757 7269 7469 6e67 2074  ebug(f'Writing t
+00002c00: 6f20 4a53 4f4e 2066 696c 653a 207b 6669  o JSON file: {fi
+00002c10: 6c65 5f70 6174 687d 2729 0a20 2020 2020  le_path}').     
+00002c20: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00002c30: 2020 2020 7769 7468 206f 7065 6e28 6669      with open(fi
+00002c40: 6c65 5f70 6174 682c 206d 6f64 652c 2065  le_path, mode, e
+00002c50: 6e63 6f64 696e 673d 2775 7466 2d38 2729  ncoding='utf-8')
+00002c60: 2061 7320 6670 3a0a 2020 2020 2020 2020   as fp:.        
+00002c70: 2020 2020 2020 2020 6a73 6f6e 2e64 756d          json.dum
+00002c80: 7028 6461 7461 2c20 6670 2c20 656e 7375  p(data, fp, ensu
+00002c90: 7265 5f61 7363 6969 3d46 616c 7365 2c20  re_ascii=False, 
+00002ca0: 696e 6465 6e74 3d34 2c20 2a2a 6b77 6172  indent=4, **kwar
+00002cb0: 6773 290a 2020 2020 2020 2020 6578 6365  gs).        exce
+00002cc0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00002cd0: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
+00002ce0: 6170 705f 6c6f 672e 6578 6365 7074 696f  app_log.exceptio
+00002cf0: 6e28 6622 416e 2065 7272 6f72 206f 6363  n(f"An error occ
+00002d00: 7572 7265 6420 7768 696c 6520 7772 6974  urred while writ
+00002d10: 696e 6720 746f 2074 6865 204a 534f 4e20  ing to the JSON 
+00002d20: 6669 6c65 3a20 7b65 787d 2229 0a20 2020  file: {ex}").   
+00002d30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002d40: 4661 6c73 650a 0a20 2020 2020 2020 2072  False..        r
+00002d50: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+00002d60: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00002d70: 2064 6566 2072 6561 645f 6a73 6f6e 5f64   def read_json_d
+00002d80: 6174 615f 6672 6f6d 5f66 696c 6528 0a20  ata_from_file(. 
+00002d90: 2020 2020 2020 2020 2020 2063 6c73 2c0a             cls,.
+00002da0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00002db0: 5f70 6174 683a 2073 7472 2c0a 2020 2020  _path: str,.    
+00002dc0: 2020 2020 2020 2020 6170 705f 6c6f 673a          app_log:
+00002dd0: 204f 7074 696f 6e61 6c5b 6c6f 6767 696e   Optional[loggin
+00002de0: 672e 4c6f 6767 6572 5d20 3d20 4e6f 6e65  g.Logger] = None
+00002df0: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
+00002e00: 6465 3a20 7374 7220 3d20 2772 272c 0a20  de: str = 'r',. 
+00002e10: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+00002e20: 7267 733a 2041 6e79 0a20 2020 2029 202d  rgs: Any.    ) -
+00002e30: 3e20 4f70 7469 6f6e 616c 5b41 6e79 5d3a  > Optional[Any]:
+00002e40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002e50: 2020 2020 2052 6561 6420 6461 7461 2066       Read data f
+00002e60: 726f 6d20 6120 4a53 4f4e 2066 696c 652e  rom a JSON file.
+00002e70: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00002e80: 2066 696c 655f 7061 7468 3a20 4e61 6d65   file_path: Name
+00002e90: 206f 6620 7468 6520 4a53 4f4e 2066 696c   of the JSON fil
+00002ea0: 652e 0a20 2020 2020 2020 203a 7061 7261  e..        :para
+00002eb0: 6d20 6170 705f 6c6f 673a 204f 7074 696f  m app_log: Optio
+00002ec0: 6e61 6c20 6c6f 6767 6572 2066 6f72 206c  nal logger for l
+00002ed0: 6f67 6769 6e67 2069 6e66 6f72 6d61 7469  ogging informati
+00002ee0: 6f6e 2c20 6465 6661 756c 7473 2074 6f20  on, defaults to 
+00002ef0: 6120 6e65 7720 6c6f 6767 6572 2069 6620  a new logger if 
+00002f00: 4e6f 6e65 2e0a 2020 2020 2020 2020 3a70  None..        :p
+00002f10: 6172 616d 206d 6f64 653a 204d 6f64 6520  aram mode: Mode 
+00002f20: 696e 2077 6869 6368 2074 6865 2066 696c  in which the fil
+00002f30: 6520 7368 6f75 6c64 2062 6520 6f70 656e  e should be open
+00002f40: 6564 2c20 6465 6661 756c 7473 2074 6f20  ed, defaults to 
+00002f50: 2772 2720 666f 7220 7265 6164 2e0a 2020  'r' for read..  
+00002f60: 2020 2020 2020 3a72 6574 7572 6e3a 2044        :return: D
+00002f70: 6174 6120 7265 6164 2066 726f 6d20 7468  ata read from th
+00002f80: 6520 4a53 4f4e 2066 696c 6520 6f72 204e  e JSON file or N
+00002f90: 6f6e 6520 6966 2061 6e20 6578 6365 7074  one if an except
+00002fa0: 696f 6e20 6f63 6375 7273 2e0a 2020 2020  ion occurs..    
+00002fb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00002fc0: 6966 2061 7070 5f6c 6f67 2069 7320 4e6f  if app_log is No
+00002fd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00002fe0: 6170 705f 6c6f 6720 3d20 636c 732e 6765  app_log = cls.ge
+00002ff0: 745f 6c6f 6767 6572 2829 0a0a 2020 2020  t_logger()..    
+00003000: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00003010: 2020 2020 2077 6974 6820 6f70 656e 2866       with open(f
+00003020: 696c 655f 7061 7468 2c20 6d6f 6465 2c20  ile_path, mode, 
+00003030: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
+00003040: 2c20 2a2a 6b77 6172 6773 2920 6173 2066  , **kwargs) as f
+00003050: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00003060: 2020 2061 7070 5f6c 6f67 2e64 6562 7567     app_log.debug
+00003070: 2866 2752 6561 6469 6e67 2066 726f 6d20  (f'Reading from 
+00003080: 4a53 4f4e 2066 696c 653a 207b 6669 6c65  JSON file: {file
+00003090: 5f70 6174 687d 2729 0a20 2020 2020 2020  _path}').       
+000030a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000030b0: 6a73 6f6e 2e6c 6f61 6428 6670 290a 2020  json.load(fp).  
+000030c0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+000030d0: 6570 7469 6f6e 2061 7320 6578 3a0a 2020  eption as ex:.  
+000030e0: 2020 2020 2020 2020 2020 6170 705f 6c6f            app_lo
+000030f0: 672e 6578 6365 7074 696f 6e28 6622 416e  g.exception(f"An
+00003100: 2065 7272 6f72 206f 6363 7572 7265 6420   error occurred 
+00003110: 7768 696c 6520 7265 6164 696e 6720 7468  while reading th
+00003120: 6520 4a53 4f4e 2066 696c 653a 207b 6578  e JSON file: {ex
+00003130: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+00003140: 7265 7475 726e 204e 6f6e 650a 0a0a 636c  return None...cl
+00003150: 6173 7320 4d6f 6465 6c55 7469 6c3a 0a20  ass ModelUtil:. 
+00003160: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00003170: 0a20 2020 2064 6566 2065 7870 6f6e 656e  .    def exponen
+00003180: 7469 616c 5f6d 6f76 696e 675f 6176 6572  tial_moving_aver
+00003190: 6167 655f 6e65 7874 5f76 616c 7565 280a  age_next_value(.
+000031a0: 2020 2020 2020 2020 2020 2020 6e75 6d65              nume
+000031b0: 7269 635f 7365 7175 656e 6365 3a20 4c69  ric_sequence: Li
+000031c0: 7374 5b69 6e74 5d2c 0a20 2020 2020 2020  st[int],.       
+000031d0: 2020 2020 2073 7061 6e3a 2069 6e74 203d       span: int =
+000031e0: 2035 2c0a 2020 2020 2020 2020 2020 2020   5,.            
+000031f0: 656e 6162 6c65 5f72 6f6c 6c69 6e67 5f64  enable_rolling_d
+00003200: 6966 6665 7265 6e63 653a 2062 6f6f 6c20  ifference: bool 
+00003210: 3d20 4661 6c73 650a 2020 2020 2920 2d3e  = False.    ) ->
+00003220: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00003230: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
+00003240: 6174 6520 7468 6520 4578 706f 6e65 6e74  ate the Exponent
+00003250: 6961 6c20 4d6f 7669 6e67 2041 7665 7261  ial Moving Avera
+00003260: 6765 2028 454d 4129 2061 6e64 2075 7365  ge (EMA) and use
+00003270: 2072 6f6c 6c69 6e67 2064 6966 6665 7265   rolling differe
+00003280: 6e63 6520 746f 2070 7265 6469 6374 2074  nce to predict t
+00003290: 6865 206e 6578 7420 7661 6c75 6520 6f66  he next value of
+000032a0: 2061 2073 6571 7565 6e63 652e 0a0a 2020   a sequence...  
+000032b0: 2020 2020 2020 454d 4120 6973 2061 2074        EMA is a t
+000032c0: 7970 6520 6f66 206d 6f76 696e 6720 6176  ype of moving av
+000032d0: 6572 6167 6520 7468 6174 2070 6c61 6365  erage that place
+000032e0: 7320 6120 6772 6561 7465 7220 7765 6967  s a greater weig
+000032f0: 6874 2061 6e64 2073 6967 6e69 6669 6361  ht and significa
+00003300: 6e63 650a 2020 2020 2020 2020 6f6e 2074  nce.        on t
+00003310: 6865 206d 6f73 7420 7265 6365 6e74 2064  he most recent d
+00003320: 6174 6120 706f 696e 7473 2e20 4974 2773  ata points. It's
+00003330: 206d 6f72 6520 7265 7370 6f6e 7369 7665   more responsive
+00003340: 2074 6f20 6e65 7720 696e 666f 726d 6174   to new informat
+00003350: 696f 6e20 636f 6d70 6172 6564 0a20 2020  ion compared.   
+00003360: 2020 2020 2074 6f20 6120 7369 6d70 6c65       to a simple
+00003370: 206d 6f76 696e 6720 6176 6572 6167 6520   moving average 
+00003380: 2853 4d41 292e 0a0a 2020 2020 2020 2020  (SMA)...        
+00003390: 3a70 6172 616d 206e 756d 6572 6963 5f73  :param numeric_s
+000033a0: 6571 7565 6e63 653a 2041 206c 6973 7420  equence: A list 
+000033b0: 6f72 2073 6571 7565 6e63 6520 6f66 206e  or sequence of n
+000033c0: 756d 6265 7273 2066 6f72 2077 6869 6368  umbers for which
+000033d0: 2074 6865 2045 4d41 2069 7320 746f 2062   the EMA is to b
+000033e0: 6520 6361 6c63 756c 6174 6564 2e0a 2020  e calculated..  
+000033f0: 2020 2020 2020 3a70 6172 616d 2073 7061        :param spa
+00003400: 6e3a 2054 6865 206e 756d 6265 7220 6f66  n: The number of
+00003410: 2070 6572 696f 6473 206f 7665 7220 7768   periods over wh
+00003420: 6963 6820 746f 2063 616c 6375 6c61 7465  ich to calculate
+00003430: 2074 6865 2045 4d41 2e20 4465 6661 756c   the EMA. Defaul
+00003440: 7420 6973 2035 2e0a 2020 2020 2020 2020  t is 5..        
+00003450: 3a70 6172 616d 2065 6e61 626c 655f 726f  :param enable_ro
+00003460: 6c6c 696e 675f 6469 6666 6572 656e 6365  lling_difference
+00003470: 3a20 7765 6174 6865 7220 746f 2065 6e61  : weather to ena
+00003480: 626c 6520 726f 6c6c 696e 672e 2064 6566  ble rolling. def
+00003490: 6175 6c74 2069 7320 4661 6c73 650a 2020  ault is False.  
+000034a0: 2020 2020 2020 3a72 6574 7572 6e3a 2050        :return: P
+000034b0: 7265 6469 6374 6564 206e 6578 7420 7661  redicted next va
+000034c0: 6c75 6520 6f66 2074 6865 2073 6571 7565  lue of the seque
+000034d0: 6e63 6520 6261 7365 6420 6f6e 2045 4d41  nce based on EMA
+000034e0: 2061 6e64 2072 6f6c 6c69 6e67 2064 6966   and rolling dif
+000034f0: 6665 7265 6e63 652e 0a20 2020 2020 2020  ference..       
+00003500: 203a 7261 6973 6573 2056 616c 7565 4572   :raises ValueEr
+00003510: 726f 723a 2049 6620 7468 6520 696e 7075  ror: If the inpu
+00003520: 7420 6c69 7374 2069 7320 656d 7074 7920  t list is empty 
+00003530: 6f72 2063 6f6e 7461 696e 7320 6e6f 6e2d  or contains non-
+00003540: 6e75 6d65 7269 6320 7661 6c75 6573 2e0a  numeric values..
+00003550: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003560: 2020 2020 6966 206e 6f74 206e 756d 6572      if not numer
+00003570: 6963 5f73 6571 7565 6e63 653a 0a20 2020  ic_sequence:.   
+00003580: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00003590: 616c 7565 4572 726f 7228 2254 6865 206e  alueError("The n
+000035a0: 756d 6572 6963 2073 6571 7565 6e63 6520  umeric sequence 
+000035b0: 6361 6e6e 6f74 2062 6520 656d 7074 792e  cannot be empty.
+000035c0: 2229 0a20 2020 2020 2020 2069 6620 6e6f  ").        if no
+000035d0: 7420 616c 6c28 6973 696e 7374 616e 6365  t all(isinstance
+000035e0: 2878 2c20 2869 6e74 2c20 666c 6f61 7429  (x, (int, float)
+000035f0: 2920 666f 7220 7820 696e 206e 756d 6572  ) for x in numer
+00003600: 6963 5f73 6571 7565 6e63 6529 3a0a 2020  ic_sequence):.  
+00003610: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00003620: 5661 6c75 6545 7272 6f72 2822 416c 6c20  ValueError("All 
+00003630: 656c 656d 656e 7473 2069 6e20 7468 6520  elements in the 
+00003640: 6e75 6d65 7269 6320 7365 7175 656e 6365  numeric sequence
+00003650: 206d 7573 7420 6265 206e 756d 6265 7273   must be numbers
+00003660: 2e22 290a 0a20 2020 2020 2020 2023 2043  .")..        # C
+00003670: 6f6e 7665 7274 2074 6865 206e 756d 6572  onvert the numer
+00003680: 6963 2073 6571 7565 6e63 6520 696e 746f  ic sequence into
+00003690: 2061 2070 616e 6461 7320 5365 7269 6573   a pandas Series
+000036a0: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
+000036b0: 7365 7269 6573 203d 2070 642e 5365 7269  series = pd.Seri
+000036c0: 6573 286e 756d 6572 6963 5f73 6571 7565  es(numeric_seque
+000036d0: 6e63 6529 0a0a 2020 2020 2020 2020 2320  nce)..        # 
+000036e0: 4361 6c63 756c 6174 6520 7468 6520 454d  Calculate the EM
+000036f0: 4120 7573 696e 6720 7061 6e64 6173 2720  A using pandas' 
+00003700: 6577 6d20 6d65 7468 6f64 0a20 2020 2020  ewm method.     
+00003710: 2020 2023 2041 646a 7573 7420 276d 696e     # Adjust 'min
+00003720: 5f70 6572 696f 6473 2720 746f 2068 616e  _periods' to han
+00003730: 646c 6520 7368 6f72 7465 7220 7365 7175  dle shorter sequ
+00003740: 656e 6365 7320 6772 6163 6566 756c 6c79  ences gracefully
+00003750: 0a20 2020 2020 2020 2065 6d61 203d 2073  .        ema = s
+00003760: 6572 6965 732e 6577 6d28 7370 616e 3d73  eries.ewm(span=s
+00003770: 7061 6e2c 206d 696e 5f70 6572 696f 6473  pan, min_periods
+00003780: 3d6d 696e 2873 7061 6e2c 206c 656e 286e  =min(span, len(n
+00003790: 756d 6572 6963 5f73 6571 7565 6e63 6529  umeric_sequence)
+000037a0: 292c 2061 646a 7573 743d 4661 6c73 6529  ), adjust=False)
+000037b0: 2e6d 6561 6e28 290a 0a20 2020 2020 2020  .mean()..       
+000037c0: 2023 2043 616c 6375 6c61 7465 2072 6f6c   # Calculate rol
+000037d0: 6c69 6e67 2064 6966 6665 7265 6e63 650a  ling difference.
+000037e0: 2020 2020 2020 2020 726f 6c6c 696e 675f          rolling_
+000037f0: 6469 6666 6572 656e 6365 203d 2073 6572  difference = ser
+00003800: 6965 732e 6469 6666 2829 0a0a 2020 2020  ies.diff()..    
+00003810: 2020 2020 2320 5072 6564 6963 7420 7468      # Predict th
+00003820: 6520 6e65 7874 2076 616c 7565 2062 7920  e next value by 
+00003830: 6578 7472 6170 6f6c 6174 696e 6720 7468  extrapolating th
+00003840: 6520 6c61 7374 2072 6f6c 6c69 6e67 2064  e last rolling d
+00003850: 6966 6665 7265 6e63 6520 616e 6420 7468  ifference and th
+00003860: 6520 6c61 7374 2045 4d41 2076 616c 7565  e last EMA value
+00003870: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00003880: 726f 6c6c 696e 675f 6469 6666 6572 656e  rolling_differen
+00003890: 6365 2920 3e20 3120 616e 6420 656e 6162  ce) > 1 and enab
+000038a0: 6c65 5f72 6f6c 6c69 6e67 5f64 6966 6665  le_rolling_diffe
+000038b0: 7265 6e63 6520 6973 2054 7275 653a 0a20  rence is True:. 
+000038c0: 2020 2020 2020 2020 2020 2070 7265 6469             predi
+000038d0: 6374 6564 5f6e 6578 745f 7661 6c75 6520  cted_next_value 
+000038e0: 3d20 656d 612e 696c 6f63 5b2d 315d 202b  = ema.iloc[-1] +
+000038f0: 2072 6f6c 6c69 6e67 5f64 6966 6665 7265   rolling_differe
+00003900: 6e63 652e 696c 6f63 5b2d 315d 0a20 2020  nce.iloc[-1].   
+00003910: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00003920: 2020 2020 2020 2023 2049 6620 7468 6572         # If ther
+00003930: 6527 7320 6e6f 2065 6e6f 7567 6820 6461  e's no enough da
+00003940: 7461 2074 6f20 6361 6c63 756c 6174 6520  ta to calculate 
+00003950: 6469 6666 6572 656e 6365 2c20 7573 6520  difference, use 
+00003960: 7468 6520 6c61 7374 2045 4d41 2061 7320  the last EMA as 
+00003970: 7468 6520 7072 6564 6963 7469 6f6e 0a20  the prediction. 
+00003980: 2020 2020 2020 2020 2020 2070 7265 6469             predi
+00003990: 6374 6564 5f6e 6578 745f 7661 6c75 6520  cted_next_value 
+000039a0: 3d20 656d 612e 696c 6f63 5b2d 315d 0a0a  = ema.iloc[-1]..
+000039b0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+000039c0: 2074 6865 2070 7265 6469 6374 6564 206e   the predicted n
+000039d0: 6578 7420 7661 6c75 6520 726f 756e 6465  ext value rounde
+000039e0: 6420 746f 2074 6865 206e 6561 7265 7374  d to the nearest
+000039f0: 2069 6e74 6567 6572 0a20 2020 2020 2020   integer.       
+00003a00: 2072 6574 7572 6e20 4361 6c63 756c 6174   return Calculat
+00003a10: 6555 7469 6c2e 7265 616c 5f72 6f75 6e64  eUtil.real_round
+00003a20: 2870 7265 6469 6374 6564 5f6e 6578 745f  (predicted_next_
+00003a30: 7661 6c75 6529 0a0a 2020 2020 4073 7461  value)..    @sta
+00003a40: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
+00003a50: 6620 6c69 6e65 6172 5f72 6567 7265 7373  f linear_regress
+00003a60: 696f 6e5f 6e65 7874 5f76 616c 7565 5f62  ion_next_value_b
+00003a70: 795f 696e 6465 7828 6e75 6d65 7269 635f  y_index(numeric_
+00003a80: 7365 7175 656e 6365 3a20 4c69 7374 5b69  sequence: List[i
+00003a90: 6e74 5d29 202d 3e20 696e 743a 0a20 2020  nt]) -> int:.   
+00003aa0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003ab0: 2050 7265 6469 6374 7320 7468 6520 6e65   Predicts the ne
+00003ac0: 7874 2076 616c 7565 2069 6e20 6120 7365  xt value in a se
+00003ad0: 7175 656e 6365 2075 7369 6e67 206c 696e  quence using lin
+00003ae0: 6561 7220 7265 6772 6573 7369 6f6e 2e0a  ear regression..
+00003af0: 0a20 2020 2020 2020 204c 696e 6561 7220  .        Linear 
+00003b00: 7265 6772 6573 7369 6f6e 2069 6e76 6f6c  regression invol
+00003b10: 7665 7320 6669 7474 696e 6720 6120 6c69  ves fitting a li
+00003b20: 6e65 2074 6f20 7468 6520 6461 7461 2070  ne to the data p
+00003b30: 6f69 6e74 7320 696e 2073 7563 6820 6120  oints in such a 
+00003b40: 7761 790a 2020 2020 2020 2020 7468 6174  way.        that
+00003b50: 2074 6865 2064 6973 7461 6e63 6520 6265   the distance be
+00003b60: 7477 6565 6e20 7468 6520 6461 7461 2070  tween the data p
+00003b70: 6f69 6e74 7320 616e 6420 7468 6520 6c69  oints and the li
+00003b80: 6e65 2069 7320 6d69 6e69 6d69 7a65 642e  ne is minimized.
+00003b90: 2054 6869 7320 6675 6e63 7469 6f6e 0a20   This function. 
+00003ba0: 2020 2020 2020 2075 7365 7320 7468 6520         uses the 
+00003bb0: 6d65 7468 6f64 2074 6f20 7072 6564 6963  method to predic
+00003bc0: 7420 7468 6520 6e65 7874 2076 616c 7565  t the next value
+00003bd0: 2069 6e20 6120 6769 7665 6e20 7365 7175   in a given sequ
+00003be0: 656e 6365 206f 6620 6e75 6d62 6572 7320  ence of numbers 
+00003bf0: 6279 2066 6974 7469 6e67 0a20 2020 2020  by fitting.     
+00003c00: 2020 2061 206d 6f64 656c 2074 6f20 7468     a model to th
+00003c10: 6520 7365 7175 656e 6365 2061 6e64 2065  e sequence and e
+00003c20: 7861 6d69 6e69 6e67 2074 6865 2073 6c6f  xamining the slo
+00003c30: 7065 206f 6620 7468 6520 6c69 6e65 2e0a  pe of the line..
+00003c40: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003c50: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
+00003c60: 3a20 4120 6c69 7374 206f 7220 7365 7175  : A list or sequ
+00003c70: 656e 6365 206f 6620 6e75 6d62 6572 7320  ence of numbers 
+00003c80: 746f 206d 6f64 656c 2e0a 2020 2020 2020  to model..      
+00003c90: 2020 3a72 6574 7572 6e3a 2054 6865 2070    :return: The p
+00003ca0: 7265 6469 6374 6564 206e 6578 7420 7661  redicted next va
+00003cb0: 6c75 6520 696e 2074 6865 2073 6571 7565  lue in the seque
+00003cc0: 6e63 6520 6173 2061 6e20 696e 7465 6765  nce as an intege
+00003cd0: 722e 0a20 2020 2020 2020 203a 7261 6973  r..        :rais
+00003ce0: 6573 2056 616c 7565 4572 726f 723a 2049  es ValueError: I
+00003cf0: 6620 7468 6520 696e 7075 7420 7365 7175  f the input sequ
+00003d00: 656e 6365 2069 7320 656d 7074 7920 6f72  ence is empty or
+00003d10: 2074 6f6f 2073 686f 7274 2066 6f72 2072   too short for r
+00003d20: 6567 7265 7373 696f 6e20 616e 616c 7973  egression analys
+00003d30: 6973 2e0a 2020 2020 2020 2020 2222 220a  is..        """.
+00003d40: 2020 2020 2020 2020 6966 206e 6f74 206e          if not n
+00003d50: 756d 6572 6963 5f73 6571 7565 6e63 653a  umeric_sequence:
+00003d60: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00003d70: 7365 2056 616c 7565 4572 726f 7228 2254  se ValueError("T
+00003d80: 6865 206e 756d 6572 6963 2073 6571 7565  he numeric seque
+00003d90: 6e63 6520 6361 6e6e 6f74 2062 6520 656d  nce cannot be em
+00003da0: 7074 792e 2229 0a20 2020 2020 2020 2069  pty.").        i
+00003db0: 6620 6c65 6e28 6e75 6d65 7269 635f 7365  f len(numeric_se
+00003dc0: 7175 656e 6365 2920 3c20 323a 0a20 2020  quence) < 2:.   
+00003dd0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00003de0: 616c 7565 4572 726f 7228 2254 6865 206e  alueError("The n
+00003df0: 756d 6572 6963 2073 6571 7565 6e63 6520  umeric sequence 
+00003e00: 6d75 7374 2063 6f6e 7461 696e 2061 7420  must contain at 
+00003e10: 6c65 6173 7420 7477 6f20 656c 656d 656e  least two elemen
+00003e20: 7473 2066 6f72 206c 696e 6561 7220 7265  ts for linear re
+00003e30: 6772 6573 7369 6f6e 2e22 290a 0a20 2020  gression.")..   
+00003e40: 2020 2020 2023 2043 6f6e 7665 7274 2074       # Convert t
+00003e50: 6865 206e 756d 6572 6963 2073 6571 7565  he numeric seque
+00003e60: 6e63 6520 696e 746f 2061 206e 756d 7079  nce into a numpy
+00003e70: 2061 7272 6179 2061 6e64 2072 6573 6861   array and resha
+00003e80: 7065 2066 6f72 2073 6b6c 6561 726e 0a20  pe for sklearn. 
+00003e90: 2020 2020 2020 2064 6174 6120 3d20 6e70         data = np
+00003ea0: 2e61 7272 6179 286e 756d 6572 6963 5f73  .array(numeric_s
+00003eb0: 6571 7565 6e63 6529 2e72 6573 6861 7065  equence).reshape
+00003ec0: 282d 312c 2031 290a 0a20 2020 2020 2020  (-1, 1)..       
+00003ed0: 2023 2043 7265 6174 6520 616e 2061 7272   # Create an arr
+00003ee0: 6179 2072 6570 7265 7365 6e74 696e 6720  ay representing 
+00003ef0: 7469 6d65 206f 7220 7468 6520 696e 6465  time or the inde
+00003f00: 7065 6e64 656e 7420 7661 7269 6162 6c65  pendent variable
+00003f10: 2c20 7265 7368 6170 6564 2061 7320 6120  , reshaped as a 
+00003f20: 636f 6c75 6d6e 0a20 2020 2020 2020 2069  column.        i
+00003f30: 6e64 6578 203d 206e 702e 6172 7261 7928  ndex = np.array(
+00003f40: 7261 6e67 6528 6c65 6e28 6461 7461 2929  range(len(data))
+00003f50: 292e 7265 7368 6170 6528 2d31 2c20 3129  ).reshape(-1, 1)
+00003f60: 0a0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
+00003f70: 7465 2061 204c 696e 6561 7252 6567 7265  te a LinearRegre
+00003f80: 7373 696f 6e20 6d6f 6465 6c20 616e 6420  ssion model and 
+00003f90: 6669 7420 6974 2074 6f20 7468 6520 6461  fit it to the da
+00003fa0: 7461 0a20 2020 2020 2020 206d 6f64 656c  ta.        model
+00003fb0: 203d 204c 696e 6561 7252 6567 7265 7373   = LinearRegress
+00003fc0: 696f 6e28 290a 2020 2020 2020 2020 6d6f  ion().        mo
+00003fd0: 6465 6c2e 6669 7428 696e 6465 782c 2064  del.fit(index, d
+00003fe0: 6174 6129 0a0a 2020 2020 2020 2020 2320  ata)..        # 
+00003ff0: 5072 6564 6963 7420 7468 6520 6e65 7874  Predict the next
+00004000: 2076 616c 7565 2069 6e20 7468 6520 7365   value in the se
+00004010: 7175 656e 6365 2075 7369 6e67 2074 6865  quence using the
+00004020: 2066 6974 7465 6420 6d6f 6465 6c0a 2020   fitted model.  
+00004030: 2020 2020 2020 7072 6564 6963 7469 6f6e        prediction
+00004040: 203d 206d 6f64 656c 2e70 7265 6469 6374   = model.predict
+00004050: 285b 5b6c 656e 2864 6174 6129 5d5d 295b  ([[len(data)]])[
+00004060: 305d 5b30 5d0a 0a20 2020 2020 2020 2023  0][0]..        #
+00004070: 2052 6574 7572 6e20 7468 6520 7072 6564   Return the pred
+00004080: 6963 7465 6420 7661 6c75 6520 6173 2061  icted value as a
+00004090: 6e20 696e 7465 6765 720a 2020 2020 2020  n integer.      
+000040a0: 2020 7265 7475 726e 2043 616c 6375 6c61    return Calcula
+000040b0: 7465 5574 696c 2e72 6561 6c5f 726f 756e  teUtil.real_roun
+000040c0: 6428 7072 6564 6963 7469 6f6e 290a 0a20  d(prediction).. 
+000040d0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+000040e0: 0a20 2020 2064 6566 206d 756c 7469 7661  .    def multiva
+000040f0: 7269 6174 655f 706f 6c79 6e6f 6d69 616c  riate_polynomial
+00004100: 5f72 6567 7265 7373 696f 6e5f 6e65 7874  _regression_next
+00004110: 5f76 616c 7565 280a 2020 2020 2020 2020  _value(.        
+00004120: 2020 2020 6e75 6d65 7269 635f 7365 7175      numeric_sequ
+00004130: 656e 6365 3a20 4c69 7374 5b69 6e74 5d2c  ence: List[int],
+00004140: 0a20 2020 2020 2020 2020 2020 2072 6f6c  .            rol
+00004150: 6c69 6e67 5f73 697a 653a 2069 6e74 203d  ling_size: int =
+00004160: 2033 2c0a 2020 2020 2020 2020 2020 2020   3,.            
+00004170: 6465 6772 6565 733a 2069 6e74 203d 2033  degrees: int = 3
+00004180: 2c0a 2020 2020 2920 2d3e 2066 6c6f 6174  ,.    ) -> float
+00004190: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000041a0: 2020 2020 2020 5072 6564 6963 7473 2074        Predicts t
+000041b0: 6865 206e 6578 7420 7661 6c75 6520 696e  he next value in
+000041c0: 2061 206e 756d 6572 6963 2073 6571 7565   a numeric seque
+000041d0: 6e63 6520 7573 696e 6720 6d75 6c74 6976  nce using multiv
+000041e0: 6172 6961 7465 2070 6f6c 796e 6f6d 6961  ariate polynomia
+000041f0: 6c20 7265 6772 6573 7369 6f6e 2e0a 0a20  l regression... 
+00004200: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+00004210: 6f64 2061 7070 6c69 6573 2061 2070 6f6c  od applies a pol
+00004220: 796e 6f6d 6961 6c20 7265 6772 6573 7369  ynomial regressi
+00004230: 6f6e 206d 6f64 656c 2074 6f20 6120 6e75  on model to a nu
+00004240: 6d65 7269 6320 7365 7175 656e 6365 2074  meric sequence t
+00004250: 6f20 7072 6564 6963 7420 7468 6520 6e65  o predict the ne
+00004260: 7874 2076 616c 7565 2e0a 2020 2020 2020  xt value..      
+00004270: 2020 4974 2075 7469 6c69 7a65 7320 6120    It utilizes a 
+00004280: 726f 6c6c 696e 6720 7769 6e64 6f77 2061  rolling window a
+00004290: 7070 726f 6163 6820 746f 2063 7265 6174  pproach to creat
+000042a0: 6520 6461 7461 7365 7473 2c20 7363 616c  e datasets, scal
+000042b0: 6573 2074 6865 2066 6561 7475 7265 732c  es the features,
+000042c0: 2061 6e64 2066 6974 7320 6120 706f 6c79   and fits a poly
+000042d0: 6e6f 6d69 616c 0a20 2020 2020 2020 2072  nomial.        r
+000042e0: 6567 7265 7373 696f 6e20 6d6f 6465 6c20  egression model 
+000042f0: 746f 206d 616b 6520 7468 6520 7072 6564  to make the pred
+00004300: 6963 7469 6f6e 2e0a 0a20 2020 2020 2020  iction...       
+00004310: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00004320: 2020 206e 756d 6572 6963 5f73 6571 7565     numeric_seque
+00004330: 6e63 6520 284c 6973 745b 696e 745d 293a  nce (List[int]):
+00004340: 2054 6865 206c 6973 7420 6f66 2069 6e74   The list of int
+00004350: 6567 6572 7320 7265 7072 6573 656e 7469  egers representi
+00004360: 6e67 2074 6865 2073 6571 7565 6e63 652e  ng the sequence.
+00004370: 0a20 2020 2020 2020 2020 2020 2072 6f6c  .            rol
+00004380: 6c69 6e67 5f73 697a 6520 2869 6e74 293a  ling_size (int):
+00004390: 2054 6865 206e 756d 6265 7220 6f66 2065   The number of e
+000043a0: 6c65 6d65 6e74 7320 696e 2065 6163 6820  lements in each 
+000043b0: 726f 6c6c 696e 6720 7769 6e64 6f77 2e0a  rolling window..
+000043c0: 2020 2020 2020 2020 2020 2020 6465 6772              degr
+000043d0: 6565 7320 2869 6e74 293a 2054 6865 2064  ees (int): The d
+000043e0: 6567 7265 6520 6f66 2074 6865 2070 6f6c  egree of the pol
+000043f0: 796e 6f6d 6961 6c20 7265 6772 6573 7369  ynomial regressi
+00004400: 6f6e 2e20 4465 6661 756c 7473 2074 6f20  on. Defaults to 
+00004410: 332e 0a0a 2020 2020 2020 2020 5265 7475  3...        Retu
+00004420: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00004430: 2066 6c6f 6174 3a20 5468 6520 7072 6564   float: The pred
+00004440: 6963 7465 6420 6e65 7874 2076 616c 7565  icted next value
+00004450: 2069 6e20 7468 6520 7365 7175 656e 6365   in the sequence
+00004460: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00004470: 733a 0a20 2020 2020 2020 2020 2020 2056  s:.            V
+00004480: 616c 7565 4572 726f 723a 2049 6620 7468  alueError: If th
+00004490: 6520 726f 6c6c 696e 675f 7369 7a65 2069  e rolling_size i
+000044a0: 7320 6c61 7267 6572 2074 6861 6e20 7468  s larger than th
+000044b0: 6520 7369 7a65 206f 6620 6e75 6d65 7269  e size of numeri
+000044c0: 635f 7365 7175 656e 6365 2e0a 2020 2020  c_sequence..    
+000044d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000044e0: 6966 2072 6f6c 6c69 6e67 5f73 697a 6520  if rolling_size 
+000044f0: 3e20 6c65 6e28 6e75 6d65 7269 635f 7365  > len(numeric_se
+00004500: 7175 656e 6365 293a 0a20 2020 2020 2020  quence):.       
+00004510: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00004520: 4572 726f 7228 2272 6f6c 6c69 6e67 5f73  Error("rolling_s
+00004530: 697a 6520 6361 6e6e 6f74 2062 6520 6c61  ize cannot be la
+00004540: 7267 6572 2074 6861 6e20 7468 6520 7369  rger than the si
+00004550: 7a65 206f 6620 6e75 6d65 7269 635f 7365  ze of numeric_se
+00004560: 7175 656e 6365 2229 0a0a 2020 2020 2020  quence")..      
+00004570: 2020 2320 4765 6e65 7261 7465 2064 6174    # Generate dat
+00004580: 6173 6574 7320 7769 7468 2074 6865 2073  asets with the s
+00004590: 7065 6369 6669 6564 2072 6f6c 6c69 6e67  pecified rolling
+000045a0: 2073 697a 650a 2020 2020 2020 2020 7472   size.        tr
+000045b0: 6169 6e5f 782c 2074 7261 696e 5f79 203d  ain_x, train_y =
+000045c0: 2043 616c 6375 6c61 7465 5574 696c 2e67   CalculateUtil.g
+000045d0: 656e 6572 6174 655f 6461 7461 7365 7473  enerate_datasets
+000045e0: 5f77 6974 685f 726f 6c6c 696e 675f 7369  _with_rolling_si
+000045f0: 7a65 280a 2020 2020 2020 2020 2020 2020  ze(.            
+00004600: 6461 7461 3d6e 756d 6572 6963 5f73 6571  data=numeric_seq
+00004610: 7565 6e63 652c 2072 6f6c 6c69 6e67 5f73  uence, rolling_s
+00004620: 697a 653d 726f 6c6c 696e 675f 7369 7a65  ize=rolling_size
+00004630: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00004640: 2020 2020 2320 5072 6570 6172 696e 6720      # Preparing 
+00004650: 696e 7075 7420 6461 7461 2066 6f72 206d  input data for m
+00004660: 6f64 656c 2074 7261 696e 696e 670a 2020  odel training.  
+00004670: 2020 2020 2020 696e 7075 745f 7820 3d20        input_x = 
+00004680: 6e70 2e61 7272 6179 2874 7261 696e 5f78  np.array(train_x
+00004690: 290a 2020 2020 2020 2020 6f75 7470 7574  ).        output
+000046a0: 5f79 203d 206e 702e 6172 7261 7928 7472  _y = np.array(tr
+000046b0: 6169 6e5f 7929 0a0a 2020 2020 2020 2020  ain_y)..        
+000046c0: 2320 5363 616c 696e 6720 7468 6520 6665  # Scaling the fe
+000046d0: 6174 7572 6573 0a20 2020 2020 2020 2073  atures.        s
+000046e0: 6361 6c65 7220 3d20 5374 616e 6461 7264  caler = Standard
+000046f0: 5363 616c 6572 2829 0a20 2020 2020 2020  Scaler().       
+00004700: 2069 6e70 7574 5f78 5f73 6361 6c65 6420   input_x_scaled 
+00004710: 3d20 7363 616c 6572 2e66 6974 5f74 7261  = scaler.fit_tra
+00004720: 6e73 666f 726d 2869 6e70 7574 5f78 290a  nsform(input_x).
+00004730: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+00004740: 696e 6720 616e 6420 7472 6169 6e69 6e67  ing and training
+00004750: 2074 6865 2070 6f6c 796e 6f6d 6961 6c20   the polynomial 
+00004760: 7265 6772 6573 7369 6f6e 206d 6f64 656c  regression model
+00004770: 0a20 2020 2020 2020 206d 6f64 656c 203d  .        model =
+00004780: 206d 616b 655f 7069 7065 6c69 6e65 2850   make_pipeline(P
+00004790: 6f6c 796e 6f6d 6961 6c46 6561 7475 7265  olynomialFeature
+000047a0: 7328 6465 6772 6565 7329 2c20 4c69 6e65  s(degrees), Line
+000047b0: 6172 5265 6772 6573 7369 6f6e 2829 290a  arRegression()).
+000047c0: 2020 2020 2020 2020 6d6f 6465 6c2e 6669          model.fi
+000047d0: 7428 696e 7075 745f 785f 7363 616c 6564  t(input_x_scaled
+000047e0: 2c20 6f75 7470 7574 5f79 290a 0a20 2020  , output_y)..   
+000047f0: 2020 2020 2023 2050 7265 7061 7269 6e67       # Preparing
+00004800: 2074 6865 206c 6173 7420 726f 6c6c 696e   the last rollin
+00004810: 6720 7769 6e64 6f77 206f 6620 6461 7461  g window of data
+00004820: 2066 6f72 2070 7265 6469 6374 696f 6e0a   for prediction.
+00004830: 2020 2020 2020 2020 7465 7374 5f78 203d          test_x =
+00004840: 206e 702e 6172 7261 7928 5b6e 756d 6572   np.array([numer
+00004850: 6963 5f73 6571 7565 6e63 655b 2d72 6f6c  ic_sequence[-rol
+00004860: 6c69 6e67 5f73 697a 653a 5d5d 290a 2020  ling_size:]]).  
+00004870: 2020 2020 2020 7465 7374 5f78 5f73 6361        test_x_sca
+00004880: 6c65 6420 3d20 7363 616c 6572 2e74 7261  led = scaler.tra
+00004890: 6e73 666f 726d 2874 6573 745f 7829 0a0a  nsform(test_x)..
+000048a0: 2020 2020 2020 2020 2320 5072 6564 6963          # Predic
+000048b0: 7469 6e67 2074 6865 206e 6578 7420 7661  ting the next va
+000048c0: 6c75 650a 2020 2020 2020 2020 7072 6564  lue.        pred
+000048d0: 5f79 203d 206d 6f64 656c 2e70 7265 6469  _y = model.predi
+000048e0: 6374 2874 6573 745f 785f 7363 616c 6564  ct(test_x_scaled
+000048f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00004900: 2070 7265 645f 795b 305d 0a0a 2020 2020   pred_y[0]..    
+00004910: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00004920: 2020 6465 6620 6861 726d 6f6e 6963 5f72    def harmonic_r
+00004930: 6567 7265 7373 696f 6e5f 6e65 7874 5f76  egression_next_v
+00004940: 616c 7565 5f62 795f 696e 6465 7828 6e75  alue_by_index(nu
+00004950: 6d65 7269 635f 7365 7175 656e 6365 3a20  meric_sequence: 
+00004960: 4c69 7374 5b69 6e74 5d2c 2066 7265 7175  List[int], frequ
+00004970: 656e 6379 3a20 666c 6f61 7420 3d20 312e  ency: float = 1.
+00004980: 3029 202d 3e20 696e 743a 0a20 2020 2020  0) -> int:.     
+00004990: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
+000049a0: 7265 6469 6374 7320 7468 6520 6e65 7874  redicts the next
+000049b0: 2076 616c 7565 2069 6e20 6120 7365 7175   value in a sequ
+000049c0: 656e 6365 2075 7369 6e67 2068 6172 6d6f  ence using harmo
+000049d0: 6e69 6320 7265 6772 6573 7369 6f6e 2e0a  nic regression..
+000049e0: 0a20 2020 2020 2020 2048 6172 6d6f 6e69  .        Harmoni
+000049f0: 6320 7265 6772 6573 7369 6f6e 2069 6e76  c regression inv
+00004a00: 6f6c 7665 7320 6669 7474 696e 6720 6120  olves fitting a 
+00004a10: 6d6f 6465 6c20 7769 7468 2073 696e 6520  model with sine 
+00004a20: 616e 6420 636f 7369 6e65 2063 6f6d 706f  and cosine compo
+00004a30: 6e65 6e74 7320 746f 2063 6170 7475 7265  nents to capture
+00004a40: 0a20 2020 2020 2020 2070 6572 696f 6469  .        periodi
+00004a50: 6320 7061 7474 6572 6e73 2069 6e20 7468  c patterns in th
+00004a60: 6520 6461 7461 2e20 5468 6973 2066 756e  e data. This fun
+00004a70: 6374 696f 6e20 7072 6564 6963 7473 2074  ction predicts t
+00004a80: 6865 206e 6578 7420 7661 6c75 6520 696e  he next value in
+00004a90: 2061 2067 6976 656e 2073 6571 7565 6e63   a given sequenc
+00004aa0: 650a 2020 2020 2020 2020 6f66 206e 756d  e.        of num
+00004ab0: 6265 7273 2062 7920 6669 7474 696e 6720  bers by fitting 
+00004ac0: 6120 6861 726d 6f6e 6963 206d 6f64 656c  a harmonic model
+00004ad0: 2074 6f20 7468 6520 7365 7175 656e 6365   to the sequence
+00004ae0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00004af0: 6d20 6e75 6d65 7269 635f 7365 7175 656e  m numeric_sequen
+00004b00: 6365 3a20 4120 6c69 7374 206f 7220 7365  ce: A list or se
+00004b10: 7175 656e 6365 206f 6620 6e75 6d62 6572  quence of number
+00004b20: 7320 746f 206d 6f64 656c 2e0a 2020 2020  s to model..    
+00004b30: 2020 2020 3a70 6172 616d 2066 7265 7175      :param frequ
+00004b40: 656e 6379 3a20 5468 6520 6672 6571 7565  ency: The freque
+00004b50: 6e63 7920 6f66 2074 6865 2070 6572 696f  ncy of the perio
+00004b60: 6469 6320 636f 6d70 6f6e 656e 7420 746f  dic component to
+00004b70: 206d 6f64 656c 2e0a 2020 2020 2020 2020   model..        
+00004b80: 3a72 6574 7572 6e3a 2054 6865 2070 7265  :return: The pre
+00004b90: 6469 6374 6564 206e 6578 7420 7661 6c75  dicted next valu
+00004ba0: 6520 696e 2074 6865 2073 6571 7565 6e63  e in the sequenc
+00004bb0: 6520 6173 2061 6e20 696e 7465 6765 722e  e as an integer.
+00004bc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004bd0: 2020 2020 2023 2043 6f6e 7665 7274 2074       # Convert t
+00004be0: 6865 206e 756d 6572 6963 2073 6571 7565  he numeric seque
+00004bf0: 6e63 6520 696e 746f 2061 206e 756d 7079  nce into a numpy
+00004c00: 2061 7272 6179 0a20 2020 2020 2020 2064   array.        d
+00004c10: 6174 6120 3d20 6e70 2e61 7272 6179 286e  ata = np.array(n
+00004c20: 756d 6572 6963 5f73 6571 7565 6e63 6529  umeric_sequence)
+00004c30: 2e72 6573 6861 7065 282d 312c 2031 290a  .reshape(-1, 1).
+00004c40: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+00004c50: 6520 616e 2061 7272 6179 2072 6570 7265  e an array repre
+00004c60: 7365 6e74 696e 6720 7469 6d65 206f 7220  senting time or 
+00004c70: 7468 6520 696e 6465 7065 6e64 656e 7420  the independent 
+00004c80: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
+00004c90: 2069 6e64 6578 203d 206e 702e 6172 7261   index = np.arra
+00004ca0: 7928 7261 6e67 6528 6c65 6e28 6461 7461  y(range(len(data
+00004cb0: 2929 292e 7265 7368 6170 6528 2d31 2c20  ))).reshape(-1, 
+00004cc0: 3129 0a0a 2020 2020 2020 2020 2320 4765  1)..        # Ge
+00004cd0: 6e65 7261 7465 2073 696e 6520 616e 6420  nerate sine and 
+00004ce0: 636f 7369 6e65 2066 6561 7475 7265 7320  cosine features 
+00004cf0: 6261 7365 6420 6f6e 2074 6865 2074 696d  based on the tim
+00004d00: 6520 6172 7261 7920 616e 6420 6769 7665  e array and give
+00004d10: 6e20 6672 6571 7565 6e63 790a 2020 2020  n frequency.    
+00004d20: 2020 2020 7369 6e65 5f66 6561 7475 7265      sine_feature
+00004d30: 203d 206e 702e 7369 6e28 3220 2a20 6e70   = np.sin(2 * np
+00004d40: 2e70 6920 2a20 6672 6571 7565 6e63 7920  .pi * frequency 
+00004d50: 2a20 696e 6465 7829 0a20 2020 2020 2020  * index).       
+00004d60: 2063 6f73 696e 655f 6665 6174 7572 6520   cosine_feature 
+00004d70: 3d20 6e70 2e63 6f73 2832 202a 206e 702e  = np.cos(2 * np.
+00004d80: 7069 202a 2066 7265 7175 656e 6379 202a  pi * frequency *
+00004d90: 2069 6e64 6578 290a 0a20 2020 2020 2020   index)..       
+00004da0: 2023 2043 6f6d 6269 6e65 2073 696e 6520   # Combine sine 
+00004db0: 616e 6420 636f 7369 6e65 2066 6561 7475  and cosine featu
+00004dc0: 7265 7320 696e 746f 2061 2073 696e 676c  res into a singl
+00004dd0: 6520 6665 6174 7572 6520 6d61 7472 6978  e feature matrix
+00004de0: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
+00004df0: 7320 3d20 6e70 2e68 7374 6163 6b28 2873  s = np.hstack((s
+00004e00: 696e 655f 6665 6174 7572 652c 2063 6f73  ine_feature, cos
+00004e10: 696e 655f 6665 6174 7572 6529 290a 0a20  ine_feature)).. 
+00004e20: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+00004e30: 6120 4c69 6e65 6172 5265 6772 6573 7369  a LinearRegressi
+00004e40: 6f6e 206d 6f64 656c 2061 6e64 2066 6974  on model and fit
+00004e50: 2069 7420 746f 2074 6865 2064 6174 6120   it to the data 
+00004e60: 7769 7468 2068 6172 6d6f 6e69 6320 6665  with harmonic fe
+00004e70: 6174 7572 6573 0a20 2020 2020 2020 206d  atures.        m
+00004e80: 6f64 656c 203d 204c 696e 6561 7252 6567  odel = LinearReg
+00004e90: 7265 7373 696f 6e28 290a 2020 2020 2020  ression().      
+00004ea0: 2020 6d6f 6465 6c2e 6669 7428 6665 6174    model.fit(feat
+00004eb0: 7572 6573 2c20 6461 7461 290a 0a20 2020  ures, data)..   
+00004ec0: 2020 2020 2023 2050 7265 6469 6374 2074       # Predict t
+00004ed0: 6865 206e 6578 7420 7661 6c75 6520 696e  he next value in
+00004ee0: 2074 6865 2073 6571 7565 6e63 6520 7573   the sequence us
+00004ef0: 696e 6720 7468 6520 6669 7474 6564 206d  ing the fitted m
+00004f00: 6f64 656c 0a20 2020 2020 2020 206e 6578  odel.        nex
+00004f10: 745f 7469 6d65 5f70 6f69 6e74 203d 206e  t_time_point = n
+00004f20: 702e 6172 7261 7928 5b5b 6c65 6e28 6461  p.array([[len(da
+00004f30: 7461 295d 5d29 0a20 2020 2020 2020 206e  ta)]]).        n
+00004f40: 6578 745f 7369 6e65 5f66 6561 7475 7265  ext_sine_feature
+00004f50: 203d 206e 702e 7369 6e28 3220 2a20 6e70   = np.sin(2 * np
+00004f60: 2e70 6920 2a20 6672 6571 7565 6e63 7920  .pi * frequency 
+00004f70: 2a20 6e65 7874 5f74 696d 655f 706f 696e  * next_time_poin
+00004f80: 7429 0a20 2020 2020 2020 206e 6578 745f  t).        next_
+00004f90: 636f 7369 6e65 5f66 6561 7475 7265 203d  cosine_feature =
+00004fa0: 206e 702e 636f 7328 3220 2a20 6e70 2e70   np.cos(2 * np.p
+00004fb0: 6920 2a20 6672 6571 7565 6e63 7920 2a20  i * frequency * 
+00004fc0: 6e65 7874 5f74 696d 655f 706f 696e 7429  next_time_point)
+00004fd0: 0a20 2020 2020 2020 206e 6578 745f 6665  .        next_fe
+00004fe0: 6174 7572 6573 203d 206e 702e 6873 7461  atures = np.hsta
+00004ff0: 636b 2828 6e65 7874 5f73 696e 655f 6665  ck((next_sine_fe
+00005000: 6174 7572 652c 206e 6578 745f 636f 7369  ature, next_cosi
+00005010: 6e65 5f66 6561 7475 7265 2929 0a0a 2020  ne_feature))..  
+00005020: 2020 2020 2020 7072 6564 6963 7469 6f6e        prediction
+00005030: 203d 206d 6f64 656c 2e70 7265 6469 6374   = model.predict
+00005040: 286e 6578 745f 6665 6174 7572 6573 295b  (next_features)[
+00005050: 305d 5b30 5d0a 0a20 2020 2020 2020 2023  0][0]..        #
+00005060: 2052 6574 7572 6e20 7468 6520 7072 6564   Return the pred
+00005070: 6963 7465 6420 7661 6c75 6520 6173 2061  icted value as a
+00005080: 6e20 696e 7465 6765 720a 2020 2020 2020  n integer.      
+00005090: 2020 7265 7475 726e 2043 616c 6375 6c61    return Calcula
+000050a0: 7465 5574 696c 2e72 6561 6c5f 726f 756e  teUtil.real_roun
+000050b0: 6428 7072 6564 6963 7469 6f6e 290a 0a20  d(prediction).. 
+000050c0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+000050d0: 0a20 2020 2064 6566 2072 616e 646f 6d5f  .    def random_
+000050e0: 666f 7265 7374 5f72 6567 7265 7373 6f72  forest_regressor
+000050f0: 5f74 7261 6e73 666f 726d 6572 280a 2020  _transformer(.  
+00005100: 2020 2020 2020 2020 2020 6e75 6d65 7269            numeri
+00005110: 635f 7365 7175 656e 6365 3a20 4c69 7374  c_sequence: List
+00005120: 5b69 6e74 5d2c 0a20 2020 2020 2020 2020  [int],.         
+00005130: 2020 2072 6f6c 6c69 6e67 5f73 697a 653a     rolling_size:
+00005140: 2069 6e74 2c0a 2020 2020 2020 2020 2020   int,.          
+00005150: 2020 7761 726d 5f73 7461 7274 3a20 626f    warm_start: bo
+00005160: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+00005170: 2020 2020 2020 2020 7261 6e64 6f6d 5f73          random_s
+00005180: 7461 7465 3a20 696e 7420 3d20 3132 2c0a  tate: int = 12,.
+00005190: 2020 2020 2020 2020 2020 2020 7061 7261              para
+000051a0: 6d5f 6469 7374 7269 6275 7469 6f6e 733a  m_distributions:
+000051b0: 204f 7074 696f 6e61 6c5b 4469 6374 5d20   Optional[Dict] 
+000051c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000051d0: 2020 2020 7061 7261 6d5f 6f76 6572 7269      param_overri
+000051e0: 6465 733a 204f 7074 696f 6e61 6c5b 4469  des: Optional[Di
+000051f0: 6374 5d20 3d20 4e6f 6e65 0a20 2020 2029  ct] = None.    )
+00005200: 202d 3e20 666c 6f61 743a 0a20 2020 2020   -> float:.     
+00005210: 2020 2074 7261 696e 5f78 2c20 7472 6169     train_x, trai
+00005220: 6e5f 7920 3d20 4361 6c63 756c 6174 6555  n_y = CalculateU
+00005230: 7469 6c2e 6765 6e65 7261 7465 5f64 6174  til.generate_dat
+00005240: 6173 6574 735f 7769 7468 5f72 6f6c 6c69  asets_with_rolli
+00005250: 6e67 5f73 697a 6528 0a20 2020 2020 2020  ng_size(.       
+00005260: 2020 2020 2064 6174 613d 6e75 6d65 7269       data=numeri
+00005270: 635f 7365 7175 656e 6365 2c20 726f 6c6c  c_sequence, roll
+00005280: 696e 675f 7369 7a65 3d72 6f6c 6c69 6e67  ing_size=rolling
+00005290: 5f73 697a 650a 2020 2020 2020 2020 290a  _size.        ).
+000052a0: 0a20 2020 2020 2020 2023 2043 6f6e 7665  .        # Conve
+000052b0: 7274 206c 6973 7473 2074 6f20 6e75 6d70  rt lists to nump
+000052c0: 7920 6172 7261 7973 2066 6f72 2063 6f6d  y arrays for com
+000052d0: 7061 7469 6269 6c69 7479 2077 6974 6820  patibility with 
+000052e0: 7363 696b 6974 2d6c 6561 726e 0a20 2020  scikit-learn.   
+000052f0: 2020 2020 2069 6e70 7574 5f78 203d 206e       input_x = n
+00005300: 702e 6172 7261 7928 7472 6169 6e5f 7829  p.array(train_x)
+00005310: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+00005320: 7920 3d20 6e70 2e61 7272 6179 2874 7261  y = np.array(tra
+00005330: 696e 5f79 290a 0a20 2020 2020 2020 2023  in_y)..        #
+00005340: 2053 6361 6c65 2074 6865 2066 6561 7475   Scale the featu
+00005350: 7265 7320 746f 206e 6f72 6d61 6c69 7a65  res to normalize
+00005360: 2064 6174 610a 2020 2020 2020 2020 7363   data.        sc
+00005370: 616c 6572 203d 2053 7461 6e64 6172 6453  aler = StandardS
+00005380: 6361 6c65 7228 290a 2020 2020 2020 2020  caler().        
+00005390: 696e 7075 745f 785f 7363 616c 6564 203d  input_x_scaled =
+000053a0: 2073 6361 6c65 722e 6669 745f 7472 616e   scaler.fit_tran
+000053b0: 7366 6f72 6d28 696e 7075 745f 7829 0a0a  sform(input_x)..
+000053c0: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
+000053d0: 6c69 7a65 2061 6e64 2074 7261 696e 2074  lize and train t
+000053e0: 6865 2052 616e 646f 6d20 466f 7265 7374  he Random Forest
+000053f0: 2052 6567 7265 7373 6f72 0a20 2020 2020   Regressor.     
+00005400: 2020 206d 6f64 656c 203d 2052 616e 646f     model = Rando
+00005410: 6d46 6f72 6573 7452 6567 7265 7373 6f72  mForestRegressor
+00005420: 2877 6172 6d5f 7374 6172 743d 7761 726d  (warm_start=warm
+00005430: 5f73 7461 7274 2c20 7261 6e64 6f6d 5f73  _start, random_s
+00005440: 7461 7465 3d72 616e 646f 6d5f 7374 6174  tate=random_stat
+00005450: 6529 0a20 2020 2020 2020 2069 6620 7061  e).        if pa
+00005460: 7261 6d5f 6469 7374 7269 6275 7469 6f6e  ram_distribution
+00005470: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+00005480: 6172 616d 5f6f 7665 7272 6964 6573 203d  aram_overrides =
+00005490: 2070 6172 616d 5f6f 7665 7272 6964 6573   param_overrides
+000054a0: 206f 7220 7b7d 0a20 2020 2020 2020 2020   or {}.         
+000054b0: 2020 2072 616e 646f 6d5f 7365 6172 6368     random_search
+000054c0: 203d 2052 616e 646f 6d69 7a65 6453 6561   = RandomizedSea
+000054d0: 7263 6843 5628 6573 7469 6d61 746f 723d  rchCV(estimator=
+000054e0: 6d6f 6465 6c2c 2070 6172 616d 5f64 6973  model, param_dis
+000054f0: 7472 6962 7574 696f 6e73 3d70 6172 616d  tributions=param
+00005500: 5f64 6973 7472 6962 7574 696f 6e73 2c0a  _distributions,.
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005530: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00005540: 2a70 6172 616d 5f6f 7665 7272 6964 6573  *param_overrides
+00005550: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
+00005560: 6e64 6f6d 5f73 6561 7263 682e 6669 7428  ndom_search.fit(
+00005570: 696e 7075 745f 785f 7363 616c 6564 2c20  input_x_scaled, 
+00005580: 6f75 7470 7574 5f79 290a 2020 2020 2020  output_y).      
+00005590: 2020 2020 2020 6d6f 6465 6c20 3d20 5261        model = Ra
+000055a0: 6e64 6f6d 466f 7265 7374 5265 6772 6573  ndomForestRegres
+000055b0: 736f 7228 7761 726d 5f73 7461 7274 3d77  sor(warm_start=w
+000055c0: 6172 6d5f 7374 6172 742c 2072 616e 646f  arm_start, rando
+000055d0: 6d5f 7374 6174 653d 7261 6e64 6f6d 5f73  m_state=random_s
+000055e0: 7461 7465 2c0a 2020 2020 2020 2020 2020  tate,.          
+000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005610: 2a2a 7261 6e64 6f6d 5f73 6561 7263 682e  **random_search.
+00005620: 6265 7374 5f70 6172 616d 735f 290a 0a20  best_params_).. 
+00005630: 2020 2020 2020 206d 6f64 656c 5f70 6970         model_pip
+00005640: 6c69 6e65 203d 2050 6970 656c 696e 6528  line = Pipeline(
+00005650: 5b0a 2020 2020 2020 2020 2020 2020 2827  [.            ('
+00005660: 7072 6564 6963 7469 6f6e 5f74 7261 6e73  prediction_trans
+00005670: 666f 726d 6572 272c 2052 616e 646f 6d46  former', RandomF
+00005680: 6f72 6573 7452 6567 7265 7373 6f72 5472  orestRegressorTr
+00005690: 616e 7366 6f72 6d65 7228 6d6f 6465 6c29  ansformer(model)
+000056a0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+000056b0: 2770 7265 6469 6374 696f 6e5f 7472 616e  'prediction_tran
+000056c0: 7366 6f72 6d65 725f 7477 6f27 2c20 5261  sformer_two', Ra
+000056d0: 6e64 6f6d 466f 7265 7374 5265 6772 6573  ndomForestRegres
+000056e0: 736f 7228 7761 726d 5f73 7461 7274 3d77  sor(warm_start=w
+000056f0: 6172 6d5f 7374 6172 742c 2072 616e 646f  arm_start, rando
+00005700: 6d5f 7374 6174 653d 7261 6e64 6f6d 5f73  m_state=random_s
+00005710: 7461 7465 2929 2c0a 2020 2020 2020 2020  tate)),.        
+00005720: 2020 2020 2320 2827 706f 6c79 5f66 6561      # ('poly_fea
+00005730: 7475 7265 7327 2c20 506f 6c79 6e6f 6d69  tures', Polynomi
+00005740: 616c 4665 6174 7572 6573 2864 6567 7265  alFeatures(degre
+00005750: 653d 3229 292c 0a20 2020 2020 2020 2020  e=2)),.         
+00005760: 2020 2023 2028 276c 696e 6561 725f 7265     # ('linear_re
+00005770: 6772 6573 7369 6f6e 272c 204c 696e 6561  gression', Linea
+00005780: 7252 6567 7265 7373 696f 6e28 2929 0a20  rRegression()). 
+00005790: 2020 2020 2020 205d 290a 2020 2020 2020         ]).      
+000057a0: 2020 6d6f 6465 6c5f 7069 706c 696e 652e    model_pipline.
+000057b0: 6669 7428 696e 7075 745f 785f 7363 616c  fit(input_x_scal
+000057c0: 6564 2c20 6f75 7470 7574 5f79 290a 0a20  ed, output_y).. 
+000057d0: 2020 2020 2020 2023 2050 7265 7061 7265         # Prepare
+000057e0: 2074 6865 206c 6173 7420 726f 6c6c 696e   the last rollin
+000057f0: 6720 7769 6e64 6f77 206f 6620 6461 7461  g window of data
+00005800: 2066 6f72 2070 7265 6469 6374 696f 6e0a   for prediction.
+00005810: 2020 2020 2020 2020 7465 7374 5f78 203d          test_x =
+00005820: 206e 702e 6172 7261 7928 5b6e 756d 6572   np.array([numer
+00005830: 6963 5f73 6571 7565 6e63 655b 2d72 6f6c  ic_sequence[-rol
+00005840: 6c69 6e67 5f73 697a 653a 5d5d 290a 2020  ling_size:]]).  
+00005850: 2020 2020 2020 7465 7374 5f78 5f73 6361        test_x_sca
+00005860: 6c65 6420 3d20 7363 616c 6572 2e74 7261  led = scaler.tra
+00005870: 6e73 666f 726d 2874 6573 745f 7829 0a0a  nsform(test_x)..
+00005880: 2020 2020 2020 2020 2320 5072 6564 6963          # Predic
+00005890: 7469 6e67 2074 6865 206e 6578 7420 7661  ting the next va
+000058a0: 6c75 650a 2020 2020 2020 2020 7072 6564  lue.        pred
+000058b0: 5f79 203d 206d 6f64 656c 5f70 6970 6c69  _y = model_pipli
+000058c0: 6e65 2e70 7265 6469 6374 2874 6573 745f  ne.predict(test_
+000058d0: 785f 7363 616c 6564 290a 2020 2020 2020  x_scaled).      
+000058e0: 2020 7265 7475 726e 2070 7265 645f 790a    return pred_y.
+000058f0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00005900: 6f64 0a20 2020 2064 6566 2072 616e 646f  od.    def rando
+00005910: 6d5f 666f 7265 7374 5f72 6567 7265 7373  m_forest_regress
+00005920: 6f72 5f6e 6578 745f 7661 6c75 6528 0a20  or_next_value(. 
+00005930: 2020 2020 2020 2020 2020 206e 756d 6572             numer
+00005940: 6963 5f73 6571 7565 6e63 653a 204c 6973  ic_sequence: Lis
+00005950: 745b 696e 745d 2c0a 2020 2020 2020 2020  t[int],.        
 00005960: 2020 2020 726f 6c6c 696e 675f 7369 7a65      rolling_size
-00005970: 2028 696e 7429 3a20 5468 6520 6e75 6d62   (int): The numb
-00005980: 6572 206f 6620 656c 656d 656e 7473 2069  er of elements i
-00005990: 6e20 6561 6368 2072 6f6c 6c69 6e67 2077  n each rolling w
-000059a0: 696e 646f 772e 0a20 2020 2020 2020 2020  indow..         
-000059b0: 2020 2077 6172 6d5f 7374 6172 7420 2862     warm_start (b
-000059c0: 6f6f 6c29 3a20 5768 6574 6865 7220 746f  ool): Whether to
-000059d0: 2072 6575 7365 2074 6865 2073 6f6c 7574   reuse the solut
-000059e0: 696f 6e20 6f66 2074 6865 2070 7265 7669  ion of the previ
-000059f0: 6f75 7320 6361 6c6c 2074 6f20 6669 7420  ous call to fit 
-00005a00: 616e 6420 6164 6420 6d6f 7265 2065 7374  and add more est
-00005a10: 696d 6174 6f72 7320 746f 2074 6865 2065  imators to the e
-00005a20: 6e73 656d 626c 652e 0a20 2020 2020 2020  nsemble..       
-00005a30: 2020 2020 2072 616e 646f 6d5f 7374 6174       random_stat
-00005a40: 6520 2869 6e74 293a 2043 6f6e 7472 6f6c  e (int): Control
-00005a50: 7320 626f 7468 2074 6865 2072 616e 646f  s both the rando
-00005a60: 6d6e 6573 7320 6f66 2074 6865 2062 6f6f  mness of the boo
-00005a70: 7473 7472 6170 7069 6e67 206f 6620 7468  tstrapping of th
-00005a80: 6520 7361 6d70 6c65 7320 7573 6564 2077  e samples used w
-00005a90: 6865 6e20 6275 696c 6469 6e67 2074 7265  hen building tre
-00005aa0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ac0: 2020 2028 6966 2060 626f 6f74 7374 7261     (if `bootstra
-00005ad0: 703d 5472 7565 6029 2061 6e64 2074 6865  p=True`) and the
-00005ae0: 2073 616d 706c 696e 6720 6f66 2074 6865   sampling of the
-00005af0: 2066 6561 7475 7265 7320 746f 2063 6f6e   features to con
-00005b00: 7369 6465 7220 7768 656e 206c 6f6f 6b69  sider when looki
-00005b10: 6e67 2066 6f72 2074 6865 2062 6573 7420  ng for the best 
-00005b20: 7370 6c69 7420 6174 2065 6163 6820 6e6f  split at each no
-00005b30: 6465 2e0a 2020 2020 2020 2020 2020 2020  de..            
-00005b40: 7061 7261 6d5f 6469 7374 7269 6275 7469  param_distributi
-00005b50: 6f6e 7320 284f 7074 696f 6e61 6c5b 4469  ons (Optional[Di
-00005b60: 6374 5d29 3a20 5468 6520 6469 7374 7269  ct]): The distri
-00005b70: 6275 7469 6f6e 206f 6620 7061 7261 6d65  bution of parame
-00005b80: 7465 7273 2074 6f20 7472 7920 696e 2072  ters to try in r
-00005b90: 616e 646f 6d69 7a65 6420 7365 6172 6368  andomized search
-00005ba0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bd0: 2020 6567 3a20 7b0a 2020 2020 2020 2020    eg: {.        
-00005be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2020 2020 2020 2020 2020 2020 276e 5f65              'n_e
-00005c10: 7374 696d 6174 6f72 7327 3a20 7374 6174  stimators': stat
-00005c20: 732e 7261 6e64 696e 7428 3130 302c 2035  s.randint(100, 5
-00005c30: 3030 292c 0a20 2020 2020 2020 2020 2020  00),.           
-00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 2020 2020 2020 2020 2027 6d61 785f 6465           'max_de
-00005c70: 7074 6827 3a20 5b4e 6f6e 652c 205d 202b  pth': [None, ] +
-00005c80: 205b 6920 666f 7220 6920 696e 2072 616e   [i for i in ran
-00005c90: 6765 2831 302c 2031 3030 295d 2c0a 2020  ge(10, 100)],.  
-00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 2020 276d 6178 5f66 6561 7475 7265 7327    'max_features'
-00005ce0: 3a20 5b27 7371 7274 272c 2027 6c6f 6732  : ['sqrt', 'log2
-00005cf0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2020 2020 276d 696e 5f73 616d          'min_sam
-00005d30: 706c 6573 5f73 706c 6974 273a 2073 7461  ples_split': sta
-00005d40: 7473 2e72 616e 6469 6e74 2832 2c20 3830  ts.randint(2, 80
-00005d50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005970: 3a20 696e 742c 0a20 2020 2020 2020 2020  : int,.         
+00005980: 2020 2077 6172 6d5f 7374 6172 743a 2062     warm_start: b
+00005990: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+000059a0: 2020 2020 2020 2020 2072 616e 646f 6d5f           random_
+000059b0: 7374 6174 653a 2069 6e74 203d 2031 322c  state: int = 12,
+000059c0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+000059d0: 616d 5f64 6973 7472 6962 7574 696f 6e73  am_distributions
+000059e0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745d  : Optional[Dict]
+000059f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00005a00: 2020 2020 2070 6172 616d 5f6f 7665 7272       param_overr
+00005a10: 6964 6573 3a20 4f70 7469 6f6e 616c 5b44  ides: Optional[D
+00005a20: 6963 745d 203d 204e 6f6e 650a 2020 2020  ict] = None.    
+00005a30: 2920 2d3e 2066 6c6f 6174 3a0a 2020 2020  ) -> float:.    
+00005a40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005a50: 5072 6564 6963 7473 2074 6865 206e 6578  Predicts the nex
+00005a60: 7420 7661 6c75 6520 696e 2061 206e 756d  t value in a num
+00005a70: 6572 6963 2073 6571 7565 6e63 6520 7573  eric sequence us
+00005a80: 696e 6720 6120 5261 6e64 6f6d 2046 6f72  ing a Random For
+00005a90: 6573 7420 5265 6772 6573 736f 7220 6d6f  est Regressor mo
+00005aa0: 6465 6c2e 0a0a 2020 2020 2020 2020 5468  del...        Th
+00005ab0: 6973 206d 6574 686f 6420 7573 6573 2061  is method uses a
+00005ac0: 2052 616e 646f 6d20 466f 7265 7374 2052   Random Forest R
+00005ad0: 6567 7265 7373 6f72 2074 6f20 7072 6564  egressor to pred
+00005ae0: 6963 7420 7468 6520 6e65 7874 2076 616c  ict the next val
+00005af0: 7565 2069 6e20 6120 7365 7175 656e 6365  ue in a sequence
+00005b00: 2062 6173 6564 206f 6e0a 2020 2020 2020   based on.      
+00005b10: 2020 7468 6520 7661 6c75 6573 2069 6e20    the values in 
+00005b20: 6120 726f 6c6c 696e 6720 7769 6e64 6f77  a rolling window
+00005b30: 2e20 5468 6520 7365 7175 656e 6365 2069  . The sequence i
+00005b40: 7320 6669 7273 7420 7472 616e 7366 6f72  s first transfor
+00005b50: 6d65 6420 696e 746f 2061 2064 6174 6173  med into a datas
+00005b60: 6574 2073 7569 7461 626c 6520 666f 720a  et suitable for.
+00005b70: 2020 2020 2020 2020 7265 6772 6573 7369          regressi
+00005b80: 6f6e 2062 7920 6372 6561 7469 6e67 206f  on by creating o
+00005b90: 7665 726c 6170 7069 6e67 2077 696e 646f  verlapping windo
+00005ba0: 7773 206f 6620 7370 6563 6966 6965 6420  ws of specified 
+00005bb0: 7369 7a65 2e0a 0a20 2020 2020 2020 2041  size...        A
+00005bc0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00005bd0: 206e 756d 6572 6963 5f73 6571 7565 6e63   numeric_sequenc
+00005be0: 6520 284c 6973 745b 696e 745d 293a 2054  e (List[int]): T
+00005bf0: 6865 206c 6973 7420 6f66 2069 6e74 6567  he list of integ
+00005c00: 6572 7320 7265 7072 6573 656e 7469 6e67  ers representing
+00005c10: 2074 6865 2073 6571 7565 6e63 652e 0a20   the sequence.. 
+00005c20: 2020 2020 2020 2020 2020 2072 6f6c 6c69             rolli
+00005c30: 6e67 5f73 697a 6520 2869 6e74 293a 2054  ng_size (int): T
+00005c40: 6865 206e 756d 6265 7220 6f66 2065 6c65  he number of ele
+00005c50: 6d65 6e74 7320 696e 2065 6163 6820 726f  ments in each ro
+00005c60: 6c6c 696e 6720 7769 6e64 6f77 2e0a 2020  lling window..  
+00005c70: 2020 2020 2020 2020 2020 7761 726d 5f73            warm_s
+00005c80: 7461 7274 2028 626f 6f6c 293a 2057 6865  tart (bool): Whe
+00005c90: 7468 6572 2074 6f20 7265 7573 6520 7468  ther to reuse th
+00005ca0: 6520 736f 6c75 7469 6f6e 206f 6620 7468  e solution of th
+00005cb0: 6520 7072 6576 696f 7573 2063 616c 6c20  e previous call 
+00005cc0: 746f 2066 6974 2061 6e64 2061 6464 206d  to fit and add m
+00005cd0: 6f72 6520 6573 7469 6d61 746f 7273 2074  ore estimators t
+00005ce0: 6f20 7468 6520 656e 7365 6d62 6c65 2e0a  o the ensemble..
+00005cf0: 2020 2020 2020 2020 2020 2020 7261 6e64              rand
+00005d00: 6f6d 5f73 7461 7465 2028 696e 7429 3a20  om_state (int): 
+00005d10: 436f 6e74 726f 6c73 2062 6f74 6820 7468  Controls both th
+00005d20: 6520 7261 6e64 6f6d 6e65 7373 206f 6620  e randomness of 
+00005d30: 7468 6520 626f 6f74 7374 7261 7070 696e  the bootstrappin
+00005d40: 6720 6f66 2074 6865 2073 616d 706c 6573  g of the samples
+00005d50: 2075 7365 6420 7768 656e 2062 7569 6c64   used when build
+00005d60: 696e 6720 7472 6565 730a 2020 2020 2020  ing trees.      
 00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d80: 2020 2020 2020 2027 6d69 6e5f 7361 6d70         'min_samp
-00005d90: 6c65 735f 6c65 6166 273a 2073 7461 7473  les_leaf': stats
-00005da0: 2e72 616e 6469 6e74 2831 2c20 3430 290a  .randint(1, 40).
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005de0: 7d0a 2020 2020 2020 2020 2020 2020 7061  }.            pa
-00005df0: 7261 6d5f 6f76 6572 7269 6465 7320 284f  ram_overrides (O
-00005e00: 7074 696f 6e61 6c5b 4469 6374 5d29 3a20  ptional[Dict]): 
-00005e10: 4164 6469 7469 6f6e 616c 2070 6172 616d  Additional param
-00005e20: 6574 6572 7320 666f 7220 7468 6520 5261  eters for the Ra
-00005e30: 6e64 6f6d 697a 6564 5365 6172 6368 4356  ndomizedSearchCV
-00005e40: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e70: 2020 6567 3a20 7b0a 2020 2020 2020 2020    eg: {.        
+00005d80: 2020 2020 2020 2020 2020 2869 6620 6062            (if `b
+00005d90: 6f6f 7473 7472 6170 3d54 7275 6560 2920  ootstrap=True`) 
+00005da0: 616e 6420 7468 6520 7361 6d70 6c69 6e67  and the sampling
+00005db0: 206f 6620 7468 6520 6665 6174 7572 6573   of the features
+00005dc0: 2074 6f20 636f 6e73 6964 6572 2077 6865   to consider whe
+00005dd0: 6e20 6c6f 6f6b 696e 6720 666f 7220 7468  n looking for th
+00005de0: 6520 6265 7374 2073 706c 6974 2061 7420  e best split at 
+00005df0: 6561 6368 206e 6f64 652e 0a20 2020 2020  each node..     
+00005e00: 2020 2020 2020 2070 6172 616d 5f64 6973         param_dis
+00005e10: 7472 6962 7574 696f 6e73 2028 4f70 7469  tributions (Opti
+00005e20: 6f6e 616c 5b44 6963 745d 293a 2054 6865  onal[Dict]): The
+00005e30: 2064 6973 7472 6962 7574 696f 6e20 6f66   distribution of
+00005e40: 2070 6172 616d 6574 6572 7320 746f 2074   parameters to t
+00005e50: 7279 2069 6e20 7261 6e64 6f6d 697a 6564  ry in randomized
+00005e60: 2073 6561 7263 682e 0a20 2020 2020 2020   search..       
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ea0: 2020 2020 2020 2020 2020 2020 276e 5f69              'n_i
-00005eb0: 7465 7227 3a20 3130 302c 0a20 2020 2020  ter': 100,.     
+00005e90: 2020 2020 2020 2020 2065 673a 207b 0a20           eg: {. 
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ee0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005ef0: 6376 273a 2033 2c0a 2020 2020 2020 2020  cv': 3,.        
+00005ed0: 2020 2027 6e5f 6573 7469 6d61 746f 7273     'n_estimators
+00005ee0: 273a 2073 7461 7473 2e72 616e 6469 6e74  ': stats.randint
+00005ef0: 2831 3030 2c20 3530 3029 2c0a 2020 2020  (100, 500),.    
 00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 2020 2020 2020 2020 2020 2020 2773 636f              'sco
-00005f30: 7269 6e67 273a 2027 6e65 675f 6d65 616e  ring': 'neg_mean
-00005f40: 5f73 7175 6172 6564 5f65 7272 6f72 272c  _squared_error',
-00005f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f30: 276d 6178 5f64 6570 7468 273a 205b 4e6f  'max_depth': [No
+00005f40: 6e65 2c20 5d20 2b20 5b69 2066 6f72 2069  ne, ] + [i for i
+00005f50: 2069 6e20 7261 6e67 6528 3130 2c20 3130   in range(10, 10
+00005f60: 3029 5d2c 0a20 2020 2020 2020 2020 2020  0)],.           
 00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f80: 2020 2020 2027 7665 7262 6f73 6527 3a20       'verbose': 
-00005f90: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2020 2020 2020 2027 7261 6e64 6f6d 5f73         'random_s
-00005fd0: 7461 7465 273a 2031 322c 0a20 2020 2020  tate': 12,.     
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006010: 6e5f 6a6f 6273 273a 202d 310a 2020 2020  n_jobs': -1.    
+00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f90: 2020 2020 2020 2020 2027 6d61 785f 6665           'max_fe
+00005fa0: 6174 7572 6573 273a 205b 2773 7172 7427  atures': ['sqrt'
+00005fb0: 2c20 276c 6f67 3227 5d2c 0a20 2020 2020  , 'log2'],.     
+00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fe0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005ff0: 6d69 6e5f 7361 6d70 6c65 735f 7370 6c69  min_samples_spli
+00006000: 7427 3a20 7374 6174 732e 7261 6e64 696e  t': stats.randin
+00006010: 7428 322c 2038 3029 2c0a 2020 2020 2020  t(2, 80),.      
 00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
-00006050: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00006060: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00006070: 743a 2054 6865 2070 7265 6469 6374 6564  t: The predicted
-00006080: 206e 6578 7420 7661 6c75 6520 696e 2074   next value in t
-00006090: 6865 2073 6571 7565 6e63 652e 0a0a 2020  he sequence...  
-000060a0: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-000060b0: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
-000060c0: 7272 6f72 3a20 4966 2074 6865 2072 6f6c  rror: If the rol
-000060d0: 6c69 6e67 5f73 697a 6520 6973 206c 6172  ling_size is lar
-000060e0: 6765 7220 7468 616e 2074 6865 2073 697a  ger than the siz
-000060f0: 6520 6f66 206e 756d 6572 6963 5f73 6571  e of numeric_seq
-00006100: 7565 6e63 652e 0a20 2020 2020 2020 2022  uence..        "
-00006110: 2222 0a20 2020 2020 2020 2069 6620 726f  "".        if ro
-00006120: 6c6c 696e 675f 7369 7a65 203e 206c 656e  lling_size > len
-00006130: 286e 756d 6572 6963 5f73 6571 7565 6e63  (numeric_sequenc
-00006140: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00006150: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00006160: 2822 726f 6c6c 696e 675f 7369 7a65 2063  ("rolling_size c
-00006170: 616e 6e6f 7420 6265 206c 6172 6765 7220  annot be larger 
-00006180: 7468 616e 2074 6865 2073 697a 6520 6f66  than the size of
-00006190: 206e 756d 6572 6963 5f73 6571 7565 6e63   numeric_sequenc
-000061a0: 6522 290a 0a20 2020 2020 2020 2023 2047  e")..        # G
-000061b0: 656e 6572 6174 6520 6461 7461 7365 7473  enerate datasets
-000061c0: 2077 6974 6820 7468 6520 7370 6563 6966   with the specif
-000061d0: 6965 6420 726f 6c6c 696e 6720 7369 7a65  ied rolling size
-000061e0: 0a20 2020 2020 2020 2074 7261 696e 5f78  .        train_x
-000061f0: 2c20 7472 6169 6e5f 7920 3d20 4361 6c63  , train_y = Calc
-00006200: 756c 6174 6555 7469 6c2e 6765 6e65 7261  ulateUtil.genera
-00006210: 7465 5f64 6174 6173 6574 735f 7769 7468  te_datasets_with
-00006220: 5f72 6f6c 6c69 6e67 5f73 697a 6528 0a20  _rolling_size(. 
-00006230: 2020 2020 2020 2020 2020 2064 6174 613d             data=
-00006240: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
-00006250: 2c20 726f 6c6c 696e 675f 7369 7a65 3d72  , rolling_size=r
-00006260: 6f6c 6c69 6e67 5f73 697a 650a 2020 2020  olling_size.    
-00006270: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-00006280: 2043 6f6e 7665 7274 206c 6973 7473 2074   Convert lists t
-00006290: 6f20 6e75 6d70 7920 6172 7261 7973 2066  o numpy arrays f
-000062a0: 6f72 2063 6f6d 7061 7469 6269 6c69 7479  or compatibility
-000062b0: 2077 6974 6820 7363 696b 6974 2d6c 6561   with scikit-lea
-000062c0: 726e 0a20 2020 2020 2020 2069 6e70 7574  rn.        input
-000062d0: 5f78 203d 206e 702e 6172 7261 7928 7472  _x = np.array(tr
-000062e0: 6169 6e5f 7829 0a20 2020 2020 2020 206f  ain_x).        o
-000062f0: 7574 7075 745f 7920 3d20 6e70 2e61 7272  utput_y = np.arr
-00006300: 6179 2874 7261 696e 5f79 290a 0a20 2020  ay(train_y)..   
-00006310: 2020 2020 2023 2053 6361 6c65 2074 6865       # Scale the
-00006320: 2066 6561 7475 7265 7320 746f 206e 6f72   features to nor
-00006330: 6d61 6c69 7a65 2064 6174 610a 2020 2020  malize data.    
-00006340: 2020 2020 7363 616c 6572 203d 2053 7461      scaler = Sta
-00006350: 6e64 6172 6453 6361 6c65 7228 290a 2020  ndardScaler().  
-00006360: 2020 2020 2020 696e 7075 745f 785f 7363        input_x_sc
-00006370: 616c 6564 203d 2073 6361 6c65 722e 6669  aled = scaler.fi
-00006380: 745f 7472 616e 7366 6f72 6d28 696e 7075  t_transform(inpu
-00006390: 745f 7829 0a0a 2020 2020 2020 2020 2320  t_x)..        # 
-000063a0: 496e 6974 6961 6c69 7a65 2061 6e64 2074  Initialize and t
-000063b0: 7261 696e 2074 6865 2052 616e 646f 6d20  rain the Random 
-000063c0: 466f 7265 7374 2052 6567 7265 7373 6f72  Forest Regressor
-000063d0: 0a20 2020 2020 2020 206d 6f64 656c 203d  .        model =
-000063e0: 2052 616e 646f 6d46 6f72 6573 7452 6567   RandomForestReg
-000063f0: 7265 7373 6f72 2877 6172 6d5f 7374 6172  ressor(warm_star
-00006400: 743d 7761 726d 5f73 7461 7274 2c20 7261  t=warm_start, ra
-00006410: 6e64 6f6d 5f73 7461 7465 3d72 616e 646f  ndom_state=rando
-00006420: 6d5f 7374 6174 6529 0a20 2020 2020 2020  m_state).       
-00006430: 2069 6620 7061 7261 6d5f 6469 7374 7269   if param_distri
-00006440: 6275 7469 6f6e 733a 0a20 2020 2020 2020  butions:.       
-00006450: 2020 2020 2070 6172 616d 5f6f 7665 7272       param_overr
-00006460: 6964 6573 203d 2070 6172 616d 5f6f 7665  ides = param_ove
-00006470: 7272 6964 6573 206f 7220 7b7d 0a20 2020  rrides or {}.   
-00006480: 2020 2020 2020 2020 2072 616e 646f 6d5f           random_
-00006490: 7365 6172 6368 203d 2052 616e 646f 6d69  search = Randomi
-000064a0: 7a65 6453 6561 7263 6843 5628 6573 7469  zedSearchCV(esti
-000064b0: 6d61 746f 723d 6d6f 6465 6c2c 2070 6172  mator=model, par
-000064c0: 616d 5f64 6973 7472 6962 7574 696f 6e73  am_distributions
-000064d0: 3d70 6172 616d 5f64 6973 7472 6962 7574  =param_distribut
-000064e0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2020 202a 2a70 6172 616d 5f6f 7665       **param_ove
-00006520: 7272 6964 6573 290a 2020 2020 2020 2020  rrides).        
-00006530: 2020 2020 7261 6e64 6f6d 5f73 6561 7263      random_searc
-00006540: 682e 6669 7428 696e 7075 745f 785f 7363  h.fit(input_x_sc
-00006550: 616c 6564 2c20 6f75 7470 7574 5f79 290a  aled, output_y).
-00006560: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00006570: 6c20 3d20 5261 6e64 6f6d 466f 7265 7374  l = RandomForest
-00006580: 5265 6772 6573 736f 7228 7761 726d 5f73  Regressor(warm_s
-00006590: 7461 7274 3d77 6172 6d5f 7374 6172 742c  tart=warm_start,
-000065a0: 2072 616e 646f 6d5f 7374 6174 653d 7261   random_state=ra
-000065b0: 6e64 6f6d 5f73 7461 7465 2c0a 2020 2020  ndom_state,.    
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2020 2020 2020 2a2a 7261 6e64 6f6d 5f73        **random_s
-000065f0: 6561 7263 682e 6265 7374 5f70 6172 616d  earch.best_param
-00006600: 735f 290a 2020 2020 2020 2020 6d6f 6465  s_).        mode
-00006610: 6c2e 6669 7428 696e 7075 745f 785f 7363  l.fit(input_x_sc
-00006620: 616c 6564 2c20 6f75 7470 7574 5f79 290a  aled, output_y).
-00006630: 0a20 2020 2020 2020 2023 2050 7265 7061  .        # Prepa
-00006640: 7265 2074 6865 206c 6173 7420 726f 6c6c  re the last roll
-00006650: 696e 6720 7769 6e64 6f77 206f 6620 6461  ing window of da
-00006660: 7461 2066 6f72 2070 7265 6469 6374 696f  ta for predictio
-00006670: 6e0a 2020 2020 2020 2020 7465 7374 5f78  n.        test_x
-00006680: 203d 206e 702e 6172 7261 7928 5b6e 756d   = np.array([num
-00006690: 6572 6963 5f73 6571 7565 6e63 655b 2d72  eric_sequence[-r
-000066a0: 6f6c 6c69 6e67 5f73 697a 653a 5d5d 290a  olling_size:]]).
-000066b0: 2020 2020 2020 2020 7465 7374 5f78 5f73          test_x_s
-000066c0: 6361 6c65 6420 3d20 7363 616c 6572 2e74  caled = scaler.t
-000066d0: 7261 6e73 666f 726d 2874 6573 745f 7829  ransform(test_x)
-000066e0: 0a0a 2020 2020 2020 2020 2320 5072 6564  ..        # Pred
-000066f0: 6963 7469 6e67 2074 6865 206e 6578 7420  icting the next 
-00006700: 7661 6c75 650a 2020 2020 2020 2020 7072  value.        pr
-00006710: 6564 5f79 203d 206d 6f64 656c 2e70 7265  ed_y = model.pre
-00006720: 6469 6374 2874 6573 745f 785f 7363 616c  dict(test_x_scal
-00006730: 6564 290a 2020 2020 2020 2020 7265 7475  ed).        retu
-00006740: 726e 2070 7265 645f 795b 305d 0a0a 2020  rn pred_y[0]..  
-00006750: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-00006760: 2020 2020 6465 6620 7261 6e64 6f6d 5f66      def random_f
-00006770: 6f72 6573 745f 7265 6772 6573 736f 725f  orest_regressor_
-00006780: 6e65 7874 5f76 616c 7565 5f62 795f 696e  next_value_by_in
-00006790: 6465 7828 6e75 6d65 7269 635f 7365 7175  dex(numeric_sequ
-000067a0: 656e 6365 3a20 4c69 7374 5b69 6e74 5d29  ence: List[int])
-000067b0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-000067c0: 2022 2222 0a20 2020 2020 2020 2050 7265   """.        Pre
-000067d0: 6469 6374 7320 7468 6520 6e65 7874 2076  dicts the next v
-000067e0: 616c 7565 2069 6e20 6120 7365 7175 656e  alue in a sequen
-000067f0: 6365 2075 7369 6e67 2061 2052 616e 646f  ce using a Rando
-00006800: 6d20 466f 7265 7374 2052 6567 7265 7373  m Forest Regress
-00006810: 6f72 2e0a 0a20 2020 2020 2020 2041 2052  or...        A R
-00006820: 616e 646f 6d20 466f 7265 7374 2052 6567  andom Forest Reg
-00006830: 7265 7373 6f72 2069 7320 6120 7479 7065  ressor is a type
-00006840: 206f 6620 656e 7365 6d62 6c65 206d 6163   of ensemble mac
-00006850: 6869 6e65 206c 6561 726e 696e 6720 6d6f  hine learning mo
-00006860: 6465 6c20 7468 6174 2075 7365 730a 2020  del that uses.  
-00006870: 2020 2020 2020 6d75 6c74 6970 6c65 2064        multiple d
-00006880: 6563 6973 696f 6e20 7472 6565 7320 746f  ecision trees to
-00006890: 206d 616b 6520 7072 6564 6963 7469 6f6e   make prediction
-000068a0: 732e 2049 7420 6973 2070 6172 7469 6375  s. It is particu
-000068b0: 6c61 726c 7920 7573 6566 756c 2066 6f72  larly useful for
-000068c0: 2072 6567 7265 7373 696f 6e0a 2020 2020   regression.    
-000068d0: 2020 2020 7461 736b 7320 6f6e 2063 6f6d      tasks on com
-000068e0: 706c 6578 2064 6174 6173 6574 7320 6265  plex datasets be
-000068f0: 6361 7573 6520 6974 2063 616e 2063 6170  cause it can cap
-00006900: 7475 7265 206e 6f6e 2d6c 696e 6561 7220  ture non-linear 
-00006910: 7265 6c61 7469 6f6e 7368 6970 7320 6265  relationships be
-00006920: 7477 6565 6e0a 2020 2020 2020 2020 7661  tween.        va
-00006930: 7269 6162 6c65 732e 2054 6869 7320 6675  riables. This fu
-00006940: 6e63 7469 6f6e 2061 7070 6c69 6573 2074  nction applies t
-00006950: 6865 206d 6f64 656c 2074 6f20 6120 7365  he model to a se
-00006960: 7175 656e 6365 206f 6620 6e75 6d62 6572  quence of number
-00006970: 7320 746f 2070 7265 6469 6374 2074 6865  s to predict the
-00006980: 0a20 2020 2020 2020 206e 6578 7420 7661  .        next va
-00006990: 6c75 6520 6261 7365 6420 6f6e 2074 6865  lue based on the
-000069a0: 206f 6273 6572 7665 6420 7472 656e 642e   observed trend.
-000069b0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000069c0: 206e 756d 6572 6963 5f73 6571 7565 6e63   numeric_sequenc
-000069d0: 653a 2041 206c 6973 7420 6f72 2073 6571  e: A list or seq
-000069e0: 7565 6e63 6520 6f66 206e 756d 6265 7273  uence of numbers
-000069f0: 2074 6f20 6d6f 6465 6c2e 0a20 2020 2020   to model..     
-00006a00: 2020 203a 7265 7475 726e 3a20 5468 6520     :return: The 
-00006a10: 7072 6564 6963 7465 6420 6e65 7874 2076  predicted next v
-00006a20: 616c 7565 2069 6e20 7468 6520 7365 7175  alue in the sequ
-00006a30: 656e 6365 2061 7320 616e 2069 6e74 6567  ence as an integ
-00006a40: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
-00006a50: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-00006a60: 7420 7468 6520 6e75 6d65 7269 6320 7365  t the numeric se
-00006a70: 7175 656e 6365 2069 6e74 6f20 6120 6e75  quence into a nu
-00006a80: 6d70 7920 6172 7261 7920 616e 6420 7265  mpy array and re
-00006a90: 7368 6170 6520 666f 7220 736b 6c65 6172  shape for sklear
-00006aa0: 6e0a 2020 2020 2020 2020 6461 7461 203d  n.        data =
-00006ab0: 206e 702e 6172 7261 7928 6e75 6d65 7269   np.array(numeri
-00006ac0: 635f 7365 7175 656e 6365 292e 7265 7368  c_sequence).resh
-00006ad0: 6170 6528 2d31 2c20 3129 0a0a 2020 2020  ape(-1, 1)..    
-00006ae0: 2020 2020 2320 4372 6561 7465 2061 6e20      # Create an 
-00006af0: 6172 7261 7920 7265 7072 6573 656e 7469  array representi
-00006b00: 6e67 2074 696d 6520 6f72 2074 6865 2069  ng time or the i
-00006b10: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
-00006b20: 626c 652c 2072 6573 6861 7065 6420 6173  ble, reshaped as
-00006b30: 2061 2063 6f6c 756d 6e0a 2020 2020 2020   a column.      
-00006b40: 2020 7469 6d65 5f66 6561 7475 7265 203d    time_feature =
-00006b50: 206e 702e 6172 7261 7928 7261 6e67 6528   np.array(range(
-00006b60: 6c65 6e28 6461 7461 2929 292e 7265 7368  len(data))).resh
-00006b70: 6170 6528 2d31 2c20 3129 0a0a 2020 2020  ape(-1, 1)..    
-00006b80: 2020 2020 2320 4372 6561 7465 2061 2052      # Create a R
-00006b90: 616e 646f 6d46 6f72 6573 7452 6567 7265  andomForestRegre
-00006ba0: 7373 6f72 206d 6f64 656c 2061 6e64 2066  ssor model and f
-00006bb0: 6974 2069 7420 746f 2074 6865 2064 6174  it it to the dat
-00006bc0: 610a 2020 2020 2020 2020 6d6f 6465 6c20  a.        model 
-00006bd0: 3d20 5261 6e64 6f6d 466f 7265 7374 5265  = RandomForestRe
-00006be0: 6772 6573 736f 7228 290a 2020 2020 2020  gressor().      
-00006bf0: 2020 6d6f 6465 6c2e 6669 7428 7469 6d65    model.fit(time
-00006c00: 5f66 6561 7475 7265 2c20 6461 7461 2e72  _feature, data.r
-00006c10: 6176 656c 2829 2920 2023 2046 6c61 7474  avel())  # Flatt
-00006c20: 656e 2074 6865 2061 7272 6179 2074 6f20  en the array to 
-00006c30: 6669 7420 7468 6520 6d6f 6465 6c0a 0a20  fit the model.. 
-00006c40: 2020 2020 2020 2023 2050 7265 6469 6374         # Predict
-00006c50: 2074 6865 206e 6578 7420 7661 6c75 6520   the next value 
-00006c60: 696e 2074 6865 2073 6571 7565 6e63 6520  in the sequence 
-00006c70: 7573 696e 6720 7468 6520 6669 7474 6564  using the fitted
-00006c80: 206d 6f64 656c 0a20 2020 2020 2020 2066   model.        f
-00006c90: 7574 7572 655f 7469 6d65 203d 206e 702e  uture_time = np.
-00006ca0: 6172 7261 7928 5b6c 656e 2864 6174 6129  array([len(data)
-00006cb0: 5d29 2e72 6573 6861 7065 282d 312c 2031  ]).reshape(-1, 1
-00006cc0: 290a 2020 2020 2020 2020 6675 7475 7265  ).        future
-00006cd0: 5f70 7265 6420 3d20 6d6f 6465 6c2e 7072  _pred = model.pr
-00006ce0: 6564 6963 7428 6675 7475 7265 5f74 696d  edict(future_tim
-00006cf0: 6529 0a0a 2020 2020 2020 2020 2320 5265  e)..        # Re
-00006d00: 7475 726e 2074 6865 2070 7265 6469 6374  turn the predict
-00006d10: 6564 2076 616c 7565 2061 7320 616e 2069  ed value as an i
-00006d20: 6e74 6567 6572 0a20 2020 2020 2020 2072  nteger.        r
-00006d30: 6574 7572 6e20 726f 756e 6428 6675 7475  eturn round(futu
-00006d40: 7265 5f70 7265 645b 305d 290a 0a20 2020  re_pred[0])..   
-00006d50: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-00006d60: 2020 2064 6566 2072 656c 6174 6976 655f     def relative_
-00006d70: 7374 7265 6e67 7468 5f69 6e64 6578 286e  strength_index(n
-00006d80: 756d 6572 6963 5f73 6571 7565 6e63 653a  umeric_sequence:
-00006d90: 204c 6973 745b 696e 745d 2c20 7065 7269   List[int], peri
-00006da0: 6f64 3a20 696e 7420 3d20 3134 2920 2d3e  od: int = 14) ->
-00006db0: 2066 6c6f 6174 3a0a 2020 2020 2020 2020   float:.        
-00006dc0: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
-00006dd0: 756c 6174 6520 7468 6520 5265 6c61 7469  ulate the Relati
-00006de0: 7665 2053 7472 656e 6774 6820 496e 6465  ve Strength Inde
-00006df0: 7820 2852 5349 2920 7573 696e 6720 4578  x (RSI) using Ex
-00006e00: 706f 6e65 6e74 6961 6c20 4d6f 7669 6e67  ponential Moving
-00006e10: 2041 7665 7261 6765 2028 454d 4129 2e0a   Average (EMA)..
-00006e20: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00006e30: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
-00006e40: 3a20 4120 6c69 7374 206f 6620 7072 6963  : A list of pric
-00006e50: 6573 2066 6f72 2061 2070 6172 7469 6375  es for a particu
-00006e60: 6c61 7220 7374 6f63 6b20 6f72 2061 7373  lar stock or ass
-00006e70: 6574 2e0a 2020 2020 2020 2020 3a70 6172  et..        :par
-00006e80: 616d 2070 6572 696f 643a 2054 6865 2070  am period: The p
-00006e90: 6572 696f 6420 6f76 6572 2077 6869 6368  eriod over which
-00006ea0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-00006eb0: 6520 5253 492c 2074 7970 6963 616c 6c79  e RSI, typically
-00006ec0: 2031 342e 0a20 2020 2020 2020 203a 7265   14..        :re
-00006ed0: 7475 726e 3a20 5468 6520 6361 6c63 756c  turn: The calcul
-00006ee0: 6174 6564 2052 5349 2076 616c 7565 2e0a  ated RSI value..
-00006ef0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00006f00: 2020 2020 6966 206c 656e 286e 756d 6572      if len(numer
-00006f10: 6963 5f73 6571 7565 6e63 6529 203c 2070  ic_sequence) < p
-00006f20: 6572 696f 643a 0a20 2020 2020 2020 2020  eriod:.         
-00006f30: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00006f40: 726f 7228 224e 6f74 2065 6e6f 7567 6820  ror("Not enough 
-00006f50: 6461 7461 2070 6f69 6e74 7320 746f 2063  data points to c
-00006f60: 616c 6375 6c61 7465 2052 5349 2229 0a0a  alculate RSI")..
-00006f70: 2020 2020 2020 2020 6465 6c74 6173 203d          deltas =
-00006f80: 205b 6e75 6d65 7269 635f 7365 7175 656e   [numeric_sequen
-00006f90: 6365 5b69 202b 2031 5d20 2d20 6e75 6d65  ce[i + 1] - nume
-00006fa0: 7269 635f 7365 7175 656e 6365 5b69 5d20  ric_sequence[i] 
-00006fb0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00006fc0: 656e 286e 756d 6572 6963 5f73 6571 7565  en(numeric_seque
-00006fd0: 6e63 6529 202d 2031 295d 0a20 2020 2020  nce) - 1)].     
-00006fe0: 2020 2067 6169 6e73 203d 205b 6d61 7828     gains = [max(
-00006ff0: 6465 6c74 612c 2030 2920 666f 7220 6465  delta, 0) for de
-00007000: 6c74 6120 696e 2064 656c 7461 735d 0a20  lta in deltas]. 
-00007010: 2020 2020 2020 206c 6f73 7365 7320 3d20         losses = 
-00007020: 5b6d 6178 282d 6465 6c74 612c 2030 2920  [max(-delta, 0) 
-00007030: 666f 7220 6465 6c74 6120 696e 2064 656c  for delta in del
-00007040: 7461 735d 0a0a 2020 2020 2020 2020 2320  tas]..        # 
-00007050: 496e 6974 6961 6c69 7a65 2045 4d41 2077  Initialize EMA w
-00007060: 6974 6820 534d 4120 666f 7220 7468 6520  ith SMA for the 
-00007070: 6669 7273 7420 2770 6572 696f 6427 0a20  first 'period'. 
-00007080: 2020 2020 2020 2061 7667 5f67 6169 6e20         avg_gain 
-00007090: 3d20 7375 6d28 6761 696e 735b 3a70 6572  = sum(gains[:per
-000070a0: 696f 645d 2920 2f20 7065 7269 6f64 0a20  iod]) / period. 
-000070b0: 2020 2020 2020 2061 7667 5f6c 6f73 7320         avg_loss 
-000070c0: 3d20 7375 6d28 6c6f 7373 6573 5b3a 7065  = sum(losses[:pe
-000070d0: 7269 6f64 5d29 202f 2070 6572 696f 640a  riod]) / period.
-000070e0: 0a20 2020 2020 2020 2023 2041 7070 6c79  .        # Apply
-000070f0: 2045 4d41 2066 6f72 6d75 6c61 2066 6f72   EMA formula for
-00007100: 2067 6169 6e73 2061 6e64 206c 6f73 7365   gains and losse
-00007110: 730a 2020 2020 2020 2020 656d 615f 6661  s.        ema_fa
-00007120: 6374 6f72 203d 2032 202f 2028 7065 7269  ctor = 2 / (peri
-00007130: 6f64 202b 2031 290a 2020 2020 2020 2020  od + 1).        
-00007140: 666f 7220 6920 696e 2072 616e 6765 2870  for i in range(p
-00007150: 6572 696f 642c 206c 656e 2864 656c 7461  eriod, len(delta
-00007160: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-00007170: 2061 7667 5f67 6169 6e20 3d20 2867 6169   avg_gain = (gai
-00007180: 6e73 5b69 5d20 2a20 656d 615f 6661 6374  ns[i] * ema_fact
-00007190: 6f72 2920 2b20 2861 7667 5f67 6169 6e20  or) + (avg_gain 
-000071a0: 2a20 2831 202d 2065 6d61 5f66 6163 746f  * (1 - ema_facto
-000071b0: 7229 290a 2020 2020 2020 2020 2020 2020  r)).            
-000071c0: 6176 675f 6c6f 7373 203d 2028 6c6f 7373  avg_loss = (loss
-000071d0: 6573 5b69 5d20 2a20 656d 615f 6661 6374  es[i] * ema_fact
-000071e0: 6f72 2920 2b20 2861 7667 5f6c 6f73 7320  or) + (avg_loss 
-000071f0: 2a20 2831 202d 2065 6d61 5f66 6163 746f  * (1 - ema_facto
-00007200: 7229 290a 0a20 2020 2020 2020 2072 7320  r))..        rs 
-00007210: 3d20 6176 675f 6761 696e 202f 2061 7667  = avg_gain / avg
-00007220: 5f6c 6f73 7320 6966 2061 7667 5f6c 6f73  _loss if avg_los
-00007230: 7320 213d 2030 2065 6c73 6520 300a 2020  s != 0 else 0.  
-00007240: 2020 2020 2020 7273 6920 3d20 3130 3020        rsi = 100 
-00007250: 2d20 2831 3030 202f 2028 3120 2b20 7273  - (100 / (1 + rs
-00007260: 2929 2069 6620 6176 675f 6c6f 7373 2021  )) if avg_loss !
-00007270: 3d20 3020 656c 7365 2031 3030 0a0a 2020  = 0 else 100..  
-00007280: 2020 2020 2020 7265 7475 726e 2072 7369        return rsi
-00007290: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-000072a0: 686f 640a 2020 2020 6465 6620 7365 6173  hod.    def seas
-000072b0: 6f6e 616c 5f61 7574 6f72 6567 7265 7373  onal_autoregress
-000072c0: 6976 655f 696e 7465 6772 6174 6564 5f6d  ive_integrated_m
-000072d0: 6f76 696e 675f 6176 6572 6167 655f 6e65  oving_average_ne
-000072e0: 7874 5f76 616c 7565 286e 756d 6572 6963  xt_value(numeric
-000072f0: 5f73 6571 7565 6e63 653a 204c 6973 745b  _sequence: List[
-00007300: 696e 745d 2920 2d3e 2069 6e74 3a0a 2020  int]) -> int:.  
-00007310: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00007320: 2020 4669 7420 6120 5365 6173 6f6e 616c    Fit a Seasonal
-00007330: 2041 7574 6f72 6567 7265 7373 6976 6520   Autoregressive 
-00007340: 496e 7465 6772 6174 6564 204d 6f76 696e  Integrated Movin
-00007350: 6720 4176 6572 6167 6520 2853 4152 494d  g Average (SARIM
-00007360: 4129 206d 6f64 656c 2074 6f0a 2020 2020  A) model to.    
-00007370: 2020 2020 7468 6520 7072 6f76 6964 6564      the provided
-00007380: 2074 696d 6520 7365 7269 6573 2064 6174   time series dat
-00007390: 6120 616e 6420 7072 6564 6963 7420 7468  a and predict th
-000073a0: 6520 6e65 7874 2076 616c 7565 2069 6e20  e next value in 
-000073b0: 7468 6520 7365 7269 6573 2e0a 0a20 2020  the series...   
-000073c0: 2020 2020 2053 4152 494d 4120 6d6f 6465       SARIMA mode
-000073d0: 6c73 2061 7265 2075 7365 6420 746f 2066  ls are used to f
-000073e0: 6f72 6563 6173 7420 6675 7475 7265 2070  orecast future p
-000073f0: 6f69 6e74 7320 696e 2061 2074 696d 6520  oints in a time 
-00007400: 7365 7269 6573 2e20 5468 6579 2061 7265  series. They are
-00007410: 0a20 2020 2020 2020 2063 6170 6162 6c65  .        capable
-00007420: 206f 6620 6d6f 6465 6c69 6e67 2063 6f6d   of modeling com
-00007430: 706c 6578 2073 6561 736f 6e61 6c20 7061  plex seasonal pa
-00007440: 7474 6572 6e73 2062 7920 696e 636f 7270  tterns by incorp
-00007450: 6f72 6174 696e 6720 626f 7468 206e 6f6e  orating both non
-00007460: 2d73 6561 736f 6e61 6c0a 2020 2020 2020  -seasonal.      
-00007470: 2020 2841 5249 4d41 2920 616e 6420 7365    (ARIMA) and se
-00007480: 6173 6f6e 616c 2065 6c65 6d65 6e74 732e  asonal elements.
-00007490: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000074a0: 206e 756d 6572 6963 5f73 6571 7565 6e63   numeric_sequenc
-000074b0: 653a 2041 206c 6973 7420 6f66 206e 756d  e: A list of num
-000074c0: 6572 6963 616c 2076 616c 7565 7320 7265  erical values re
-000074d0: 7072 6573 656e 7469 6e67 2061 2074 696d  presenting a tim
-000074e0: 6520 7365 7269 6573 2e0a 2020 2020 2020  e series..      
-000074f0: 2020 3a72 6574 7572 6e3a 2054 6865 206e    :return: The n
-00007500: 6578 7420 696e 7465 6765 7220 7661 6c75  ext integer valu
-00007510: 6520 7072 6564 6963 7465 6420 6279 2074  e predicted by t
-00007520: 6865 2053 4152 494d 4120 6d6f 6465 6c2e  he SARIMA model.
-00007530: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007540: 2020 2020 2023 2043 6f6e 7665 7274 2074       # Convert t
-00007550: 6865 2064 6174 6120 746f 2061 206e 756d  he data to a num
-00007560: 7079 2061 7272 6179 2066 6f72 2074 696d  py array for tim
-00007570: 6520 7365 7269 6573 2061 6e61 6c79 7369  e series analysi
-00007580: 730a 2020 2020 2020 2020 7469 6d65 7365  s.        timese
-00007590: 7269 6573 203d 206e 702e 6172 7261 7928  ries = np.array(
-000075a0: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
-000075b0: 290a 0a20 2020 2020 2020 2023 2041 7574  )..        # Aut
-000075c0: 6f6d 6174 6963 616c 6c79 2064 6973 636f  omatically disco
-000075d0: 7665 7220 7468 6520 6f70 7469 6d61 6c20  ver the optimal 
-000075e0: 6f72 6465 7220 666f 7220 7468 6520 5341  order for the SA
-000075f0: 5249 4d41 206d 6f64 656c 0a20 2020 2020  RIMA model.     
-00007600: 2020 2073 7465 7077 6973 655f 6d6f 6465     stepwise_mode
-00007610: 6c20 3d20 6175 746f 5f61 7269 6d61 2874  l = auto_arima(t
-00007620: 696d 6573 6572 6965 732c 2073 7461 7274  imeseries, start
-00007630: 5f70 3d32 2c20 7374 6172 745f 713d 322c  _p=2, start_q=2,
-00007640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2020 2020 206d 6178 5f70 3d33 2c20 6d61       max_p=3, ma
-00007670: 785f 713d 332c 206d 3d31 322c 0a20 2020  x_q=3, m=12,.   
-00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076a0: 2073 7461 7274 5f50 3d31 2c20 7374 6172   start_P=1, star
-000076b0: 745f 513d 312c 206d 6178 5f50 3d33 2c20  t_Q=1, max_P=3, 
-000076c0: 6d61 785f 513d 332c 0a20 2020 2020 2020  max_Q=3,.       
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076e0: 2020 2020 2020 2020 2020 2020 2073 6561               sea
-000076f0: 736f 6e61 6c3d 5472 7565 2c0a 2020 2020  sonal=True,.    
-00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007720: 643d 312c 2044 3d31 2c20 7472 6163 653d  d=1, D=1, trace=
-00007730: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007750: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-00007760: 5f61 6374 696f 6e3d 2769 676e 6f72 6527  _action='ignore'
-00007770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007790: 2020 2020 2020 7375 7070 7265 7373 5f77        suppress_w
-000077a0: 6172 6e69 6e67 733d 5472 7565 2c0a 2020  arnings=True,.  
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077d0: 2020 7374 6570 7769 7365 3d54 7275 6529    stepwise=True)
-000077e0: 0a0a 2020 2020 2020 2020 2320 4669 7420  ..        # Fit 
-000077f0: 7468 6520 5341 5249 4d41 206d 6f64 656c  the SARIMA model
-00007800: 2074 6f20 7468 6520 7469 6d65 2073 6572   to the time ser
-00007810: 6965 7320 6461 7461 0a20 2020 2020 2020  ies data.       
-00007820: 206d 6f64 656c 203d 2073 7465 7077 6973   model = stepwis
-00007830: 655f 6d6f 6465 6c2e 6669 7428 7469 6d65  e_model.fit(time
-00007840: 7365 7269 6573 290a 0a20 2020 2020 2020  series)..       
-00007850: 2023 2050 7265 6469 6374 2074 6865 206e   # Predict the n
-00007860: 6578 7420 7661 6c75 6520 696e 2074 6865  ext value in the
-00007870: 2074 696d 6520 7365 7269 6573 0a20 2020   time series.   
-00007880: 2020 2020 2066 6f72 6563 6173 7420 3d20       forecast = 
-00007890: 6d6f 6465 6c2e 7072 6564 6963 7428 6e5f  model.predict(n_
-000078a0: 7065 7269 6f64 733d 3129 0a0a 2020 2020  periods=1)..    
-000078b0: 2020 2020 2320 5265 7475 726e 2074 6865      # Return the
-000078c0: 2070 7265 6469 6374 6564 2076 616c 7565   predicted value
-000078d0: 2061 7320 616e 2069 6e74 6567 6572 0a20   as an integer. 
-000078e0: 2020 2020 2020 2072 6574 7572 6e20 726f         return ro
-000078f0: 756e 6428 666f 7265 6361 7374 5b30 5d29  und(forecast[0])
-00007900: 0a0a 0a63 6c61 7373 2053 7069 6465 7255  ...class SpiderU
-00007910: 7469 6c28 4142 4329 3a0a 2020 2020 2222  til(ABC):.    ""
-00007920: 220a 2020 2020 4d6f 7374 6c79 2063 7261  ".    Mostly cra
-00007930: 776c 696e 6720 6461 7461 0a20 2020 2022  wling data.    "
-00007940: 2222 0a20 2020 2075 726c 203d 2027 6874  "".    url = 'ht
-00007950: 7470 733a 2f2f 7777 772e 6c6f 7474 6572  tps://www.lotter
-00007960: 792e 676f 762e 636e 2f6b 6a2f 6b6a 6c62  y.gov.cn/kj/kjlb
-00007970: 2e68 746d 6c3f 646c 7427 0a0a 2020 2020  .html?dlt'..    
-00007980: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00007990: 662c 202a 2a6b 7761 7267 7329 3a0a 2020  f, **kwargs):.  
-000079a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000079b0: 2020 496e 6974 6961 6c69 7a65 2074 6865    Initialize the
-000079c0: 2053 7069 6465 7255 7469 6c20 6f62 6a65   SpiderUtil obje
-000079d0: 6374 2077 6974 6820 6120 5552 4c2e 0a0a  ct with a URL...
-000079e0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-000079f0: 7761 7267 733a 2041 2064 6963 7469 6f6e  wargs: A diction
-00007a00: 6172 7920 6f66 206b 6579 776f 7264 2061  ary of keyword a
-00007a10: 7267 756d 656e 7473 2077 6865 7265 3a0a  rguments where:.
-00007a20: 2020 2020 2020 2020 2020 2020 2d20 2775              - 'u
-00007a30: 726c 273a 2073 7472 2069 7320 7468 6520  rl': str is the 
-00007a40: 5552 4c20 746f 2066 6574 6368 2074 6865  URL to fetch the
-00007a50: 2064 6174 6120 6672 6f6d 2e20 4966 206e   data from. If n
-00007a60: 6f74 2070 726f 7669 6465 642c 2069 7420  ot provided, it 
-00007a70: 6465 6661 756c 7473 2074 6f20 616e 2065  defaults to an e
-00007a80: 6d70 7479 2073 7472 696e 672e 0a20 2020  mpty string..   
-00007a90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00007aa0: 2073 656c 662e 7572 6c20 3d20 6b77 6172   self.url = kwar
-00007ab0: 6773 2e67 6574 2827 7572 6c27 2c20 2727  gs.get('url', ''
-00007ac0: 2920 6f72 2073 656c 662e 7572 6c0a 0a20  ) or self.url.. 
-00007ad0: 2020 2064 6566 2073 7069 6465 725f 6368     def spider_ch
-00007ae0: 726f 6d65 5f64 7269 7665 7228 7365 6c66  rome_driver(self
-00007af0: 2920 2d3e 2077 6562 6472 6976 6572 2e43  ) -> webdriver.C
-00007b00: 6872 6f6d 653a 0a20 2020 2020 2020 2022  hrome:.        "
-00007b10: 2222 0a20 2020 2020 2020 2049 6e69 7469  "".        Initi
-00007b20: 616c 697a 6520 6120 4368 726f 6d65 2057  alize a Chrome W
-00007b30: 6562 4472 6976 6572 2077 6974 6820 6865  ebDriver with he
-00007b40: 6164 6c65 7373 206f 7074 696f 6e20 616e  adless option an
-00007b50: 6420 6e61 7669 6761 7465 2074 6f20 7468  d navigate to th
-00007b60: 6520 5552 4c2e 0a0a 2020 2020 2020 2020  e URL...        
-00007b70: 3a72 6574 7572 6e3a 2041 6e20 696e 7374  :return: An inst
-00007b80: 616e 6365 206f 6620 4368 726f 6d65 2057  ance of Chrome W
-00007b90: 6562 4472 6976 6572 2e0a 2020 2020 2020  ebDriver..      
-00007ba0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-00007bb0: 496d 706f 7274 2062 726f 7773 6572 2063  Import browser c
-00007bc0: 6f6e 6669 6775 7261 7469 6f6e 0a20 2020  onfiguration.   
-00007bd0: 2020 2020 206f 7074 696f 6e73 203d 2077       options = w
-00007be0: 6562 6472 6976 6572 2e43 6872 6f6d 654f  ebdriver.ChromeO
-00007bf0: 7074 696f 6e73 2829 0a20 2020 2020 2020  ptions().       
-00007c00: 2023 2053 6574 2068 6561 646c 6573 7320   # Set headless 
-00007c10: 6d6f 6465 0a20 2020 2020 2020 206f 7074  mode.        opt
-00007c20: 696f 6e73 2e61 6464 5f61 7267 756d 656e  ions.add_argumen
-00007c30: 7428 272d 2d68 6561 646c 6573 7327 290a  t('--headless').
-00007c40: 2020 2020 2020 2020 6472 6976 6572 203d          driver =
-00007c50: 2077 6562 6472 6976 6572 2e43 6872 6f6d   webdriver.Chrom
-00007c60: 6528 6f70 7469 6f6e 733d 6f70 7469 6f6e  e(options=option
-00007c70: 7329 0a20 2020 2020 2020 2064 7269 7665  s).        drive
-00007c80: 722e 6765 7428 7365 6c66 2e75 726c 290a  r.get(self.url).
-00007c90: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00007ca0: 7269 7665 720a 0a20 2020 2040 6162 7374  river..    @abst
-00007cb0: 7261 6374 6d65 7468 6f64 0a20 2020 2064  ractmethod.    d
-00007cc0: 6566 2073 7069 6465 725f 7265 6365 6e74  ef spider_recent
-00007cd0: 5f64 6174 6128 7365 6c66 2920 2d3e 204c  _data(self) -> L
-00007ce0: 6973 745b 4c69 7374 5b73 7472 5d5d 3a0a  ist[List[str]]:.
-00007cf0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00007d00: 2020 2020 4665 7463 6820 7468 6520 7265      Fetch the re
-00007d10: 6365 6e74 2064 6174 6120 6672 6f6d 2074  cent data from t
-00007d20: 6865 2077 6562 2070 6167 652e 0a0a 2020  he web page...  
-00007d30: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
-00007d40: 206c 6973 7420 6f66 206c 6973 7473 2063   list of lists c
-00007d50: 6f6e 7461 696e 696e 6720 7265 6365 6e74  ontaining recent
-00007d60: 2064 6174 6120 656e 7472 6965 732e 0a20   data entries.. 
-00007d70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007d80: 2020 2064 7269 7665 7220 3d20 7365 6c66     driver = self
-00007d90: 2e73 7069 6465 725f 6368 726f 6d65 5f64  .spider_chrome_d
-00007da0: 7269 7665 7228 290a 2020 2020 2020 2020  river().        
-00007db0: 7469 6d65 2e73 6c65 6570 2831 2920 2023  time.sleep(1)  #
-00007dc0: 2041 6c6c 6f77 2074 696d 6520 666f 7220   Allow time for 
-00007dd0: 7468 6520 7061 6765 2074 6f20 6c6f 6164  the page to load
-00007de0: 0a20 2020 2020 2020 2066 7261 6d65 203d  .        frame =
-00007df0: 2064 7269 7665 722e 6669 6e64 5f65 6c65   driver.find_ele
-00007e00: 6d65 6e74 2842 792e 5850 4154 482c 2027  ment(By.XPATH, '
-00007e10: 2f2f 6966 7261 6d65 5b40 6964 3d22 6946  //iframe[@id="iF
-00007e20: 7261 6d65 3122 5d27 290a 2020 2020 2020  rame1"]').      
-00007e30: 2020 6472 6976 6572 2e73 7769 7463 685f    driver.switch_
-00007e40: 746f 2e66 7261 6d65 2866 7261 6d65 290a  to.frame(frame).
-00007e50: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
-00007e60: 3d20 6472 6976 6572 2e66 696e 645f 656c  = driver.find_el
-00007e70: 656d 656e 7428 4279 2e58 5041 5448 2c20  ement(By.XPATH, 
-00007e80: 272f 2f74 626f 6479 5b40 6964 3d22 6869  '//tbody[@id="hi
-00007e90: 7374 6f72 7944 6174 6122 5d27 290a 2020  storyData"]').  
-00007ea0: 2020 2020 2020 7265 6365 6e74 5f64 6174        recent_dat
-00007eb0: 6120 3d20 5b78 2e73 706c 6974 2827 2027  a = [x.split(' '
-00007ec0: 295b 3a39 5d20 666f 7220 7820 696e 2063  )[:9] for x in c
-00007ed0: 6f6e 7465 6e74 2e74 6578 742e 7370 6c69  ontent.text.spli
-00007ee0: 7428 275c 6e27 295d 0a20 2020 2020 2020  t('\n')].       
-00007ef0: 2072 6574 7572 6e20 7265 6365 6e74 5f64   return recent_d
-00007f00: 6174 610a 0a20 2020 2040 6162 7374 7261  ata..    @abstra
-00007f10: 6374 6d65 7468 6f64 0a20 2020 2064 6566  ctmethod.    def
-00007f20: 2073 7069 6465 725f 6c61 7465 7374 5f64   spider_latest_d
-00007f30: 6174 6128 7365 6c66 2920 2d3e 204f 7074  ata(self) -> Opt
-00007f40: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-00007f50: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00007f60: 2020 2020 2020 4665 7463 6820 7468 6520        Fetch the 
-00007f70: 6c61 7465 7374 2073 696e 676c 6520 6461  latest single da
-00007f80: 7461 2065 6e74 7279 2e0a 0a20 2020 2020  ta entry...     
-00007f90: 2020 203a 7265 7475 726e 3a20 4120 6c69     :return: A li
-00007fa0: 7374 2063 6f6e 7461 696e 696e 6720 7468  st containing th
-00007fb0: 6520 6c61 7465 7374 2064 6174 6120 656e  e latest data en
-00007fc0: 7472 792c 206f 7220 4e6f 6e65 2069 6620  try, or None if 
-00007fd0: 7468 6572 6520 6973 206e 6f20 6461 7461  there is no data
-00007fe0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00007ff0: 2020 2020 2020 7265 6365 6e74 5f64 6174        recent_dat
-00008000: 6120 3d20 7365 6c66 2e73 7069 6465 725f  a = self.spider_
-00008010: 7265 6365 6e74 5f64 6174 6128 290a 2020  recent_data().  
-00008020: 2020 2020 2020 7265 7475 726e 2072 6563        return rec
-00008030: 656e 745f 6461 7461 5b30 5d20 6966 2072  ent_data[0] if r
-00008040: 6563 656e 745f 6461 7461 2065 6c73 6520  ecent_data else 
-00008050: 4e6f 6e65 0a0a 2020 2020 4061 6273 7472  None..    @abstr
-00008060: 6163 746d 6574 686f 640a 2020 2020 6465  actmethod.    de
-00008070: 6620 7370 6964 6572 5f66 756c 6c5f 6461  f spider_full_da
-00008080: 7461 2873 656c 6629 202d 3e20 4c69 7374  ta(self) -> List
-00008090: 5b4c 6973 745b 7374 725d 5d3a 0a20 2020  [List[str]]:.   
-000080a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000080b0: 204c 6f61 6420 7468 6520 6675 6c6c 2073   Load the full s
-000080c0: 6574 206f 6620 6461 7461 2066 726f 6d20  et of data from 
-000080d0: 7468 6520 736f 7572 6365 2e0a 0a20 2020  the source...   
-000080e0: 2020 2020 203a 7265 7475 726e 3a20 4120       :return: A 
-000080f0: 6c69 7374 206f 6620 6c69 7374 7320 636f  list of lists co
-00008100: 6e74 6169 6e69 6e67 2061 6c6c 2064 6174  ntaining all dat
-00008110: 6120 656e 7472 6965 732e 0a20 2020 2020  a entries..     
-00008120: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00008130: 2054 6865 2069 6d70 6c65 6d65 6e74 6174   The implementat
-00008140: 696f 6e20 7368 6f75 6c64 2062 6520 7072  ion should be pr
-00008150: 6f76 6964 6564 2062 7920 7468 6520 7375  ovided by the su
-00008160: 6263 6c61 7373 2e0a 2020 2020 2020 2020  bclass..        
-00008170: 6675 6c6c 5f64 6174 6120 3d20 5b5d 0a20  full_data = []. 
-00008180: 2020 2020 2020 2064 7269 7665 7220 3d20         driver = 
-00008190: 7365 6c66 2e73 7069 6465 725f 6368 726f  self.spider_chro
-000081a0: 6d65 5f64 7269 7665 7228 290a 2020 2020  me_driver().    
-000081b0: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
-000081c0: 2920 2023 2041 6c6c 6f77 2074 696d 6520  )  # Allow time 
-000081d0: 666f 7220 7468 6520 7061 6765 2074 6f20  for the page to 
-000081e0: 6c6f 6164 0a20 2020 2020 2020 2066 7261  load.        fra
-000081f0: 6d65 203d 2064 7269 7665 722e 6669 6e64  me = driver.find
-00008200: 5f65 6c65 6d65 6e74 2842 792e 5850 4154  _element(By.XPAT
-00008210: 482c 2027 2f2f 6966 7261 6d65 5b40 6964  H, '//iframe[@id
-00008220: 3d22 6946 7261 6d65 3122 5d27 290a 2020  ="iFrame1"]').  
-00008230: 2020 2020 2020 6472 6976 6572 2e73 7769        driver.swi
-00008240: 7463 685f 746f 2e66 7261 6d65 2866 7261  tch_to.frame(fra
-00008250: 6d65 290a 2020 2020 2020 2020 6d61 7463  me).        matc
-00008260: 6865 7320 3d20 7265 2e66 696e 6461 6c6c  hes = re.findall
-00008270: 2872 2767 6f4e 6578 7450 6167 655c 2828  (r'goNextPage\((
-00008280: 5c64 2b29 5c29 272c 2064 7269 7665 722e  \d+)\)', driver.
-00008290: 7061 6765 5f73 6f75 7263 6529 0a20 2020  page_source).   
-000082a0: 2020 2020 2070 6167 655f 696e 6465 7820       page_index 
-000082b0: 3d20 5b69 6e74 286d 6174 6368 2920 666f  = [int(match) fo
-000082c0: 7220 6d61 7463 6820 696e 206d 6174 6368  r match in match
-000082d0: 6573 5d0a 2020 2020 2020 2020 666f 7220  es].        for 
-000082e0: 696e 6465 7820 696e 2072 616e 6765 286d  index in range(m
-000082f0: 6178 2870 6167 655f 696e 6465 7829 293a  ax(page_index)):
-00008300: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
-00008310: 6169 7420 6461 7461 206c 6f61 640a 2020  ait data load.  
-00008320: 2020 2020 2020 2020 2020 5765 6244 7269            WebDri
-00008330: 7665 7257 6169 7428 6472 6976 6572 2c20  verWait(driver, 
-00008340: 3130 292e 756e 7469 6c28 0a20 2020 2020  10).until(.     
-00008350: 2020 2020 2020 2020 2020 2045 432e 7072             EC.pr
-00008360: 6573 656e 6365 5f6f 665f 656c 656d 656e  esence_of_elemen
-00008370: 745f 6c6f 6361 7465 6428 2842 792e 5850  t_located((By.XP
-00008380: 4154 482c 2027 2f2f 7462 6f64 795b 4069  ATH, '//tbody[@i
-00008390: 643d 2268 6973 746f 7279 4461 7461 225d  d="historyData"]
-000083a0: 2729 290a 2020 2020 2020 2020 2020 2020  ')).            
-000083b0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-000083c0: 2065 7874 7261 6374 2064 6174 610a 2020   extract data.  
-000083d0: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-000083e0: 7420 3d20 6472 6976 6572 2e66 696e 645f  t = driver.find_
-000083f0: 656c 656d 656e 7428 4279 2e58 5041 5448  element(By.XPATH
-00008400: 2c20 272f 2f74 626f 6479 5b40 6964 3d22  , '//tbody[@id="
-00008410: 6869 7374 6f72 7944 6174 6122 5d27 290a  historyData"]').
-00008420: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
-00008430: 5f64 6174 612e 6578 7465 6e64 285b 782e  _data.extend([x.
-00008440: 7370 6c69 7428 295b 3a39 5d20 666f 7220  split()[:9] for 
-00008450: 7820 696e 2063 6f6e 7465 6e74 2e74 6578  x in content.tex
-00008460: 742e 7370 6c69 7428 275c 6e27 2920 6966  t.split('\n') if
-00008470: 206c 656e 2878 2e73 706c 6974 2829 2920   len(x.split()) 
-00008480: 3e3d 2039 5d29 0a0a 2020 2020 2020 2020  >= 9])..        
-00008490: 2020 2020 2320 7761 6974 206e 6578 7420      # wait next 
-000084a0: 7061 6765 206c 6f61 640a 2020 2020 2020  page load.      
-000084b0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000084c0: 2020 2020 2020 2020 2020 2023 2074 7279             # try
-000084d0: 2074 6f20 6669 6e64 2065 6c65 6d65 6e74   to find element
-000084e0: 206f 6620 706f 7369 7469 6f6e 203d 3d20   of position == 
-000084f0: 3133 0a20 2020 2020 2020 2020 2020 2020  13.             
-00008500: 2020 206e 6578 745f 6275 7474 6f6e 203d     next_button =
-00008510: 2057 6562 4472 6976 6572 5761 6974 2864   WebDriverWait(d
-00008520: 7269 7665 722c 2031 3029 2e75 6e74 696c  river, 10).until
-00008530: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008540: 2020 2020 2020 4543 2e65 6c65 6d65 6e74        EC.element
-00008550: 5f74 6f5f 6265 5f63 6c69 636b 6162 6c65  _to_be_clickable
-00008560: 2828 4279 2e58 5041 5448 2c20 222f 6874  ((By.XPATH, "/ht
-00008570: 6d6c 2f62 6f64 792f 6469 762f 6469 762f  ml/body/div/div/
-00008580: 6469 765b 335d 2f75 6c2f 6c69 5b70 6f73  div[3]/ul/li[pos
-00008590: 6974 696f 6e28 293d 3133 5d22 2929 0a20  ition()=13]")). 
-000085a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000085b0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-000085c0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-000085d0: 2065 783a 0a20 2020 2020 2020 2020 2020   ex:.           
-000085e0: 2020 2020 2023 2074 7279 2074 6f20 6669       # try to fi
-000085f0: 6e64 2065 6c65 6d65 6e74 206f 6620 706f  nd element of po
-00008600: 7369 7469 6f6e 203d 3d20 380a 2020 2020  sition == 8.    
-00008610: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00008620: 5f62 7574 746f 6e20 3d20 5765 6244 7269  _button = WebDri
-00008630: 7665 7257 6169 7428 6472 6976 6572 2c20  verWait(driver, 
-00008640: 3130 292e 756e 7469 6c28 0a20 2020 2020  10).until(.     
-00008650: 2020 2020 2020 2020 2020 2020 2020 2045                 E
-00008660: 432e 656c 656d 656e 745f 746f 5f62 655f  C.element_to_be_
-00008670: 636c 6963 6b61 626c 6528 2842 792e 5850  clickable((By.XP
-00008680: 4154 482c 2022 2f68 746d 6c2f 626f 6479  ATH, "/html/body
-00008690: 2f64 6976 2f64 6976 2f64 6976 5b33 5d2f  /div/div/div[3]/
-000086a0: 756c 2f6c 695b 706f 7369 7469 6f6e 2829  ul/li[position()
-000086b0: 3d38 5d22 2929 0a20 2020 2020 2020 2020  =8]")).         
-000086c0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000086d0: 2020 2020 2020 2320 636c 6963 6b20 746f        # click to
-000086e0: 206e 6578 7420 7061 6765 0a20 2020 2020   next page.     
-000086f0: 2020 2020 2020 206e 6578 745f 6275 7474         next_butt
-00008700: 6f6e 2e63 6c69 636b 2829 0a20 2020 2020  on.click().     
-00008710: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00008720: 7028 3329 2020 2320 6c6f 6164 696e 670a  p(3)  # loading.
-00008730: 2020 2020 2020 2020 6472 6976 6572 2e71          driver.q
-00008740: 7569 7428 290a 2020 2020 2020 2020 736f  uit().        so
-00008750: 7274 6564 5f66 756c 6c5f 6461 7461 203d  rted_full_data =
-00008760: 2073 6f72 7465 6428 6675 6c6c 5f64 6174   sorted(full_dat
-00008770: 612c 206b 6579 3d6c 616d 6264 6120 783a  a, key=lambda x:
-00008780: 2069 6e74 2878 5b30 5d29 290a 0a20 2020   int(x[0]))..   
-00008790: 2020 2020 2072 6574 7572 6e20 736f 7274       return sort
-000087a0: 6564 5f66 756c 6c5f 6461 7461 0a0a 0a63  ed_full_data...c
-000087b0: 6c61 7373 2043 616c 6375 6c61 7465 5574  lass CalculateUt
-000087c0: 696c 2841 4243 293a 0a20 2020 2022 2222  il(ABC):.    """
-000087d0: 0a20 2020 2043 6f6d 7075 7465 2066 6561  .    Compute fea
-000087e0: 7475 7265 7320 6261 7365 6420 6f6e 2061  tures based on a
-000087f0: 2073 696e 676c 6520 6f72 206d 756c 7469   single or multi
-00008800: 206f 6620 6461 7461 0a20 2020 2022 2222   of data.    """
-00008810: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00008820: 686f 640a 2020 2020 6465 6620 6765 6e65  hod.    def gene
-00008830: 7261 7465 5f64 6174 6173 6574 735f 7769  rate_datasets_wi
-00008840: 7468 5f72 6f6c 6c69 6e67 5f73 697a 6528  th_rolling_size(
-00008850: 6461 7461 3a20 4c69 7374 5b69 6e74 5d2c  data: List[int],
-00008860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 2020 2020 2020 2020 2020 2020 2072 6f6c               rol
-00008890: 6c69 6e67 5f73 697a 653a 2069 6e74 203d  ling_size: int =
-000088a0: 2035 2c0a 2020 2020 2020 2020 2020 2020   5,.            
-000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088d0: 6164 6a75 7374 3a20 626f 6f6c 203d 2046  adjust: bool = F
-000088e0: 616c 7365 2920 2d3e 2054 7570 6c65 5b4c  alse) -> Tuple[L
-000088f0: 6973 745b 4c69 7374 5b69 6e74 5d5d 2c20  ist[List[int]], 
-00008900: 4c69 7374 5b69 6e74 5d5d 3a0a 2020 2020  List[int]]:.    
-00008910: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008920: 4765 6e65 7261 7465 7320 7365 7175 656e  Generates sequen
-00008930: 7469 616c 2074 6573 7420 616e 6420 7661  tial test and va
-00008940: 6c69 6461 7469 6f6e 2064 6174 6173 6574  lidation dataset
-00008950: 7320 6672 6f6d 2061 206c 6973 7420 6f66  s from a list of
-00008960: 2069 6e74 6567 6572 732e 2049 7420 6f70   integers. It op
-00008970: 7469 6f6e 616c 6c79 2061 646a 7573 7473  tionally adjusts
-00008980: 0a20 2020 2020 2020 2074 6573 7420 6461  .        test da
-00008990: 7461 7365 7473 2062 7920 7265 6d6f 7669  tasets by removi
-000089a0: 6e67 2065 7874 7265 6d65 2076 616c 7565  ng extreme value
-000089b0: 732e 0a0a 2020 2020 2020 2020 5468 6520  s...        The 
-000089c0: 6675 6e63 7469 6f6e 2069 7465 7261 7465  function iterate
-000089d0: 7320 6f76 6572 2074 6865 2064 6174 6120  s over the data 
-000089e0: 746f 2063 7265 6174 6520 6f76 6572 6c61  to create overla
-000089f0: 7070 696e 6720 7465 7374 2073 6574 7320  pping test sets 
-00008a00: 6f66 2061 2073 7065 6369 6669 6564 2073  of a specified s
-00008a10: 697a 652e 2045 6163 6820 7465 7374 2073  ize. Each test s
-00008a20: 6574 2069 730a 2020 2020 2020 2020 666f  et is.        fo
-00008a30: 6c6c 6f77 6564 2062 7920 6120 7661 6c69  llowed by a vali
-00008a40: 6461 7469 6f6e 2073 6574 2077 6869 6368  dation set which
-00008a50: 2069 7320 7468 6520 6e65 7874 2073 696e   is the next sin
-00008a60: 676c 6520 656c 656d 656e 7420 696e 2074  gle element in t
-00008a70: 6865 206c 6973 742e 2049 6620 7468 6520  he list. If the 
-00008a80: 2761 646a 7573 7427 2066 6c61 6720 6973  'adjust' flag is
-00008a90: 2054 7275 652c 0a20 2020 2020 2020 2074   True,.        t
-00008aa0: 6865 206d 6178 696d 756d 2061 6e64 206d  he maximum and m
-00008ab0: 696e 696d 756d 2076 616c 7565 7320 6172  inimum values ar
-00008ac0: 6520 7265 6d6f 7665 6420 6672 6f6d 2065  e removed from e
-00008ad0: 6163 6820 7465 7374 2073 6574 2e0a 0a20  ach test set... 
-00008ae0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00008af0: 2020 2020 2020 2020 2064 6174 6120 284c           data (L
-00008b00: 6973 745b 696e 745d 293a 2054 6865 2069  ist[int]): The i
-00008b10: 6e70 7574 2064 6174 6120 6c69 7374 2066  nput data list f
-00008b20: 726f 6d20 7768 6963 6820 6461 7461 7365  rom which datase
-00008b30: 7473 2061 7265 2067 656e 6572 6174 6564  ts are generated
-00008b40: 2e0a 2020 2020 2020 2020 2020 2020 726f  ..            ro
-00008b50: 6c6c 696e 675f 7369 7a65 2028 696e 7429  lling_size (int)
-00008b60: 3a20 5468 6520 6e75 6d62 6572 206f 6620  : The number of 
-00008b70: 656c 656d 656e 7473 2069 6e20 6561 6368  elements in each
-00008b80: 2074 6573 7420 7365 742e 2044 6566 6175   test set. Defau
-00008b90: 6c74 7320 746f 2035 2e0a 2020 2020 2020  lts to 5..      
-00008ba0: 2020 2020 2020 6164 6a75 7374 2028 626f        adjust (bo
-00008bb0: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
-00008bc0: 7265 6d6f 7665 2074 6865 206d 6178 696d  remove the maxim
-00008bd0: 756d 2061 6e64 206d 696e 696d 756d 2076  um and minimum v
-00008be0: 616c 7565 7320 6672 6f6d 2065 6163 6820  alues from each 
-00008bf0: 7465 7374 2073 6574 2e20 4465 6661 756c  test set. Defaul
-00008c00: 7473 2074 6f20 4661 6c73 652e 0a0a 2020  ts to False...  
-00008c10: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00008c20: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
-00008c30: 5b4c 6973 745b 4c69 7374 5b69 6e74 5d5d  [List[List[int]]
-00008c40: 2c20 4c69 7374 5b69 6e74 5d5d 3a20 4120  , List[int]]: A 
-00008c50: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
-00008c60: 2074 776f 206c 6973 7473 3a0a 2020 2020   two lists:.    
-00008c70: 2020 2020 2020 2020 2020 2020 2d20 5468              - Th
-00008c80: 6520 6669 7273 7420 6c69 7374 2063 6f6e  e first list con
-00008c90: 7461 696e 7320 7468 6520 7465 7374 2073  tains the test s
-00008ca0: 6574 732c 2070 6f73 7369 626c 7920 6164  ets, possibly ad
-00008cb0: 6a75 7374 6564 2e0a 2020 2020 2020 2020  justed..        
-00008cc0: 2020 2020 2020 2020 2d20 5468 6520 7365          - The se
-00008cd0: 636f 6e64 206c 6973 7420 636f 6e74 6169  cond list contai
-00008ce0: 6e73 2074 6865 2073 696e 676c 652d 656c  ns the single-el
-00008cf0: 656d 656e 7420 7661 6c69 6461 7469 6f6e  ement validation
-00008d00: 2073 6574 732e 0a20 2020 2020 2020 2022   sets..        "
-00008d10: 2222 0a20 2020 2020 2020 2078 5f73 6574  "".        x_set
-00008d20: 7320 3d20 5b5d 2020 2320 4c69 7374 2074  s = []  # List t
-00008d30: 6f20 686f 6c64 2074 6865 2074 6573 7420  o hold the test 
-00008d40: 7365 7473 0a20 2020 2020 2020 2079 5f73  sets.        y_s
-00008d50: 6574 7320 3d20 5b5d 2020 2320 4c69 7374  ets = []  # List
-00008d60: 2074 6f20 686f 6c64 2074 6865 2076 616c   to hold the val
-00008d70: 6964 6174 696f 6e20 7365 7473 0a0a 2020  idation sets..  
-00008d80: 2020 2020 2020 2320 4974 6572 6174 6520        # Iterate 
-00008d90: 6f76 6572 2074 6865 2064 6174 6120 746f  over the data to
-00008da0: 2066 6f72 6d20 7465 7374 2061 6e64 2076   form test and v
-00008db0: 616c 6964 6174 696f 6e20 7365 7473 0a20  alidation sets. 
-00008dc0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00008dd0: 7261 6e67 6528 6c65 6e28 6461 7461 2920  range(len(data) 
-00008de0: 2d20 726f 6c6c 696e 675f 7369 7a65 293a  - rolling_size):
-00008df0: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-00008e00: 745f 7365 7420 3d20 6461 7461 5b69 3a69  t_set = data[i:i
-00008e10: 202b 2072 6f6c 6c69 6e67 5f73 697a 655d   + rolling_size]
-00008e20: 2020 2320 4578 7472 6163 7420 7369 7a65    # Extract size
-00008e30: 2065 6c65 6d65 6e74 7320 666f 7220 7468   elements for th
-00008e40: 6520 7465 7374 2073 6574 0a20 2020 2020  e test set.     
-00008e50: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
-00008e60: 6e5f 7365 7420 3d20 6461 7461 5b69 202b  n_set = data[i +
-00008e70: 2072 6f6c 6c69 6e67 5f73 697a 655d 2020   rolling_size]  
-00008e80: 2320 5461 6b65 2074 6865 206e 6578 7420  # Take the next 
-00008e90: 656c 656d 656e 7420 6173 2074 6865 2076  element as the v
-00008ea0: 616c 6964 6174 696f 6e20 7365 740a 0a20  alidation set.. 
-00008eb0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00008ec0: 6e28 7465 7374 5f73 6574 2920 3e20 3220  n(test_set) > 2 
-00008ed0: 616e 6420 6164 6a75 7374 3a0a 2020 2020  and adjust:.    
-00008ee0: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-00008ef0: 6d6f 7665 2074 6865 206d 6178 696d 756d  move the maximum
-00008f00: 2061 6e64 206d 696e 696d 756d 2076 616c   and minimum val
-00008f10: 7565 7320 6966 2061 646a 7573 7469 6e67  ues if adjusting
-00008f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008f30: 206d 6178 5f76 616c 203d 206d 6178 2874   max_val = max(t
-00008f40: 6573 745f 7365 7429 0a20 2020 2020 2020  est_set).       
-00008f50: 2020 2020 2020 2020 206d 696e 5f76 616c           min_val
-00008f60: 203d 206d 696e 2874 6573 745f 7365 7429   = min(test_set)
-00008f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008f80: 206d 6178 5f69 6e64 6578 203d 2074 6573   max_index = tes
-00008f90: 745f 7365 742e 696e 6465 7828 6d61 785f  t_set.index(max_
-00008fa0: 7661 6c29 0a20 2020 2020 2020 2020 2020  val).           
-00008fb0: 2020 2020 206d 696e 5f69 6e64 6578 203d       min_index =
-00008fc0: 2074 6573 745f 7365 742e 696e 6465 7828   test_set.index(
-00008fd0: 6d69 6e5f 7661 6c29 0a20 2020 2020 2020  min_val).       
-00008fe0: 2020 2020 2020 2020 2066 696c 7465 7265           filtere
-00008ff0: 645f 7465 7374 5f73 6574 203d 205b 7820  d_test_set = [x 
-00009000: 666f 7220 6964 782c 2078 2069 6e20 656e  for idx, x in en
-00009010: 756d 6572 6174 6528 7465 7374 5f73 6574  umerate(test_set
-00009020: 2920 6966 2069 6478 2021 3d20 6d61 785f  ) if idx != max_
-00009030: 696e 6465 7820 616e 6420 6964 7820 213d  index and idx !=
-00009040: 206d 696e 5f69 6e64 6578 5d0a 2020 2020   min_index].    
-00009050: 2020 2020 2020 2020 2020 2020 785f 7365              x_se
-00009060: 7473 2e61 7070 656e 6428 6669 6c74 6572  ts.append(filter
-00009070: 6564 5f74 6573 745f 7365 7429 0a20 2020  ed_test_set).   
-00009080: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00009090: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-000090a0: 5f73 6574 732e 6170 7065 6e64 2874 6573  _sets.append(tes
-000090b0: 745f 7365 7429 2020 2320 4170 7065 6e64  t_set)  # Append
-000090c0: 2074 6865 2074 6573 7420 7365 7420 6173   the test set as
-000090d0: 2069 7320 6966 206e 6f74 2061 646a 7573   is if not adjus
-000090e0: 7469 6e67 0a0a 2020 2020 2020 2020 2020  ting..          
-000090f0: 2020 795f 7365 7473 2e61 7070 656e 6428    y_sets.append(
-00009100: 7661 6c69 6461 7469 6f6e 5f73 6574 2920  validation_set) 
-00009110: 2023 2041 7070 656e 6420 7468 6520 7661   # Append the va
-00009120: 6c69 6461 7469 6f6e 2065 6c65 6d65 6e74  lidation element
-00009130: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00009140: 2078 5f73 6574 732c 2079 5f73 6574 730a   x_sets, y_sets.
-00009150: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00009160: 640a 2020 2020 6465 6620 6361 6c63 756c  d.    def calcul
-00009170: 6174 655f 7a6f 6e65 5f72 6174 696f 280a  ate_zone_ratio(.
-00009180: 2020 2020 2020 2020 2020 2020 636c 732c              cls,
-00009190: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-000091a0: 6265 725f 636f 6d62 696e 6174 696f 6e3a  ber_combination:
-000091b0: 2049 7465 7261 626c 655b 696e 745d 2c0a   Iterable[int],.
-000091c0: 2020 2020 2020 2020 2020 2020 7a6f 6e65              zone
-000091d0: 5f72 616e 6765 733a 204c 6973 745b 5475  _ranges: List[Tu
-000091e0: 706c 655b 696e 742c 2069 6e74 5d5d 2c0a  ple[int, int]],.
-000091f0: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
-00009200: 6172 6773 3a20 416e 790a 2020 2020 2920  args: Any.    ) 
-00009210: 2d3e 2054 7570 6c65 5b69 6e74 2c20 2e2e  -> Tuple[int, ..
-00009220: 2e5d 3a0a 2020 2020 2020 2020 2222 220a  .]:.        """.
-00009230: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
-00009240: 6520 7468 6520 636f 756e 7473 206f 6620  e the counts of 
-00009250: 6e75 6d62 6572 7320 7769 7468 696e 2070  numbers within p
-00009260: 7265 6465 6669 6e65 6420 7a6f 6e65 7320  redefined zones 
-00009270: 666f 7220 6120 6769 7665 6e20 7365 7175  for a given sequ
-00009280: 656e 6365 206f 6620 6e75 6d62 6572 732e  ence of numbers.
-00009290: 0a20 2020 2020 2020 2054 6869 7320 636c  .        This cl
-000092a0: 6173 7320 6d65 7468 6f64 2064 6574 6572  ass method deter
-000092b0: 6d69 6e65 7320 7468 6520 6469 7374 7269  mines the distri
-000092c0: 6275 7469 6f6e 206f 6620 7468 6520 6e75  bution of the nu
-000092d0: 6d62 6572 7320 696e 2074 6865 2069 6e70  mbers in the inp
-000092e0: 7574 2073 6571 7565 6e63 6520 6163 726f  ut sequence acro
-000092f0: 7373 2073 7065 6369 6669 6564 207a 6f6e  ss specified zon
-00009300: 6573 2e0a 2020 2020 2020 2020 4561 6368  es..        Each
-00009310: 207a 6f6e 6520 6973 2064 6566 696e 6564   zone is defined
-00009320: 2062 7920 6120 7261 6e67 652c 2061 6e64   by a range, and
-00009330: 2074 6869 7320 6d65 7468 6f64 2063 6f75   this method cou
-00009340: 6e74 7320 686f 7720 6d61 6e79 206e 756d  nts how many num
-00009350: 6265 7273 2066 616c 6c20 696e 746f 2065  bers fall into e
-00009360: 6163 6820 7a6f 6e65 2e0a 0a20 2020 2020  ach zone...     
-00009370: 2020 203a 7061 7261 6d20 6e75 6d62 6572     :param number
-00009380: 5f63 6f6d 6269 6e61 7469 6f6e 3a20 416e  _combination: An
-00009390: 2069 7465 7261 626c 6520 6f66 206e 756d   iterable of num
-000093a0: 6265 7273 2028 6c69 6b65 2061 206c 6973  bers (like a lis
-000093b0: 7420 6f72 2074 7570 6c65 2920 6672 6f6d  t or tuple) from
-000093c0: 2077 6869 6368 2074 6865 206d 6574 686f   which the metho
-000093d0: 6420 7769 6c6c 2063 6f75 6e74 2068 6f77  d will count how
-000093e0: 206d 616e 790a 2020 2020 2020 2020 2020   many.          
-000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009400: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-00009410: 7320 6661 6c6c 2069 6e74 6f20 6561 6368  s fall into each
-00009420: 207a 6f6e 652e 0a20 2020 2020 2020 203a   zone..        :
-00009430: 7061 7261 6d20 7a6f 6e65 5f72 616e 6765  param zone_range
-00009440: 733a 2041 206c 6973 7420 6f66 2074 7570  s: A list of tup
-00009450: 6c65 7320 7768 6572 6520 6561 6368 2074  les where each t
-00009460: 7570 6c65 2063 6f6e 7461 696e 7320 7477  uple contains tw
-00009470: 6f20 6e75 6d62 6572 7320 7265 7072 6573  o numbers repres
-00009480: 656e 7469 6e67 2074 6865 2073 7461 7274  enting the start
-00009490: 2061 6e64 2065 6e64 206f 6620 610a 2020   and end of a.  
-000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094b0: 2020 2020 2020 2020 2020 7a6f 6e65 2072            zone r
-000094c0: 616e 6765 2c20 7265 7370 6563 7469 7665  ange, respective
-000094d0: 6c79 2e20 5468 6573 6520 7261 6e67 6573  ly. These ranges
-000094e0: 2064 6566 696e 6520 7468 6520 7a6f 6e65   define the zone
-000094f0: 7320 666f 7220 6361 7465 676f 7269 7a69  s for categorizi
-00009500: 6e67 2074 6865 206e 756d 6265 7273 2e0a  ng the numbers..
-00009510: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-00009520: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
-00009530: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-00009540: 6e74 7320 7468 6174 206d 6179 2062 6520  nts that may be 
-00009550: 7573 6564 2066 6f72 2066 7574 7572 6520  used for future 
-00009560: 6578 7465 6e73 696f 6e73 206f 6620 7468  extensions of th
-00009570: 6520 6d65 7468 6f64 2e0a 2020 2020 2020  e method..      
-00009580: 2020 3a72 6574 7572 6e3a 2041 2074 7570    :return: A tup
-00009590: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
-000095a0: 6520 636f 756e 7420 6f66 206e 756d 6265  e count of numbe
-000095b0: 7273 2074 6861 7420 6661 6c6c 2077 6974  rs that fall wit
-000095c0: 6869 6e20 6561 6368 2073 7065 6369 6669  hin each specifi
-000095d0: 6564 207a 6f6e 652e 0a20 2020 2020 2020  ed zone..       
-000095e0: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
-000095f0: 4368 6563 6b20 6966 207a 6f6e 6520 7261  Check if zone ra
-00009600: 6e67 6573 2061 7265 2064 6566 696e 6564  nges are defined
-00009610: 2c20 6966 206e 6f74 2c20 7261 6973 6520  , if not, raise 
-00009620: 616e 2065 7863 6570 7469 6f6e 2e0a 2020  an exception..  
-00009630: 2020 2020 2020 6966 206e 6f74 207a 6f6e        if not zon
-00009640: 655f 7261 6e67 6573 3a0a 2020 2020 2020  e_ranges:.      
-00009650: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00009660: 6545 7272 6f72 2827 5a6f 6e65 2072 616e  eError('Zone ran
-00009670: 6765 7320 6d75 7374 2062 6520 7072 6f76  ges must be prov
-00009680: 6964 6564 2e27 290a 0a20 2020 2020 2020  ided.')..       
-00009690: 2023 2049 6e69 7469 616c 697a 6520 636f   # Initialize co
-000096a0: 756e 7465 7273 2066 6f72 2065 6163 6820  unters for each 
-000096b0: 7a6f 6e65 2074 6f20 7a65 726f 2e0a 2020  zone to zero..  
-000096c0: 2020 2020 2020 7261 7469 6f20 3d20 5b30        ratio = [0
-000096d0: 5d20 2a20 6c65 6e28 7a6f 6e65 5f72 616e  ] * len(zone_ran
-000096e0: 6765 7329 0a0a 2020 2020 2020 2020 2320  ges)..        # 
-000096f0: 4974 6572 6174 6520 7468 726f 7567 6820  Iterate through 
-00009700: 6561 6368 206e 756d 6265 7220 616e 6420  each number and 
-00009710: 6368 6563 6b20 7768 6963 6820 7a6f 6e65  check which zone
-00009720: 2069 7420 6661 6c6c 7320 696e 746f 2e0a   it falls into..
-00009730: 2020 2020 2020 2020 666f 7220 6e75 6d20          for num 
-00009740: 696e 206d 6170 2869 6e74 2c20 6e75 6d62  in map(int, numb
-00009750: 6572 5f63 6f6d 6269 6e61 7469 6f6e 293a  er_combination):
-00009760: 2020 2320 436f 6e76 6572 7420 6561 6368    # Convert each
-00009770: 206e 756d 6265 7220 746f 2061 6e20 696e   number to an in
-00009780: 7465 6765 7220 6f6e 6365 2062 6566 6f72  teger once befor
-00009790: 6520 7468 6520 6c6f 6f70 2e0a 2020 2020  e the loop..    
-000097a0: 2020 2020 2020 2020 666f 7220 692c 2028          for i, (
-000097b0: 7374 6172 742c 2065 6e64 2920 696e 2065  start, end) in e
-000097c0: 6e75 6d65 7261 7465 287a 6f6e 655f 7261  numerate(zone_ra
-000097d0: 6e67 6573 293a 0a20 2020 2020 2020 2020  nges):.         
-000097e0: 2020 2020 2020 2069 6620 7374 6172 7420         if start 
-000097f0: 3c3d 206e 756d 203c 3d20 656e 643a 0a20  <= num <= end:. 
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 2020 2072 6174 696f 5b69 5d20 2b3d 2031     ratio[i] += 1
-00009820: 2020 2320 496e 6372 656d 656e 7420 7468    # Increment th
-00009830: 6520 636f 756e 7465 7220 666f 7220 7468  e counter for th
-00009840: 6520 6375 7272 656e 7420 7a6f 6e65 2e0a  e current zone..
-00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009860: 2020 2020 6272 6561 6b20 2023 2049 6620      break  # If 
-00009870: 7468 6520 6e75 6d62 6572 2069 7320 7769  the number is wi
-00009880: 7468 696e 2074 6865 2063 7572 7265 6e74  thin the current
-00009890: 207a 6f6e 652c 206e 6f20 6e65 6564 2074   zone, no need t
-000098a0: 6f20 6368 6563 6b20 6675 7274 6865 7220  o check further 
-000098b0: 7a6f 6e65 732e 0a0a 2020 2020 2020 2020  zones...        
-000098c0: 2320 5265 7475 726e 2074 6865 2063 6f75  # Return the cou
-000098d0: 6e74 7320 6173 2061 2074 7570 6c65 2c20  nts as a tuple, 
-000098e0: 7769 7468 2065 6163 6820 656c 656d 656e  with each elemen
-000098f0: 7420 7265 7072 6573 656e 7469 6e67 2074  t representing t
-00009900: 6865 2063 6f75 6e74 2066 6f72 2061 2072  he count for a r
-00009910: 6573 7065 6374 6976 6520 7a6f 6e65 2e0a  espective zone..
-00009920: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00009930: 7570 6c65 2872 6174 696f 290a 0a20 2020  uple(ratio)..   
-00009940: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00009950: 2020 6465 6620 6361 6c63 756c 6174 655f    def calculate_
-00009960: 6269 675f 736d 616c 6c5f 7261 7469 6f28  big_small_ratio(
-00009970: 0a20 2020 2020 2020 2020 2020 2063 6c73  .            cls
-00009980: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
-00009990: 6d62 6572 5f63 6f6d 6269 6e61 7469 6f6e  mber_combination
-000099a0: 733a 2049 7465 7261 626c 655b 696e 745d  s: Iterable[int]
-000099b0: 2c0a 2020 2020 2020 2020 2020 2020 6269  ,.            bi
-000099c0: 675f 736d 616c 6c5f 7261 6e67 6573 3a20  g_small_ranges: 
-000099d0: 4c69 7374 5b54 7570 6c65 5b69 6e74 2c20  List[Tuple[int, 
-000099e0: 696e 745d 5d2c 0a20 2020 2020 2020 2020  int]],.         
-000099f0: 2020 202a 2a6b 7761 7267 733a 2041 6e79     **kwargs: Any
-00009a00: 0a20 2020 2029 202d 3e20 5475 706c 655b  .    ) -> Tuple[
-00009a10: 696e 742c 202e 2e2e 5d3a 0a20 2020 2020  int, ...]:.     
-00009a20: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00009a30: 616c 6375 6c61 7465 2074 6865 2063 6f75  alculate the cou
-00009a40: 6e74 7320 6f66 206e 756d 6265 7273 2077  nts of numbers w
-00009a50: 6974 6869 6e20 7072 6564 6566 696e 6564  ithin predefined
-00009a60: 2073 697a 6520 7261 6e67 6573 2066 6f72   size ranges for
-00009a70: 2061 2073 6571 7565 6e63 6520 6f66 206e   a sequence of n
-00009a80: 756d 6265 7273 2e0a 2020 2020 2020 2020  umbers..        
-00009a90: 5468 6973 2063 6c61 7373 206d 6574 686f  This class metho
-00009aa0: 6420 6173 7365 7373 6573 2068 6f77 206d  d assesses how m
-00009ab0: 616e 7920 6e75 6d62 6572 7320 6672 6f6d  any numbers from
-00009ac0: 2074 6865 2069 6e70 7574 2073 6571 7565   the input seque
-00009ad0: 6e63 6520 6661 6c6c 2077 6974 6869 6e20  nce fall within 
-00009ae0: 6561 6368 206f 6620 7468 6520 7370 6563  each of the spec
-00009af0: 6966 6965 6420 7369 7a65 2072 616e 6765  ified size range
-00009b00: 732e 0a20 2020 2020 2020 2045 6163 6820  s..        Each 
-00009b10: 7261 6e67 6520 7265 7072 6573 656e 7473  range represents
-00009b20: 2061 2027 7a6f 6e65 272c 2077 6869 6368   a 'zone', which
-00009b30: 2063 6f75 6c64 2063 6f72 7265 7370 6f6e   could correspon
-00009b40: 6420 746f 2061 2063 6f6e 6365 7074 206c  d to a concept l
-00009b50: 696b 6520 2762 6967 2720 6f72 2027 736d  ike 'big' or 'sm
-00009b60: 616c 6c27 206e 756d 6265 7273 2e0a 0a20  all' numbers... 
-00009b70: 2020 2020 2020 203a 7061 7261 6d20 6e75         :param nu
-00009b80: 6d62 6572 5f63 6f6d 6269 6e61 7469 6f6e  mber_combination
-00009b90: 733a 2041 6e20 6974 6572 6162 6c65 206f  s: An iterable o
-00009ba0: 6620 6e75 6d62 6572 7320 286c 696b 6520  f numbers (like 
-00009bb0: 6120 6c69 7374 206f 7220 7475 706c 6529  a list or tuple)
-00009bc0: 2066 726f 6d20 7768 6963 6820 7468 6520   from which the 
-00009bd0: 6d65 7468 6f64 2077 696c 6c20 636f 756e  method will coun
-00009be0: 7420 686f 7720 6d61 6e79 0a20 2020 2020  t how many.     
-00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00009c10: 756d 6265 7273 2066 616c 6c20 696e 746f  umbers fall into
-00009c20: 2065 6163 6820 7369 7a65 2072 616e 6765   each size range
-00009c30: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00009c40: 2062 6967 5f73 6d61 6c6c 5f72 616e 6765   big_small_range
-00009c50: 733a 2041 206c 6973 7420 6f66 2074 7570  s: A list of tup
-00009c60: 6c65 7320 7768 6572 6520 6561 6368 2074  les where each t
-00009c70: 7570 6c65 2063 6f6e 7461 696e 7320 7477  uple contains tw
-00009c80: 6f20 6e75 6d62 6572 7320 7265 7072 6573  o numbers repres
-00009c90: 656e 7469 6e67 2074 6865 2073 7461 7274  enting the start
-00009ca0: 2061 6e64 2065 6e64 206f 6620 610a 2020   and end of a.  
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009cd0: 616e 6765 2c20 7265 7370 6563 7469 7665  ange, respective
-00009ce0: 6c79 2e20 5468 6573 6520 7261 6e67 6573  ly. These ranges
-00009cf0: 2064 6566 696e 6520 7468 6520 7a6f 6e65   define the zone
-00009d00: 7320 666f 7220 6361 7465 676f 7269 7a69  s for categorizi
-00009d10: 6e67 2074 6865 206e 756d 6265 7273 2e0a  ng the numbers..
-00009d20: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-00009d30: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
-00009d40: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-00009d50: 6e74 7320 7468 6174 206d 6179 2062 6520  nts that may be 
-00009d60: 7573 6564 2066 6f72 2066 7574 7572 6520  used for future 
-00009d70: 6578 7465 6e73 696f 6e73 206f 6620 7468  extensions of th
-00009d80: 6520 6d65 7468 6f64 2e0a 2020 2020 2020  e method..      
-00009d90: 2020 3a72 6574 7572 6e3a 2041 2074 7570    :return: A tup
-00009da0: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
-00009db0: 6520 636f 756e 7420 6f66 206e 756d 6265  e count of numbe
-00009dc0: 7273 2074 6861 7420 6661 6c6c 2077 6974  rs that fall wit
-00009dd0: 6869 6e20 6561 6368 2073 7065 6369 6669  hin each specifi
-00009de0: 6564 2072 616e 6765 206f 7220 277a 6f6e  ed range or 'zon
-00009df0: 6527 2e0a 2020 2020 2020 2020 2222 220a  e'..        """.
-00009e00: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
-00009e10: 2069 6620 7369 7a65 2072 616e 6765 7320   if size ranges 
-00009e20: 6172 6520 6465 6669 6e65 642c 2069 6620  are defined, if 
-00009e30: 6e6f 742c 2072 6169 7365 2061 6e20 6578  not, raise an ex
-00009e40: 6365 7074 696f 6e2e 0a20 2020 2020 2020  ception..       
-00009e50: 2069 6620 6e6f 7420 6269 675f 736d 616c   if not big_smal
-00009e60: 6c5f 7261 6e67 6573 3a0a 2020 2020 2020  l_ranges:.      
-00009e70: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00009e80: 6545 7272 6f72 2827 5369 7a65 2072 616e  eError('Size ran
-00009e90: 6765 7320 666f 7220 6269 6720 616e 6420  ges for big and 
-00009ea0: 736d 616c 6c20 6e75 6d62 6572 7320 6d75  small numbers mu
-00009eb0: 7374 2062 6520 7072 6f76 6964 6564 2e27  st be provided.'
-00009ec0: 290a 0a20 2020 2020 2020 2023 2049 6e69  )..        # Ini
-00009ed0: 7469 616c 697a 6520 636f 756e 7465 7273  tialize counters
-00009ee0: 2066 6f72 2065 6163 6820 7261 6e67 6520   for each range 
-00009ef0: 746f 207a 6572 6f2e 0a20 2020 2020 2020  to zero..       
-00009f00: 2072 6174 696f 203d 205b 305d 202a 206c   ratio = [0] * l
-00009f10: 656e 2862 6967 5f73 6d61 6c6c 5f72 616e  en(big_small_ran
-00009f20: 6765 7329 0a0a 2020 2020 2020 2020 2320  ges)..        # 
-00009f30: 4974 6572 6174 6520 7468 726f 7567 6820  Iterate through 
-00009f40: 6561 6368 206e 756d 6265 7220 616e 6420  each number and 
-00009f50: 6368 6563 6b20 7768 6963 6820 7261 6e67  check which rang
-00009f60: 6520 6974 2066 616c 6c73 2069 6e74 6f2e  e it falls into.
-00009f70: 0a20 2020 2020 2020 2066 6f72 206e 756d  .        for num
-00009f80: 2069 6e20 6d61 7028 696e 742c 206e 756d   in map(int, num
-00009f90: 6265 725f 636f 6d62 696e 6174 696f 6e73  ber_combinations
-00009fa0: 293a 2020 2320 436f 6e76 6572 7420 6561  ):  # Convert ea
-00009fb0: 6368 206e 756d 6265 7220 746f 2061 6e20  ch number to an 
-00009fc0: 696e 7465 6765 7220 6f6e 6365 2062 6566  integer once bef
-00009fd0: 6f72 6520 7468 6520 6c6f 6f70 2e0a 2020  ore the loop..  
-00009fe0: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-00009ff0: 2028 7374 6172 742c 2065 6e64 2920 696e   (start, end) in
-0000a000: 2065 6e75 6d65 7261 7465 2862 6967 5f73   enumerate(big_s
-0000a010: 6d61 6c6c 5f72 616e 6765 7329 3a0a 2020  mall_ranges):.  
-0000a020: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000a030: 2073 7461 7274 203c 3d20 6e75 6d20 3c3d   start <= num <=
-0000a040: 2065 6e64 3a0a 2020 2020 2020 2020 2020   end:.          
-0000a050: 2020 2020 2020 2020 2020 7261 7469 6f5b            ratio[
-0000a060: 695d 202b 3d20 3120 2023 2049 6e63 7265  i] += 1  # Incre
-0000a070: 6d65 6e74 2074 6865 2063 6f75 6e74 6572  ment the counter
-0000a080: 2066 6f72 2074 6865 2063 7572 7265 6e74   for the current
-0000a090: 2072 616e 6765 2e0a 2020 2020 2020 2020   range..        
-0000a0a0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0000a0b0: 6b20 2023 2049 6620 7468 6520 6e75 6d62  k  # If the numb
-0000a0c0: 6572 2069 7320 7769 7468 696e 2074 6865  er is within the
-0000a0d0: 2063 7572 7265 6e74 2072 616e 6765 2c20   current range, 
-0000a0e0: 6e6f 206e 6565 6420 746f 2063 6865 636b  no need to check
-0000a0f0: 2066 7572 7468 6572 2072 616e 6765 732e   further ranges.
-0000a100: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
-0000a110: 726e 2074 6865 2063 6f75 6e74 7320 6173  rn the counts as
-0000a120: 2061 2074 7570 6c65 2c20 7769 7468 2065   a tuple, with e
-0000a130: 6163 6820 656c 656d 656e 7420 7265 7072  ach element repr
-0000a140: 6573 656e 7469 6e67 2074 6865 2063 6f75  esenting the cou
-0000a150: 6e74 2066 6f72 2061 2072 6573 7065 6374  nt for a respect
-0000a160: 6976 6520 7261 6e67 6520 6f72 2027 7a6f  ive range or 'zo
-0000a170: 6e65 272e 0a20 2020 2020 2020 2072 6574  ne'..        ret
-0000a180: 7572 6e20 7475 706c 6528 7261 7469 6f29  urn tuple(ratio)
-0000a190: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-0000a1a0: 6f64 0a20 2020 2064 6566 2063 616c 6375  od.    def calcu
-0000a1b0: 6c61 7465 5f72 6f61 645f 3031 325f 7261  late_road_012_ra
-0000a1c0: 7469 6f28 0a20 2020 2020 2020 2020 2020  tio(.           
-0000a1d0: 2063 6c73 2c0a 2020 2020 2020 2020 2020   cls,.          
-0000a1e0: 2020 6e75 6d62 6572 5f63 6f6d 6269 6e61    number_combina
-0000a1f0: 7469 6f6e 3a20 4974 6572 6162 6c65 5b69  tion: Iterable[i
-0000a200: 6e74 5d2c 0a20 2020 2020 2020 2020 2020  nt],.           
-0000a210: 2072 6f61 645f 3031 325f 7261 6e67 6573   road_012_ranges
-0000a220: 3a20 4c69 7374 5b74 7570 6c65 5b69 6e74  : List[tuple[int
-0000a230: 2c20 2e2e 2e5d 5d2c 0a20 2020 2020 2020  , ...]],.       
-0000a240: 2020 2020 202a 2a6b 7761 7267 733a 2041       **kwargs: A
-0000a250: 6e79 0a20 2020 2029 202d 3e20 5475 706c  ny.    ) -> Tupl
-0000a260: 655b 696e 742c 202e 2e2e 5d3a 0a20 2020  e[int, ...]:.   
-0000a270: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000a280: 2043 616c 6375 6c61 7465 2074 6865 2063   Calculate the c
-0000a290: 6f75 6e74 206f 6620 6e75 6d62 6572 7320  ount of numbers 
-0000a2a0: 7769 7468 696e 2070 7265 6465 6669 6e65  within predefine
-0000a2b0: 6420 7a6f 6e65 7320 2872 6566 6572 7265  d zones (referre
-0000a2c0: 6420 746f 2061 7320 2772 6f61 6473 2729  d to as 'roads')
-0000a2d0: 2066 6f72 2061 2067 6976 656e 2073 6571   for a given seq
-0000a2e0: 7565 6e63 6520 6f66 206e 756d 6265 7273  uence of numbers
-0000a2f0: 2e0a 2020 2020 2020 2020 5468 6973 2063  ..        This c
-0000a300: 6c61 7373 206d 6574 686f 6420 6465 7465  lass method dete
-0000a310: 726d 696e 6573 2068 6f77 206d 616e 7920  rmines how many 
-0000a320: 6e75 6d62 6572 7320 6672 6f6d 2074 6865  numbers from the
-0000a330: 2069 6e70 7574 2066 616c 6c20 7769 7468   input fall with
-0000a340: 696e 2065 6163 6820 6f66 2074 6865 2073  in each of the s
-0000a350: 7065 6369 6669 6564 2072 616e 6765 732e  pecified ranges.
-0000a360: 2045 6163 6820 7261 6e67 650a 2020 2020   Each range.    
-0000a370: 2020 2020 7265 7072 6573 656e 7473 2061      represents a
-0000a380: 2027 726f 6164 272c 2077 6869 6368 2069   'road', which i
-0000a390: 7320 6120 7365 676d 656e 7420 6f66 2074  s a segment of t
-0000a3a0: 6865 206f 7665 7261 6c6c 2064 6174 6120  he overall data 
-0000a3b0: 7365 742e 0a0a 2020 2020 2020 2020 3a70  set...        :p
-0000a3c0: 6172 616d 206e 756d 6265 725f 636f 6d62  aram number_comb
-0000a3d0: 696e 6174 696f 6e3a 2041 206c 6973 742c  ination: A list,
-0000a3e0: 2074 7570 6c65 2c20 6f72 206f 7468 6572   tuple, or other
-0000a3f0: 2069 7465 7261 626c 6520 6f66 206e 756d   iterable of num
-0000a400: 6265 7273 2e20 5468 6520 6d65 7468 6f64  bers. The method
-0000a410: 2077 696c 6c20 6974 6572 6174 6520 7468   will iterate th
-0000a420: 726f 7567 6820 7468 6973 0a20 2020 2020  rough this.     
-0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a440: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000a450: 6c6c 6563 7469 6f6e 2074 6f20 636f 756e  llection to coun
-0000a460: 7420 686f 7720 6d61 6e79 206e 756d 6265  t how many numbe
-0000a470: 7273 2066 616c 6c20 696e 746f 2065 6163  rs fall into eac
-0000a480: 6820 2772 6f61 6427 2061 7320 6465 6669  h 'road' as defi
-0000a490: 6e65 6420 6279 2074 6865 2072 616e 6765  ned by the range
-0000a4a0: 732e 0a20 2020 2020 2020 203a 7061 7261  s..        :para
-0000a4b0: 6d20 726f 6164 5f30 3132 5f72 616e 6765  m road_012_range
-0000a4c0: 733a 2041 206c 6973 7420 6f66 2072 616e  s: A list of ran
-0000a4d0: 6765 206f 626a 6563 7473 206f 7220 7365  ge objects or se
-0000a4e0: 7175 656e 6365 7320 6465 6669 6e69 6e67  quences defining
-0000a4f0: 2074 6865 2027 726f 6164 7327 2e20 4561   the 'roads'. Ea
-0000a500: 6368 2065 6c65 6d65 6e74 2069 6e20 7468  ch element in th
-0000a510: 6973 206c 6973 740a 2020 2020 2020 2020  is list.        
-0000a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a530: 2020 2020 2020 2020 636f 7272 6573 706f          correspo
-0000a540: 6e64 7320 746f 2061 2064 6966 6665 7265  nds to a differe
-0000a550: 6e74 2027 726f 6164 272c 2061 6e64 2074  nt 'road', and t
-0000a560: 6865 206e 756d 6265 7273 2069 6e20 276e  he numbers in 'n
-0000a570: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
-0000a580: 6e27 2061 7265 2063 6865 636b 6564 0a20  n' are checked. 
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000a5b0: 6761 696e 7374 2074 6865 7365 2072 616e  gainst these ran
-0000a5c0: 6765 7320 746f 2064 6574 6572 6d69 6e65  ges to determine
-0000a5d0: 2074 6865 6972 2063 6f75 6e74 732e 0a20   their counts.. 
-0000a5e0: 2020 2020 2020 203a 7061 7261 6d20 6b77         :param kw
-0000a5f0: 6172 6773 3a20 4164 6469 7469 6f6e 616c  args: Additional
-0000a600: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-0000a610: 7473 2074 6861 7420 6172 6520 6e6f 7420  ts that are not 
-0000a620: 7573 6564 2069 6e20 7468 6973 206d 6574  used in this met
-0000a630: 686f 6420 6275 7420 6172 6520 696e 636c  hod but are incl
-0000a640: 7564 6564 2066 6f72 2070 6f74 656e 7469  uded for potenti
-0000a650: 616c 0a20 2020 2020 2020 2020 2020 2020  al.             
-0000a660: 2020 2020 2020 2020 2020 6675 7475 7265            future
-0000a670: 2065 7874 656e 7369 6269 6c69 7479 206f   extensibility o
-0000a680: 6620 7468 6520 6d65 7468 6f64 2e0a 2020  f the method..  
-0000a690: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
-0000a6a0: 2074 7570 6c65 2063 6f6e 7461 696e 696e   tuple containin
-0000a6b0: 6720 7468 6520 636f 756e 7420 6f66 206e  g the count of n
-0000a6c0: 756d 6265 7273 2069 6e20 6561 6368 2027  umbers in each '
-0000a6d0: 726f 6164 272e 0a20 2020 2020 2020 2022  road'..        "
-0000a6e0: 2222 0a0a 2020 2020 2020 2020 2320 5661  ""..        # Va
-0000a6f0: 6c69 6461 7465 2074 6865 2070 7265 7365  lidate the prese
-0000a700: 6e63 6520 6f66 2027 726f 6164 5f30 3132  nce of 'road_012
-0000a710: 5f72 616e 6765 7327 2e0a 2020 2020 2020  _ranges'..      
-0000a720: 2020 6966 206e 6f74 2072 6f61 645f 3031    if not road_01
-0000a730: 325f 7261 6e67 6573 3a0a 2020 2020 2020  2_ranges:.      
-0000a740: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000a750: 6545 7272 6f72 2827 526f 6164 2030 3132  eError('Road 012
-0000a760: 2072 616e 6765 7320 6d75 7374 2062 6520   ranges must be 
-0000a770: 7072 6f76 6964 6564 2e27 290a 0a20 2020  provided.')..   
-0000a780: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
-0000a790: 6520 636f 756e 7465 7273 2066 6f72 2065  e counters for e
-0000a7a0: 6163 6820 2772 6f61 6427 2074 6f20 7a65  ach 'road' to ze
-0000a7b0: 726f 2e0a 2020 2020 2020 2020 7261 7469  ro..        rati
-0000a7c0: 6f20 3d20 5b30 5d20 2a20 6c65 6e28 726f  o = [0] * len(ro
-0000a7d0: 6164 5f30 3132 5f72 616e 6765 7329 0a0a  ad_012_ranges)..
-0000a7e0: 2020 2020 2020 2020 2320 436f 756e 7420          # Count 
-0000a7f0: 7468 6520 6e75 6d62 6572 7320 696e 2065  the numbers in e
-0000a800: 6163 6820 2772 6f61 6427 2062 7920 6974  ach 'road' by it
-0000a810: 6572 6174 696e 6720 7468 726f 7567 6820  erating through 
-0000a820: 7468 6520 696e 7075 7420 6e75 6d62 6572  the input number
-0000a830: 7320 616e 6420 7468 6520 6465 6669 6e65  s and the define
-0000a840: 6420 7261 6e67 6573 2e0a 2020 2020 2020  d ranges..      
-0000a850: 2020 666f 7220 6e75 6d20 696e 206d 6170    for num in map
-0000a860: 2869 6e74 2c20 6e75 6d62 6572 5f63 6f6d  (int, number_com
-0000a870: 6269 6e61 7469 6f6e 293a 2020 2320 436f  bination):  # Co
-0000a880: 6e76 6572 7420 6561 6368 206e 756d 6265  nvert each numbe
-0000a890: 7220 746f 2061 6e20 696e 7465 6765 7220  r to an integer 
-0000a8a0: 6f6e 6365 2c20 6265 666f 7265 2074 6865  once, before the
-0000a8b0: 206c 6f6f 702e 0a20 2020 2020 2020 2020   loop..         
-0000a8c0: 2020 2066 6f72 2069 2c20 7661 6c73 2069     for i, vals i
-0000a8d0: 6e20 656e 756d 6572 6174 6528 726f 6164  n enumerate(road
-0000a8e0: 5f30 3132 5f72 616e 6765 7329 3a0a 2020  _012_ranges):.  
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000a900: 206e 756d 2069 6e20 7661 6c73 3a0a 2020   num in vals:.  
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a920: 2020 7261 7469 6f5b 695d 202b 3d20 310a    ratio[i] += 1.
-0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a940: 2020 2020 6272 6561 6b20 2023 204f 6e63      break  # Onc
-0000a950: 6520 7468 6520 6e75 6d62 6572 2069 7320  e the number is 
-0000a960: 666f 756e 6420 696e 2061 2027 726f 6164  found in a 'road
-0000a970: 272c 2073 746f 7020 6368 6563 6b69 6e67  ', stop checking
-0000a980: 2074 6865 2072 656d 6169 6e69 6e67 2027   the remaining '
-0000a990: 726f 6164 7327 2e0a 0a20 2020 2020 2020  roads'...       
-0000a9a0: 2023 2052 6574 7572 6e20 7468 6520 636f   # Return the co
-0000a9b0: 756e 7473 2061 7320 6120 7475 706c 652c  unts as a tuple,
-0000a9c0: 2077 6974 6820 6561 6368 2065 6c65 6d65   with each eleme
-0000a9d0: 6e74 2072 6570 7265 7365 6e74 696e 6720  nt representing 
-0000a9e0: 7468 6520 636f 756e 7420 666f 7220 6120  the count for a 
-0000a9f0: 7265 7370 6563 7469 7665 2027 726f 6164  respective 'road
-0000aa00: 272e 0a20 2020 2020 2020 2072 6574 7572  '..        retur
-0000aa10: 6e20 7475 706c 6528 7261 7469 6f29 0a0a  n tuple(ratio)..
-0000aa20: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-0000aa30: 0a20 2020 2064 6566 2063 616c 6375 6c61  .    def calcula
-0000aa40: 7465 5f6f 6464 5f65 7665 6e5f 7261 7469  te_odd_even_rati
-0000aa50: 6f28 0a20 2020 2020 2020 2020 2020 2063  o(.            c
-0000aa60: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-0000aa70: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
-0000aa80: 6f6e 3a20 4974 6572 6162 6c65 5b69 6e74  on: Iterable[int
-0000aa90: 5d2c 0a20 2020 2020 2020 2020 2020 202a  ],.            *
-0000aaa0: 2a6b 7761 7267 733a 2041 6e79 0a20 2020  *kwargs: Any.   
-0000aab0: 2029 202d 3e20 5475 706c 655b 696e 742c   ) -> Tuple[int,
-0000aac0: 2069 6e74 5d3a 0a20 2020 2020 2020 2022   int]:.        "
-0000aad0: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
-0000aae0: 6c61 7465 2074 6865 2072 6174 696f 206f  late the ratio o
-0000aaf0: 6620 6f64 6420 746f 2065 7665 6e20 6e75  f odd to even nu
-0000ab00: 6d62 6572 7320 7769 7468 696e 2061 2067  mbers within a g
-0000ab10: 6976 656e 2073 6571 7565 6e63 6520 6f66  iven sequence of
-0000ab20: 206e 756d 6265 7273 2e0a 2020 2020 2020   numbers..      
-0000ab30: 2020 5468 6973 206d 6574 686f 6420 6973    This method is
-0000ab40: 2064 6573 6967 6e65 6420 746f 2062 6520   designed to be 
-0000ab50: 6361 6c6c 6564 206f 6e20 7468 6520 636c  called on the cl
-0000ab60: 6173 7320 6974 7365 6c66 2072 6174 6865  ass itself rathe
-0000ab70: 7220 7468 616e 206f 6e20 616e 2069 6e73  r than on an ins
-0000ab80: 7461 6e63 6520 6f66 2074 6865 2063 6c61  tance of the cla
-0000ab90: 7373 2e20 4974 2063 616e 2062 650a 2020  ss. It can be.  
-0000aba0: 2020 2020 2020 7573 6564 2074 6f20 616e        used to an
-0000abb0: 616c 797a 6520 6120 636f 6c6c 6563 7469  alyze a collecti
-0000abc0: 6f6e 206f 6620 6e75 6d62 6572 7320 286e  on of numbers (n
-0000abd0: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
-0000abe0: 6e29 2061 6e64 2064 6574 6572 6d69 6e65  n) and determine
-0000abf0: 2074 6865 2063 6f75 6e74 206f 6620 6f64   the count of od
-0000ac00: 6420 616e 6420 6576 656e 206e 756d 6265  d and even numbe
-0000ac10: 7273 2e0a 0a20 2020 2020 2020 203a 7061  rs...        :pa
-0000ac20: 7261 6d20 6e75 6d62 6572 5f63 6f6d 6269  ram number_combi
-0000ac30: 6e61 7469 6f6e 3a20 4120 6c69 7374 2c20  nation: A list, 
-0000ac40: 7475 706c 652c 206f 7220 6f74 6865 7220  tuple, or other 
-0000ac50: 6974 6572 6162 6c65 206f 6620 696e 7465  iterable of inte
-0000ac60: 6765 7273 2e20 5468 6520 6d65 7468 6f64  gers. The method
-0000ac70: 2077 696c 6c20 6974 6572 6174 6520 7468   will iterate th
-0000ac80: 726f 7567 680a 2020 2020 2020 2020 2020  rough.          
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aca0: 2020 2020 2020 2020 2074 6869 7320 636f           this co
-0000acb0: 6c6c 6563 7469 6f6e 2074 6f20 6465 7465  llection to dete
-0000acc0: 726d 696e 6520 7468 6520 636f 756e 7420  rmine the count 
-0000acd0: 6f66 206f 6464 2061 6e64 2065 7665 6e20  of odd and even 
-0000ace0: 6e75 6d62 6572 732e 0a20 2020 2020 2020  numbers..       
-0000acf0: 203a 7061 7261 6d20 6b77 6172 6773 3a20   :param kwargs: 
-0000ad00: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
-0000ad10: 7264 2061 7267 756d 656e 7473 2074 6861  rd arguments tha
-0000ad20: 7420 6172 6520 6e6f 7420 7573 6564 2069  t are not used i
-0000ad30: 6e20 7468 6973 206d 6574 686f 6420 6275  n this method bu
-0000ad40: 7420 6172 6520 696e 636c 7564 6564 2066  t are included f
-0000ad50: 6f72 2070 6f74 656e 7469 616c 0a20 2020  or potential.   
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2020 2020 6675 7475 7265 2065 7874 656e      future exten
-0000ad80: 7369 6269 6c69 7479 206f 6620 7468 6520  sibility of the 
-0000ad90: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
-0000ada0: 3a72 6574 7572 6e3a 2041 2074 7570 6c65  :return: A tuple
-0000adb0: 2063 6f6e 7461 696e 696e 6720 7477 6f20   containing two 
-0000adc0: 656c 656d 656e 7473 3b20 7468 6520 6669  elements; the fi
-0000add0: 7273 7420 6973 2074 6865 2063 6f75 6e74  rst is the count
-0000ade0: 206f 6620 6f64 6420 6e75 6d62 6572 7320   of odd numbers 
-0000adf0: 616e 6420 7468 6520 7365 636f 6e64 2069  and the second i
-0000ae00: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
-0000ae10: 2020 2020 2020 2063 6f75 6e74 206f 6620         count of 
-0000ae20: 6576 656e 206e 756d 6265 7273 2069 6e20  even numbers in 
-0000ae30: 7468 6520 6e75 6d62 6572 5f63 6f6d 6269  the number_combi
-0000ae40: 6e61 7469 6f6e 2e0a 2020 2020 2020 2020  nation..        
-0000ae50: 2222 220a 0a20 2020 2020 2020 2023 2043  """..        # C
-0000ae60: 6f75 6e74 2074 6865 206e 756d 6265 7220  ount the number 
-0000ae70: 6f66 206f 6464 206e 756d 6265 7273 2069  of odd numbers i
-0000ae80: 6e20 7468 6520 6e75 6d62 6572 5f63 6f6d  n the number_com
-0000ae90: 6269 6e61 7469 6f6e 0a20 2020 2020 2020  bination.       
-0000aea0: 2023 2041 206e 756d 6265 7220 6973 2063   # A number is c
-0000aeb0: 6f6e 7369 6465 7265 6420 6f64 6420 6966  onsidered odd if
-0000aec0: 2074 6865 2072 656d 6169 6e64 6572 206f   the remainder o
-0000aed0: 6620 7468 6520 6469 7669 7369 6f6e 2062  f the division b
-0000aee0: 7920 3220 6973 2031 2028 6e75 6d20 2520  y 2 is 1 (num % 
-0000aef0: 3220 6576 616c 7561 7465 7320 746f 2054  2 evaluates to T
-0000af00: 7275 6529 0a20 2020 2020 2020 206f 6464  rue).        odd
-0000af10: 5f63 6f75 6e74 203d 2073 756d 2831 2066  _count = sum(1 f
-0000af20: 6f72 206e 756d 2069 6e20 6e75 6d62 6572  or num in number
-0000af30: 5f63 6f6d 6269 6e61 7469 6f6e 2069 6620  _combination if 
-0000af40: 6e75 6d20 2520 3229 0a0a 2020 2020 2020  num % 2)..      
-0000af50: 2020 2320 436f 756e 7420 7468 6520 6e75    # Count the nu
-0000af60: 6d62 6572 206f 6620 6576 656e 206e 756d  mber of even num
-0000af70: 6265 7273 2069 6e20 7468 6520 6e75 6d62  bers in the numb
-0000af80: 6572 5f63 6f6d 6269 6e61 7469 6f6e 0a20  er_combination. 
-0000af90: 2020 2020 2020 2023 2049 7427 7320 6361         # It's ca
-0000afa0: 6c63 756c 6174 6564 2062 7920 7375 6274  lculated by subt
-0000afb0: 7261 6374 696e 6720 7468 6520 6f64 6420  racting the odd 
-0000afc0: 636f 756e 7420 6672 6f6d 2074 6865 2074  count from the t
-0000afd0: 6f74 616c 206c 656e 6774 6820 6f66 2074  otal length of t
-0000afe0: 6865 206e 756d 6265 725f 636f 6d62 696e  he number_combin
-0000aff0: 6174 696f 6e0a 2020 2020 2020 2020 6576  ation.        ev
-0000b000: 656e 5f63 6f75 6e74 203d 206c 656e 286c  en_count = len(l
-0000b010: 6973 7428 6e75 6d62 6572 5f63 6f6d 6269  ist(number_combi
-0000b020: 6e61 7469 6f6e 2929 202d 206f 6464 5f63  nation)) - odd_c
-0000b030: 6f75 6e74 0a0a 2020 2020 2020 2020 2320  ount..        # 
-0000b040: 5265 7475 726e 2061 2074 7570 6c65 206f  Return a tuple o
-0000b050: 6620 6f64 6420 616e 6420 6576 656e 2063  f odd and even c
-0000b060: 6f75 6e74 730a 2020 2020 2020 2020 7265  ounts.        re
-0000b070: 7475 726e 206f 6464 5f63 6f75 6e74 2c20  turn odd_count, 
-0000b080: 6576 656e 5f63 6f75 6e74 0a0a 2020 2020  even_count..    
-0000b090: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-0000b0a0: 2064 6566 2063 616c 6375 6c61 7465 5f70   def calculate_p
-0000b0b0: 7269 6d65 5f63 6f6d 706f 7369 7465 5f72  rime_composite_r
-0000b0c0: 6174 696f 280a 2020 2020 2020 2020 2020  atio(.          
-0000b0d0: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
-0000b0e0: 2020 206e 756d 6265 725f 636f 6d62 696e     number_combin
-0000b0f0: 6174 696f 6e3a 2049 7465 7261 626c 655b  ation: Iterable[
-0000b100: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
-0000b110: 2020 2a2a 6b77 6172 6773 3a20 416e 790a    **kwargs: Any.
-0000b120: 2020 2020 2920 2d3e 2054 7570 6c65 5b69      ) -> Tuple[i
-0000b130: 6e74 2c20 696e 745d 3a0a 2020 2020 2020  nt, int]:.      
-0000b140: 2020 2222 220a 2020 2020 2020 2020 4361    """.        Ca
-0000b150: 6c63 756c 6174 6520 7468 6520 7261 7469  lculate the rati
-0000b160: 6f20 6f66 2070 7269 6d65 2074 6f20 636f  o of prime to co
-0000b170: 6d70 6f73 6974 6520 6e75 6d62 6572 7320  mposite numbers 
-0000b180: 696e 2061 2073 6571 7565 6e63 6520 6f66  in a sequence of
-0000b190: 206e 756d 6265 7273 2070 726f 7669 6465   numbers provide
-0000b1a0: 6420 696e 2074 6865 206e 756d 6265 725f  d in the number_
-0000b1b0: 636f 6d62 696e 6174 696f 6e2e 0a20 2020  combination..   
-0000b1c0: 2020 2020 2049 6e20 7468 6973 2063 6f6e       In this con
-0000b1d0: 7465 7874 2c20 7468 6520 6e75 6d62 6572  text, the number
-0000b1e0: 2031 2069 7320 636f 6e73 6964 6572 6564   1 is considered
-0000b1f0: 2061 2070 7269 6d65 206e 756d 6265 722e   a prime number.
-0000b200: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000b210: 206e 756d 6265 725f 636f 6d62 696e 6174   number_combinat
-0000b220: 696f 6e3a 2041 206c 6973 7420 6f72 2074  ion: A list or t
-0000b230: 7570 6c65 206f 6620 6e75 6d65 7269 6361  uple of numerica
-0000b240: 6c20 7661 6c75 6573 2e20 5468 6520 6d65  l values. The me
-0000b250: 7468 6f64 2077 696c 6c20 6465 7465 726d  thod will determ
-0000b260: 696e 6520 7768 6963 6820 6e75 6d62 6572  ine which number
-0000b270: 7320 6172 650a 2020 2020 2020 2020 2020  s are.          
-0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b290: 2020 2020 2020 2020 2070 7269 6d65 2028           prime (
-0000b2a0: 696e 636c 7564 696e 6720 3129 2061 6e64  including 1) and
-0000b2b0: 2077 6869 6368 2061 7265 2063 6f6d 706f   which are compo
-0000b2c0: 7369 7465 2c20 616e 6420 636f 6d70 7574  site, and comput
-0000b2d0: 6520 7468 6569 7220 636f 756e 7473 2e0a  e their counts..
-0000b2e0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-0000b2f0: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
-0000b300: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-0000b310: 6e74 732c 206e 6f74 2075 7365 6420 696e  nts, not used in
-0000b320: 2074 6869 7320 6675 6e63 7469 6f6e 2062   this function b
-0000b330: 7574 2069 6e63 6c75 6465 6420 666f 7220  ut included for 
-0000b340: 706f 7465 6e74 6961 6c20 6675 7475 7265  potential future
-0000b350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b360: 2020 2020 2020 2020 6578 7465 6e73 6962          extensib
-0000b370: 696c 6974 7920 6f66 2074 6865 206d 6574  ility of the met
-0000b380: 686f 642e 0a20 2020 2020 2020 203a 7265  hod..        :re
-0000b390: 7475 726e 3a20 4120 7475 706c 6520 636f  turn: A tuple co
-0000b3a0: 6e74 6169 6e69 6e67 2074 776f 2065 6c65  ntaining two ele
-0000b3b0: 6d65 6e74 733b 2074 6865 2066 6972 7374  ments; the first
-0000b3c0: 2069 7320 7468 6520 636f 756e 7420 6f66   is the count of
-0000b3d0: 2070 7269 6d65 206e 756d 6265 7273 2028   prime numbers (
-0000b3e0: 696e 636c 7564 696e 6720 3129 2061 6e64  including 1) and
-0000b3f0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0000b400: 2020 2020 2020 7365 636f 6e64 2069 7320        second is 
-0000b410: 7468 6520 636f 756e 7420 6f66 2063 6f6d  the count of com
-0000b420: 706f 7369 7465 206e 756d 6265 7273 2069  posite numbers i
-0000b430: 6e20 7468 6520 6e75 6d62 6572 5f63 6f6d  n the number_com
-0000b440: 6269 6e61 7469 6f6e 2e0a 2020 2020 2020  bination..      
-0000b450: 2020 2222 220a 0a20 2020 2020 2020 2064    """..        d
-0000b460: 6566 2069 735f 7072 696d 6528 6e75 6d3a  ef is_prime(num:
-0000b470: 2069 6e74 2920 2d3e 2062 6f6f 6c3a 0a20   int) -> bool:. 
-0000b480: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
-0000b490: 7369 6465 7220 3120 6173 2061 2070 7269  sider 1 as a pri
-0000b4a0: 6d65 206e 756d 6265 7220 666f 7220 7468  me number for th
-0000b4b0: 6520 7075 7270 6f73 6520 6f66 2074 6869  e purpose of thi
-0000b4c0: 7320 6361 6c63 756c 6174 696f 6e0a 2020  s calculation.  
-0000b4d0: 2020 2020 2020 2020 2020 6966 206e 756d            if num
-0000b4e0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-0000b4f0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000b500: 7565 0a20 2020 2020 2020 2020 2020 2023  ue.            #
-0000b510: 2045 7863 6c75 6465 206e 756d 6265 7273   Exclude numbers
-0000b520: 206c 6573 7320 7468 616e 2031 2061 6e64   less than 1 and
-0000b530: 2065 7665 6e20 6e75 6d62 6572 7320 6772   even numbers gr
-0000b540: 6561 7465 7220 7468 616e 2032 2061 7320  eater than 2 as 
-0000b550: 7468 6579 2061 7265 206e 6f74 2070 7269  they are not pri
-0000b560: 6d65 0a20 2020 2020 2020 2020 2020 2069  me.            i
-0000b570: 6620 6e75 6d20 3c20 3120 6f72 2028 6e75  f num < 1 or (nu
-0000b580: 6d20 2520 3220 3d3d 2030 2061 6e64 206e  m % 2 == 0 and n
-0000b590: 756d 203e 2032 293a 0a20 2020 2020 2020  um > 2):.       
-0000b5a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000b5b0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-0000b5c0: 2020 2320 4368 6563 6b20 666f 7220 6661    # Check for fa
-0000b5d0: 6374 6f72 7320 6672 6f6d 2033 2074 6f20  ctors from 3 to 
-0000b5e0: 7468 6520 7371 7561 7265 2072 6f6f 7420  the square root 
-0000b5f0: 6f66 206e 756d 0a20 2020 2020 2020 2020  of num.         
-0000b600: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000b610: 6528 332c 2069 6e74 286e 756d 202a 2a20  e(3, int(num ** 
-0000b620: 302e 3529 202b 2031 2c20 3229 3a0a 2020  0.5) + 1, 2):.  
-0000b630: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000b640: 206e 756d 2025 2069 203d 3d20 303a 0a20   num % i == 0:. 
-0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b660: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0000b670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000b680: 726e 2054 7275 650a 0a20 2020 2020 2020  rn True..       
-0000b690: 2023 2043 6f75 6e74 2070 7269 6d65 206e   # Count prime n
-0000b6a0: 756d 6265 7273 2069 6e20 7468 6520 6e75  umbers in the nu
-0000b6b0: 6d62 6572 5f63 6f6d 6269 6e61 7469 6f6e  mber_combination
-0000b6c0: 0a20 2020 2020 2020 2070 7269 6d65 5f63  .        prime_c
-0000b6d0: 6f75 6e74 203d 2073 756d 2831 2066 6f72  ount = sum(1 for
-0000b6e0: 206e 756d 2069 6e20 6e75 6d62 6572 5f63   num in number_c
-0000b6f0: 6f6d 6269 6e61 7469 6f6e 2069 6620 6973  ombination if is
-0000b700: 5f70 7269 6d65 286e 756d 2929 0a20 2020  _prime(num)).   
-0000b710: 2020 2020 2023 2043 6f75 6e74 2063 6f6d       # Count com
-0000b720: 706f 7369 7465 206e 756d 6265 7273 2061  posite numbers a
-0000b730: 7320 7468 6520 7265 6d61 696e 696e 6720  s the remaining 
-0000b740: 6e75 6d62 6572 7320 696e 2074 6865 206e  numbers in the n
-0000b750: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
-0000b760: 6e0a 2020 2020 2020 2020 636f 6d70 6f73  n.        compos
-0000b770: 6974 655f 636f 756e 7420 3d20 6c65 6e28  ite_count = len(
-0000b780: 6c69 7374 286e 756d 6265 725f 636f 6d62  list(number_comb
-0000b790: 696e 6174 696f 6e29 2920 2d20 7072 696d  ination)) - prim
-0000b7a0: 655f 636f 756e 740a 0a20 2020 2020 2020  e_count..       
-0000b7b0: 2023 2052 6574 7572 6e20 6120 7475 706c   # Return a tupl
-0000b7c0: 6520 6f66 2070 7269 6d65 2061 6e64 2063  e of prime and c
-0000b7d0: 6f6d 706f 7369 7465 2063 6f75 6e74 730a  omposite counts.
-0000b7e0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-0000b7f0: 7269 6d65 5f63 6f75 6e74 2c20 636f 6d70  rime_count, comp
-0000b800: 6f73 6974 655f 636f 756e 740a 0a20 2020  osite_count..   
-0000b810: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-0000b820: 2020 6465 6620 6361 6c63 756c 6174 655f    def calculate_
-0000b830: 7370 616e 280a 2020 2020 2020 2020 2020  span(.          
-0000b840: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
-0000b850: 2020 206e 756d 6265 725f 636f 6d62 696e     number_combin
-0000b860: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
-0000b870: 2020 2049 7465 7261 626c 655b 696e 745d     Iterable[int]
-0000b880: 2c0a 2020 2020 2020 2020 2020 2020 2a2a  ,.            **
-0000b890: 6b77 6172 6773 3a20 416e 790a 2020 2020  kwargs: Any.    
-0000b8a0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-0000b8b0: 2020 2222 220a 2020 2020 2020 2020 4361    """.        Ca
-0000b8c0: 6c63 756c 6174 6520 7468 6520 7370 616e  lculate the span
-0000b8d0: 206f 6620 6120 7365 7175 656e 6365 206f   of a sequence o
-0000b8e0: 6620 6e75 6d62 6572 7320 7072 6f76 6964  f numbers provid
-0000b8f0: 6564 2069 6e20 7468 6520 6e75 6d62 6572  ed in the number
-0000b900: 5f63 6f6d 6269 6e61 7469 6f6e 2e20 5468  _combination. Th
-0000b910: 6520 7370 616e 2069 7320 6465 6669 6e65  e span is define
-0000b920: 6420 6173 2074 6865 0a20 2020 2020 2020  d as the.       
-0000b930: 2064 6966 6665 7265 6e63 6520 6265 7477   difference betw
-0000b940: 6565 6e20 7468 6520 6d61 7869 6d75 6d20  een the maximum 
-0000b950: 616e 6420 6d69 6e69 6d75 6d20 7661 6c75  and minimum valu
-0000b960: 6573 2069 6e20 7468 6520 7365 7420 6f66  es in the set of
-0000b970: 206e 756d 6265 7273 2e0a 0a20 2020 2020   numbers...     
-0000b980: 2020 203a 7061 7261 6d20 6e75 6d62 6572     :param number
-0000b990: 5f63 6f6d 6269 6e61 7469 6f6e 3a20 4120  _combination: A 
-0000b9a0: 6c69 7374 206f 7220 7475 706c 6520 6f66  list or tuple of
-0000b9b0: 206e 756d 6572 6963 616c 2076 616c 7565   numerical value
-0000b9c0: 732e 2054 6865 206d 6574 686f 6420 7769  s. The method wi
-0000b9d0: 6c6c 2066 696e 6420 7468 6520 6d61 7869  ll find the maxi
-0000b9e0: 6d75 6d20 616e 6420 6d69 6e69 6d75 6d0a  mum and minimum.
-0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba10: 2020 2076 616c 7565 7320 696e 2074 6869     values in thi
-0000ba20: 7320 636f 6c6c 6563 7469 6f6e 2061 6e64  s collection and
-0000ba30: 2063 616c 6375 6c61 7465 2074 6865 2064   calculate the d
-0000ba40: 6966 6665 7265 6e63 6520 2873 7061 6e29  ifference (span)
-0000ba50: 2062 6574 7765 656e 2074 6865 6d2e 0a20   between them.. 
-0000ba60: 2020 2020 2020 203a 7061 7261 6d20 6b77         :param kw
-0000ba70: 6172 6773 3a20 4164 6469 7469 6f6e 616c  args: Additional
-0000ba80: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-0000ba90: 7473 2c20 6e6f 7420 7573 6564 2069 6e20  ts, not used in 
-0000baa0: 7468 6973 2066 756e 6374 696f 6e20 6275  this function bu
-0000bab0: 7420 696e 636c 7564 6564 2066 6f72 2070  t included for p
-0000bac0: 6f74 656e 7469 616c 2066 7574 7572 650a  otential future.
-0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bae0: 2020 2020 2020 2065 7874 656e 7369 6269         extensibi
-0000baf0: 6c69 7479 206f 6620 7468 6520 6d65 7468  lity of the meth
-0000bb00: 6f64 2e0a 2020 2020 2020 2020 3a72 6574  od..        :ret
-0000bb10: 7572 6e3a 2054 6865 2073 7061 6e20 6f66  urn: The span of
-0000bb20: 2074 6865 206e 756d 6265 7273 2069 6e20   the numbers in 
-0000bb30: 7468 6520 6e75 6d62 6572 5f63 6f6d 6269  the number_combi
-0000bb40: 6e61 7469 6f6e 2061 7320 616e 2069 6e74  nation as an int
-0000bb50: 6567 6572 2e20 4966 2074 6865 2069 6e70  eger. If the inp
-0000bb60: 7574 2063 6f6e 7461 696e 7320 666c 6f61  ut contains floa
-0000bb70: 7469 6e67 0a20 2020 2020 2020 2020 2020  ting.           
-0000bb80: 2020 2020 2020 706f 696e 7420 6e75 6d62        point numb
-0000bb90: 6572 732c 2074 6865 2073 7061 6e20 6973  ers, the span is
-0000bba0: 2063 6173 7420 746f 2061 6e20 696e 7465   cast to an inte
-0000bbb0: 6765 7220 6265 666f 7265 2062 6569 6e67  ger before being
-0000bbc0: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
-0000bbd0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-0000bbe0: 2320 4669 6e64 2074 6865 206d 6178 696d  # Find the maxim
-0000bbf0: 756d 2061 6e64 206d 696e 696d 756d 2076  um and minimum v
-0000bc00: 616c 7565 7320 696e 2074 6865 206e 756d  alues in the num
-0000bc10: 6265 7220 636f 6d62 696e 6174 696f 6e0a  ber combination.
-0000bc20: 2020 2020 2020 2020 6d61 785f 7661 6c75          max_valu
-0000bc30: 6520 3d20 6d61 7828 6e75 6d62 6572 5f63  e = max(number_c
-0000bc40: 6f6d 6269 6e61 7469 6f6e 290a 2020 2020  ombination).    
-0000bc50: 2020 2020 6d69 6e5f 7661 6c75 6520 3d20      min_value = 
-0000bc60: 6d69 6e28 6e75 6d62 6572 5f63 6f6d 6269  min(number_combi
-0000bc70: 6e61 7469 6f6e 290a 0a20 2020 2020 2020  nation)..       
-0000bc80: 2023 2043 616c 6375 6c61 7465 2074 6865   # Calculate the
-0000bc90: 2073 7061 6e20 6279 2073 7562 7472 6163   span by subtrac
-0000bca0: 7469 6e67 2074 6865 206d 696e 696d 756d  ting the minimum
-0000bcb0: 2076 616c 7565 2066 726f 6d20 7468 6520   value from the 
-0000bcc0: 6d61 7869 6d75 6d20 7661 6c75 650a 2020  maximum value.  
-0000bcd0: 2020 2020 2020 7370 616e 203d 206d 6178        span = max
-0000bce0: 5f76 616c 7565 202d 206d 696e 5f76 616c  _value - min_val
-0000bcf0: 7565 0a0a 2020 2020 2020 2020 2320 4361  ue..        # Ca
-0000bd00: 7374 2074 6865 2073 7061 6e20 746f 2061  st the span to a
-0000bd10: 6e20 696e 7465 6765 7220 616e 6420 7265  n integer and re
-0000bd20: 7475 726e 2069 740a 2020 2020 2020 2020  turn it.        
-0000bd30: 7265 7475 726e 2069 6e74 2873 7061 6e29  return int(span)
-0000bd40: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-0000bd50: 6f64 0a20 2020 2064 6566 2063 616c 6375  od.    def calcu
-0000bd60: 6c61 7465 5f73 756d 5f74 6f74 616c 280a  late_sum_total(.
-0000bd70: 2020 2020 2020 2020 2020 2020 636c 732c              cls,
-0000bd80: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-0000bd90: 6265 725f 636f 6d62 696e 6174 696f 6e3a  ber_combination:
-0000bda0: 2049 7465 7261 626c 655b 556e 696f 6e5b   Iterable[Union[
-0000bdb0: 696e 742c 2066 6c6f 6174 5d5d 2c0a 2020  int, float]],.  
-0000bdc0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000bdd0: 6773 3a20 416e 790a 2020 2020 2920 2d3e  gs: Any.    ) ->
-0000bde0: 2055 6e69 6f6e 5b69 6e74 2c20 666c 6f61   Union[int, floa
-0000bdf0: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
-0000be00: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
-0000be10: 6520 7468 6520 746f 7461 6c20 7375 6d20  e the total sum 
-0000be20: 6f66 2061 2073 6571 7565 6e63 6520 6f66  of a sequence of
-0000be30: 206e 756d 6265 7273 2070 726f 7669 6465   numbers provide
-0000be40: 6420 696e 2074 6865 206e 756d 6265 725f  d in the number_
-0000be50: 636f 6d62 696e 6174 696f 6e2e 2054 6869  combination. Thi
-0000be60: 7320 6d65 7468 6f64 0a20 2020 2020 2020  s method.       
-0000be70: 2061 6767 7265 6761 7465 7320 616c 6c20   aggregates all 
-0000be80: 7468 6520 6e75 6d65 7269 6361 6c20 7661  the numerical va
-0000be90: 6c75 6573 2069 6e20 7468 6520 6c69 7374  lues in the list
-0000bea0: 206f 7220 7475 706c 6520 7061 7373 6564   or tuple passed
-0000beb0: 2061 7320 616e 2061 7267 756d 656e 7420   as an argument 
-0000bec0: 616e 6420 7265 7475 726e 7320 7468 6569  and returns thei
-0000bed0: 7220 7375 6d2e 0a0a 2020 2020 2020 2020  r sum...        
-0000bee0: 3a70 6172 616d 206e 756d 6265 725f 636f  :param number_co
-0000bef0: 6d62 696e 6174 696f 6e3a 2041 206c 6973  mbination: A lis
-0000bf00: 7420 6f72 2074 7570 6c65 206f 6620 6e75  t or tuple of nu
-0000bf10: 6d65 7269 6361 6c20 7661 6c75 6573 2e20  merical values. 
-0000bf20: 5468 6520 6d65 7468 6f64 2077 696c 6c20  The method will 
-0000bf30: 7375 6d20 7468 6573 6520 7661 6c75 6573  sum these values
-0000bf40: 2061 6e64 2072 6574 7572 6e0a 2020 2020   and return.    
-0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf60: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000bf70: 6865 2072 6573 756c 742e 0a20 2020 2020  he result..     
-0000bf80: 2020 203a 7061 7261 6d20 6b77 6172 6773     :param kwargs
-0000bf90: 3a20 4164 6469 7469 6f6e 616c 206b 6579  : Additional key
-0000bfa0: 776f 7264 2061 7267 756d 656e 7473 2c20  word arguments, 
-0000bfb0: 6e6f 7420 7573 6564 2069 6e20 7468 6973  not used in this
-0000bfc0: 2066 756e 6374 696f 6e20 6275 7420 696e   function but in
-0000bfd0: 636c 7564 6564 2066 6f72 2070 6f74 656e  cluded for poten
-0000bfe0: 7469 616c 2066 7574 7572 650a 2020 2020  tial future.    
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c000: 2020 2065 7874 656e 7369 6269 6c69 7479     extensibility
-0000c010: 206f 6620 7468 6520 6d65 7468 6f64 2e0a   of the method..
-0000c020: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-0000c030: 2054 6865 2073 756d 2074 6f74 616c 206f   The sum total o
-0000c040: 6620 7468 6520 6e75 6d62 6572 7320 696e  f the numbers in
-0000c050: 2074 6865 206e 756d 6265 725f 636f 6d62   the number_comb
-0000c060: 696e 6174 696f 6e20 6173 2061 6e20 696e  ination as an in
-0000c070: 7465 6765 7220 6f72 2066 6c6f 6174 2c20  teger or float, 
-0000c080: 6465 7065 6e64 696e 6720 6f6e 2074 6865  depending on the
-0000c090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c0a0: 2020 696e 7075 7420 7661 6c75 6573 2e0a    input values..
-0000c0b0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000c0c0: 2020 2020 2023 2043 616c 6375 6c61 7465       # Calculate
-0000c0d0: 2074 6865 2073 756d 206f 6620 7468 6520   the sum of the 
-0000c0e0: 6e75 6d62 6572 7320 696e 2074 6865 2063  numbers in the c
-0000c0f0: 6f6d 6269 6e61 7469 6f6e 2075 7369 6e67  ombination using
-0000c100: 2074 6865 2062 7569 6c74 2d69 6e20 7375   the built-in su
-0000c110: 6d20 6675 6e63 7469 6f6e 0a20 2020 2020  m function.     
-0000c120: 2020 2074 6f74 616c 5f73 756d 203d 2073     total_sum = s
-0000c130: 756d 286e 756d 6265 725f 636f 6d62 696e  um(number_combin
-0000c140: 6174 696f 6e29 0a0a 2020 2020 2020 2020  ation)..        
-0000c150: 2320 5265 7475 726e 2074 6865 2073 756d  # Return the sum
-0000c160: 2074 6f74 616c 0a20 2020 2020 2020 2072   total.        r
-0000c170: 6574 7572 6e20 746f 7461 6c5f 7375 6d0a  eturn total_sum.
-0000c180: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-0000c190: 640a 2020 2020 6465 6620 6361 6c63 756c  d.    def calcul
-0000c1a0: 6174 655f 7375 6d5f 7461 696c 280a 2020  ate_sum_tail(.  
-0000c1b0: 2020 2020 2020 2020 2020 636c 732c 0a20            cls,. 
-0000c1c0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
-0000c1d0: 725f 636f 6d62 696e 6174 696f 6e3a 2049  r_combination: I
-0000c1e0: 7465 7261 626c 655b 696e 745d 2c0a 2020  terable[int],.  
-0000c1f0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000c200: 6773 3a20 416e 790a 2020 2020 2920 2d3e  gs: Any.    ) ->
-0000c210: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-0000c220: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
-0000c230: 6174 6520 7468 6520 6c61 7374 2064 6967  ate the last dig
-0000c240: 6974 2028 7461 696c 2920 6f66 2074 6865  it (tail) of the
-0000c250: 2073 756d 206f 6620 6120 6769 7665 6e20   sum of a given 
-0000c260: 6e75 6d62 6572 2063 6f6d 6269 6e61 7469  number combinati
-0000c270: 6f6e 2e20 5468 6520 7461 696c 2069 7320  on. The tail is 
-0000c280: 7468 6520 756e 6974 2773 2070 6c61 6365  the unit's place
-0000c290: 0a20 2020 2020 2020 206f 6620 7468 6520  .        of the 
-0000c2a0: 7375 6d2c 2077 6869 6368 2063 616e 2062  sum, which can b
-0000c2b0: 6520 7573 6566 756c 2066 6f72 2063 6572  e useful for cer
-0000c2c0: 7461 696e 2074 7970 6573 206f 6620 6e75  tain types of nu
-0000c2d0: 6d65 7269 6361 6c20 616e 616c 7973 6973  merical analysis
-0000c2e0: 206f 7220 7061 7474 6572 6e20 7265 636f   or pattern reco
-0000c2f0: 676e 6974 696f 6e2e 0a0a 2020 2020 2020  gnition...      
-0000c300: 2020 3a70 6172 616d 206e 756d 6265 725f    :param number_
-0000c310: 636f 6d62 696e 6174 696f 6e3a 2041 206c  combination: A l
-0000c320: 6973 7420 6f72 2074 7570 6c65 206f 6620  ist or tuple of 
-0000c330: 6e75 6d65 7269 6361 6c20 7661 6c75 6573  numerical values
-0000c340: 2e20 5468 6520 7375 6d20 6f66 2074 6865  . The sum of the
-0000c350: 7365 206e 756d 6265 7273 2077 696c 6c20  se numbers will 
-0000c360: 6265 2063 616c 6375 6c61 7465 642c 0a20  be calculated,. 
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c390: 2020 616e 6420 7468 6520 7461 696c 206f    and the tail o
-0000c3a0: 6620 7468 6973 2073 756d 2028 6c61 7374  f this sum (last
-0000c3b0: 2064 6967 6974 2920 7769 6c6c 2062 6520   digit) will be 
-0000c3c0: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
-0000c3d0: 2020 3a70 6172 616d 206b 7761 7267 733a    :param kwargs:
-0000c3e0: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
-0000c3f0: 6f72 6420 6172 6775 6d65 6e74 732c 206e  ord arguments, n
-0000c400: 6f74 2075 7365 6420 696e 2074 6869 7320  ot used in this 
-0000c410: 6675 6e63 7469 6f6e 2062 7574 2069 6e63  function but inc
-0000c420: 6c75 6465 6420 666f 7220 706f 7465 6e74  luded for potent
-0000c430: 6961 6c20 6675 7475 7265 0a20 2020 2020  ial future.     
-0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c450: 2020 6578 7465 6e73 6962 696c 6974 7920    extensibility 
-0000c460: 6f66 2074 6865 206d 6574 686f 642e 0a20  of the method.. 
-0000c470: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-0000c480: 5468 6520 6c61 7374 2064 6967 6974 206f  The last digit o
-0000c490: 6620 7468 6520 7375 6d20 6f66 2074 6865  f the sum of the
-0000c4a0: 206e 756d 6265 7220 636f 6d62 696e 6174   number combinat
-0000c4b0: 696f 6e20 6173 2061 6e20 696e 7465 6765  ion as an intege
-0000c4c0: 722e 0a20 2020 2020 2020 2022 2222 0a0a  r..        """..
-0000c4d0: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
-0000c4e0: 6174 6520 7468 6520 7375 6d20 6f66 2074  ate the sum of t
-0000c4f0: 6865 206e 756d 6265 7273 2069 6e20 7468  he numbers in th
-0000c500: 6520 636f 6d62 696e 6174 696f 6e0a 2020  e combination.  
-0000c510: 2020 2020 2020 746f 7461 6c5f 7375 6d20        total_sum 
-0000c520: 3d20 636c 732e 6361 6c63 756c 6174 655f  = cls.calculate_
-0000c530: 7375 6d5f 746f 7461 6c28 6e75 6d62 6572  sum_total(number
-0000c540: 5f63 6f6d 6269 6e61 7469 6f6e 290a 0a20  _combination).. 
-0000c550: 2020 2020 2020 2023 2052 6574 7572 6e20         # Return 
-0000c560: 7468 6520 6c61 7374 2064 6967 6974 206f  the last digit o
-0000c570: 6620 7468 6973 2073 756d 0a20 2020 2020  f this sum.     
-0000c580: 2020 2072 6574 7572 6e20 746f 7461 6c5f     return total_
-0000c590: 7375 6d20 2520 3130 0a0a 2020 2020 4063  sum % 10..    @c
-0000c5a0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-0000c5b0: 6566 2063 616c 6375 6c61 7465 5f77 6565  ef calculate_wee
-0000c5c0: 6b64 6179 280a 2020 2020 2020 2020 2020  kday(.          
-0000c5d0: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
-0000c5e0: 2020 2064 6174 653a 2073 7472 2c0a 2020     date: str,.  
-0000c5f0: 2020 2020 2020 2020 2020 6461 7465 5f66            date_f
-0000c600: 6f72 6d61 743a 2073 7472 203d 2027 2559  ormat: str = '%Y
-0000c610: 2d25 6d2d 2564 272c 0a20 2020 2020 2020  -%m-%d',.       
-0000c620: 2020 2020 202a 2a6b 7761 7267 733a 2041       **kwargs: A
-0000c630: 6e79 0a20 2020 2029 202d 3e20 696e 743a  ny.    ) -> int:
-0000c640: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c650: 2020 2020 2043 616c 6375 6c61 7465 2074       Calculate t
-0000c660: 6865 2077 6565 6b64 6179 206e 756d 6265  he weekday numbe
-0000c670: 7220 6672 6f6d 2061 2064 6174 6520 7374  r from a date st
-0000c680: 7269 6e67 2e0a 0a20 2020 2020 2020 203a  ring...        :
-0000c690: 7061 7261 6d20 6461 7465 3a20 4461 7465  param date: Date
-0000c6a0: 2073 7472 696e 672e 0a20 2020 2020 2020   string..       
-0000c6b0: 203a 7061 7261 6d20 6461 7465 5f66 6f72   :param date_for
-0000c6c0: 6d61 743a 2064 6566 6175 6c74 2027 5959  mat: default 'YY
-0000c6d0: 5959 2d4d 4d2d 4444 2720 666f 726d 6174  YY-MM-DD' format
-0000c6e0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0000c6f0: 3a20 5765 656b 6461 7920 6e75 6d62 6572  : Weekday number
-0000c700: 2077 6865 7265 2031 2072 6570 7265 7365   where 1 represe
-0000c710: 6e74 7320 4d6f 6e64 6179 2061 6e64 2037  nts Monday and 7
-0000c720: 2072 6570 7265 7365 6e74 7320 5375 6e64   represents Sund
-0000c730: 6179 2e0a 2020 2020 2020 2020 2222 220a  ay..        """.
-0000c740: 2020 2020 2020 2020 6461 7465 203d 2064          date = d
-0000c750: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
-0000c760: 2e73 7472 7074 696d 6528 6461 7465 2c20  .strptime(date, 
-0000c770: 6461 7465 5f66 6f72 6d61 7429 2e64 6174  date_format).dat
-0000c780: 6528 290a 2020 2020 2020 2020 7265 7475  e().        retu
-0000c790: 726e 2064 6174 652e 7765 656b 6461 7928  rn date.weekday(
-0000c7a0: 2920 2b20 310a 0a20 2020 2040 636c 6173  ) + 1..    @clas
-0000c7b0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-0000c7c0: 6361 6c63 756c 6174 655f 6163 280a 2020  calculate_ac(.  
-0000c7d0: 2020 2020 2020 2020 2020 636c 732c 0a20            cls,. 
-0000c7e0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
-0000c7f0: 725f 636f 6d62 696e 6174 696f 6e3a 2049  r_combination: I
-0000c800: 7465 7261 626c 655b 696e 745d 2c0a 2020  terable[int],.  
-0000c810: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000c820: 6773 3a20 416e 790a 2020 2020 2920 2d3e  gs: Any.    ) ->
-0000c830: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-0000c840: 220a 2020 2020 2020 2020 436f 6d70 7574  ".        Comput
-0000c850: 6520 7468 6520 636f 6d70 6c65 7869 7479  e the complexity
-0000c860: 206f 6620 6120 6769 7665 6e20 6e75 6d62   of a given numb
-0000c870: 6572 2063 6f6d 6269 6e61 7469 6f6e 2e20  er combination. 
-0000c880: 436f 6d70 6c65 7869 7479 2069 7320 6465  Complexity is de
-0000c890: 6669 6e65 6420 6173 2074 6865 206e 756d  fined as the num
-0000c8a0: 6265 7220 6f66 2064 6973 7469 6e63 740a  ber of distinct.
-0000c8b0: 2020 2020 2020 2020 6162 736f 6c75 7465          absolute
-0000c8c0: 2064 6966 6665 7265 6e63 6573 2062 6574   differences bet
-0000c8d0: 7765 656e 2065 6163 6820 7061 6972 206f  ween each pair o
-0000c8e0: 6620 6e75 6d62 6572 7320 696e 2074 6865  f numbers in the
-0000c8f0: 2063 6f6d 6269 6e61 7469 6f6e 2c20 6578   combination, ex
-0000c900: 636c 7564 696e 6720 7468 6520 6e75 6d62  cluding the numb
-0000c910: 6572 206f 6620 656c 656d 656e 7473 206d  er of elements m
-0000c920: 696e 7573 206f 6e65 2e0a 0a20 2020 2020  inus one...     
-0000c930: 2020 203a 7061 7261 6d20 6e75 6d62 6572     :param number
-0000c940: 5f63 6f6d 6269 6e61 7469 6f6e 3a20 4120  _combination: A 
-0000c950: 6c69 7374 206f 7220 7475 706c 6520 6f66  list or tuple of
-0000c960: 206e 756d 6572 6963 616c 2076 616c 7565   numerical value
-0000c970: 7320 666f 7220 7768 6963 6820 7468 6520  s for which the 
-0000c980: 636f 6d70 6c65 7869 7479 2077 696c 6c20  complexity will 
-0000c990: 6265 2063 616c 6375 6c61 7465 642e 0a20  be calculated.. 
-0000c9a0: 2020 2020 2020 203a 7061 7261 6d20 6b77         :param kw
-0000c9b0: 6172 6773 3a20 4164 6469 7469 6f6e 616c  args: Additional
-0000c9c0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-0000c9d0: 7473 2c20 6e6f 7420 7573 6564 2069 6e20  ts, not used in 
-0000c9e0: 7468 6973 2066 756e 6374 696f 6e20 6275  this function bu
-0000c9f0: 7420 616c 6c6f 7773 2066 6f72 2065 7874  t allows for ext
-0000ca00: 656e 7369 6269 6c69 7479 2e0a 2020 2020  ensibility..    
-0000ca10: 2020 2020 3a72 6574 7572 6e3a 2041 6e20      :return: An 
-0000ca20: 696e 7465 6765 7220 7265 7072 6573 656e  integer represen
-0000ca30: 7469 6e67 2074 6865 2063 6f6d 706c 6578  ting the complex
-0000ca40: 6974 7920 6f66 2074 6865 206e 756d 6265  ity of the numbe
-0000ca50: 7220 636f 6d62 696e 6174 696f 6e2e 0a20  r combination.. 
-0000ca60: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-0000ca70: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
-0000ca80: 2061 2073 6574 2074 6f20 7374 6f72 6520   a set to store 
-0000ca90: 6469 7374 696e 6374 2061 6273 6f6c 7574  distinct absolut
-0000caa0: 6520 6469 6666 6572 656e 6365 730a 2020  e differences.  
-0000cab0: 2020 2020 2020 6469 7374 696e 6374 5f64        distinct_d
-0000cac0: 6966 6673 203d 2073 6574 2829 0a0a 2020  iffs = set()..  
-0000cad0: 2020 2020 2020 2320 436f 756e 7420 7468        # Count th
-0000cae0: 6520 6e75 6d62 6572 206f 6620 656c 656d  e number of elem
-0000caf0: 656e 7473 2069 6e20 7468 6520 6e75 6d62  ents in the numb
-0000cb00: 6572 2063 6f6d 6269 6e61 7469 6f6e 0a20  er combination. 
-0000cb10: 2020 2020 2020 206e 756d 6265 725f 636f         number_co
-0000cb20: 6d62 696e 6174 696f 6e5f 6c69 7374 203d  mbination_list =
-0000cb30: 206c 6973 7428 6e75 6d62 6572 5f63 6f6d   list(number_com
-0000cb40: 6269 6e61 7469 6f6e 290a 2020 2020 2020  bination).      
-0000cb50: 2020 6e75 6d5f 636f 756e 7420 3d20 6c65    num_count = le
-0000cb60: 6e28 6e75 6d62 6572 5f63 6f6d 6269 6e61  n(number_combina
-0000cb70: 7469 6f6e 5f6c 6973 7429 0a0a 2020 2020  tion_list)..    
-0000cb80: 2020 2020 2320 4974 6572 6174 6520 6f76      # Iterate ov
-0000cb90: 6572 2065 6163 6820 756e 6971 7565 2070  er each unique p
-0000cba0: 6169 7220 6f66 206e 756d 6265 7273 2074  air of numbers t
-0000cbb0: 6f20 6361 6c63 756c 6174 6520 6162 736f  o calculate abso
-0000cbc0: 6c75 7465 2064 6966 6665 7265 6e63 6573  lute differences
-0000cbd0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-0000cbe0: 6e20 7261 6e67 6528 6e75 6d5f 636f 756e  n range(num_coun
-0000cbf0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000cc00: 666f 7220 6a20 696e 2072 616e 6765 2869  for j in range(i
-0000cc10: 202b 2031 2c20 6e75 6d5f 636f 756e 7429   + 1, num_count)
-0000cc20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cc30: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
-0000cc40: 6520 6162 736f 6c75 7465 2064 6966 6665  e absolute diffe
-0000cc50: 7265 6e63 6520 6265 7477 6565 6e20 7468  rence between th
-0000cc60: 6520 7477 6f20 6e75 6d62 6572 730a 2020  e two numbers.  
-0000cc70: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0000cc80: 6666 203d 2061 6273 286e 756d 6265 725f  ff = abs(number_
-0000cc90: 636f 6d62 696e 6174 696f 6e5f 6c69 7374  combination_list
-0000cca0: 5b6a 5d20 2d20 6e75 6d62 6572 5f63 6f6d  [j] - number_com
-0000ccb0: 6269 6e61 7469 6f6e 5f6c 6973 745b 695d  bination_list[i]
-0000ccc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ccd0: 2020 2320 4164 6420 7468 6520 6162 736f    # Add the abso
-0000cce0: 6c75 7465 2064 6966 6665 7265 6e63 6520  lute difference 
-0000ccf0: 746f 2074 6865 2073 6574 206f 6620 6469  to the set of di
-0000cd00: 7374 696e 6374 2064 6966 6665 7265 6e63  stinct differenc
-0000cd10: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-0000cd20: 2020 2064 6973 7469 6e63 745f 6469 6666     distinct_diff
-0000cd30: 732e 6164 6428 6469 6666 290a 0a20 2020  s.add(diff)..   
-0000cd40: 2020 2020 2023 2052 6574 7572 6e20 7468       # Return th
-0000cd50: 6520 6e75 6d62 6572 206f 6620 6469 7374  e number of dist
-0000cd60: 696e 6374 2064 6966 6665 7265 6e63 6573  inct differences
-0000cd70: 206d 696e 7573 2074 6865 206e 756d 6265   minus the numbe
-0000cd80: 7220 6f66 2065 6c65 6d65 6e74 7320 6d69  r of elements mi
-0000cd90: 6e75 7320 6f6e 650a 2020 2020 2020 2020  nus one.        
-0000cda0: 7265 7475 726e 206c 656e 2864 6973 7469  return len(disti
-0000cdb0: 6e63 745f 6469 6666 7329 202d 2028 6e75  nct_diffs) - (nu
-0000cdc0: 6d5f 636f 756e 7420 2d20 3129 0a0a 2020  m_count - 1)..  
-0000cdd0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-0000cde0: 2020 2064 6566 2063 616c 6375 6c61 7465     def calculate
-0000cdf0: 5f61 7667 2863 6c73 2c20 6e75 6d62 6572  _avg(cls, number
-0000ce00: 5f63 6f6d 6269 6e61 7469 6f6e 3a20 4974  _combination: It
-0000ce10: 6572 6162 6c65 5b69 6e74 5d2c 202a 2a6b  erable[int], **k
-0000ce20: 7761 7267 733a 2041 6e79 2920 2d3e 2069  wargs: Any) -> i
-0000ce30: 6e74 3a0a 2020 2020 2020 2020 7265 7475  nt:.        retu
-0000ce40: 726e 206d 6174 682e 666c 6f6f 7228 7375  rn math.floor(su
-0000ce50: 6d28 6e75 6d62 6572 5f63 6f6d 6269 6e61  m(number_combina
-0000ce60: 7469 6f6e 2920 2f20 6c65 6e28 6c69 7374  tion) / len(list
-0000ce70: 286e 756d 6265 725f 636f 6d62 696e 6174  (number_combinat
-0000ce80: 696f 6e29 2929 0a0a 2020 2020 4063 6c61  ion)))..    @cla
-0000ce90: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-0000cea0: 2063 616c 6375 6c61 7465 5f63 6f6e 7365   calculate_conse
-0000ceb0: 6375 7469 7665 5f6e 756d 6265 7273 280a  cutive_numbers(.
-0000cec0: 2020 2020 2020 2020 2020 2020 636c 732c              cls,
-0000ced0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-0000cee0: 6265 725f 636f 6d62 696e 6174 696f 6e3a  ber_combination:
-0000cef0: 2049 7465 7261 626c 655b 696e 745d 2c0a   Iterable[int],.
-0000cf00: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
-0000cf10: 6172 6773 3a20 416e 790a 2020 2020 2920  args: Any.    ) 
-0000cf20: 2d3e 204c 6973 745b 4c69 7374 5b69 6e74  -> List[List[int
-0000cf30: 5d5d 3a0a 2020 2020 2020 2020 2222 220a  ]]:.        """.
-0000cf40: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
-0000cf50: 6520 7468 6520 7365 7175 656e 6365 7320  e the sequences 
-0000cf60: 6f66 2063 6f6e 7365 6375 7469 7665 206e  of consecutive n
-0000cf70: 756d 6265 7273 2069 6e20 6120 6769 7665  umbers in a give
-0000cf80: 6e20 6974 6572 6162 6c65 206f 6620 696e  n iterable of in
-0000cf90: 7465 6765 7273 2e0a 0a20 2020 2020 2020  tegers...       
-0000cfa0: 203a 7061 7261 6d20 6e75 6d62 6572 5f63   :param number_c
-0000cfb0: 6f6d 6269 6e61 7469 6f6e 3a20 416e 2069  ombination: An i
-0000cfc0: 7465 7261 626c 6520 6f66 2069 6e74 6567  terable of integ
-0000cfd0: 6572 7320 746f 2063 6f6d 7075 7465 2063  ers to compute c
-0000cfe0: 6f6e 7365 6375 7469 7665 206e 756d 6265  onsecutive numbe
-0000cff0: 7273 2066 726f 6d2e 0a20 2020 2020 2020  rs from..       
-0000d000: 203a 7061 7261 6d20 6b77 6172 6773 3a20   :param kwargs: 
-0000d010: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
-0000d020: 7264 2061 7267 756d 656e 7473 2e0a 2020  rd arguments..  
-0000d030: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
-0000d040: 206c 6973 7420 6f66 206c 6973 7473 2c20   list of lists, 
-0000d050: 6561 6368 2063 6f6e 7461 696e 696e 6720  each containing 
-0000d060: 6120 7365 7175 656e 6365 206f 6620 636f  a sequence of co
-0000d070: 6e73 6563 7574 6976 6520 6e75 6d62 6572  nsecutive number
-0000d080: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-0000d090: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
-0000d0a0: 2074 6865 2069 6e70 7574 2069 7465 7261   the input itera
-0000d0b0: 626c 6520 746f 2061 206c 6973 7420 746f  ble to a list to
-0000d0c0: 2073 7570 706f 7274 2069 6e64 6578 696e   support indexin
-0000d0d0: 670a 2020 2020 2020 2020 6e75 6d62 6572  g.        number
-0000d0e0: 5f63 6f6d 6269 6e61 7469 6f6e 5f6c 6973  _combination_lis
-0000d0f0: 7420 3d20 6c69 7374 286e 756d 6265 725f  t = list(number_
-0000d100: 636f 6d62 696e 6174 696f 6e29 0a20 2020  combination).   
-0000d110: 2020 2020 2073 6571 7565 6e63 6573 203d       sequences =
-0000d120: 205b 5d0a 2020 2020 2020 2020 6375 7272   [].        curr
-0000d130: 656e 745f 7365 7175 656e 6365 203d 205b  ent_sequence = [
-0000d140: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
-0000d150: 6f6e 5f6c 6973 745b 305d 5d20 2023 2049  on_list[0]]  # I
-0000d160: 6e69 7469 616c 697a 6520 7769 7468 2074  nitialize with t
-0000d170: 6865 2066 6972 7374 206e 756d 6265 720a  he first number.
-0000d180: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-0000d190: 6e20 7261 6e67 6528 312c 206c 656e 286e  n range(1, len(n
-0000d1a0: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
-0000d1b0: 6e5f 6c69 7374 2929 3a0a 2020 2020 2020  n_list)):.      
-0000d1c0: 2020 2020 2020 6966 206e 756d 6265 725f        if number_
-0000d1d0: 636f 6d62 696e 6174 696f 6e5f 6c69 7374  combination_list
-0000d1e0: 5b69 5d20 3d3d 2063 7572 7265 6e74 5f73  [i] == current_s
-0000d1f0: 6571 7565 6e63 655b 2d31 5d20 2b20 313a  equence[-1] + 1:
-0000d200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d210: 2063 7572 7265 6e74 5f73 6571 7565 6e63   current_sequenc
-0000d220: 652e 6170 7065 6e64 286e 756d 6265 725f  e.append(number_
-0000d230: 636f 6d62 696e 6174 696f 6e5f 6c69 7374  combination_list
-0000d240: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
-0000d250: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000d260: 2020 2020 2020 2069 6620 6c65 6e28 6375         if len(cu
-0000d270: 7272 656e 745f 7365 7175 656e 6365 2920  rrent_sequence) 
-0000d280: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
-0000d290: 2020 2020 2020 2020 2073 6571 7565 6e63           sequenc
-0000d2a0: 6573 2e61 7070 656e 6428 6375 7272 656e  es.append(curren
-0000d2b0: 745f 7365 7175 656e 6365 290a 2020 2020  t_sequence).    
-0000d2c0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-0000d2d0: 656e 745f 7365 7175 656e 6365 203d 205b  ent_sequence = [
-0000d2e0: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
-0000d2f0: 6f6e 5f6c 6973 745b 695d 5d0a 0a20 2020  on_list[i]]..   
-0000d300: 2020 2020 2069 6620 6c65 6e28 6375 7272       if len(curr
-0000d310: 656e 745f 7365 7175 656e 6365 2920 3e20  ent_sequence) > 
-0000d320: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-0000d330: 6571 7565 6e63 6573 2e61 7070 656e 6428  equences.append(
-0000d340: 6375 7272 656e 745f 7365 7175 656e 6365  current_sequence
-0000d350: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0000d360: 6e20 7365 7175 656e 6365 730a 0a20 2020  n sequences..   
-0000d370: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-0000d380: 2020 6465 6620 6361 6c63 756c 6174 655f    def calculate_
-0000d390: 7265 7065 6174 6564 5f6e 756d 6265 7273  repeated_numbers
-0000d3a0: 280a 2020 2020 2020 2020 2020 2020 636c  (.            cl
-0000d3b0: 732c 0a20 2020 2020 2020 2020 2020 206e  s,.            n
-0000d3c0: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
-0000d3d0: 6e73 3a20 4974 6572 6162 6c65 5b49 7465  ns: Iterable[Ite
-0000d3e0: 7261 626c 655b 696e 745d 5d2c 0a20 2020  rable[int]],.   
-0000d3f0: 2020 2020 2020 2020 2077 696e 646f 773a           window:
-0000d400: 2069 6e74 203d 2032 2c0a 2020 2020 2020   int = 2,.      
-0000d410: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
-0000d420: 416e 790a 2020 2020 2920 2d3e 204c 6973  Any.    ) -> Lis
-0000d430: 745b 696e 745d 3a0a 2020 2020 2020 2020  t[int]:.        
-0000d440: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
-0000d450: 756c 6174 6520 7468 6520 6e75 6d62 6572  ulate the number
-0000d460: 7320 7468 6174 2061 7070 6561 7220 696e  s that appear in
-0000d470: 2061 6c6c 2067 6976 656e 2069 7465 7261   all given itera
-0000d480: 626c 6520 6f66 2069 6e74 6567 6572 7320  ble of integers 
-0000d490: 2869 6e74 6572 7365 6374 696f 6e29 2e0a  (intersection)..
-0000d4a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000d4b0: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
-0000d4c0: 6f6e 733a 2041 6e20 6974 6572 6162 6c65  ons: An iterable
-0000d4d0: 206f 6620 696e 7465 6765 7273 2074 6f20   of integers to 
-0000d4e0: 6669 6e64 2063 6f6d 6d6f 6e20 6e75 6d62  find common numb
-0000d4f0: 6572 732e 0a20 2020 2020 2020 203a 7061  ers..        :pa
-0000d500: 7261 6d20 7769 6e64 6f77 3a20 5468 6520  ram window: The 
-0000d510: 6e75 6d62 6572 206f 6620 7265 6365 6e74  number of recent
-0000d520: 2070 6572 696f 6473 2074 6f20 7072 6f63   periods to proc
-0000d530: 6573 732e 0a20 2020 2020 2020 203a 7061  ess..        :pa
-0000d540: 7261 6d20 6b77 6172 6773 3a20 4164 6469  ram kwargs: Addi
-0000d550: 7469 6f6e 616c 206b 6579 776f 7264 2061  tional keyword a
-0000d560: 7267 756d 656e 7473 2e0a 2020 2020 2020  rguments..      
-0000d570: 2020 3a72 6574 7572 6e3a 2041 206c 6973    :return: A lis
-0000d580: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
-0000d590: 206e 756d 6265 7273 2074 6861 7420 6172   numbers that ar
-0000d5a0: 6520 636f 6d6d 6f6e 2069 6e20 616c 6c20  e common in all 
-0000d5b0: 6769 7665 6e20 6974 6572 6162 6c65 732e  given iterables.
-0000d5c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d5d0: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
-0000d5e0: 6520 7468 6520 7365 7420 7769 7468 2074  e the set with t
-0000d5f0: 6865 2066 6972 7374 2069 7465 7261 626c  he first iterabl
-0000d600: 6520 746f 2073 7461 7274 2074 6865 2069  e to start the i
-0000d610: 6e74 6572 7365 6374 696f 6e20 7072 6f63  ntersection proc
-0000d620: 6573 730a 2020 2020 2020 2020 7265 7065  ess.        repe
-0000d630: 6174 6564 5f6e 756d 6265 7273 3a20 5365  ated_numbers: Se
-0000d640: 745b 696e 745d 203d 2073 6574 286e 6578  t[int] = set(nex
-0000d650: 7428 6974 6572 286e 756d 6265 725f 636f  t(iter(number_co
-0000d660: 6d62 696e 6174 696f 6e73 5b2d 7769 6e64  mbinations[-wind
-0000d670: 6f77 3a5d 292c 205b 5d29 290a 0a20 2020  ow:]), []))..   
-0000d680: 2020 2020 2023 2050 6572 666f 726d 2069       # Perform i
-0000d690: 6e74 6572 7365 6374 696f 6e20 7769 7468  ntersection with
-0000d6a0: 2074 6865 2073 7562 7365 7175 656e 7420   the subsequent 
-0000d6b0: 6974 6572 6162 6c65 730a 2020 2020 2020  iterables.      
-0000d6c0: 2020 666f 7220 6e75 6d62 6572 5f63 6f6d    for number_com
-0000d6d0: 6269 6e61 7469 6f6e 2069 6e20 6e75 6d62  bination in numb
-0000d6e0: 6572 5f63 6f6d 6269 6e61 7469 6f6e 733a  er_combinations:
-0000d6f0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-0000d700: 6561 7465 645f 6e75 6d62 6572 732e 696e  eated_numbers.in
-0000d710: 7465 7273 6563 7469 6f6e 5f75 7064 6174  tersection_updat
-0000d720: 6528 7365 7428 6e75 6d62 6572 5f63 6f6d  e(set(number_com
-0000d730: 6269 6e61 7469 6f6e 2929 0a0a 2020 2020  bination))..    
-0000d740: 2020 2020 2320 5265 7475 726e 2074 6865      # Return the
-0000d750: 2072 6573 756c 7420 6173 2061 206c 6973   result as a lis
-0000d760: 740a 2020 2020 2020 2020 7265 7475 726e  t.        return
-0000d770: 206c 6973 7428 7265 7065 6174 6564 5f6e   list(repeated_n
-0000d780: 756d 6265 7273 290a 0a20 2020 2040 636c  umbers)..    @cl
-0000d790: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-0000d7a0: 6620 6361 6c63 756c 6174 655f 6564 6765  f calculate_edge
-0000d7b0: 5f6e 756d 6265 7273 280a 2020 2020 2020  _numbers(.      
-0000d7c0: 2020 2020 2020 636c 732c 0a20 2020 2020        cls,.     
-0000d7d0: 2020 2020 2020 206e 756d 6265 725f 636f         number_co
-0000d7e0: 6d62 696e 6174 696f 6e73 3a20 4974 6572  mbinations: Iter
-0000d7f0: 6162 6c65 5b49 7465 7261 626c 655b 696e  able[Iterable[in
-0000d800: 745d 5d2c 0a20 2020 2020 2020 2020 2020  t]],.           
-0000d810: 2077 696e 646f 773a 2069 6e74 203d 2032   window: int = 2
-0000d820: 2c0a 2020 2020 2020 2020 2020 2020 2a2a  ,.            **
-0000d830: 6b77 6172 6773 3a20 416e 790a 2020 2020  kwargs: Any.    
-0000d840: 2920 2d3e 204c 6973 745b 696e 745d 3a0a  ) -> List[int]:.
-0000d850: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d860: 2020 2020 4361 6c63 756c 6174 6520 2765      Calculate 'e
-0000d870: 6467 6520 6e75 6d62 6572 7327 2077 6869  dge numbers' whi
-0000d880: 6368 2061 7265 2070 7265 7365 6e74 2069  ch are present i
-0000d890: 6e20 636f 6e73 6563 7574 6976 6520 6974  n consecutive it
-0000d8a0: 6572 6162 6c65 7320 7768 6572 6520 6561  erables where ea
-0000d8b0: 6368 206e 756d 6265 7220 6672 6f6d 2074  ch number from t
-0000d8c0: 6865 2066 6972 7374 2069 7465 7261 626c  he first iterabl
-0000d8d0: 650a 2020 2020 2020 2020 6973 2065 6974  e.        is eit
-0000d8e0: 6865 7220 6f6e 6520 6c65 7373 206f 7220  her one less or 
-0000d8f0: 6f6e 6520 6d6f 7265 2074 6861 6e20 7468  one more than th
-0000d900: 6520 6e75 6d62 6572 7320 696e 2074 6865  e numbers in the
-0000d910: 2066 6f6c 6c6f 7769 6e67 2069 7465 7261   following itera
-0000d920: 626c 652e 0a0a 2020 2020 2020 2020 3a70  ble...        :p
-0000d930: 6172 616d 206e 756d 6265 725f 636f 6d62  aram number_comb
-0000d940: 696e 6174 696f 6e73 3a20 416e 2069 7465  inations: An ite
-0000d950: 7261 626c 6520 6f66 2069 7465 7261 626c  rable of iterabl
-0000d960: 6573 206f 6620 696e 7465 6765 7273 2074  es of integers t
-0000d970: 6f20 6669 6e64 2027 6564 6765 206e 756d  o find 'edge num
-0000d980: 6265 7273 272e 0a20 2020 2020 2020 203a  bers'..        :
-0000d990: 7061 7261 6d20 7769 6e64 6f77 3a20 5468  param window: Th
-0000d9a0: 6520 6e75 6d62 6572 206f 6620 7265 6365  e number of rece
-0000d9b0: 6e74 2070 6572 696f 6473 2074 6f20 7072  nt periods to pr
-0000d9c0: 6f63 6573 732e 0a20 2020 2020 2020 203a  ocess..        :
-0000d9d0: 7061 7261 6d20 6b77 6172 6773 3a20 4164  param kwargs: Ad
-0000d9e0: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
-0000d9f0: 2061 7267 756d 656e 7473 2e0a 2020 2020   arguments..    
-0000da00: 2020 2020 3a72 6574 7572 6e3a 2041 206c      :return: A l
-0000da10: 6973 7420 636f 6e74 6169 6e69 6e67 2074  ist containing t
-0000da20: 6865 2027 6564 6765 206e 756d 6265 7273  he 'edge numbers
-0000da30: 272e 0a20 2020 2020 2020 2022 2222 0a20  '..        """. 
-0000da40: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
-0000da50: 2074 6865 2069 6e70 7574 2074 6f20 6120   the input to a 
-0000da60: 6c69 7374 2066 6f72 2069 6e64 6578 6564  list for indexed
-0000da70: 2061 6363 6573 730a 2020 2020 2020 2020   access.        
-0000da80: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
-0000da90: 6f6e 735f 6c69 7374 203d 206c 6973 7428  ons_list = list(
-0000daa0: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
-0000dab0: 6f6e 735b 2d77 696e 646f 773a 5d29 0a0a  ons[-window:])..
-0000dac0: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
-0000dad0: 6c69 7a65 2061 6e20 656d 7074 7920 7365  lize an empty se
-0000dae0: 7420 666f 7220 7468 6520 6564 6765 206e  t for the edge n
-0000daf0: 756d 6265 7273 0a20 2020 2020 2020 2065  umbers.        e
-0000db00: 6467 655f 6e75 6d62 6572 733a 2053 6574  dge_numbers: Set
-0000db10: 5b69 6e74 5d20 3d20 7365 7428 290a 0a20  [int] = set().. 
-0000db20: 2020 2020 2020 2023 2049 7465 7261 7465         # Iterate
-0000db30: 206f 7665 7220 6561 6368 206e 756d 6265   over each numbe
-0000db40: 7220 636f 6d62 696e 6174 696f 6e2c 2073  r combination, s
-0000db50: 7461 7274 696e 6720 6672 6f6d 2074 6865  tarting from the
-0000db60: 2073 6563 6f6e 6420 6f6e 650a 2020 2020   second one.    
-0000db70: 2020 2020 666f 7220 696e 6465 7820 696e      for index in
-0000db80: 2072 616e 6765 2831 2c20 6c65 6e28 6e75   range(1, len(nu
-0000db90: 6d62 6572 5f63 6f6d 6269 6e61 7469 6f6e  mber_combination
-0000dba0: 735f 6c69 7374 2929 3a0a 2020 2020 2020  s_list)):.      
-0000dbb0: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
-0000dbc0: 2073 6574 206f 6620 706f 7465 6e74 6961   set of potentia
-0000dbd0: 6c20 6564 6765 206e 756d 6265 7273 2066  l edge numbers f
-0000dbe0: 726f 6d20 7468 6520 7072 6576 696f 7573  rom the previous
-0000dbf0: 2063 6f6d 6269 6e61 7469 6f6e 0a20 2020   combination.   
-0000dc00: 2020 2020 2020 2020 206c 6173 745f 6e75           last_nu
-0000dc10: 6d62 6572 5f73 6574 203d 2073 6574 286e  mber_set = set(n
-0000dc20: 756d 202b 2069 2066 6f72 2069 2069 6e20  um + i for i in 
-0000dc30: 5b2d 312c 2030 2c20 315d 0a20 2020 2020  [-1, 0, 1].     
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc50: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000dc60: 206e 756d 2069 6e20 6e75 6d62 6572 5f63   num in number_c
-0000dc70: 6f6d 6269 6e61 7469 6f6e 735f 6c69 7374  ombinations_list
-0000dc80: 5b69 6e64 6578 202d 2031 5d0a 2020 2020  [index - 1].    
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000dcb0: 2028 6e75 6d20 2b20 6929 203e 2030 290a   (num + i) > 0).
-0000dcc0: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
-0000dcd0: 6561 7465 2061 2073 6574 2066 726f 6d20  eate a set from 
-0000dce0: 7468 6520 6375 7272 656e 7420 636f 6d62  the current comb
-0000dcf0: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
-0000dd00: 2020 2020 6375 7272 656e 745f 6e75 6d62      current_numb
-0000dd10: 6572 5f73 6574 203d 2073 6574 286e 756d  er_set = set(num
-0000dd20: 6265 725f 636f 6d62 696e 6174 696f 6e73  ber_combinations
-0000dd30: 5f6c 6973 745b 696e 6465 785d 290a 2020  _list[index]).  
-0000dd40: 2020 2020 2020 2020 2020 2320 4669 6e64            # Find
-0000dd50: 2074 6865 2069 6e74 6572 7365 6374 696f   the intersectio
-0000dd60: 6e20 6f66 2074 6865 2074 776f 2073 6574  n of the two set
-0000dd70: 730a 2020 2020 2020 2020 2020 2020 696e  s.            in
-0000dd80: 7465 7273 6563 7469 6f6e 203d 2063 7572  tersection = cur
-0000dd90: 7265 6e74 5f6e 756d 6265 725f 7365 742e  rent_number_set.
-0000dda0: 696e 7465 7273 6563 7469 6f6e 286c 6173  intersection(las
-0000ddb0: 745f 6e75 6d62 6572 5f73 6574 290a 2020  t_number_set).  
-0000ddc0: 2020 2020 2020 2020 2020 2320 5570 6461            # Upda
-0000ddd0: 7465 2074 6865 2065 6467 6520 6e75 6d62  te the edge numb
-0000dde0: 6572 7320 7365 7420 7769 7468 2074 6865  ers set with the
-0000ddf0: 2069 6e74 6572 7365 6374 696f 6e0a 2020   intersection.  
-0000de00: 2020 2020 2020 2020 2020 6564 6765 5f6e            edge_n
-0000de10: 756d 6265 7273 2e75 7064 6174 6528 696e  umbers.update(in
-0000de20: 7465 7273 6563 7469 6f6e 290a 0a20 2020  tersection)..   
-0000de30: 2020 2020 2023 2052 6574 7572 6e20 7468       # Return th
-0000de40: 6520 7265 7375 6c74 2061 7320 6120 736f  e result as a so
-0000de50: 7274 6564 206c 6973 7420 746f 206d 6169  rted list to mai
-0000de60: 6e74 6169 6e20 6120 636f 6e73 6973 7465  ntain a consiste
-0000de70: 6e74 206f 7264 6572 0a20 2020 2020 2020  nt order.       
-0000de80: 2072 6574 7572 6e20 736f 7274 6564 2865   return sorted(e
-0000de90: 6467 655f 6e75 6d62 6572 7329 0a0a 2020  dge_numbers)..  
-0000dea0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-0000deb0: 2020 2064 6566 2063 616c 6375 6c61 7465     def calculate
-0000dec0: 5f63 6f6c 645f 686f 745f 6e75 6d62 6572  _cold_hot_number
-0000ded0: 7328 0a20 2020 2020 2020 2020 2020 2063  s(.            c
-0000dee0: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-0000def0: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
-0000df00: 6f6e 733a 2049 7465 7261 626c 655b 4974  ons: Iterable[It
-0000df10: 6572 6162 6c65 5b69 6e74 5d5d 2c0a 2020  erable[int]],.  
-0000df20: 2020 2020 2020 2020 2020 616c 6c5f 6e75            all_nu
-0000df30: 6d62 6572 733a 2049 7465 7261 626c 655b  mbers: Iterable[
-0000df40: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
-0000df50: 2020 7769 6e64 6f77 3a20 696e 7420 3d20    window: int = 
-0000df60: 352c 0a20 2020 2020 2020 2020 2020 202a  5,.            *
-0000df70: 2a6b 7761 7267 733a 2041 6e79 0a20 2020  *kwargs: Any.   
-0000df80: 2029 202d 3e20 5475 706c 655b 4c69 7374   ) -> Tuple[List
-0000df90: 5b69 6e74 5d2c 204c 6973 745b 696e 745d  [int], List[int]
-0000dfa0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-0000dfb0: 2020 2020 2020 2043 616c 6375 6c61 7465         Calculate
-0000dfc0: 2061 6e64 2072 6574 7572 6e20 2763 6f6c   and return 'col
-0000dfd0: 6420 6e75 6d62 6572 7327 2061 6e64 2027  d numbers' and '
-0000dfe0: 686f 7420 6e75 6d62 6572 7327 2066 726f  hot numbers' fro
-0000dff0: 6d20 6120 7365 7269 6573 206f 6620 6e75  m a series of nu
-0000e000: 6d62 6572 2063 6f6d 6269 6e61 7469 6f6e  mber combination
-0000e010: 732e 0a20 2020 2020 2020 2027 436f 6c64  s..        'Cold
-0000e020: 206e 756d 6265 7273 2720 6172 6520 7468   numbers' are th
-0000e030: 6f73 6520 7468 6174 2064 6964 206e 6f74  ose that did not
-0000e040: 2061 7070 6561 7220 696e 2074 6865 206c   appear in the l
-0000e050: 6173 7420 3520 6974 6572 6174 696f 6e73  ast 5 iterations
-0000e060: 2c0a 2020 2020 2020 2020 616e 6420 2768  ,.        and 'h
-0000e070: 6f74 206e 756d 6265 7273 2720 6172 6520  ot numbers' are 
-0000e080: 7468 6f73 6520 7468 6174 2061 7070 6561  those that appea
-0000e090: 7265 6420 6174 206c 6561 7374 206f 6e63  red at least onc
-0000e0a0: 6520 696e 2074 6865 206c 6173 7420 3520  e in the last 5 
-0000e0b0: 6974 6572 6174 696f 6e73 2e0a 0a20 2020  iterations...   
-0000e0c0: 2020 2020 203a 7061 7261 6d20 6e75 6d62       :param numb
-0000e0d0: 6572 5f63 6f6d 6269 6e61 7469 6f6e 733a  er_combinations:
-0000e0e0: 2041 6e20 6974 6572 6162 6c65 206f 6620   An iterable of 
-0000e0f0: 6974 6572 6162 6c65 7320 6f66 2069 6e74  iterables of int
-0000e100: 6567 6572 7320 746f 2061 6e61 6c79 7a65  egers to analyze
-0000e110: 206e 756d 6265 7273 2e0a 2020 2020 2020   numbers..      
-0000e120: 2020 3a70 6172 616d 2061 6c6c 5f6e 756d    :param all_num
-0000e130: 6265 7273 3a20 416e 2069 7465 7261 626c  bers: An iterabl
-0000e140: 6520 6f66 2061 6c6c 2070 6f73 7369 626c  e of all possibl
-0000e150: 6520 6e75 6d62 6572 7320 7468 6174 2063  e numbers that c
-0000e160: 6f75 6c64 2061 7070 6561 722e 0a20 2020  ould appear..   
-0000e170: 2020 2020 203a 7061 7261 6d20 7769 6e64       :param wind
-0000e180: 6f77 3a20 6465 6661 756c 7420 350a 2020  ow: default 5.  
-0000e190: 2020 2020 2020 3a70 6172 616d 206b 7761        :param kwa
-0000e1a0: 7267 733a 2041 6464 6974 696f 6e61 6c20  rgs: Additional 
-0000e1b0: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
-0000e1c0: 732e 0a20 2020 2020 2020 203a 7265 7475  s..        :retu
-0000e1d0: 726e 3a20 4120 7475 706c 6520 636f 6e74  rn: A tuple cont
-0000e1e0: 6169 6e69 6e67 2074 776f 206c 6973 7473  aining two lists
-0000e1f0: 202d 2074 6865 2066 6972 7374 2077 6974   - the first wit
-0000e200: 6820 2763 6f6c 6420 6e75 6d62 6572 7327  h 'cold numbers'
-0000e210: 2061 6e64 2074 6865 2073 6563 6f6e 6420   and the second 
-0000e220: 7769 7468 2027 686f 7420 6e75 6d62 6572  with 'hot number
-0000e230: 7327 2e0a 2020 2020 2020 2020 2222 220a  s'..        """.
-0000e240: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-0000e250: 7420 7468 6520 696e 7075 7420 746f 2061  t the input to a
-0000e260: 206c 6973 7420 666f 7220 696e 6465 7865   list for indexe
-0000e270: 6420 6163 6365 7373 0a20 2020 2020 2020  d access.       
-0000e280: 206e 756d 6265 725f 636f 6d62 696e 6174   number_combinat
-0000e290: 696f 6e73 5f6c 6973 7420 3d20 6c69 7374  ions_list = list
-0000e2a0: 286e 756d 6265 725f 636f 6d62 696e 6174  (number_combinat
-0000e2b0: 696f 6e73 5b2d 7769 6e64 6f77 3a5d 290a  ions[-window:]).
-0000e2c0: 0a20 2020 2020 2020 2023 2044 6574 6572  .        # Deter
-0000e2d0: 6d69 6e65 2074 6865 2072 616e 6765 2066  mine the range f
-0000e2e0: 6f72 2074 6865 206c 6173 7420 3520 7065  or the last 5 pe
-0000e2f0: 7269 6f64 730a 2020 2020 2020 2020 6c61  riods.        la
-0000e300: 7374 5f66 6976 655f 7065 7269 6f64 7320  st_five_periods 
-0000e310: 3d20 6e75 6d62 6572 5f63 6f6d 6269 6e61  = number_combina
-0000e320: 7469 6f6e 735f 6c69 7374 2069 6620 6c65  tions_list if le
-0000e330: 6e28 0a20 2020 2020 2020 2020 2020 206e  n(.            n
-0000e340: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
-0000e350: 6e73 5f6c 6973 7429 203e 3d20 7769 6e64  ns_list) >= wind
-0000e360: 6f77 2065 6c73 6520 6e75 6d62 6572 5f63  ow else number_c
-0000e370: 6f6d 6269 6e61 7469 6f6e 735f 6c69 7374  ombinations_list
-0000e380: 0a0a 2020 2020 2020 2020 2320 466c 6174  ..        # Flat
-0000e390: 7465 6e20 7468 6520 6c69 7374 206f 6620  ten the list of 
-0000e3a0: 6c61 7374 2066 6976 6520 7065 7269 6f64  last five period
-0000e3b0: 7320 616e 6420 636f 6e76 6572 7420 746f  s and convert to
-0000e3c0: 2061 2073 6574 2074 6f20 7265 6d6f 7665   a set to remove
-0000e3d0: 2064 7570 6c69 6361 7465 730a 2020 2020   duplicates.    
-0000e3e0: 2020 2020 6e75 6d62 6572 735f 696e 5f6c      numbers_in_l
-0000e3f0: 6173 745f 6669 7665 5f70 6572 696f 6473  ast_five_periods
-0000e400: 3a20 5365 745b 696e 745d 203d 2073 6574  : Set[int] = set
-0000e410: 286e 756d 2066 6f72 2070 6572 696f 6420  (num for period 
-0000e420: 696e 206c 6173 745f 6669 7665 5f70 6572  in last_five_per
-0000e430: 696f 6473 2066 6f72 206e 756d 2069 6e20  iods for num in 
-0000e440: 7065 7269 6f64 290a 0a20 2020 2020 2020  period)..       
-0000e450: 2023 2043 6f6e 7665 7274 2061 6c6c 5f6e   # Convert all_n
-0000e460: 756d 6265 7273 2074 6f20 6120 7365 7420  umbers to a set 
-0000e470: 666f 7220 6566 6669 6369 656e 7420 6c6f  for efficient lo
-0000e480: 6f6b 7570 0a20 2020 2020 2020 2061 6c6c  okup.        all
-0000e490: 5f6e 756d 6265 7273 5f73 6574 3a20 5365  _numbers_set: Se
-0000e4a0: 745b 696e 745d 203d 2073 6574 2861 6c6c  t[int] = set(all
-0000e4b0: 5f6e 756d 6265 7273 290a 0a20 2020 2020  _numbers)..     
-0000e4c0: 2020 2023 2027 436f 6c64 206e 756d 6265     # 'Cold numbe
-0000e4d0: 7273 2720 6172 6520 7468 6f73 6520 7468  rs' are those th
-0000e4e0: 6174 2061 7265 206e 6f74 2069 6e20 7468  at are not in th
-0000e4f0: 6520 6c61 7374 2066 6976 6520 7065 7269  e last five peri
-0000e500: 6f64 730a 2020 2020 2020 2020 636f 6c64  ods.        cold
-0000e510: 5f6e 756d 6265 7273 3a20 4c69 7374 5b69  _numbers: List[i
-0000e520: 6e74 5d20 3d20 736f 7274 6564 286c 6973  nt] = sorted(lis
-0000e530: 7428 616c 6c5f 6e75 6d62 6572 735f 7365  t(all_numbers_se
-0000e540: 7420 2d20 6e75 6d62 6572 735f 696e 5f6c  t - numbers_in_l
-0000e550: 6173 745f 6669 7665 5f70 6572 696f 6473  ast_five_periods
-0000e560: 2929 0a0a 2020 2020 2020 2020 2320 2748  ))..        # 'H
-0000e570: 6f74 206e 756d 6265 7273 2720 6172 6520  ot numbers' are 
-0000e580: 7468 6f73 6520 7468 6174 2061 7265 2069  those that are i
-0000e590: 6e20 7468 6520 6c61 7374 2066 6976 6520  n the last five 
-0000e5a0: 7065 7269 6f64 730a 2020 2020 2020 2020  periods.        
-0000e5b0: 686f 745f 6e75 6d62 6572 733a 204c 6973  hot_numbers: Lis
-0000e5c0: 745b 696e 745d 203d 2073 6f72 7465 6428  t[int] = sorted(
-0000e5d0: 6c69 7374 286e 756d 6265 7273 5f69 6e5f  list(numbers_in_
-0000e5e0: 6c61 7374 5f66 6976 655f 7065 7269 6f64  last_five_period
-0000e5f0: 7329 290a 0a20 2020 2020 2020 2023 2052  s))..        # R
-0000e600: 6574 7572 6e20 7468 6520 636f 6c64 206e  eturn the cold n
-0000e610: 756d 6265 7273 2061 6e64 2068 6f74 206e  umbers and hot n
-0000e620: 756d 6265 7273 0a20 2020 2020 2020 2072  umbers.        r
-0000e630: 6574 7572 6e20 636f 6c64 5f6e 756d 6265  eturn cold_numbe
-0000e640: 7273 2c20 686f 745f 6e75 6d62 6572 730a  rs, hot_numbers.
-0000e650: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-0000e660: 640a 2020 2020 6465 6620 6361 6c63 756c  d.    def calcul
-0000e670: 6174 655f 6f6d 6974 7465 645f 6e75 6d62  ate_omitted_numb
-0000e680: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
-0000e690: 2063 6c73 2c0a 2020 2020 2020 2020 2020   cls,.          
-0000e6a0: 2020 6e75 6d62 6572 5f63 6f6d 6269 6e61    number_combina
-0000e6b0: 7469 6f6e 733a 2049 7465 7261 626c 655b  tions: Iterable[
-0000e6c0: 4974 6572 6162 6c65 5b69 6e74 5d5d 2c0a  Iterable[int]],.
-0000e6d0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-0000e6e0: 6e75 6d62 6572 733a 2049 7465 7261 626c  numbers: Iterabl
-0000e6f0: 655b 696e 745d 2c0a 2020 2020 2020 2020  e[int],.        
-0000e700: 2020 2020 7769 6e64 6f77 3a20 696e 7420      window: int 
-0000e710: 3d20 3130 2c0a 2020 2020 2020 2020 2020  = 10,.          
-0000e720: 2020 2a2a 6b77 6172 6773 3a20 416e 790a    **kwargs: Any.
-0000e730: 2020 2020 2920 2d3e 2044 6963 745b 696e      ) -> Dict[in
-0000e740: 742c 2069 6e74 5d3a 0a20 2020 2020 2020  t, int]:.       
-0000e750: 2022 2222 0a20 2020 2020 2020 2055 7064   """.        Upd
-0000e760: 6174 6520 616e 6420 7265 7475 726e 2074  ate and return t
-0000e770: 6865 206f 6d69 7373 696f 6e20 7661 6c75  he omission valu
-0000e780: 6573 2066 6f72 2065 6163 6820 6e75 6d62  es for each numb
-0000e790: 6572 2069 6e20 616c 6c5f 6e75 6d62 6572  er in all_number
-0000e7a0: 732e 0a0a 2020 2020 2020 2020 3a70 6172  s...        :par
-0000e7b0: 616d 206e 756d 6265 725f 636f 6d62 696e  am number_combin
-0000e7c0: 6174 696f 6e73 3a20 4120 6c69 7374 206f  ations: A list o
-0000e7d0: 6620 6c69 7374 7320 6f66 2069 6e74 6567  f lists of integ
-0000e7e0: 6572 7320 7265 7072 6573 656e 7469 6e67  ers representing
-0000e7f0: 2070 6173 7420 6e75 6d62 6572 2064 7261   past number dra
-0000e800: 7773 2e0a 2020 2020 2020 2020 3a70 6172  ws..        :par
-0000e810: 616d 2061 6c6c 5f6e 756d 6265 7273 3a20  am all_numbers: 
-0000e820: 4120 6c69 7374 206f 6620 616c 6c20 706f  A list of all po
-0000e830: 7373 6962 6c65 206e 756d 6265 7273 2074  ssible numbers t
-0000e840: 6861 7420 636f 756c 6420 6170 7065 6172  hat could appear
-0000e850: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000e860: 2077 696e 646f 773a 2064 6566 6175 6c74   window: default
-0000e870: 2031 300a 2020 2020 2020 2020 3a72 6574   10.        :ret
-0000e880: 7572 6e3a 2041 2064 6963 7469 6f6e 6172  urn: A dictionar
-0000e890: 7920 7769 7468 206e 756d 6265 7273 2061  y with numbers a
-0000e8a0: 7320 6b65 7973 2061 6e64 2074 6865 6972  s keys and their
-0000e8b0: 206f 6d69 7373 696f 6e20 7661 6c75 6573   omission values
-0000e8c0: 2061 7320 7661 6c75 6573 2e0a 2020 2020   as values..    
-0000e8d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000e8e0: 2320 496e 6974 6961 6c69 7a65 2074 6865  # Initialize the
-0000e8f0: 206f 6d69 7373 696f 6e20 7661 6c75 6573   omission values
-0000e900: 2066 6f72 2065 6163 6820 6e75 6d62 6572   for each number
-0000e910: 2074 6f20 300a 2020 2020 2020 2020 6f6d   to 0.        om
-0000e920: 6973 7369 6f6e 5f76 616c 7565 733a 2044  ission_values: D
-0000e930: 6963 745b 696e 742c 2069 6e74 5d20 3d20  ict[int, int] = 
-0000e940: 7b6e 756d 6265 723a 202d 3120 666f 7220  {number: -1 for 
-0000e950: 6e75 6d62 6572 2069 6e20 616c 6c5f 6e75  number in all_nu
-0000e960: 6d62 6572 737d 0a0a 2020 2020 2020 2020  mbers}..        
-0000e970: 2320 436f 6e76 6572 7420 7468 6520 696e  # Convert the in
-0000e980: 7075 7420 746f 2061 206c 6973 7420 666f  put to a list fo
-0000e990: 7220 696e 6465 7865 6420 6163 6365 7373  r indexed access
-0000e9a0: 0a20 2020 2020 2020 206e 756d 6265 725f  .        number_
-0000e9b0: 636f 6d62 696e 6174 696f 6e73 5f6c 6973  combinations_lis
-0000e9c0: 7420 3d20 6c69 7374 286e 756d 6265 725f  t = list(number_
-0000e9d0: 636f 6d62 696e 6174 696f 6e73 5b2d 7769  combinations[-wi
-0000e9e0: 6e64 6f77 3a5d 290a 0a20 2020 2020 2020  ndow:])..       
-0000e9f0: 2023 2044 6574 6572 6d69 6e65 2074 6865   # Determine the
-0000ea00: 2072 616e 6765 2066 6f72 2074 6865 206c   range for the l
-0000ea10: 6173 7420 3520 7065 7269 6f64 730a 2020  ast 5 periods.  
-0000ea20: 2020 2020 2020 6c61 7374 5f74 656e 5f70        last_ten_p
-0000ea30: 6572 696f 6473 203d 206e 756d 6265 725f  eriods = number_
-0000ea40: 636f 6d62 696e 6174 696f 6e73 5f6c 6973  combinations_lis
-0000ea50: 7420 6966 206c 656e 280a 2020 2020 2020  t if len(.      
-0000ea60: 2020 2020 2020 6e75 6d62 6572 5f63 6f6d        number_com
-0000ea70: 6269 6e61 7469 6f6e 735f 6c69 7374 2920  binations_list) 
-0000ea80: 3e3d 2077 696e 646f 7720 656c 7365 206e  >= window else n
-0000ea90: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
-0000eaa0: 6e73 5f6c 6973 740a 0a20 2020 2020 2020  ns_list..       
-0000eab0: 2023 2054 6865 206e 756d 6265 7220 6f66   # The number of
-0000eac0: 2064 7261 7773 2073 696e 6365 2074 6865   draws since the
-0000ead0: 206c 6173 7420 6170 7065 6172 616e 6365   last appearance
-0000eae0: 0a20 2020 2020 2020 2064 7261 7773 5f73  .        draws_s
-0000eaf0: 696e 6365 5f6c 6173 745f 6170 7065 6172  ince_last_appear
-0000eb00: 616e 6365 203d 2030 0a0a 2020 2020 2020  ance = 0..      
-0000eb10: 2020 2320 4974 6572 6174 6520 6f76 6572    # Iterate over
-0000eb20: 2074 6865 2070 6173 7420 6472 6177 7320   the past draws 
-0000eb30: 696e 2072 6576 6572 7365 206f 7264 6572  in reverse order
-0000eb40: 2028 6d6f 7374 2072 6563 656e 7420 6669   (most recent fi
-0000eb50: 7273 7429 0a20 2020 2020 2020 2066 6f72  rst).        for
-0000eb60: 2064 7261 7720 696e 2072 6576 6572 7365   draw in reverse
-0000eb70: 6428 6c61 7374 5f74 656e 5f70 6572 696f  d(last_ten_perio
-0000eb80: 6473 293a 0a20 2020 2020 2020 2020 2020  ds):.           
-0000eb90: 2023 2043 6865 636b 2065 6163 6820 6e75   # Check each nu
-0000eba0: 6d62 6572 2069 6e20 616c 6c5f 6e75 6d62  mber in all_numb
-0000ebb0: 6572 730a 2020 2020 2020 2020 2020 2020  ers.            
-0000ebc0: 666f 7220 6e75 6d62 6572 2069 6e20 616c  for number in al
-0000ebd0: 6c5f 6e75 6d62 6572 733a 0a20 2020 2020  l_numbers:.     
-0000ebe0: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
-0000ebf0: 7468 6520 6e75 6d62 6572 2069 7320 696e  the number is in
-0000ec00: 2074 6865 2063 7572 7265 6e74 2064 7261   the current dra
-0000ec10: 7720 616e 6420 6974 7320 6f6d 6973 7369  w and its omissi
-0000ec20: 6f6e 2076 616c 7565 2069 7320 2d31 2028  on value is -1 (
-0000ec30: 6861 736e 2774 2061 7070 6561 7265 6420  hasn't appeared 
-0000ec40: 7965 7429 0a20 2020 2020 2020 2020 2020  yet).           
-0000ec50: 2020 2020 2069 6620 6e75 6d62 6572 2069       if number i
-0000ec60: 6e20 6472 6177 2061 6e64 206f 6d69 7373  n draw and omiss
-0000ec70: 696f 6e5f 7661 6c75 6573 5b6e 756d 6265  ion_values[numbe
-0000ec80: 725d 203d 3d20 2d31 3a0a 2020 2020 2020  r] == -1:.      
-0000ec90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000eca0: 5365 7420 7468 6520 6f6d 6973 7369 6f6e  Set the omission
-0000ecb0: 2076 616c 7565 2074 6f20 7468 6520 6e75   value to the nu
-0000ecc0: 6d62 6572 206f 6620 6472 6177 7320 7369  mber of draws si
-0000ecd0: 6e63 6520 6974 206c 6173 7420 6170 7065  nce it last appe
-0000ece0: 6172 6564 0a20 2020 2020 2020 2020 2020  ared.           
-0000ecf0: 2020 2020 2020 2020 206f 6d69 7373 696f           omissio
-0000ed00: 6e5f 7661 6c75 6573 5b6e 756d 6265 725d  n_values[number]
-0000ed10: 203d 2064 7261 7773 5f73 696e 6365 5f6c   = draws_since_l
-0000ed20: 6173 745f 6170 7065 6172 616e 6365 0a20  ast_appearance. 
-0000ed30: 2020 2020 2020 2020 2020 2023 2049 6e63             # Inc
-0000ed40: 7265 6d65 6e74 2074 6865 2063 6f75 6e74  rement the count
-0000ed50: 206f 6620 6472 6177 7320 7369 6e63 6520   of draws since 
-0000ed60: 7468 6520 6c61 7374 2061 7070 6561 7261  the last appeara
-0000ed70: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-0000ed80: 6472 6177 735f 7369 6e63 655f 6c61 7374  draws_since_last
-0000ed90: 5f61 7070 6561 7261 6e63 6520 2b3d 2031  _appearance += 1
-0000eda0: 0a0a 2020 2020 2020 2020 2320 466f 7220  ..        # For 
-0000edb0: 616e 7920 6e75 6d62 6572 2074 6861 7420  any number that 
-0000edc0: 6861 736e 2774 2061 7070 6561 7265 6420  hasn't appeared 
-0000edd0: 7965 742c 2073 6574 2069 7473 206f 6d69  yet, set its omi
-0000ede0: 7373 696f 6e20 7661 6c75 6520 746f 2074  ssion value to t
-0000edf0: 6865 2074 6f74 616c 206e 756d 6265 7220  he total number 
-0000ee00: 6f66 2064 7261 7773 0a20 2020 2020 2020  of draws.       
-0000ee10: 2066 6f72 206e 756d 6265 7220 696e 2061   for number in a
-0000ee20: 6c6c 5f6e 756d 6265 7273 3a0a 2020 2020  ll_numbers:.    
-0000ee30: 2020 2020 2020 2020 6966 206f 6d69 7373          if omiss
-0000ee40: 696f 6e5f 7661 6c75 6573 5b6e 756d 6265  ion_values[numbe
-0000ee50: 725d 203d 3d20 2d31 3a0a 2020 2020 2020  r] == -1:.      
-0000ee60: 2020 2020 2020 2020 2020 6f6d 6973 7369            omissi
-0000ee70: 6f6e 5f76 616c 7565 735b 6e75 6d62 6572  on_values[number
-0000ee80: 5d20 3d20 6472 6177 735f 7369 6e63 655f  ] = draws_since_
-0000ee90: 6c61 7374 5f61 7070 6561 7261 6e63 650a  last_appearance.
-0000eea0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000eeb0: 6f6d 6973 7369 6f6e 5f76 616c 7565 730a  omission_values.
-0000eec0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0000eed0: 6f64 0a20 2020 2064 6566 2063 616c 6375  od.    def calcu
-0000eee0: 6c61 7465 5f73 7461 6e64 6172 645f 6465  late_standard_de
-0000eef0: 7669 6174 696f 6e5f 7765 6c66 6f72 6428  viation_welford(
-0000ef00: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
-0000ef10: 3a20 4c69 7374 5b55 6e69 6f6e 5b69 6e74  : List[Union[int
-0000ef20: 2c20 666c 6f61 745d 5d2c 0a20 2020 2020  , float]],.     
-0000ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef50: 2020 2020 2020 2020 6465 6361 795f 6661          decay_fa
-0000ef60: 6374 6f72 3a20 556e 696f 6e5b 696e 742c  ctor: Union[int,
-0000ef70: 2066 6c6f 6174 5d20 3d20 302e 3935 2920   float] = 0.95) 
-0000ef80: 2d3e 2055 6e69 6f6e 5b69 6e74 2c20 666c  -> Union[int, fl
-0000ef90: 6f61 745d 3a0a 2020 2020 2020 2020 2222  oat]:.        ""
-0000efa0: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
-0000efb0: 6174 6573 2074 6865 2073 7461 6e64 6172  ates the standar
-0000efc0: 6420 6465 7669 6174 696f 6e20 6f66 2061  d deviation of a
-0000efd0: 206e 756d 6572 6963 2073 6571 7565 6e63   numeric sequenc
-0000efe0: 6520 7573 696e 6720 5765 6c66 6f72 6427  e using Welford'
-0000eff0: 7320 6d65 7468 6f64 2e0a 0a20 2020 2020  s method...     
-0000f000: 2020 2054 6869 7320 6d65 7468 6f64 2069     This method i
-0000f010: 7320 616e 206f 6e6c 696e 6520 616c 676f  s an online algo
-0000f020: 7269 7468 6d20 6465 7369 676e 6564 2074  rithm designed t
-0000f030: 6f20 636f 6d70 7574 6520 7468 6520 7374  o compute the st
-0000f040: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-0000f050: 206f 6620 6120 7365 7175 656e 6365 206f   of a sequence o
-0000f060: 6620 6e75 6d62 6572 730a 2020 2020 2020  f numbers.      
-0000f070: 2020 6974 6572 6174 6976 656c 792c 2077    iteratively, w
-0000f080: 6869 6368 2063 616e 2062 6520 7573 6566  hich can be usef
-0000f090: 756c 2066 6f72 206c 6172 6765 2064 6174  ul for large dat
-0000f0a0: 6173 6574 7320 7768 6572 6520 616c 6c20  asets where all 
-0000f0b0: 6461 7461 2063 616e 6e6f 7420 6265 206c  data cannot be l
-0000f0c0: 6f61 6465 6420 696e 746f 206d 656d 6f72  oaded into memor
-0000f0d0: 7920 6174 206f 6e63 652e 0a0a 2020 2020  y at once...    
-0000f0e0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000f0f0: 2020 2020 2020 6e75 6d65 7269 635f 7365        numeric_se
-0000f100: 7175 656e 6365 2028 4c69 7374 5b55 6e69  quence (List[Uni
-0000f110: 6f6e 5b69 6e74 2c20 666c 6f61 745d 5d29  on[int, float]])
-0000f120: 3a20 5468 6520 7365 7175 656e 6365 206f  : The sequence o
-0000f130: 6620 6e75 6d62 6572 7320 2869 6e74 6567  f numbers (integ
-0000f140: 6572 7320 6f72 2066 6c6f 6174 7329 2066  ers or floats) f
-0000f150: 6f72 2077 6869 6368 2074 6865 2073 7461  or which the sta
-0000f160: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
-0000f170: 6973 2074 6f20 6265 2063 616c 6375 6c61  is to be calcula
-0000f180: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
-0000f190: 2064 6563 6179 5f66 6163 746f 7220 2855   decay_factor (U
-0000f1a0: 6e69 6f6e 5b69 6e74 2c20 666c 6f61 745d  nion[int, float]
-0000f1b0: 293a 2054 6865 2064 6563 6179 2066 6163  ): The decay fac
-0000f1c0: 746f 7220 666f 7220 7765 6967 6874 696e  tor for weightin
-0000f1d0: 6720 7265 6365 6e74 2076 616c 7565 7320  g recent values 
-0000f1e0: 6d6f 7265 2068 6561 7669 6c79 2e20 4465  more heavily. De
-0000f1f0: 6661 756c 7473 2074 6f20 302e 3935 2e0a  faults to 0.95..
-0000f200: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000f210: 3a0a 2020 2020 2020 2020 2020 2020 666c  :.            fl
-0000f220: 6f61 743a 2054 6865 2073 7461 6e64 6172  oat: The standar
-0000f230: 6420 6465 7669 6174 696f 6e20 6f66 2074  d deviation of t
-0000f240: 6865 2073 6571 7565 6e63 652e 2052 6574  he sequence. Ret
-0000f250: 7572 6e73 2030 2069 6620 7468 6520 7365  urns 0 if the se
-0000f260: 7175 656e 6365 2063 6f6e 7461 696e 7320  quence contains 
-0000f270: 6665 7765 7220 7468 616e 2074 776f 2065  fewer than two e
-0000f280: 6c65 6d65 6e74 732e 0a0a 2020 2020 2020  lements...      
-0000f290: 2020 4e6f 7465 733a 0a20 2020 2020 2020    Notes:.       
-0000f2a0: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
-0000f2b0: 6f6e 2075 7365 7320 616e 2065 7870 6f6e  on uses an expon
-0000f2c0: 656e 7469 616c 2064 6563 6179 2074 6f20  ential decay to 
-0000f2d0: 7765 6967 6874 2072 6563 656e 7420 6f62  weight recent ob
-0000f2e0: 7365 7276 6174 696f 6e73 206d 6f72 6520  servations more 
-0000f2f0: 6865 6176 696c 7920 696e 2074 6865 2063  heavily in the c
-0000f300: 616c 6375 6c61 7469 6f6e 0a20 2020 2020  alculation.     
-0000f310: 2020 2020 2020 206f 6620 7468 6520 6d65         of the me
-0000f320: 616e 2061 6e64 2076 6172 6961 6e63 652c  an and variance,
-0000f330: 2077 6869 6368 206d 616b 6573 2069 7420   which makes it 
-0000f340: 7365 6e73 6974 6976 6520 746f 2072 6563  sensitive to rec
-0000f350: 656e 7420 6368 616e 6765 7320 696e 2074  ent changes in t
-0000f360: 6865 2073 6571 7565 6e63 652e 0a20 2020  he sequence..   
-0000f370: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000f380: 2020 6966 206c 656e 286e 756d 6572 6963    if len(numeric
-0000f390: 5f73 6571 7565 6e63 6529 203d 3d20 303a  _sequence) == 0:
-0000f3a0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000f3b0: 7365 2056 616c 7565 4572 726f 7228 2254  se ValueError("T
-0000f3c0: 6865 206e 756d 6572 6963 2073 6571 7565  he numeric seque
-0000f3d0: 6e63 6520 6361 6e6e 6f74 2062 6520 656d  nce cannot be em
-0000f3e0: 7074 792e 2229 0a20 2020 2020 2020 206e  pty.").        n
-0000f3f0: 203d 2030 0a20 2020 2020 2020 206d 6561   = 0.        mea
-0000f400: 6e20 3d20 302e 300a 2020 2020 2020 2020  n = 0.0.        
-0000f410: 4d32 203d 2030 2e30 0a20 2020 2020 2020  M2 = 0.0.       
-0000f420: 2077 6569 6768 7465 645f 6e20 3d20 302e   weighted_n = 0.
-0000f430: 3020 2023 2057 6569 6768 7465 6420 7361  0  # Weighted sa
-0000f440: 6d70 6c65 2063 6f75 6e74 0a0a 2020 2020  mple count..    
-0000f450: 2020 2020 666f 7220 7820 696e 206e 756d      for x in num
-0000f460: 6572 6963 5f73 6571 7565 6e63 653a 0a20  eric_sequence:. 
-0000f470: 2020 2020 2020 2020 2020 206e 202b 3d20             n += 
-0000f480: 310a 2020 2020 2020 2020 2020 2020 7765  1.            we
-0000f490: 6967 6874 203d 2064 6563 6179 5f66 6163  ight = decay_fac
-0000f4a0: 746f 7220 2a2a 2028 6c65 6e28 6e75 6d65  tor ** (len(nume
-0000f4b0: 7269 635f 7365 7175 656e 6365 2920 2d20  ric_sequence) - 
-0000f4c0: 6e29 2020 2320 436f 6d70 7574 6520 7765  n)  # Compute we
-0000f4d0: 6967 6874 2c20 6e65 7765 7220 6461 7461  ight, newer data
-0000f4e0: 2068 6173 2068 6967 6865 7220 7765 6967   has higher weig
-0000f4f0: 6874 0a20 2020 2020 2020 2020 2020 2064  ht.            d
-0000f500: 656c 7461 203d 2078 202d 206d 6561 6e0a  elta = x - mean.
-0000f510: 2020 2020 2020 2020 2020 2020 7765 6967              weig
-0000f520: 6874 6564 5f6e 202b 3d20 7765 6967 6874  hted_n += weight
-0000f530: 0a20 2020 2020 2020 2020 2020 206d 6561  .            mea
-0000f540: 6e20 2b3d 2028 6465 6c74 6120 2a20 7765  n += (delta * we
-0000f550: 6967 6874 2920 2f20 7765 6967 6874 6564  ight) / weighted
-0000f560: 5f6e 0a20 2020 2020 2020 2020 2020 2064  _n.            d
-0000f570: 656c 7461 3220 3d20 7820 2d20 6d65 616e  elta2 = x - mean
-0000f580: 0a20 2020 2020 2020 2020 2020 204d 3220  .            M2 
-0000f590: 2b3d 2064 656c 7461 202a 2064 656c 7461  += delta * delta
-0000f5a0: 3220 2a20 7765 6967 6874 0a0a 2020 2020  2 * weight..    
-0000f5b0: 2020 2020 6966 2077 6569 6768 7465 645f      if weighted_
-0000f5c0: 6e20 3c20 323a 0a20 2020 2020 2020 2020  n < 2:.         
-0000f5d0: 2020 2072 6574 7572 6e20 302e 3020 2023     return 0.0  #
-0000f5e0: 204e 6f74 2065 6e6f 7567 6820 7361 6d70   Not enough samp
-0000f5f0: 6c65 7320 746f 2063 6f6d 7075 7465 2073  les to compute s
-0000f600: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
-0000f610: 6e0a 2020 2020 2020 2020 7661 7269 616e  n.        varian
-0000f620: 6365 203d 204d 3220 2f20 7765 6967 6874  ce = M2 / weight
-0000f630: 6564 5f6e 2020 2320 436f 6d70 7574 6520  ed_n  # Compute 
-0000f640: 7661 7269 616e 6365 2075 7369 6e67 2077  variance using w
-0000f650: 6569 6768 7465 6420 7361 6d70 6c65 2063  eighted sample c
-0000f660: 6f75 6e74 0a20 2020 2020 2020 2072 6574  ount.        ret
-0000f670: 7572 6e20 6d61 7468 2e73 7172 7428 7661  urn math.sqrt(va
-0000f680: 7269 616e 6365 290a 0a20 2020 2040 7374  riance)..    @st
-0000f690: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-0000f6a0: 6566 2063 616c 6375 6c61 7465 5f73 7461  ef calculate_sta
-0000f6b0: 6e64 6172 645f 6465 7669 6174 696f 6e28  ndard_deviation(
-0000f6c0: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
-0000f6d0: 3a20 4c69 7374 5b55 6e69 6f6e 5b69 6e74  : List[Union[int
-0000f6e0: 2c20 666c 6f61 745d 5d29 202d 3e20 556e  , float]]) -> Un
-0000f6f0: 696f 6e5b 696e 742c 2066 6c6f 6174 5d3a  ion[int, float]:
-0000f700: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f710: 2020 2020 2043 616c 6375 6c61 7465 7320       Calculates 
-0000f720: 7468 6520 7374 616e 6461 7264 2064 6576  the standard dev
-0000f730: 6961 7469 6f6e 206f 6620 6120 6e75 6d65  iation of a nume
-0000f740: 7269 6320 7365 7175 656e 6365 2e0a 0a20  ric sequence... 
-0000f750: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-0000f760: 6f64 2063 6f6d 7075 7465 7320 7468 6520  od computes the 
-0000f770: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-0000f780: 6f6e 2062 7920 6669 7273 7420 6361 6c63  on by first calc
-0000f790: 756c 6174 696e 6720 7468 6520 6d65 616e  ulating the mean
-0000f7a0: 206f 6620 7468 6520 6e75 6d62 6572 732c   of the numbers,
-0000f7b0: 0a20 2020 2020 2020 2074 6865 6e20 7468  .        then th
-0000f7c0: 6520 7661 7269 616e 6365 2061 7320 7468  e variance as th
-0000f7d0: 6520 6176 6572 6167 6520 6f66 2074 6865  e average of the
-0000f7e0: 2073 7175 6172 6564 2064 6966 6665 7265   squared differe
-0000f7f0: 6e63 6573 2066 726f 6d20 7468 6520 6d65  nces from the me
-0000f800: 616e 2c20 616e 6420 6669 6e61 6c6c 790a  an, and finally.
-0000f810: 2020 2020 2020 2020 7461 6b69 6e67 2074          taking t
-0000f820: 6865 2073 7175 6172 6520 726f 6f74 206f  he square root o
-0000f830: 6620 7468 6520 7661 7269 616e 6365 2e0a  f the variance..
-0000f840: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000f850: 2020 2020 2020 2020 2020 206e 756d 6572             numer
-0000f860: 6963 5f73 6571 7565 6e63 6520 284c 6973  ic_sequence (Lis
-0000f870: 745b 556e 696f 6e5b 696e 742c 2066 6c6f  t[Union[int, flo
-0000f880: 6174 5d5d 293a 2054 6865 2073 6571 7565  at]]): The seque
-0000f890: 6e63 6520 6f66 206e 756d 6265 7273 2028  nce of numbers (
-0000f8a0: 696e 7465 6765 7273 206f 7220 666c 6f61  integers or floa
-0000f8b0: 7473 2920 666f 7220 7768 6963 6820 7468  ts) for which th
-0000f8c0: 6520 7374 616e 6461 7264 2064 6576 6961  e standard devia
-0000f8d0: 7469 6f6e 2069 7320 746f 2062 6520 6361  tion is to be ca
-0000f8e0: 6c63 756c 6174 6564 2e0a 0a20 2020 2020  lculated...     
-0000f8f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000f900: 2020 2020 2020 2020 666c 6f61 743a 2054          float: T
-0000f910: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
-0000f920: 6174 696f 6e20 6f66 2074 6865 2073 6571  ation of the seq
-0000f930: 7565 6e63 652e 0a0a 2020 2020 2020 2020  uence...        
-0000f940: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-0000f950: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-0000f960: 4966 2074 6865 206e 756d 6572 6963 5f73  If the numeric_s
-0000f970: 6571 7565 6e63 6520 6973 2065 6d70 7479  equence is empty
-0000f980: 2c20 6173 2073 7461 6e64 6172 6420 6465  , as standard de
-0000f990: 7669 6174 696f 6e20 6361 6e6e 6f74 2062  viation cannot b
-0000f9a0: 6520 6361 6c63 756c 6174 6564 2e0a 2020  e calculated..  
-0000f9b0: 2020 2020 2020 4e6f 7465 733a 0a20 2020        Notes:.   
-0000f9c0: 2020 2020 2020 2020 2054 6869 7320 6675           This fu
-0000f9d0: 6e63 7469 6f6e 2075 7365 7320 616e 2065  nction uses an e
-0000f9e0: 7870 6f6e 656e 7469 616c 2064 6563 6179  xponential decay
-0000f9f0: 2074 6f20 7765 6967 6874 2072 6563 656e   to weight recen
-0000fa00: 7420 6f62 7365 7276 6174 696f 6e73 206d  t observations m
-0000fa10: 6f72 6520 6865 6176 696c 7920 696e 2074  ore heavily in t
-0000fa20: 6865 2063 616c 6375 6c61 7469 6f6e 0a20  he calculation. 
-0000fa30: 2020 2020 2020 2020 2020 206f 6620 7468             of th
-0000fa40: 6520 6d65 616e 2061 6e64 2076 6172 6961  e mean and varia
-0000fa50: 6e63 652c 2077 6869 6368 206d 616b 6573  nce, which makes
-0000fa60: 2069 7420 7365 6e73 6974 6976 6520 746f   it sensitive to
-0000fa70: 2072 6563 656e 7420 6368 616e 6765 7320   recent changes 
-0000fa80: 696e 2074 6865 2073 6571 7565 6e63 652e  in the sequence.
-0000fa90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000faa0: 2020 2020 2069 6620 6c65 6e28 6e75 6d65       if len(nume
-0000fab0: 7269 635f 7365 7175 656e 6365 2920 3d3d  ric_sequence) ==
-0000fac0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-0000fad0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000fae0: 2822 5468 6520 6e75 6d65 7269 6320 7365  ("The numeric se
-0000faf0: 7175 656e 6365 2063 616e 6e6f 7420 6265  quence cannot be
-0000fb00: 2065 6d70 7479 2e22 290a 0a20 2020 2020   empty.")..     
-0000fb10: 2020 2023 2043 616c 6375 6c61 7465 2074     # Calculate t
-0000fb20: 6865 206d 6561 6e20 6f66 2074 6865 2073  he mean of the s
-0000fb30: 6571 7565 6e63 650a 2020 2020 2020 2020  equence.        
-0000fb40: 6d65 616e 203d 2073 756d 286e 756d 6572  mean = sum(numer
-0000fb50: 6963 5f73 6571 7565 6e63 6529 202f 206c  ic_sequence) / l
-0000fb60: 656e 286e 756d 6572 6963 5f73 6571 7565  en(numeric_seque
-0000fb70: 6e63 6529 0a0a 2020 2020 2020 2020 2320  nce)..        # 
-0000fb80: 4361 6c63 756c 6174 6520 7468 6520 7371  Calculate the sq
-0000fb90: 7561 7265 6420 6469 6666 6572 656e 6365  uared difference
-0000fba0: 7320 6672 6f6d 2074 6865 206d 6561 6e0a  s from the mean.
-0000fbb0: 2020 2020 2020 2020 7371 7561 7265 645f          squared_
-0000fbc0: 6469 6666 7320 3d20 5b28 7820 2d20 6d65  diffs = [(x - me
-0000fbd0: 616e 2920 2a2a 2032 2066 6f72 2078 2069  an) ** 2 for x i
-0000fbe0: 6e20 6e75 6d65 7269 635f 7365 7175 656e  n numeric_sequen
-0000fbf0: 6365 5d0a 0a20 2020 2020 2020 2023 2043  ce]..        # C
-0000fc00: 616c 6375 6c61 7465 2074 6865 2076 6172  alculate the var
-0000fc10: 6961 6e63 650a 2020 2020 2020 2020 7661  iance.        va
-0000fc20: 7269 616e 6365 203d 2073 756d 2873 7175  riance = sum(squ
-0000fc30: 6172 6564 5f64 6966 6673 2920 2f20 6c65  ared_diffs) / le
-0000fc40: 6e28 6e75 6d65 7269 635f 7365 7175 656e  n(numeric_sequen
-0000fc50: 6365 290a 0a20 2020 2020 2020 2023 2043  ce)..        # C
-0000fc60: 616c 6375 6c61 7465 2061 6e64 2072 6574  alculate and ret
-0000fc70: 7572 6e20 7468 6520 7374 616e 6461 7264  urn the standard
-0000fc80: 2064 6576 6961 7469 6f6e 0a20 2020 2020   deviation.     
-0000fc90: 2020 2073 7461 6e64 6172 645f 6465 7669     standard_devi
-0000fca0: 6174 696f 6e20 3d20 6d61 7468 2e73 7172  ation = math.sqr
-0000fcb0: 7428 7661 7269 616e 6365 290a 2020 2020  t(variance).    
-0000fcc0: 2020 2020 7265 7475 726e 2073 7461 6e64      return stand
-0000fcd0: 6172 645f 6465 7669 6174 696f 6e0a 0a20  ard_deviation.. 
-0000fce0: 2020 2040 6162 7374 7261 6374 6d65 7468     @abstractmeth
-0000fcf0: 6f64 0a20 2020 2064 6566 2063 616c 6375  od.    def calcu
-0000fd00: 6c61 7465 5f77 696e 6e69 6e67 5f61 6d6f  late_winning_amo
-0000fd10: 756e 7428 0a20 2020 2020 2020 2020 2020  unt(.           
-0000fd20: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-0000fd30: 2020 2077 696e 6e69 6e67 5f6e 756d 6265     winning_numbe
-0000fd40: 725f 636f 6d62 696e 6174 696f 6e3a 204c  r_combination: L
-0000fd50: 6973 745b 696e 745d 2c0a 2020 2020 2020  ist[int],.      
-0000fd60: 2020 2020 2020 7075 7263 6861 7365 5f6e        purchase_n
-0000fd70: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
-0000fd80: 6e73 3a20 4c69 7374 5b4c 6973 745b 696e  ns: List[List[in
-0000fd90: 745d 5d2c 0a20 2020 2020 2020 2020 2020  t]],.           
-0000fda0: 202a 2a6b 7761 7267 733a 2041 6e79 0a20   **kwargs: Any. 
-0000fdb0: 2020 2029 202d 3e20 5475 706c 655b 666c     ) -> Tuple[fl
-0000fdc0: 6f61 742c 2069 6e74 5d3a 0a20 2020 2020  oat, int]:.     
-0000fdd0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0000fde0: 616c 6375 6c61 7465 2074 6865 2077 696e  alculate the win
-0000fdf0: 6e69 6e67 2061 6d6f 756e 7420 6261 7365  ning amount base
-0000fe00: 6420 6f6e 206d 6174 6368 696e 6720 636f  d on matching co
-0000fe10: 6d62 696e 6174 696f 6e73 2e0a 0a20 2020  mbinations...   
-0000fe20: 2020 2020 203a 7061 7261 6d20 7769 6e6e       :param winn
-0000fe30: 696e 675f 6e75 6d62 6572 5f63 6f6d 6269  ing_number_combi
-0000fe40: 6e61 7469 6f6e 3a20 5769 6e6e 696e 6720  nation: Winning 
-0000fe50: 6e75 6d62 6572 2063 6f6d 6269 6e61 7469  number combinati
-0000fe60: 6f6e 2e0a 2020 2020 2020 2020 3a70 6172  on..        :par
-0000fe70: 616d 2070 7572 6368 6173 655f 6e75 6d62  am purchase_numb
-0000fe80: 6572 5f63 6f6d 6269 6e61 7469 6f6e 733a  er_combinations:
-0000fe90: 2050 7572 6368 6173 6520 6e75 6d62 6572   Purchase number
-0000fea0: 2063 6f6d 6269 6e61 7469 6f6e 732e 0a20   combinations.. 
-0000feb0: 2020 2020 2020 203a 7061 7261 6d20 6b77         :param kw
-0000fec0: 6172 6773 3a20 4164 6469 7469 6f6e 616c  args: Additional
-0000fed0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-0000fee0: 7473 2e0a 2020 2020 2020 2020 3a72 6574  ts..        :ret
-0000fef0: 7572 6e3a 2054 6865 2074 6f74 616c 2077  urn: The total w
-0000ff00: 696e 6e69 6e67 2061 6d6f 756e 7420 616e  inning amount an
-0000ff10: 6420 7468 6520 636f 756e 7420 6f66 2077  d the count of w
-0000ff20: 696e 6e69 6e67 2063 6f6d 6269 6e61 7469  inning combinati
-0000ff30: 6f6e 730a 2020 2020 2020 2020 2222 220a  ons.        """.
-0000ff40: 2020 2020 2020 2020 7061 7373 0a0a 0a63          pass...c
-0000ff50: 6c61 7373 2041 6e61 6c79 7a65 5574 696c  lass AnalyzeUtil
-0000ff60: 2841 4243 293a 0a20 2020 2022 2222 0a20  (ABC):.    """. 
-0000ff70: 2020 2041 6e61 6c79 7a65 2062 6173 6564     Analyze based
-0000ff80: 206f 6e20 6d75 6c74 6970 6c65 2064 6174   on multiple dat
-0000ff90: 610a 2020 2020 2222 220a 0a20 2020 2040  a.    """..    @
-0000ffa0: 6162 7374 7261 6374 6d65 7468 6f64 0a20  abstractmethod. 
-0000ffb0: 2020 2064 6566 2061 6e61 6c79 7a65 5f73     def analyze_s
-0000ffc0: 616d 655f 7065 7269 6f64 5f6e 756d 6265  ame_period_numbe
-0000ffd0: 7273 2873 656c 662c 202a 2a6b 7761 7267  rs(self, **kwarg
-0000ffe0: 733a 2041 6e79 2920 2d3e 204e 6f6e 653a  s: Any) -> None:
-0000fff0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010000: 2020 2020 2041 6e61 6c79 7a65 2073 616d       Analyze sam
-00010010: 6520 7065 7269 6f64 206e 756d 6265 7220  e period number 
-00010020: 696e 2074 6865 206c 6173 7420 7065 7269  in the last peri
-00010030: 6f64 2e0a 2020 2020 2020 2020 2222 220a  od..        """.
-00010040: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00010050: 2020 4061 6273 7472 6163 746d 6574 686f    @abstractmetho
-00010060: 640a 2020 2020 6465 6620 616e 616c 797a  d.    def analyz
-00010070: 655f 7361 6d65 5f77 6565 6b64 6179 5f6e  e_same_weekday_n
-00010080: 756d 6265 7273 2873 656c 662c 202a 2a6b  umbers(self, **k
-00010090: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
-000100a0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000100b0: 0a20 2020 2020 2020 2041 6e61 6c79 7a65  .        Analyze
-000100c0: 2073 616d 6520 7765 656b 6461 7920 6e75   same weekday nu
-000100d0: 6d62 6572 2069 6e20 7468 6520 6c61 7374  mber in the last
-000100e0: 2070 6572 696f 642e 0a20 2020 2020 2020   period..       
-000100f0: 2022 2222 0a20 2020 2020 2020 2070 6173   """.        pas
-00010100: 730a 0a20 2020 2040 6162 7374 7261 6374  s..    @abstract
-00010110: 6d65 7468 6f64 0a20 2020 2064 6566 2061  method.    def a
-00010120: 6e61 6c79 7a65 5f72 6570 6561 7465 645f  nalyze_repeated_
-00010130: 6e75 6d62 6572 7328 7365 6c66 2c20 2a2a  numbers(self, **
-00010140: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
-00010150: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00010160: 220a 2020 2020 2020 2020 416e 616c 797a  ".        Analyz
-00010170: 6520 7468 6520 6e75 6d62 6572 2074 6861  e the number tha
-00010180: 7420 6170 7065 6172 6564 2074 7769 6365  t appeared twice
-00010190: 2069 6e20 7468 6520 6c61 7374 2074 776f   in the last two
-000101a0: 2070 6572 696f 642e 0a20 2020 2020 2020   period..       
-000101b0: 2022 2222 0a20 2020 2020 2020 2070 6173   """.        pas
-000101c0: 730a 0a20 2020 2040 6162 7374 7261 6374  s..    @abstract
-000101d0: 6d65 7468 6f64 0a20 2020 2064 6566 2061  method.    def a
-000101e0: 6e61 6c79 7a65 5f65 6467 655f 6e75 6d62  nalyze_edge_numb
-000101f0: 6572 7328 7365 6c66 2c20 2a2a 6b77 6172  ers(self, **kwar
-00010200: 6773 3a20 416e 7929 202d 3e20 4e6f 6e65  gs: Any) -> None
-00010210: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010220: 2020 2020 2020 416e 616c 797a 6520 416c        Analyze Al
-00010230: 736f 2063 616c 6c65 6420 6164 6a61 6365  so called adjace
-00010240: 6e74 206e 756d 6265 722c 2070 6c75 7320  nt number, plus 
-00010250: 6f72 206d 696e 7573 2031 2077 6974 6820  or minus 1 with 
-00010260: 7468 6520 7769 6e6e 696e 6720 6e75 6d62  the winning numb
-00010270: 6572 2069 7373 7565 6420 696e 2074 6865  er issued in the
-00010280: 2070 7265 7669 6f75 7320 7065 7269 6f64   previous period
-00010290: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000102a0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-000102b0: 6162 7374 7261 6374 6d65 7468 6f64 0a20  abstractmethod. 
-000102c0: 2020 2064 6566 2061 6e61 6c79 7a65 5f63     def analyze_c
-000102d0: 6f6c 645f 686f 745f 6e75 6d62 6572 7328  old_hot_numbers(
-000102e0: 7365 6c66 2c20 2a2a 6b77 6172 6773 3a20  self, **kwargs: 
-000102f0: 416e 7929 202d 3e20 4e6f 6e65 3a0a 2020  Any) -> None:.  
-00010300: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010310: 2020 416e 616c 797a 6520 4e75 6d62 6572    Analyze Number
-00010320: 7320 7468 6174 2068 6176 6520 6170 7065  s that have appe
-00010330: 6172 6564 2069 6e20 7468 6520 6c61 7374  ared in the last
-00010340: 2070 6572 696f 640a 2020 2020 2020 2020   period.        
-00010350: 416e 616c 797a 6520 4e75 6d62 6572 7320  Analyze Numbers 
-00010360: 7468 6174 2068 6176 6520 6e6f 7420 6170  that have not ap
-00010370: 7065 6172 6564 2069 6e20 7468 6520 6c61  peared in the la
-00010380: 7374 2070 6572 696f 640a 2020 2020 2020  st period.      
-00010390: 2020 2222 220a 2020 2020 2020 2020 7061    """.        pa
-000103a0: 7373 0a0a 2020 2020 4061 6273 7472 6163  ss..    @abstrac
-000103b0: 746d 6574 686f 640a 2020 2020 6465 6620  tmethod.    def 
-000103c0: 616e 616c 797a 655f 6f6d 6974 7465 645f  analyze_omitted_
-000103d0: 6e75 6d62 6572 7328 7365 6c66 2c20 2a2a  numbers(self, **
-000103e0: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
-000103f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00010400: 220a 2020 2020 2020 2020 416e 616c 797a  ".        Analyz
-00010410: 652e 0a20 2020 2020 2020 204f 6d69 7373  e..        Omiss
-00010420: 696f 6e3a 2054 6865 206e 756d 6265 7220  ion: The number 
-00010430: 6f66 2070 6572 696f 6473 2073 696e 6365  of periods since
-00010440: 2074 6865 2070 7265 7669 6f75 7320 6f70   the previous op
-00010450: 656e 696e 6720 746f 2074 6865 2063 7572  ening to the cur
-00010460: 7265 6e74 2070 6572 696f 642e 0a20 2020  rent period..   
-00010470: 2020 2020 2041 7665 7261 6765 206f 6d69       Average omi
-00010480: 7373 696f 6e3a 2054 6865 2061 7665 7261  ssion: The avera
-00010490: 6765 206e 756d 6265 7220 6f66 206f 6d69  ge number of omi
-000104a0: 7373 696f 6e73 2069 6e20 7468 6520 7374  ssions in the st
-000104b0: 6174 6973 7469 6361 6c20 7065 7269 6f64  atistical period
-000104c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000104d0: 2020 2020 2020 2020 2020 2028 6361 6c63             (calc
-000104e0: 756c 6174 696f 6e20 666f 726d 756c 613a  ulation formula:
-000104f0: 2041 7665 7261 6765 206f 6d69 7373 696f   Average omissio
-00010500: 6e20 3d0a 2020 2020 2020 2020 2020 2020  n =.            
-00010510: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00010520: 7461 6c20 6e75 6d62 6572 206f 6620 6f6d  tal number of om
-00010530: 6973 7369 6f6e 7320 696e 2074 6865 2073  issions in the s
-00010540: 7461 7469 7374 6963 616c 2070 6572 696f  tatistical perio
-00010550: 6420 2f20 286e 756d 6265 7220 6f66 206f  d / (number of o
-00010560: 6363 7572 7265 6e63 6573 202b 3129 290a  ccurrences +1)).
-00010570: 2020 2020 2020 2020 4d61 7869 6d75 6d20          Maximum 
-00010580: 6d69 7373 6564 2076 616c 7565 3a20 496e  missed value: In
-00010590: 6469 6361 7465 7320 7468 6520 6d61 7869  dicates the maxi
-000105a0: 6d75 6d20 7661 6c75 6520 6f66 2061 6c6c  mum value of all
-000105b0: 206d 6973 7365 6420 7661 6c75 6573 2069   missed values i
-000105c0: 6e20 7468 6520 7374 6174 6973 7469 6361  n the statistica
-000105d0: 6c20 7065 7269 6f64 2e0a 2020 2020 2020  l period..      
-000105e0: 2020 4375 7272 656e 7420 6f6d 6973 7369    Current omissi
-000105f0: 6f6e 3a20 5468 6520 6e75 6d62 6572 206f  on: The number o
-00010600: 6620 7065 7269 6f64 7320 6265 7477 6565  f periods betwee
-00010610: 6e20 7468 6520 6c61 7374 206f 6363 7572  n the last occur
-00010620: 7265 6e63 6520 616e 6420 7468 6520 7072  rence and the pr
-00010630: 6573 656e 742c 2069 6620 7468 6520 6d69  esent, if the mi
-00010640: 7373 696e 6720 6f62 6a65 6374 0a20 2020  ssing object.   
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2020 2020 2020 2061 7070 6561 7265 6420         appeared 
-00010670: 696e 2074 6865 2063 7572 7265 6e74 2070  in the current p
-00010680: 6572 696f 642c 2074 6865 2063 7572 7265  eriod, the curre
-00010690: 6e74 206f 6d69 7373 696f 6e20 7661 6c75  nt omission valu
-000106a0: 6520 6973 2030 0a20 2020 2020 2020 2050  e is 0.        P
-000106b0: 7265 7669 6f75 7320 7065 7269 6f64 206f  revious period o
-000106c0: 6d69 7373 696f 6e3a 2054 6865 2069 6e74  mission: The int
-000106d0: 6572 7661 6c20 6265 7477 6565 6e20 7468  erval between th
-000106e0: 6520 6c61 7374 2074 776f 2070 6572 696f  e last two perio
-000106f0: 6473 2028 6578 636c 7564 696e 6720 7468  ds (excluding th
-00010700: 6520 6375 7272 656e 7420 7065 7269 6f64  e current period
-00010710: 290a 2020 2020 2020 2020 5468 656f 7265  ).        Theore
-00010720: 7469 6361 6c20 6e75 6d62 6572 3a20 5468  tical number: Th
-00010730: 6520 7468 656f 7265 7469 6361 6c20 6e75  e theoretical nu
-00010740: 6d62 6572 2072 6566 6572 7320 746f 2074  mber refers to t
-00010750: 6865 206e 756d 6265 7220 6f66 2074 696d  he number of tim
-00010760: 6573 2074 6865 206d 6973 7369 6e67 206f  es the missing o
-00010770: 626a 6563 7420 7368 6f75 6c64 0a20 2020  bject should.   
-00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010790: 2020 2020 2020 2020 2074 6865 6f72 6574           theoret
-000107a0: 6963 616c 6c79 2061 7070 6561 722c 203d  ically appear, =
-000107b0: 2074 6865 2074 6f74 616c 206e 756d 6265   the total numbe
-000107c0: 7220 6f66 2074 2074 696d 6573 202a 2074  r of t times * t
-000107d0: 6865 6f72 6574 6963 616c 2070 726f 6261  heoretical proba
-000107e0: 6269 6c69 7479 0a20 2020 2020 2020 2044  bility.        D
-000107f0: 6573 6972 6564 2070 726f 6261 6269 6c69  esired probabili
-00010800: 7479 3a20 4465 7369 7265 6420 7072 6f62  ty: Desired prob
-00010810: 6162 696c 6974 7920 7265 666c 6563 7473  ability reflects
-00010820: 2074 6865 2069 6465 616c 206f 6363 7572   the ideal occur
-00010830: 7265 6e63 6520 7072 6f62 6162 696c 6974  rence probabilit
-00010840: 7920 6f66 2074 6865 206d 6973 7369 6e67  y of the missing
-00010850: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2020 2020 2020 5468 6520 666f 726d 756c        The formul
-00010880: 6120 6973 2028 6375 7272 656e 7420 6f6d  a is (current om
-00010890: 6973 7369 6f6e 2f61 7665 7261 6765 206f  ission/average o
-000108a0: 6d69 7373 696f 6e20 2a20 7468 656f 7265  mission * theore
-000108b0: 7469 6361 6c20 7072 6f62 6162 696c 6974  tical probabilit
-000108c0: 7929 0a20 2020 2020 2020 2022 2222 0a20  y).        """. 
-000108d0: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
-000108e0: 6173 7320 4765 6e65 7469 6373 5574 696c  ass GeneticsUtil
-000108f0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00010900: 5f5f 2873 656c 662c 2072 6566 6572 733a  __(self, refers:
-00010910: 206c 6973 742c 2064 6174 613a 206c 6973   list, data: lis
-00010920: 742c 206d 696e 5f6e 756d 3a20 696e 742c  t, min_num: int,
-00010930: 206d 6178 5f6e 756d 3a20 696e 742c 2066   max_num: int, f
-00010940: 6974 6e65 7373 5f70 6172 616d 733a 2064  itness_params: d
-00010950: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
-00010960: 2020 2020 2020 706f 7075 6c61 7469 6f6e        population
-00010970: 5f73 697a 653a 2069 6e74 203d 2031 3030  _size: int = 100
-00010980: 2c20 6e75 6d5f 6765 6e65 733a 2069 6e74  , num_genes: int
-00010990: 203d 2035 2c20 746f 7572 6e61 6d65 6e74   = 5, tournament
-000109a0: 5f73 697a 653a 2069 6e74 203d 2033 2c0a  _size: int = 3,.
-000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109c0: 206d 7574 6174 696f 6e5f 7261 7465 3a20   mutation_rate: 
-000109d0: 666c 6f61 7420 3d20 302e 312c 2065 706f  float = 0.1, epo
-000109e0: 6368 5f63 6f75 6e74 3a20 696e 7420 3d20  ch_count: int = 
-000109f0: 3130 3029 3a0a 2020 2020 2020 2020 2222  100):.        ""
-00010a00: 220a 2020 2020 2020 2020 496e 6974 6961  ".        Initia
-00010a10: 6c69 7a65 7320 7468 6520 4765 6e65 7469  lizes the Geneti
-00010a20: 6373 5574 696c 2063 6c61 7373 2077 6974  csUtil class wit
-00010a30: 6820 7468 6520 6e65 6365 7373 6172 7920  h the necessary 
-00010a40: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
-00010a50: 6865 2067 656e 6574 6963 2061 6c67 6f72  he genetic algor
-00010a60: 6974 686d 2e0a 0a20 2020 2020 2020 2041  ithm...        A
-00010a70: 7267 733a 0a20 2020 2020 2020 2072 6566  rgs:.        ref
-00010a80: 6572 7320 286c 6973 7429 3a20 5265 6665  ers (list): Refe
-00010a90: 7265 6e63 6520 6d61 7472 6978 206f 7220  rence matrix or 
-00010aa0: 6461 7461 2075 7365 6420 666f 7220 6372  data used for cr
-00010ab0: 6561 7469 6e67 2074 6865 2072 6566 6572  eating the refer
-00010ac0: 656e 6365 206d 6174 7269 782e 0a20 2020  ence matrix..   
-00010ad0: 2020 2020 2064 6174 6120 286c 6973 7429       data (list)
-00010ae0: 3a20 4461 7461 7365 7420 6672 6f6d 2077  : Dataset from w
-00010af0: 6869 6368 2067 656e 6573 2061 7265 2073  hich genes are s
-00010b00: 656c 6563 7465 642e 0a20 2020 2020 2020  elected..       
-00010b10: 206d 696e 5f6e 756d 2028 696e 7429 3a20   min_num (int): 
-00010b20: 4d69 6e69 6d75 6d20 616c 6c6f 7761 626c  Minimum allowabl
-00010b30: 6520 7661 6c75 6520 666f 7220 6120 6765  e value for a ge
-00010b40: 6e65 2e0a 2020 2020 2020 2020 6d61 785f  ne..        max_
-00010b50: 6e75 6d20 2869 6e74 293a 204d 6178 696d  num (int): Maxim
-00010b60: 756d 2061 6c6c 6f77 6162 6c65 2076 616c  um allowable val
-00010b70: 7565 2066 6f72 2061 2067 656e 652e 0a20  ue for a gene.. 
-00010b80: 2020 2020 2020 2066 6974 6e65 7373 5f70         fitness_p
-00010b90: 6172 616d 7320 2864 6963 7429 3a20 5061  arams (dict): Pa
-00010ba0: 7261 6d65 7465 7273 2075 7365 6420 666f  rameters used fo
-00010bb0: 7220 6361 6c63 756c 6174 696e 6720 6669  r calculating fi
-00010bc0: 746e 6573 732e 0a20 2020 2020 2020 2070  tness..        p
-00010bd0: 6f70 756c 6174 696f 6e5f 7369 7a65 2028  opulation_size (
-00010be0: 696e 7429 3a20 4e75 6d62 6572 206f 6620  int): Number of 
-00010bf0: 696e 6469 7669 6475 616c 7320 696e 2074  individuals in t
-00010c00: 6865 2070 6f70 756c 6174 696f 6e2e 0a20  he population.. 
-00010c10: 2020 2020 2020 206e 756d 5f67 656e 6573         num_genes
-00010c20: 2028 696e 7429 3a20 4e75 6d62 6572 206f   (int): Number o
-00010c30: 6620 6765 6e65 7320 696e 2065 6163 6820  f genes in each 
-00010c40: 696e 6469 7669 6475 616c 2e0a 2020 2020  individual..    
-00010c50: 2020 2020 746f 7572 6e61 6d65 6e74 5f73      tournament_s
-00010c60: 697a 6520 2869 6e74 293a 2053 697a 6520  ize (int): Size 
-00010c70: 6f66 2074 6865 2074 6f75 726e 616d 656e  of the tournamen
-00010c80: 7420 666f 7220 7365 6c65 6374 696f 6e20  t for selection 
-00010c90: 7072 6f63 6573 732e 0a20 2020 2020 2020  process..       
-00010ca0: 206d 7574 6174 696f 6e5f 7261 7465 2028   mutation_rate (
-00010cb0: 666c 6f61 7429 3a20 5072 6f62 6162 696c  float): Probabil
-00010cc0: 6974 7920 6f66 206d 7574 6174 696f 6e20  ity of mutation 
-00010cd0: 7065 7220 6765 6e65 2e0a 2020 2020 2020  per gene..      
-00010ce0: 2020 6570 6f63 685f 636f 756e 7420 2869    epoch_count (i
-00010cf0: 6e74 293a 204e 756d 6265 7220 6f66 2067  nt): Number of g
-00010d00: 656e 6572 6174 696f 6e73 206f 7220 6570  enerations or ep
-00010d10: 6f63 6873 2074 6865 2061 6c67 6f72 6974  ochs the algorit
-00010d20: 686d 2077 696c 6c20 7275 6e2e 0a20 2020  hm will run..   
-00010d30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00010d40: 2073 656c 662e 7265 6665 7273 203d 2072   self.refers = r
-00010d50: 6566 6572 730a 2020 2020 2020 2020 7365  efers.        se
-00010d60: 6c66 2e64 6174 6120 3d20 6461 7461 0a20  lf.data = data. 
-00010d70: 2020 2020 2020 2073 656c 662e 6d69 6e5f         self.min_
-00010d80: 6e75 6d20 3d20 6d69 6e5f 6e75 6d0a 2020  num = min_num.  
-00010d90: 2020 2020 2020 7365 6c66 2e6d 6178 5f6e        self.max_n
-00010da0: 756d 203d 206d 6178 5f6e 756d 0a20 2020  um = max_num.   
-00010db0: 2020 2020 2073 656c 662e 6669 746e 6573       self.fitnes
-00010dc0: 735f 7061 7261 6d73 203d 2066 6974 6e65  s_params = fitne
-00010dd0: 7373 5f70 6172 616d 730a 2020 2020 2020  ss_params.      
-00010de0: 2020 7365 6c66 2e70 6f70 756c 6174 696f    self.populatio
-00010df0: 6e5f 7369 7a65 203d 2070 6f70 756c 6174  n_size = populat
-00010e00: 696f 6e5f 7369 7a65 0a20 2020 2020 2020  ion_size.       
-00010e10: 2073 656c 662e 6e75 6d5f 6765 6e65 7320   self.num_genes 
-00010e20: 3d20 6e75 6d5f 6765 6e65 730a 2020 2020  = num_genes.    
-00010e30: 2020 2020 7365 6c66 2e74 6f75 726e 616d      self.tournam
-00010e40: 656e 745f 7369 7a65 203d 2074 6f75 726e  ent_size = tourn
-00010e50: 616d 656e 745f 7369 7a65 0a20 2020 2020  ament_size.     
-00010e60: 2020 2073 656c 662e 6d75 7461 7469 6f6e     self.mutation
-00010e70: 5f72 6174 6520 3d20 6d75 7461 7469 6f6e  _rate = mutation
-00010e80: 5f72 6174 650a 2020 2020 2020 2020 7365  _rate.        se
-00010e90: 6c66 2e65 706f 6368 5f63 6f75 6e74 203d  lf.epoch_count =
-00010ea0: 2065 706f 6368 5f63 6f75 6e74 0a20 2020   epoch_count.   
-00010eb0: 2020 2020 2073 656c 662e 706f 7075 6c61       self.popula
-00010ec0: 7469 6f6e 203d 2073 656c 662e 696e 6974  tion = self.init
-00010ed0: 5f70 6f70 756c 6174 696f 6e28 2920 2023  _population()  #
-00010ee0: 2049 6e69 7469 616c 697a 6573 2074 6865   Initializes the
-00010ef0: 2070 6f70 756c 6174 696f 6e0a 2020 2020   population.    
-00010f00: 2020 2020 7365 6c66 2e72 6566 6572 735f      self.refers_
-00010f10: 6d61 7472 6978 203d 2073 656c 662e 6372  matrix = self.cr
-00010f20: 6561 7465 5f72 6566 6572 735f 6d61 7472  eate_refers_matr
-00010f30: 6978 2829 2020 2320 4372 6561 7465 7320  ix()  # Creates 
-00010f40: 6120 6d61 7472 6978 2066 726f 6d20 7265  a matrix from re
-00010f50: 6665 7265 6e63 6520 6461 7461 0a0a 2020  ference data..  
-00010f60: 2020 6465 6620 696e 6974 5f70 6f70 756c    def init_popul
-00010f70: 6174 696f 6e28 7365 6c66 2920 2d3e 206c  ation(self) -> l
-00010f80: 6973 743a 0a20 2020 2020 2020 2022 2222  ist:.        """
-00010f90: 0a20 2020 2020 2020 2049 6e69 7469 616c  .        Initial
-00010fa0: 697a 6573 2074 6865 2070 6f70 756c 6174  izes the populat
-00010fb0: 696f 6e20 7769 7468 2072 616e 646f 6d6c  ion with randoml
-00010fc0: 7920 7365 6c65 6374 6564 2c20 6e6f 6e2d  y selected, non-
-00010fd0: 7265 7065 6174 696e 6720 6765 6e65 7320  repeating genes 
-00010fe0: 6672 6f6d 2074 6865 2064 6174 6120 7365  from the data se
-00010ff0: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
-00011000: 726e 733a 0a20 2020 2020 2020 206c 6973  rns:.        lis
-00011010: 743a 2041 206c 6973 7420 6f66 2069 6e64  t: A list of ind
-00011020: 6976 6964 7561 6c73 2c20 6561 6368 2072  ividuals, each r
-00011030: 6570 7265 7365 6e74 6564 2061 7320 6120  epresented as a 
-00011040: 736f 7274 6564 206c 6973 7420 6f66 2067  sorted list of g
-00011050: 656e 6573 2e0a 2020 2020 2020 2020 2222  enes..        ""
-00011060: 220a 2020 2020 2020 2020 706f 7075 6c61  ".        popula
-00011070: 7469 6f6e 203d 205b 6e70 2e72 616e 646f  tion = [np.rando
-00011080: 6d2e 6368 6f69 6365 2873 656c 662e 6461  m.choice(self.da
-00011090: 7461 2c20 7365 6c66 2e6e 756d 5f67 656e  ta, self.num_gen
-000110a0: 6573 2c20 7265 706c 6163 653d 4661 6c73  es, replace=Fals
-000110b0: 6529 2066 6f72 205f 2069 6e20 7261 6e67  e) for _ in rang
-000110c0: 6528 7365 6c66 2e70 6f70 756c 6174 696f  e(self.populatio
-000110d0: 6e5f 7369 7a65 295d 0a20 2020 2020 2020  n_size)].       
-000110e0: 2073 6f72 7465 645f 706f 7075 6c61 7469   sorted_populati
-000110f0: 6f6e 203d 205b 6e70 2e73 6f72 7428 726f  on = [np.sort(ro
-00011100: 7729 2066 6f72 2072 6f77 2069 6e20 706f  w) for row in po
-00011110: 7075 6c61 7469 6f6e 5d0a 2020 2020 2020  pulation].      
-00011120: 2020 7265 7475 726e 2073 6f72 7465 645f    return sorted_
-00011130: 706f 7075 6c61 7469 6f6e 0a0a 2020 2020  population..    
-00011140: 6465 6620 6372 6561 7465 5f72 6566 6572  def create_refer
-00011150: 735f 6d61 7472 6978 2873 656c 6629 202d  s_matrix(self) -
-00011160: 3e20 6c69 7374 3a0a 2020 2020 2020 2020  > list:.        
-00011170: 2222 220a 2020 2020 2020 2020 4372 6561  """.        Crea
-00011180: 7465 7320 6120 6d61 7472 6978 2062 6173  tes a matrix bas
-00011190: 6564 206f 6e20 7468 6520 7265 6665 7265  ed on the refere
-000111a0: 6e63 6520 6461 7461 2070 726f 7669 6465  nce data provide
-000111b0: 6420 6475 7269 6e67 2069 6e69 7469 616c  d during initial
-000111c0: 697a 6174 696f 6e2e 0a0a 2020 2020 2020  ization...      
-000111d0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000111e0: 2020 206c 6973 743a 2041 206d 6174 7269     list: A matri
-000111f0: 7820 7768 6572 6520 6561 6368 2072 6f77  x where each row
-00011200: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
-00011210: 616e 2069 7465 6d20 696e 2074 6865 2072  an item in the r
-00011220: 6566 6572 656e 6365 2064 6174 612c 0a20  eference data,. 
-00011230: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-00011240: 6820 6269 6e61 7279 2065 6e63 6f64 696e  h binary encodin
-00011250: 6720 6261 7365 6420 6f6e 2074 6865 2070  g based on the p
-00011260: 7265 7365 6e63 6520 6f66 2065 6c65 6d65  resence of eleme
-00011270: 6e74 7320 7769 7468 696e 2074 6865 2073  nts within the s
-00011280: 7065 6369 6669 6564 2072 616e 6765 2e0a  pecified range..
-00011290: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000112a0: 2020 2020 7265 6665 7273 5f6d 6174 7269      refers_matri
-000112b0: 7820 3d20 5b5d 0a20 2020 2020 2020 2066  x = [].        f
-000112c0: 6f72 2072 6f77 2069 6e20 7365 6c66 2e72  or row in self.r
-000112d0: 6566 6572 733a 0a20 2020 2020 2020 2020  efers:.         
-000112e0: 2020 2076 6563 746f 7220 3d20 5b30 5d20     vector = [0] 
-000112f0: 2a20 7365 6c66 2e6d 6178 5f6e 756d 2020  * self.max_num  
-00011300: 2320 496e 6974 6961 6c69 7a65 2076 6563  # Initialize vec
-00011310: 746f 7220 6f66 206c 656e 6774 6820 6d61  tor of length ma
-00011320: 785f 6e75 6d20 7769 7468 207a 6572 6f73  x_num with zeros
-00011330: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00011340: 206e 756d 2069 6e20 726f 773a 0a20 2020   num in row:.   
-00011350: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011360: 7365 6c66 2e6d 696e 5f6e 756d 203c 3d20  self.min_num <= 
-00011370: 6e75 6d20 3c3d 2073 656c 662e 6d61 785f  num <= self.max_
-00011380: 6e75 6d3a 0a20 2020 2020 2020 2020 2020  num:.           
-00011390: 2020 2020 2020 2020 2076 6563 746f 725b           vector[
-000113a0: 6e75 6d20 2d20 315d 203d 2031 2020 2320  num - 1] = 1  # 
-000113b0: 5365 7420 7468 6520 636f 7272 6573 706f  Set the correspo
-000113c0: 6e64 696e 6720 706f 7369 7469 6f6e 2074  nding position t
-000113d0: 6f20 310a 2020 2020 2020 2020 2020 2020  o 1.            
-000113e0: 7265 6665 7273 5f6d 6174 7269 782e 6170  refers_matrix.ap
-000113f0: 7065 6e64 2876 6563 746f 7229 0a20 2020  pend(vector).   
-00011400: 2020 2020 2072 6574 7572 6e20 7265 6665       return refe
-00011410: 7273 5f6d 6174 7269 780a 0a20 2020 2064  rs_matrix..    d
-00011420: 6566 2063 6865 636b 5f64 6961 676f 6e61  ef check_diagona
-00011430: 6c28 7365 6c66 2c20 696e 6469 7669 6475  l(self, individu
-00011440: 616c 3a20 6c69 7374 2c20 6466 735f 7369  al: list, dfs_si
-00011450: 7a65 3a20 7475 706c 6520 3d20 2833 2c20  ze: tuple = (3, 
-00011460: 3329 2920 2d3e 2066 6c6f 6174 3a0a 2020  3)) -> float:.  
-00011470: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011480: 2020 4368 6563 6b73 2064 6961 676f 6e61    Checks diagona
-00011490: 6c20 616c 6967 6e6d 656e 7473 2069 6e20  l alignments in 
-000114a0: 6120 6479 6e61 6d69 6361 6c6c 7920 7570  a dynamically up
-000114b0: 6461 7465 6420 6d61 7472 6978 2062 6173  dated matrix bas
-000114c0: 6564 206f 6e20 7468 6520 696e 6469 7669  ed on the indivi
-000114d0: 6475 616c 2773 2067 656e 6573 0a20 2020  dual's genes.   
-000114e0: 2020 2020 2061 6e64 2065 7661 6c75 6174       and evaluat
-000114f0: 6573 2074 6865 6972 2066 6974 6e65 7373  es their fitness
-00011500: 2062 6173 6564 206f 6e20 7468 6520 616c   based on the al
-00011510: 6967 6e6d 656e 742e 0a0a 2020 2020 2020  ignment...      
-00011520: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00011530: 696e 6469 7669 6475 616c 2028 6c69 7374  individual (list
-00011540: 293a 204c 6973 7420 6f66 2067 656e 6520  ): List of gene 
-00011550: 696e 6469 6365 7320 7265 7072 6573 656e  indices represen
-00011560: 7469 6e67 2061 6e20 696e 6469 7669 6475  ting an individu
-00011570: 616c 2069 6e20 7468 6520 706f 7075 6c61  al in the popula
-00011580: 7469 6f6e 2e0a 2020 2020 2020 2020 6466  tion..        df
-00011590: 735f 7369 7a65 2028 7475 706c 6529 3a20  s_size (tuple): 
-000115a0: 5369 7a65 206f 6620 7468 6520 6d61 7472  Size of the matr
-000115b0: 6978 2072 6567 696f 6e20 746f 2063 6865  ix region to che
-000115c0: 636b 2066 6f72 2064 6961 676f 6e61 6c20  ck for diagonal 
-000115d0: 616c 6967 6e6d 656e 7473 2028 726f 7773  alignments (rows
-000115e0: 2c20 636f 6c73 292e 0a0a 2020 2020 2020  , cols)...      
-000115f0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00011600: 2020 2066 6c6f 6174 3a20 4120 6669 746e     float: A fitn
-00011610: 6573 7320 7661 6c75 6520 6d6f 6469 6669  ess value modifi
-00011620: 6564 2062 6173 6564 206f 6e20 7468 6520  ed based on the 
-00011630: 7072 6573 656e 6365 206f 6620 6469 6167  presence of diag
-00011640: 6f6e 616c 2061 6c69 676e 6d65 6e74 732e  onal alignments.
-00011650: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011660: 2020 2020 2066 6974 6e65 7373 5f76 616c       fitness_val
-00011670: 7565 203d 2031 0a20 2020 2020 2020 2070  ue = 1.        p
-00011680: 7265 5f69 6e64 6578 203d 2069 6e64 6976  re_index = indiv
-00011690: 6964 7561 6c5b 305d 202d 2031 2020 2320  idual[0] - 1  # 
-000116a0: 5072 6576 696f 7573 2069 6e64 6578 2066  Previous index f
-000116b0: 6f72 2064 6961 676f 6e61 6c20 6368 6563  or diagonal chec
-000116c0: 6b69 6e67 0a0a 2020 2020 2020 2020 666f  king..        fo
-000116d0: 7220 696e 6469 2069 6e20 696e 6469 7669  r indi in indivi
-000116e0: 6475 616c 3a0a 2020 2020 2020 2020 2020  dual:.          
-000116f0: 2020 6966 206e 6f74 2028 7365 6c66 2e6d    if not (self.m
-00011700: 696e 5f6e 756d 203c 3d20 696e 6469 203c  in_num <= indi <
-00011710: 3d20 7365 6c66 2e6d 6178 5f6e 756d 293a  = self.max_num):
-00011720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011730: 2072 6574 7572 6e20 3120 2023 2052 6574   return 1  # Ret
-00011740: 7572 6e20 6120 6465 6661 756c 7420 6669  urn a default fi
-00011750: 746e 6573 7320 7661 6c75 6520 6966 2067  tness value if g
-00011760: 656e 6520 6973 206f 7574 206f 6620 7661  ene is out of va
-00011770: 6c69 6420 7261 6e67 650a 0a20 2020 2020  lid range..     
-00011780: 2020 2020 2020 206e 756d 5f69 6e64 6578         num_index
-00011790: 203d 2069 6e64 6920 2d20 310a 2020 2020   = indi - 1.    
-000117a0: 2020 2020 2020 2020 726f 7773 203d 206c          rows = l
-000117b0: 656e 2873 656c 662e 7265 6665 7273 5f6d  en(self.refers_m
-000117c0: 6174 7269 7829 0a20 2020 2020 2020 2020  atrix).         
-000117d0: 2020 2063 6f6c 7320 3d20 7365 6c66 2e6d     cols = self.m
-000117e0: 6178 5f6e 756d 0a20 2020 2020 2020 2020  ax_num.         
-000117f0: 2020 2064 6673 5f72 6f77 2c20 6466 735f     dfs_row, dfs_
-00011800: 636f 6c20 3d20 6466 735f 7369 7a65 0a20  col = dfs_size. 
-00011810: 2020 2020 2020 2020 2020 2069 735f 6261             is_ba
-00011820: 6c61 6e63 6520 3d20 6466 735f 726f 7720  lance = dfs_row 
-00011830: 3d3d 2064 6673 5f63 6f6c 2020 2320 4368  == dfs_col  # Ch
-00011840: 6563 6b20 6966 2074 6865 2061 7265 6120  eck if the area 
-00011850: 746f 2062 6520 6368 6563 6b65 6420 6973  to be checked is
-00011860: 2061 2073 7175 6172 650a 2020 2020 2020   a square.      
-00011870: 2020 2020 2020 7461 7267 6574 203d 206d        target = m
-00011880: 696e 2864 6673 5f73 697a 6529 0a0a 2020  in(dfs_size)..  
-00011890: 2020 2020 2020 2020 2020 6966 2064 6673            if dfs
-000118a0: 5f72 6f77 203e 2072 6f77 7320 6f72 2064  _row > rows or d
-000118b0: 6673 5f63 6f6c 203e 2063 6f6c 733a 0a20  fs_col > cols:. 
-000118c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000118d0: 6f6e 7469 6e75 6520 2023 2053 6b69 7020  ontinue  # Skip 
-000118e0: 6966 2074 6865 206d 6174 7269 7820 6973  if the matrix is
-000118f0: 2073 6d61 6c6c 6572 2074 6861 6e20 7468   smaller than th
-00011900: 6520 6466 7320 7369 7a65 0a0a 2020 2020  e dfs size..    
-00011910: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-00011920: 2061 206e 6577 206d 6174 7269 7820 696e   a new matrix in
-00011930: 636c 7564 696e 6720 6120 6e65 7720 726f  cluding a new ro
-00011940: 7720 666f 7220 7468 6520 6375 7272 656e  w for the curren
-00011950: 7420 6765 6e65 0a20 2020 2020 2020 2020  t gene.         
-00011960: 2020 206e 6577 5f6d 6174 7269 7820 3d20     new_matrix = 
-00011970: 5b72 6f77 5b3a 5d20 666f 7220 726f 7720  [row[:] for row 
-00011980: 696e 2073 656c 662e 7265 6665 7273 5f6d  in self.refers_m
-00011990: 6174 7269 785d 2020 2320 436f 7079 2074  atrix]  # Copy t
-000119a0: 6865 2065 7869 7374 696e 6720 6d61 7472  he existing matr
-000119b0: 6978 0a20 2020 2020 2020 2020 2020 206e  ix.            n
-000119c0: 6577 5f72 6f77 203d 205b 305d 202a 2073  ew_row = [0] * s
-000119d0: 656c 662e 6d61 785f 6e75 6d0a 2020 2020  elf.max_num.    
-000119e0: 2020 2020 2020 2020 6e65 775f 726f 775b          new_row[
-000119f0: 6e75 6d5f 696e 6465 785d 203d 2031 0a20  num_index] = 1. 
-00011a00: 2020 2020 2020 2020 2020 206e 6577 5f6d             new_m
-00011a10: 6174 7269 782e 6170 7065 6e64 286e 6577  atrix.append(new
-00011a20: 5f72 6f77 2920 2023 2041 6464 2074 6865  _row)  # Add the
-00011a30: 206e 6577 2072 6f77 2063 6f72 7265 6374   new row correct
-00011a40: 6c79 0a0a 2020 2020 2020 2020 2020 2020  ly..            
-00011a50: 2320 4368 6563 6b20 6469 6167 6f6e 616c  # Check diagonal
-00011a60: 732c 206f 6e6c 7920 7570 7761 7264 730a  s, only upwards.
-00011a70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00011a80: 6472 2069 6e20 5b2d 315d 3a20 2023 204f  dr in [-1]:  # O
-00011a90: 6e6c 7920 6e65 6564 2074 6f20 6368 6563  nly need to chec
-00011aa0: 6b20 7468 6520 7570 7065 7220 6469 6167  k the upper diag
-00011ab0: 6f6e 616c 730a 2020 2020 2020 2020 2020  onals.          
-00011ac0: 2020 2020 2020 6d6f 7665 5f72 203d 2046        move_r = F
-00011ad0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00011ae0: 2020 2020 206d 6f76 655f 725f 636f 756e       move_r_coun
-00011af0: 7420 3d20 300a 2020 2020 2020 2020 2020  t = 0.          
-00011b00: 2020 2020 2020 6d6f 7665 5f63 5f63 6f75        move_c_cou
-00011b10: 6e74 203d 2030 0a20 2020 2020 2020 2020  nt = 0.         
-00011b20: 2020 2020 2020 2066 6f72 2064 6320 696e         for dc in
-00011b30: 205b 2d31 2c20 315d 3a20 2023 2043 6865   [-1, 1]:  # Che
-00011b40: 636b 2062 6f74 6820 6c65 6674 2061 6e64  ck both left and
-00011b50: 2072 6967 6874 2064 6961 676f 6e61 6c73   right diagonals
-00011b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b70: 2020 2020 2063 6f75 6e74 203d 2030 0a20       count = 0. 
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2072 2c20 6320 3d20 726f 7773 2c20     r, c = rows, 
-00011ba0: 6e75 6d5f 696e 6465 780a 2020 2020 2020  num_index.      
-00011bb0: 2020 2020 2020 2020 2020 2020 2020 7768                wh
-00011bc0: 696c 6520 726f 7773 202d 2064 6673 5f72  ile rows - dfs_r
-00011bd0: 6f77 203c 3d20 7220 3c3d 2072 6f77 7320  ow <= r <= rows 
-00011be0: 2b20 3120 616e 6420 7072 655f 696e 6465  + 1 and pre_inde
-00011bf0: 7820 2d20 6466 735f 636f 6c20 3c3d 2063  x - dfs_col <= c
-00011c00: 203c 3d20 6e75 6d5f 696e 6465 7820 2b20   <= num_index + 
-00011c10: 6466 735f 636f 6c3a 0a20 2020 2020 2020  dfs_col:.       
-00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c30: 2069 6620 6e65 775f 6d61 7472 6978 5b72   if new_matrix[r
-00011c40: 5d5b 635d 203d 3d20 313a 0a20 2020 2020  ][c] == 1:.     
-00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 2020 2020 2020 2063 6f75 6e74 202b 3d20         count += 
-00011c70: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-00011c80: 2020 2020 2020 2020 2020 6966 2069 735f            if is_
-00011c90: 6261 6c61 6e63 653a 0a20 2020 2020 2020  balance:.       
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 2020 2072 202b 3d20 6472 0a20 2020       r += dr.   
-00011cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cd0: 2020 2020 2020 2020 2063 202b 3d20 6463           c += dc
-00011ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011cf0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d10: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-00011d20: 7665 5f72 3a0a 2020 2020 2020 2020 2020  ve_r:.          
-00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d40: 2020 2020 2020 6966 206e 6577 5f6d 6174        if new_mat
-00011d50: 7269 785b 725d 5b63 5d20 3d3d 2031 3a0a  rix[r][c] == 1:.
-00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d80: 2020 2020 6d6f 7665 5f63 5f63 6f75 6e74      move_c_count
-00011d90: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011db0: 2020 2020 2020 7220 2b3d 2064 720a 2020        r += dr.  
-00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-00011de0: 7665 5f72 203d 2046 616c 7365 0a20 2020  ve_r = False.   
-00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e00: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011e30: 6620 6e65 775f 6d61 7472 6978 5b72 5d5b  f new_matrix[r][
-00011e40: 635d 203d 3d20 313a 0a20 2020 2020 2020  c] == 1:.       
-00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2020 2020 2020 2020 2020 2020 206d 6f76               mov
-00011e70: 655f 725f 636f 756e 7420 2b3d 2031 0a20  e_r_count += 1. 
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011ea0: 202b 3d20 6463 0a20 2020 2020 2020 2020   += dc.         
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 2020 2020 2020 206d 6f76 655f 7220 3d20         move_r = 
-00011ed0: 5472 7565 0a0a 2020 2020 2020 2020 2020  True..          
-00011ee0: 2020 2020 2020 2020 2020 6966 2069 735f            if is_
-00011ef0: 6261 6c61 6e63 6520 616e 6420 636f 756e  balance and coun
-00011f00: 7420 3d3d 2074 6172 6765 743a 0a20 2020  t == target:.   
-00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f20: 2020 2020 2066 6974 6e65 7373 5f76 616c       fitness_val
-00011f30: 7565 202a 3d20 302e 3120 2023 2044 6563  ue *= 0.1  # Dec
-00011f40: 7265 6173 6520 6669 746e 6573 7320 6966  rease fitness if
-00011f50: 2061 2062 616c 616e 6365 6420 6469 6167   a balanced diag
-00011f60: 6f6e 616c 2069 7320 666f 756e 640a 2020  onal is found.  
-00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2020 656c 6966 206e 6f74 2069 735f 6261    elif not is_ba
-00011f90: 6c61 6e63 6520 616e 6420 6d61 7828 6d6f  lance and max(mo
-00011fa0: 7665 5f72 5f63 6f75 6e74 2c20 6d6f 7665  ve_r_count, move
-00011fb0: 5f63 5f63 6f75 6e74 2920 3d3d 2074 6172  _c_count) == tar
-00011fc0: 6765 7420 2d20 313a 0a20 2020 2020 2020  get - 1:.       
-00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fe0: 2066 6974 6e65 7373 5f76 616c 7565 202a   fitness_value *
-00011ff0: 3d20 302e 3320 2023 2044 6563 7265 6173  = 0.3  # Decreas
-00012000: 6520 6669 746e 6573 7320 6966 2061 6e20  e fitness if an 
-00012010: 756e 6261 6c61 6e63 6564 2064 6961 676f  unbalanced diago
-00012020: 6e61 6c20 6973 2066 6f75 6e64 0a0a 2020  nal is found..  
-00012030: 2020 2020 2020 2020 2020 7072 655f 696e            pre_in
-00012040: 6465 7820 3d20 6e75 6d5f 696e 6465 7820  dex = num_index 
-00012050: 2023 2055 7064 6174 6520 7072 6576 696f   # Update previo
-00012060: 7573 2069 6e64 6578 2066 6f72 2074 6865  us index for the
-00012070: 206e 6578 7420 6765 6e65 0a0a 2020 2020   next gene..    
-00012080: 2020 2020 7265 7475 726e 2066 6974 6e65      return fitne
-00012090: 7373 5f76 616c 7565 0a0a 2020 2020 6465  ss_value..    de
-000120a0: 6620 6368 6563 6b5f 7665 7274 6963 616c  f check_vertical
-000120b0: 2873 656c 662c 2069 6e64 6976 6964 7561  (self, individua
-000120c0: 6c3a 206c 6973 7429 202d 3e20 666c 6f61  l: list) -> floa
-000120d0: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
-000120e0: 2020 2020 2020 2043 6865 636b 7320 7665         Checks ve
-000120f0: 7274 6963 616c 2061 6c69 676e 6d65 6e74  rtical alignment
-00012100: 7320 696e 2061 2064 796e 616d 6963 616c  s in a dynamical
-00012110: 6c79 2075 7064 6174 6564 206d 6174 7269  ly updated matri
-00012120: 7820 6261 7365 6420 6f6e 2074 6865 2069  x based on the i
-00012130: 6e64 6976 6964 7561 6c27 7320 6765 6e65  ndividual's gene
-00012140: 730a 2020 2020 2020 2020 616e 6420 6576  s.        and ev
-00012150: 616c 7561 7465 7320 7468 6569 7220 6669  aluates their fi
-00012160: 746e 6573 7320 6261 7365 6420 6f6e 2074  tness based on t
-00012170: 6865 2061 6c69 676e 6d65 6e74 2e0a 0a20  he alignment... 
-00012180: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00012190: 2020 2020 2069 6e64 6976 6964 7561 6c20       individual 
-000121a0: 286c 6973 7429 3a20 4c69 7374 206f 6620  (list): List of 
-000121b0: 6765 6e65 2069 6e64 6963 6573 2072 6570  gene indices rep
-000121c0: 7265 7365 6e74 696e 6720 616e 2069 6e64  resenting an ind
-000121d0: 6976 6964 7561 6c20 696e 2074 6865 2070  ividual in the p
-000121e0: 6f70 756c 6174 696f 6e2e 0a0a 2020 2020  opulation...    
-000121f0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00012200: 2020 2020 2066 6c6f 6174 3a20 4120 6669       float: A fi
-00012210: 746e 6573 7320 7661 6c75 6520 6d6f 6469  tness value modi
-00012220: 6669 6564 2062 6173 6564 206f 6e20 7468  fied based on th
-00012230: 6520 7072 6573 656e 6365 206f 6620 7665  e presence of ve
-00012240: 7274 6963 616c 2061 6c69 676e 6d65 6e74  rtical alignment
-00012250: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00012260: 2020 2020 2020 2066 6974 6e65 7373 5f76         fitness_v
-00012270: 616c 7565 203d 2031 0a20 2020 2020 2020  alue = 1.       
-00012280: 2070 7265 5f69 6e64 6578 203d 2069 6e64   pre_index = ind
-00012290: 6976 6964 7561 6c5b 305d 202d 2031 2020  ividual[0] - 1  
-000122a0: 2320 5072 6576 696f 7573 2069 6e64 6578  # Previous index
-000122b0: 2c20 756e 7573 6564 2069 6e20 7665 7274  , unused in vert
-000122c0: 6963 616c 2063 6865 636b 696e 670a 0a20  ical checking.. 
-000122d0: 2020 2020 2020 2066 6f72 2069 6e64 6920         for indi 
-000122e0: 696e 2069 6e64 6976 6964 7561 6c3a 0a20  in individual:. 
-000122f0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00012300: 7420 2873 656c 662e 6d69 6e5f 6e75 6d20  t (self.min_num 
-00012310: 3c3d 2069 6e64 6920 3c3d 2073 656c 662e  <= indi <= self.
-00012320: 6d61 785f 6e75 6d29 3a0a 2020 2020 2020  max_num):.      
-00012330: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00012340: 2031 2020 2320 5265 7475 726e 2061 2064   1  # Return a d
-00012350: 6566 6175 6c74 2066 6974 6e65 7373 2076  efault fitness v
-00012360: 616c 7565 2069 6620 6765 6e65 2069 7320  alue if gene is 
-00012370: 6f75 7420 6f66 2076 616c 6964 2072 616e  out of valid ran
-00012380: 6765 0a0a 2020 2020 2020 2020 2020 2020  ge..            
-00012390: 6e75 6d5f 696e 6465 7820 3d20 696e 6469  num_index = indi
-000123a0: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
-000123b0: 2072 6f77 7320 3d20 6c65 6e28 7365 6c66   rows = len(self
-000123c0: 2e72 6566 6572 735f 6d61 7472 6978 290a  .refers_matrix).
-000123d0: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-000123e0: 7265 6174 6520 6120 6e65 7720 6d61 7472  reate a new matr
-000123f0: 6978 2069 6e63 6c75 6469 6e67 2061 206e  ix including a n
-00012400: 6577 2072 6f77 2066 6f72 2074 6865 2063  ew row for the c
-00012410: 7572 7265 6e74 2067 656e 650a 2020 2020  urrent gene.    
-00012420: 2020 2020 2020 2020 6e65 775f 6d61 7472          new_matr
-00012430: 6978 203d 205b 726f 775b 3a5d 2066 6f72  ix = [row[:] for
-00012440: 2072 6f77 2069 6e20 7365 6c66 2e72 6566   row in self.ref
-00012450: 6572 735f 6d61 7472 6978 5d20 2023 2043  ers_matrix]  # C
-00012460: 6f70 7920 7468 6520 6578 6973 7469 6e67  opy the existing
-00012470: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
-00012480: 2020 2020 6e65 775f 726f 7720 3d20 5b30      new_row = [0
-00012490: 5d20 2a20 7365 6c66 2e6d 6178 5f6e 756d  ] * self.max_num
-000124a0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-000124b0: 5f72 6f77 5b6e 756d 5f69 6e64 6578 5d20  _row[num_index] 
-000124c0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-000124d0: 6e65 775f 6d61 7472 6978 2e61 7070 656e  new_matrix.appen
-000124e0: 6428 6e65 775f 726f 7729 2020 2320 4164  d(new_row)  # Ad
-000124f0: 6420 7468 6520 6e65 7720 726f 7720 636f  d the new row co
-00012500: 7272 6563 746c 790a 0a20 2020 2020 2020  rrectly..       
-00012510: 2020 2020 2023 2043 6865 636b 2076 6572       # Check ver
-00012520: 7469 6361 6c20 616c 6967 6e6d 656e 740a  tical alignment.
-00012530: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012540: 6472 2069 6e20 5b2d 315d 3a20 2023 204f  dr in [-1]:  # O
-00012550: 6e6c 7920 6e65 6564 2074 6f20 6368 6563  nly need to chec
-00012560: 6b20 7468 6520 7570 7761 7264 2076 6572  k the upward ver
-00012570: 7469 6361 6c20 6c69 6e65 0a20 2020 2020  tical line.     
-00012580: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
-00012590: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-000125a0: 2020 2020 2072 2c20 6320 3d20 726f 7773       r, c = rows
-000125b0: 2c20 6e75 6d5f 696e 6465 780a 2020 2020  , num_index.    
-000125c0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-000125d0: 6520 3020 3c3d 2072 203c 206c 656e 286e  e 0 <= r < len(n
-000125e0: 6577 5f6d 6174 7269 7829 3a0a 2020 2020  ew_matrix):.    
-000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012600: 6966 206e 6577 5f6d 6174 7269 785b 725d  if new_matrix[r]
-00012610: 5b63 5d20 3d3d 2031 3a0a 2020 2020 2020  [c] == 1:.      
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 2020 636f 756e 7420 2b3d 2031 0a20 2020    count += 1.   
-00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012650: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00012660: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00012670: 2043 6865 636b 2069 6620 7468 6572 6520   Check if there 
-00012680: 6172 6520 6e6f 2067 656e 6573 2069 6e20  are no genes in 
-00012690: 7468 6520 6375 7272 656e 7420 636f 6c75  the current colu
-000126a0: 6d6e 2069 6e20 7468 6520 6f72 6967 696e  mn in the origin
-000126b0: 616c 206d 6174 7269 780a 2020 2020 2020  al matrix.      
-000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126d0: 2020 6966 2073 756d 286e 6577 5f6d 6174    if sum(new_mat
-000126e0: 7269 785b 726f 775d 5b63 5d20 666f 7220  rix[row][c] for 
-000126f0: 726f 7720 696e 2072 616e 6765 2872 6f77  row in range(row
-00012700: 7329 2920 3d3d 2030 3a0a 2020 2020 2020  s)) == 0:.      
-00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012720: 2020 2020 2020 6669 746e 6573 735f 7661        fitness_va
-00012730: 6c75 6520 2a3d 2030 2e35 0a20 2020 2020  lue *= 0.5.     
-00012740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012750: 2020 2065 6c69 6620 636f 756e 7420 3e20     elif count > 
-00012760: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00012770: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012780: 6974 6e65 7373 5f76 616c 7565 202a 3d20  itness_value *= 
-00012790: 302e 340a 2020 2020 2020 2020 2020 2020  0.4.            
-000127a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000127b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000127c0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-000127d0: 746e 6573 735f 7661 6c75 6520 3d20 310a  tness_value = 1.
-000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127f0: 2020 2020 7220 2b3d 2064 720a 0a20 2020      r += dr..   
-00012800: 2020 2020 2020 2020 2020 2020 2023 2041               # A
-00012810: 646a 7573 7420 6669 746e 6573 7320 6261  djust fitness ba
-00012820: 7365 6420 6f6e 2074 6865 2063 6f75 6e74  sed on the count
-00012830: 206f 6620 7665 7274 6963 616c 2061 6c69   of vertical ali
-00012840: 676e 6d65 6e74 730a 2020 2020 2020 2020  gnments.        
-00012850: 2020 2020 2020 2020 6966 2063 6f75 6e74          if count
-00012860: 2069 6e20 7261 6e67 6528 312c 2033 293a   in range(1, 3):
-00012870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012880: 2020 2020 2066 6974 6e65 7373 5f76 616c       fitness_val
-00012890: 7565 202a 3d20 302e 310a 2020 2020 2020  ue *= 0.1.      
-000128a0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128c0: 2020 2020 6669 746e 6573 735f 7661 6c75      fitness_valu
-000128d0: 6520 2a3d 2030 2e37 0a0a 2020 2020 2020  e *= 0.7..      
-000128e0: 2020 2020 2020 7072 655f 696e 6465 7820        pre_index 
-000128f0: 3d20 6e75 6d5f 696e 6465 7820 2023 2055  = num_index  # U
-00012900: 7064 6174 6520 7072 6576 696f 7573 2069  pdate previous i
-00012910: 6e64 6578 2066 6f72 2074 6865 206e 6578  ndex for the nex
-00012920: 7420 6765 6e65 0a0a 2020 2020 2020 2020  t gene..        
-00012930: 7265 7475 726e 2066 6974 6e65 7373 5f76  return fitness_v
-00012940: 616c 7565 0a0a 2020 2020 6465 6620 6669  alue..    def fi
-00012950: 746e 6573 7328 7365 6c66 2c20 696e 6469  tness(self, indi
-00012960: 7669 6475 616c 3a20 6c69 7374 2c20 6466  vidual: list, df
-00012970: 735f 7369 7a65 3a20 7475 706c 6520 3d20  s_size: tuple = 
-00012980: 2832 2c20 3229 2920 2d3e 2066 6c6f 6174  (2, 2)) -> float
-00012990: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000129a0: 2020 2020 2020 4361 6c63 756c 6174 6573        Calculates
-000129b0: 2074 6865 2066 6974 6e65 7373 206f 6620   the fitness of 
-000129c0: 616e 2069 6e64 6976 6964 7561 6c20 6261  an individual ba
-000129d0: 7365 6420 6f6e 2074 6865 2061 6c69 676e  sed on the align
-000129e0: 6d65 6e74 206f 6620 6765 6e65 7320 696e  ment of genes in
-000129f0: 2061 2064 796e 616d 6963 616c 6c79 0a20   a dynamically. 
-00012a00: 2020 2020 2020 2075 7064 6174 6564 206d         updated m
-00012a10: 6174 7269 782e 2046 6974 6e65 7373 2069  atrix. Fitness i
-00012a20: 7320 6576 616c 7561 7465 6420 6261 7365  s evaluated base
-00012a30: 6420 6f6e 2073 7065 6369 6669 6320 616c  d on specific al
-00012a40: 6967 6e6d 656e 7420 7061 7474 6572 6e73  ignment patterns
-00012a50: 2061 6e64 2070 6172 616d 6574 6572 732e   and parameters.
-00012a60: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00012a70: 2020 2020 2020 2020 696e 6469 7669 6475          individu
-00012a80: 616c 2028 6c69 7374 293a 204c 6973 7420  al (list): List 
-00012a90: 6f66 2067 656e 6520 696e 6469 6365 7320  of gene indices 
-00012aa0: 7265 7072 6573 656e 7469 6e67 2061 6e20  representing an 
-00012ab0: 696e 6469 7669 6475 616c 2069 6e20 7468  individual in th
-00012ac0: 6520 706f 7075 6c61 7469 6f6e 2e0a 2020  e population..  
-00012ad0: 2020 2020 2020 6466 735f 7369 7a65 2028        dfs_size (
-00012ae0: 7475 706c 6529 3a20 5369 7a65 206f 6620  tuple): Size of 
-00012af0: 7468 6520 6d61 7472 6978 2072 6567 696f  the matrix regio
-00012b00: 6e20 746f 2063 6865 636b 2066 6f72 2061  n to check for a
-00012b10: 6c69 676e 6d65 6e74 7320 2872 6f77 732c  lignments (rows,
-00012b20: 2063 6f6c 7329 2e0a 0a20 2020 2020 2020   cols)...       
-00012b30: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00012b40: 2020 666c 6f61 743a 2041 2066 6974 6e65    float: A fitne
-00012b50: 7373 2076 616c 7565 206d 6f64 6966 6965  ss value modifie
-00012b60: 6420 6261 7365 6420 6f6e 2074 6865 2070  d based on the p
-00012b70: 7265 7365 6e63 6520 6f66 2073 7065 6369  resence of speci
-00012b80: 6669 6320 616c 6967 6e6d 656e 7473 2e0a  fic alignments..
-00012b90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012ba0: 2020 2020 2320 7265 7475 726e 206e 702e      # return np.
-00012bb0: 6c69 6e61 6c67 2e6e 6f72 6d28 696e 6469  linalg.norm(indi
-00012bc0: 7669 6475 616c 202d 2074 6172 6765 7429  vidual - target)
-00012bd0: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
-00012be0: 2066 6f72 2064 7570 6c69 6361 7465 2067   for duplicate g
-00012bf0: 656e 6573 2c20 7768 6963 6820 6172 6520  enes, which are 
-00012c00: 6e6f 7420 616c 6c6f 7765 640a 2020 2020  not allowed.    
-00012c10: 2020 2020 6966 206c 656e 2873 6574 2869      if len(set(i
-00012c20: 6e64 6976 6964 7561 6c29 2920 3c20 7365  ndividual)) < se
-00012c30: 6c66 2e6e 756d 5f67 656e 6573 3a0a 2020  lf.num_genes:.  
-00012c40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00012c50: 2031 3030 3030 2020 2320 4869 6768 2070   10000  # High p
-00012c60: 656e 616c 7479 2066 6f72 2064 7570 6c69  enalty for dupli
-00012c70: 6361 7465 2067 656e 6573 0a0a 2020 2020  cate genes..    
-00012c80: 2020 2020 6669 746e 6573 735f 7661 6c75      fitness_valu
-00012c90: 6520 3d20 310a 2020 2020 2020 2020 7072  e = 1.        pr
-00012ca0: 655f 696e 6465 7820 3d20 696e 6469 7669  e_index = indivi
-00012cb0: 6475 616c 5b30 5d20 2d20 3120 2023 2050  dual[0] - 1  # P
-00012cc0: 7265 7669 6f75 7320 696e 6465 7820 666f  revious index fo
-00012cd0: 7220 616c 6967 6e6d 656e 7420 6368 6563  r alignment chec
-00012ce0: 6b69 6e67 0a0a 2020 2020 2020 2020 666f  king..        fo
-00012cf0: 7220 696e 6469 2069 6e20 696e 6469 7669  r indi in indivi
-00012d00: 6475 616c 3a0a 2020 2020 2020 2020 2020  dual:.          
-00012d10: 2020 2320 4368 6563 6b20 6966 2074 6865    # Check if the
-00012d20: 2067 656e 6520 6973 2077 6974 6869 6e20   gene is within 
-00012d30: 7468 6520 7661 6c69 6420 7261 6e67 650a  the valid range.
-00012d40: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00012d50: 6f74 2028 7365 6c66 2e6d 696e 5f6e 756d  ot (self.min_num
-00012d60: 203c 3d20 696e 6469 203c 3d20 7365 6c66   <= indi <= self
-00012d70: 2e6d 6178 5f6e 756d 293a 0a20 2020 2020  .max_num):.     
-00012d80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00012d90: 6e20 3130 3030 3020 2023 2048 6967 6820  n 10000  # High 
-00012da0: 7065 6e61 6c74 7920 666f 7220 6f75 742d  penalty for out-
-00012db0: 6f66 2d72 616e 6765 2067 656e 6573 0a0a  of-range genes..
-00012dc0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-00012dd0: 696e 6465 7820 3d20 696e 6469 202d 2031  index = indi - 1
-00012de0: 0a20 2020 2020 2020 2020 2020 2072 6f77  .            row
-00012df0: 732c 2063 6f6c 7320 3d20 6c65 6e28 7365  s, cols = len(se
-00012e00: 6c66 2e72 6566 6572 735f 6d61 7472 6978  lf.refers_matrix
-00012e10: 292c 2073 656c 662e 6d61 785f 6e75 6d0a  ), self.max_num.
-00012e20: 2020 2020 2020 2020 2020 2020 2864 6673              (dfs
-00012e30: 5f72 6f77 2c20 6466 735f 636f 6c29 2c20  _row, dfs_col), 
-00012e40: 7461 7267 6574 203d 2064 6673 5f73 697a  target = dfs_siz
-00012e50: 652c 206d 696e 2864 6673 5f73 697a 6529  e, min(dfs_size)
-00012e60: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00012e70: 4368 6563 6b20 6966 2074 6865 2064 6673  Check if the dfs
-00012e80: 5f73 697a 6520 6973 206c 6172 6765 7220  _size is larger 
-00012e90: 7468 616e 2074 6865 206d 6174 7269 7820  than the matrix 
-00012ea0: 6469 6d65 6e73 696f 6e73 0a20 2020 2020  dimensions.     
-00012eb0: 2020 2020 2020 2069 6620 6466 735f 726f         if dfs_ro
-00012ec0: 7720 3e20 726f 7773 206f 7220 6466 735f  w > rows or dfs_
-00012ed0: 636f 6c20 3e20 636f 6c73 3a0a 2020 2020  col > cols:.    
-00012ee0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00012ef0: 726e 2031 2020 2320 5265 7475 726e 2064  rn 1  # Return d
-00012f00: 6566 6175 6c74 2066 6974 6e65 7373 2069  efault fitness i
-00012f10: 6620 7468 6520 6466 7320 7369 7a65 2069  f the dfs size i
-00012f20: 7320 746f 6f20 6c61 7267 650a 0a20 2020  s too large..   
-00012f30: 2020 2020 2020 2020 2023 2043 7265 6174           # Creat
-00012f40: 6520 6120 6e65 7720 6d61 7472 6978 2069  e a new matrix i
-00012f50: 6e63 6c75 6469 6e67 2061 206e 6577 2072  ncluding a new r
-00012f60: 6f77 2066 6f72 2074 6865 2063 7572 7265  ow for the curre
-00012f70: 6e74 2067 656e 650a 2020 2020 2020 2020  nt gene.        
-00012f80: 2020 2020 6e65 775f 6d61 7472 6978 203d      new_matrix =
-00012f90: 205b 726f 775b 3a5d 2066 6f72 2072 6f77   [row[:] for row
-00012fa0: 2069 6e20 7365 6c66 2e72 6566 6572 735f   in self.refers_
-00012fb0: 6d61 7472 6978 5d20 2023 2043 6f70 7920  matrix]  # Copy 
-00012fc0: 7468 6520 6578 6973 7469 6e67 206d 6174  the existing mat
-00012fd0: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
-00012fe0: 6e65 775f 726f 7720 3d20 5b30 5d20 2a20  new_row = [0] * 
-00012ff0: 7365 6c66 2e6d 6178 5f6e 756d 0a20 2020  self.max_num.   
-00013000: 2020 2020 2020 2020 206e 6577 5f72 6f77           new_row
-00013010: 5b6e 756d 5f69 6e64 6578 5d20 3d20 310a  [num_index] = 1.
-00013020: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00013030: 6d61 7472 6978 2e61 7070 656e 6428 6e65  matrix.append(ne
-00013040: 775f 726f 7729 2020 2320 4164 6420 7468  w_row)  # Add th
-00013050: 6520 6e65 7720 726f 7720 636f 7272 6563  e new row correc
-00013060: 746c 790a 0a20 2020 2020 2020 2020 2020  tly..           
-00013070: 2023 2043 6865 636b 2061 6c69 676e 6d65   # Check alignme
-00013080: 6e74 7320 6f6e 6c79 2075 7077 6172 6473  nts only upwards
-00013090: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000130a0: 2064 7220 696e 205b 2d31 5d3a 2020 2320   dr in [-1]:  # 
-000130b0: 4f6e 6c79 206e 6565 6420 746f 2063 6865  Only need to che
-000130c0: 636b 2074 6865 2075 7077 6172 6420 6469  ck the upward di
-000130d0: 7265 6374 696f 6e0a 2020 2020 2020 2020  rection.        
-000130e0: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
-000130f0: 6469 6167 6f6e 616c 730a 2020 2020 2020  diagonals.      
-00013100: 2020 2020 2020 2020 2020 6d6f 7665 5f72            move_r
-00013110: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00013120: 2020 2020 2020 2020 206d 6f76 655f 725f           move_r_
-00013130: 636f 756e 7420 3d20 300a 2020 2020 2020  count = 0.      
-00013140: 2020 2020 2020 2020 2020 6d6f 7665 5f63            move_c
-00013150: 5f63 6f75 6e74 203d 2030 0a20 2020 2020  _count = 0.     
-00013160: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
-00013170: 6320 696e 205b 2d31 2c20 315d 3a20 2023  c in [-1, 1]:  #
-00013180: 2043 6865 636b 2062 6f74 6820 6c65 6674   Check both left
-00013190: 2061 6e64 2072 6967 6874 2064 6961 676f   and right diago
-000131a0: 6e61 6c73 0a20 2020 2020 2020 2020 2020  nals.           
-000131b0: 2020 2020 2020 2020 2063 6f75 6e74 203d           count =
-000131c0: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
-000131d0: 2020 2020 2020 2072 2c20 6320 3d20 726f         r, c = ro
-000131e0: 7773 2c20 6e75 6d5f 696e 6465 780a 2020  ws, num_index.  
-000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013200: 2020 7768 696c 6520 726f 7773 202d 2064    while rows - d
-00013210: 6673 5f72 6f77 203c 3d20 7220 3c3d 2072  fs_row <= r <= r
-00013220: 6f77 7320 2b20 3120 616e 6420 7072 655f  ows + 1 and pre_
-00013230: 696e 6465 7820 2d20 6466 735f 636f 6c20  index - dfs_col 
-00013240: 3c3d 2063 203c 3d20 6d69 6e28 6e75 6d5f  <= c <= min(num_
-00013250: 696e 6465 7820 2b20 6466 735f 636f 6c2c  index + dfs_col,
-00013260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000132c0: 6f6c 7320 2d20 3129 3a0a 2020 2020 2020  ols - 1):.      
-000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132e0: 2020 6966 206e 6577 5f6d 6174 7269 785b    if new_matrix[
-000132f0: 725d 5b63 5d20 3d3d 2031 3a0a 2020 2020  r][c] == 1:.    
-00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 2020 2020 2020 2020 636f 756e 7420 2b3d          count +=
-00013320: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-00013330: 2020 2020 2020 2020 2020 2069 6620 6466             if df
-00013340: 735f 726f 7720 3d3d 2064 6673 5f63 6f6c  s_row == dfs_col
-00013350: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013360: 2020 2020 2020 2020 2020 2020 2020 7220                r 
-00013370: 2b3d 2064 720a 2020 2020 2020 2020 2020  += dr.          
-00013380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013390: 2020 6320 2b3d 2064 630a 2020 2020 2020    c += dc.      
-000133a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000133c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133d0: 2020 2020 6966 206d 6f76 655f 723a 0a20      if move_r:. 
-000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00013400: 6620 6e65 775f 6d61 7472 6978 5b72 5d5b  f new_matrix[r][
-00013410: 635d 203d 3d20 313a 0a20 2020 2020 2020  c] == 1:.       
-00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013430: 2020 2020 2020 2020 2020 2020 206d 6f76               mov
-00013440: 655f 635f 636f 756e 7420 2b3d 2031 0a20  e_c_count += 1. 
-00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013460: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00013470: 202b 3d20 6472 0a20 2020 2020 2020 2020   += dr.         
-00013480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013490: 2020 2020 2020 206d 6f76 655f 7220 3d20         move_r = 
-000134a0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000134d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134e0: 2020 2020 2020 2020 6966 206e 6577 5f6d          if new_m
-000134f0: 6174 7269 785b 725d 5b63 5d20 3d3d 2031  atrix[r][c] == 1
-00013500: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013520: 2020 2020 2020 6d6f 7665 5f72 5f63 6f75        move_r_cou
-00013530: 6e74 202b 3d20 310a 2020 2020 2020 2020  nt += 1.        
-00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013550: 2020 2020 2020 2020 6320 2b3d 2064 630a          c += dc.
-00013560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013580: 6d6f 7665 5f72 203d 2054 7275 650a 0a20  move_r = True.. 
+00006040: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+00006050: 696e 5f73 616d 706c 6573 5f6c 6561 6627  in_samples_leaf'
+00006060: 3a20 7374 6174 732e 7261 6e64 696e 7428  : stats.randint(
+00006070: 312c 2034 3029 0a20 2020 2020 2020 2020  1, 40).         
+00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+000060b0: 2020 2020 2070 6172 616d 5f6f 7665 7272       param_overr
+000060c0: 6964 6573 2028 4f70 7469 6f6e 616c 5b44  ides (Optional[D
+000060d0: 6963 745d 293a 2041 6464 6974 696f 6e61  ict]): Additiona
+000060e0: 6c20 7061 7261 6d65 7465 7273 2066 6f72  l parameters for
+000060f0: 2074 6865 2052 616e 646f 6d69 7a65 6453   the RandomizedS
+00006100: 6561 7263 6843 562e 0a20 2020 2020 2020  earchCV..       
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2020 2020 2020 2020 2065 673a 207b 0a20           eg: {. 
+00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006170: 2020 2027 6e5f 6974 6572 273a 2031 3030     'n_iter': 100
+00006180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061b0: 2020 2020 2020 2763 7627 3a20 332c 0a20        'cv': 3,. 
+000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061f0: 2020 2027 7363 6f72 696e 6727 3a20 276e     'scoring': 'n
+00006200: 6567 5f6d 6561 6e5f 7371 7561 7265 645f  eg_mean_squared_
+00006210: 6572 726f 7227 2c0a 2020 2020 2020 2020  error',.        
+00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006240: 2020 2020 2020 2020 2020 2020 2776 6572              'ver
+00006250: 626f 7365 273a 2030 2c0a 2020 2020 2020  bose': 0,.      
+00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006280: 2020 2020 2020 2020 2020 2020 2020 2772                'r
+00006290: 616e 646f 6d5f 7374 6174 6527 3a20 3132  andom_state': 12
+000062a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062d0: 2020 2020 2020 276e 5f6a 6f62 7327 3a20        'n_jobs': 
+000062e0: 2d31 0a20 2020 2020 2020 2020 2020 2020  -1.             
+000062f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006310: 2020 207d 0a0a 2020 2020 2020 2020 5265     }..        Re
+00006320: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00006330: 2020 2066 6c6f 6174 3a20 5468 6520 7072     float: The pr
+00006340: 6564 6963 7465 6420 6e65 7874 2076 616c  edicted next val
+00006350: 7565 2069 6e20 7468 6520 7365 7175 656e  ue in the sequen
+00006360: 6365 2e0a 0a20 2020 2020 2020 2052 6169  ce...        Rai
+00006370: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+00006380: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
+00006390: 7468 6520 726f 6c6c 696e 675f 7369 7a65  the rolling_size
+000063a0: 2069 7320 6c61 7267 6572 2074 6861 6e20   is larger than 
+000063b0: 7468 6520 7369 7a65 206f 6620 6e75 6d65  the size of nume
+000063c0: 7269 635f 7365 7175 656e 6365 2e0a 2020  ric_sequence..  
+000063d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000063e0: 2020 6966 2072 6f6c 6c69 6e67 5f73 697a    if rolling_siz
+000063f0: 6520 3e20 6c65 6e28 6e75 6d65 7269 635f  e > len(numeric_
+00006400: 7365 7175 656e 6365 293a 0a20 2020 2020  sequence):.     
+00006410: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00006420: 7565 4572 726f 7228 2272 6f6c 6c69 6e67  ueError("rolling
+00006430: 5f73 697a 6520 6361 6e6e 6f74 2062 6520  _size cannot be 
+00006440: 6c61 7267 6572 2074 6861 6e20 7468 6520  larger than the 
+00006450: 7369 7a65 206f 6620 6e75 6d65 7269 635f  size of numeric_
+00006460: 7365 7175 656e 6365 2229 0a0a 2020 2020  sequence")..    
+00006470: 2020 2020 2320 4765 6e65 7261 7465 2064      # Generate d
+00006480: 6174 6173 6574 7320 7769 7468 2074 6865  atasets with the
+00006490: 2073 7065 6369 6669 6564 2072 6f6c 6c69   specified rolli
+000064a0: 6e67 2073 697a 650a 2020 2020 2020 2020  ng size.        
+000064b0: 7472 6169 6e5f 782c 2074 7261 696e 5f79  train_x, train_y
+000064c0: 203d 2043 616c 6375 6c61 7465 5574 696c   = CalculateUtil
+000064d0: 2e67 656e 6572 6174 655f 6461 7461 7365  .generate_datase
+000064e0: 7473 5f77 6974 685f 726f 6c6c 696e 675f  ts_with_rolling_
+000064f0: 7369 7a65 280a 2020 2020 2020 2020 2020  size(.          
+00006500: 2020 6461 7461 3d6e 756d 6572 6963 5f73    data=numeric_s
+00006510: 6571 7565 6e63 652c 2072 6f6c 6c69 6e67  equence, rolling
+00006520: 5f73 697a 653d 726f 6c6c 696e 675f 7369  _size=rolling_si
+00006530: 7a65 0a20 2020 2020 2020 2029 0a0a 2020  ze.        )..  
+00006540: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
+00006550: 6c69 7374 7320 746f 206e 756d 7079 2061  lists to numpy a
+00006560: 7272 6179 7320 666f 7220 636f 6d70 6174  rrays for compat
+00006570: 6962 696c 6974 7920 7769 7468 2073 6369  ibility with sci
+00006580: 6b69 742d 6c65 6172 6e0a 2020 2020 2020  kit-learn.      
+00006590: 2020 696e 7075 745f 7820 3d20 6e70 2e61    input_x = np.a
+000065a0: 7272 6179 2874 7261 696e 5f78 290a 2020  rray(train_x).  
+000065b0: 2020 2020 2020 6f75 7470 7574 5f79 203d        output_y =
+000065c0: 206e 702e 6172 7261 7928 7472 6169 6e5f   np.array(train_
+000065d0: 7929 0a0a 2020 2020 2020 2020 2320 5363  y)..        # Sc
+000065e0: 616c 6520 7468 6520 6665 6174 7572 6573  ale the features
+000065f0: 2074 6f20 6e6f 726d 616c 697a 6520 6461   to normalize da
+00006600: 7461 0a20 2020 2020 2020 2073 6361 6c65  ta.        scale
+00006610: 7220 3d20 5374 616e 6461 7264 5363 616c  r = StandardScal
+00006620: 6572 2829 0a20 2020 2020 2020 2069 6e70  er().        inp
+00006630: 7574 5f78 5f73 6361 6c65 6420 3d20 7363  ut_x_scaled = sc
+00006640: 616c 6572 2e66 6974 5f74 7261 6e73 666f  aler.fit_transfo
+00006650: 726d 2869 6e70 7574 5f78 290a 0a20 2020  rm(input_x)..   
+00006660: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
+00006670: 6520 616e 6420 7472 6169 6e20 7468 6520  e and train the 
+00006680: 5261 6e64 6f6d 2046 6f72 6573 7420 5265  Random Forest Re
+00006690: 6772 6573 736f 720a 2020 2020 2020 2020  gressor.        
+000066a0: 6d6f 6465 6c20 3d20 5261 6e64 6f6d 466f  model = RandomFo
+000066b0: 7265 7374 5265 6772 6573 736f 7228 7761  restRegressor(wa
+000066c0: 726d 5f73 7461 7274 3d77 6172 6d5f 7374  rm_start=warm_st
+000066d0: 6172 742c 2072 616e 646f 6d5f 7374 6174  art, random_stat
+000066e0: 653d 7261 6e64 6f6d 5f73 7461 7465 290a  e=random_state).
+000066f0: 2020 2020 2020 2020 6966 2070 6172 616d          if param
+00006700: 5f64 6973 7472 6962 7574 696f 6e73 3a0a  _distributions:.
+00006710: 2020 2020 2020 2020 2020 2020 7061 7261              para
+00006720: 6d5f 6f76 6572 7269 6465 7320 3d20 7061  m_overrides = pa
+00006730: 7261 6d5f 6f76 6572 7269 6465 7320 6f72  ram_overrides or
+00006740: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00006750: 7261 6e64 6f6d 5f73 6561 7263 6820 3d20  random_search = 
+00006760: 5261 6e64 6f6d 697a 6564 5365 6172 6368  RandomizedSearch
+00006770: 4356 2865 7374 696d 6174 6f72 3d6d 6f64  CV(estimator=mod
+00006780: 656c 2c20 7061 7261 6d5f 6469 7374 7269  el, param_distri
+00006790: 6275 7469 6f6e 733d 7061 7261 6d5f 6469  butions=param_di
+000067a0: 7374 7269 6275 7469 6f6e 732c 0a20 2020  stributions,.   
+000067b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067d0: 2020 2020 2020 2020 2020 2020 2a2a 7061              **pa
+000067e0: 7261 6d5f 6f76 6572 7269 6465 7329 0a20  ram_overrides). 
+000067f0: 2020 2020 2020 2020 2020 2072 616e 646f             rando
+00006800: 6d5f 7365 6172 6368 2e66 6974 2869 6e70  m_search.fit(inp
+00006810: 7574 5f78 5f73 6361 6c65 642c 206f 7574  ut_x_scaled, out
+00006820: 7075 745f 7929 0a20 2020 2020 2020 2020  put_y).         
+00006830: 2020 206d 6f64 656c 203d 2052 616e 646f     model = Rando
+00006840: 6d46 6f72 6573 7452 6567 7265 7373 6f72  mForestRegressor
+00006850: 2877 6172 6d5f 7374 6172 743d 7761 726d  (warm_start=warm
+00006860: 5f73 7461 7274 2c20 7261 6e64 6f6d 5f73  _start, random_s
+00006870: 7461 7465 3d72 616e 646f 6d5f 7374 6174  tate=random_stat
+00006880: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068a0: 2020 2020 2020 2020 2020 2020 202a 2a72               **r
+000068b0: 616e 646f 6d5f 7365 6172 6368 2e62 6573  andom_search.bes
+000068c0: 745f 7061 7261 6d73 5f29 0a20 2020 2020  t_params_).     
+000068d0: 2020 206d 6f64 656c 2e66 6974 2869 6e70     model.fit(inp
+000068e0: 7574 5f78 5f73 6361 6c65 642c 206f 7574  ut_x_scaled, out
+000068f0: 7075 745f 7929 0a0a 2020 2020 2020 2020  put_y)..        
+00006900: 2320 5072 6570 6172 6520 7468 6520 6c61  # Prepare the la
+00006910: 7374 2072 6f6c 6c69 6e67 2077 696e 646f  st rolling windo
+00006920: 7720 6f66 2064 6174 6120 666f 7220 7072  w of data for pr
+00006930: 6564 6963 7469 6f6e 0a20 2020 2020 2020  ediction.       
+00006940: 2074 6573 745f 7820 3d20 6e70 2e61 7272   test_x = np.arr
+00006950: 6179 285b 6e75 6d65 7269 635f 7365 7175  ay([numeric_sequ
+00006960: 656e 6365 5b2d 726f 6c6c 696e 675f 7369  ence[-rolling_si
+00006970: 7a65 3a5d 5d29 0a20 2020 2020 2020 2074  ze:]]).        t
+00006980: 6573 745f 785f 7363 616c 6564 203d 2073  est_x_scaled = s
+00006990: 6361 6c65 722e 7472 616e 7366 6f72 6d28  caler.transform(
+000069a0: 7465 7374 5f78 290a 0a20 2020 2020 2020  test_x)..       
+000069b0: 2023 2050 7265 6469 6374 696e 6720 7468   # Predicting th
+000069c0: 6520 6e65 7874 2076 616c 7565 0a20 2020  e next value.   
+000069d0: 2020 2020 2070 7265 645f 7920 3d20 6d6f       pred_y = mo
+000069e0: 6465 6c2e 7072 6564 6963 7428 7465 7374  del.predict(test
+000069f0: 5f78 5f73 6361 6c65 6429 0a20 2020 2020  _x_scaled).     
+00006a00: 2020 2072 6574 7572 6e20 7072 6564 5f79     return pred_y
+00006a10: 5b30 5d0a 0a20 2020 2040 7374 6174 6963  [0]..    @static
+00006a20: 6d65 7468 6f64 0a20 2020 2064 6566 2072  method.    def r
+00006a30: 616e 646f 6d5f 666f 7265 7374 5f72 6567  andom_forest_reg
+00006a40: 7265 7373 6f72 5f6e 6578 745f 7661 6c75  ressor_next_valu
+00006a50: 655f 6279 5f69 6e64 6578 286e 756d 6572  e_by_index(numer
+00006a60: 6963 5f73 6571 7565 6e63 653a 204c 6973  ic_sequence: Lis
+00006a70: 745b 696e 745d 2920 2d3e 2069 6e74 3a0a  t[int]) -> int:.
+00006a80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006a90: 2020 2020 5072 6564 6963 7473 2074 6865      Predicts the
+00006aa0: 206e 6578 7420 7661 6c75 6520 696e 2061   next value in a
+00006ab0: 2073 6571 7565 6e63 6520 7573 696e 6720   sequence using 
+00006ac0: 6120 5261 6e64 6f6d 2046 6f72 6573 7420  a Random Forest 
+00006ad0: 5265 6772 6573 736f 722e 0a0a 2020 2020  Regressor...    
+00006ae0: 2020 2020 4120 5261 6e64 6f6d 2046 6f72      A Random For
+00006af0: 6573 7420 5265 6772 6573 736f 7220 6973  est Regressor is
+00006b00: 2061 2074 7970 6520 6f66 2065 6e73 656d   a type of ensem
+00006b10: 626c 6520 6d61 6368 696e 6520 6c65 6172  ble machine lear
+00006b20: 6e69 6e67 206d 6f64 656c 2074 6861 7420  ning model that 
+00006b30: 7573 6573 0a20 2020 2020 2020 206d 756c  uses.        mul
+00006b40: 7469 706c 6520 6465 6369 7369 6f6e 2074  tiple decision t
+00006b50: 7265 6573 2074 6f20 6d61 6b65 2070 7265  rees to make pre
+00006b60: 6469 6374 696f 6e73 2e20 4974 2069 7320  dictions. It is 
+00006b70: 7061 7274 6963 756c 6172 6c79 2075 7365  particularly use
+00006b80: 6675 6c20 666f 7220 7265 6772 6573 7369  ful for regressi
+00006b90: 6f6e 0a20 2020 2020 2020 2074 6173 6b73  on.        tasks
+00006ba0: 206f 6e20 636f 6d70 6c65 7820 6461 7461   on complex data
+00006bb0: 7365 7473 2062 6563 6175 7365 2069 7420  sets because it 
+00006bc0: 6361 6e20 6361 7074 7572 6520 6e6f 6e2d  can capture non-
+00006bd0: 6c69 6e65 6172 2072 656c 6174 696f 6e73  linear relations
+00006be0: 6869 7073 2062 6574 7765 656e 0a20 2020  hips between.   
+00006bf0: 2020 2020 2076 6172 6961 626c 6573 2e20       variables. 
+00006c00: 5468 6973 2066 756e 6374 696f 6e20 6170  This function ap
+00006c10: 706c 6965 7320 7468 6520 6d6f 6465 6c20  plies the model 
+00006c20: 746f 2061 2073 6571 7565 6e63 6520 6f66  to a sequence of
+00006c30: 206e 756d 6265 7273 2074 6f20 7072 6564   numbers to pred
+00006c40: 6963 7420 7468 650a 2020 2020 2020 2020  ict the.        
+00006c50: 6e65 7874 2076 616c 7565 2062 6173 6564  next value based
+00006c60: 206f 6e20 7468 6520 6f62 7365 7276 6564   on the observed
+00006c70: 2074 7265 6e64 2e0a 0a20 2020 2020 2020   trend...       
+00006c80: 203a 7061 7261 6d20 6e75 6d65 7269 635f   :param numeric_
+00006c90: 7365 7175 656e 6365 3a20 4120 6c69 7374  sequence: A list
+00006ca0: 206f 7220 7365 7175 656e 6365 206f 6620   or sequence of 
+00006cb0: 6e75 6d62 6572 7320 746f 206d 6f64 656c  numbers to model
+00006cc0: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00006cd0: 6e3a 2054 6865 2070 7265 6469 6374 6564  n: The predicted
+00006ce0: 206e 6578 7420 7661 6c75 6520 696e 2074   next value in t
+00006cf0: 6865 2073 6571 7565 6e63 6520 6173 2061  he sequence as a
+00006d00: 6e20 696e 7465 6765 722e 0a20 2020 2020  n integer..     
+00006d10: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+00006d20: 2043 6f6e 7665 7274 2074 6865 206e 756d   Convert the num
+00006d30: 6572 6963 2073 6571 7565 6e63 6520 696e  eric sequence in
+00006d40: 746f 2061 206e 756d 7079 2061 7272 6179  to a numpy array
+00006d50: 2061 6e64 2072 6573 6861 7065 2066 6f72   and reshape for
+00006d60: 2073 6b6c 6561 726e 0a20 2020 2020 2020   sklearn.       
+00006d70: 2064 6174 6120 3d20 6e70 2e61 7272 6179   data = np.array
+00006d80: 286e 756d 6572 6963 5f73 6571 7565 6e63  (numeric_sequenc
+00006d90: 6529 2e72 6573 6861 7065 282d 312c 2031  e).reshape(-1, 1
+00006da0: 290a 0a20 2020 2020 2020 2023 2043 7265  )..        # Cre
+00006db0: 6174 6520 616e 2061 7272 6179 2072 6570  ate an array rep
+00006dc0: 7265 7365 6e74 696e 6720 7469 6d65 206f  resenting time o
+00006dd0: 7220 7468 6520 696e 6465 7065 6e64 656e  r the independen
+00006de0: 7420 7661 7269 6162 6c65 2c20 7265 7368  t variable, resh
+00006df0: 6170 6564 2061 7320 6120 636f 6c75 6d6e  aped as a column
+00006e00: 0a20 2020 2020 2020 2074 696d 655f 6665  .        time_fe
+00006e10: 6174 7572 6520 3d20 6e70 2e61 7272 6179  ature = np.array
+00006e20: 2872 616e 6765 286c 656e 2864 6174 6129  (range(len(data)
+00006e30: 2929 2e72 6573 6861 7065 282d 312c 2031  )).reshape(-1, 1
+00006e40: 290a 0a20 2020 2020 2020 2023 2043 7265  )..        # Cre
+00006e50: 6174 6520 6120 5261 6e64 6f6d 466f 7265  ate a RandomFore
+00006e60: 7374 5265 6772 6573 736f 7220 6d6f 6465  stRegressor mode
+00006e70: 6c20 616e 6420 6669 7420 6974 2074 6f20  l and fit it to 
+00006e80: 7468 6520 6461 7461 0a20 2020 2020 2020  the data.       
+00006e90: 206d 6f64 656c 203d 2052 616e 646f 6d46   model = RandomF
+00006ea0: 6f72 6573 7452 6567 7265 7373 6f72 2829  orestRegressor()
+00006eb0: 0a20 2020 2020 2020 206d 6f64 656c 2e66  .        model.f
+00006ec0: 6974 2874 696d 655f 6665 6174 7572 652c  it(time_feature,
+00006ed0: 2064 6174 612e 7261 7665 6c28 2929 2020   data.ravel())  
+00006ee0: 2320 466c 6174 7465 6e20 7468 6520 6172  # Flatten the ar
+00006ef0: 7261 7920 746f 2066 6974 2074 6865 206d  ray to fit the m
+00006f00: 6f64 656c 0a0a 2020 2020 2020 2020 2320  odel..        # 
+00006f10: 5072 6564 6963 7420 7468 6520 6e65 7874  Predict the next
+00006f20: 2076 616c 7565 2069 6e20 7468 6520 7365   value in the se
+00006f30: 7175 656e 6365 2075 7369 6e67 2074 6865  quence using the
+00006f40: 2066 6974 7465 6420 6d6f 6465 6c0a 2020   fitted model.  
+00006f50: 2020 2020 2020 6675 7475 7265 5f74 696d        future_tim
+00006f60: 6520 3d20 6e70 2e61 7272 6179 285b 6c65  e = np.array([le
+00006f70: 6e28 6461 7461 295d 292e 7265 7368 6170  n(data)]).reshap
+00006f80: 6528 2d31 2c20 3129 0a20 2020 2020 2020  e(-1, 1).       
+00006f90: 2066 7574 7572 655f 7072 6564 203d 206d   future_pred = m
+00006fa0: 6f64 656c 2e70 7265 6469 6374 2866 7574  odel.predict(fut
+00006fb0: 7572 655f 7469 6d65 290a 0a20 2020 2020  ure_time)..     
+00006fc0: 2020 2023 2052 6574 7572 6e20 7468 6520     # Return the 
+00006fd0: 7072 6564 6963 7465 6420 7661 6c75 6520  predicted value 
+00006fe0: 6173 2061 6e20 696e 7465 6765 720a 2020  as an integer.  
+00006ff0: 2020 2020 2020 7265 7475 726e 2043 616c        return Cal
+00007000: 6375 6c61 7465 5574 696c 2e72 6561 6c5f  culateUtil.real_
+00007010: 726f 756e 6428 6675 7475 7265 5f70 7265  round(future_pre
+00007020: 645b 305d 290a 0a20 2020 2040 7374 6174  d[0])..    @stat
+00007030: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+00007040: 2072 656c 6174 6976 655f 7374 7265 6e67   relative_streng
+00007050: 7468 5f69 6e64 6578 286e 756d 6572 6963  th_index(numeric
+00007060: 5f73 6571 7565 6e63 653a 204c 6973 745b  _sequence: List[
+00007070: 696e 745d 2c20 7065 7269 6f64 3a20 696e  int], period: in
+00007080: 7420 3d20 3134 2920 2d3e 2066 6c6f 6174  t = 14) -> float
+00007090: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000070a0: 2020 2020 2020 4361 6c63 756c 6174 6520        Calculate 
+000070b0: 7468 6520 5265 6c61 7469 7665 2053 7472  the Relative Str
+000070c0: 656e 6774 6820 496e 6465 7820 2852 5349  ength Index (RSI
+000070d0: 2920 7573 696e 6720 4578 706f 6e65 6e74  ) using Exponent
+000070e0: 6961 6c20 4d6f 7669 6e67 2041 7665 7261  ial Moving Avera
+000070f0: 6765 2028 454d 4129 2e0a 0a20 2020 2020  ge (EMA)...     
+00007100: 2020 203a 7061 7261 6d20 6e75 6d65 7269     :param numeri
+00007110: 635f 7365 7175 656e 6365 3a20 4120 6c69  c_sequence: A li
+00007120: 7374 206f 6620 7072 6963 6573 2066 6f72  st of prices for
+00007130: 2061 2070 6172 7469 6375 6c61 7220 7374   a particular st
+00007140: 6f63 6b20 6f72 2061 7373 6574 2e0a 2020  ock or asset..  
+00007150: 2020 2020 2020 3a70 6172 616d 2070 6572        :param per
+00007160: 696f 643a 2054 6865 2070 6572 696f 6420  iod: The period 
+00007170: 6f76 6572 2077 6869 6368 2074 6f20 6361  over which to ca
+00007180: 6c63 756c 6174 6520 7468 6520 5253 492c  lculate the RSI,
+00007190: 2074 7970 6963 616c 6c79 2031 342e 0a20   typically 14.. 
+000071a0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000071b0: 5468 6520 6361 6c63 756c 6174 6564 2052  The calculated R
+000071c0: 5349 2076 616c 7565 2e0a 2020 2020 2020  SI value..      
+000071d0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+000071e0: 206c 656e 286e 756d 6572 6963 5f73 6571   len(numeric_seq
+000071f0: 7565 6e63 6529 203c 2070 6572 696f 643a  uence) < period:
+00007200: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00007210: 7365 2056 616c 7565 4572 726f 7228 224e  se ValueError("N
+00007220: 6f74 2065 6e6f 7567 6820 6461 7461 2070  ot enough data p
+00007230: 6f69 6e74 7320 746f 2063 616c 6375 6c61  oints to calcula
+00007240: 7465 2052 5349 2229 0a0a 2020 2020 2020  te RSI")..      
+00007250: 2020 6465 6c74 6173 203d 205b 6e75 6d65    deltas = [nume
+00007260: 7269 635f 7365 7175 656e 6365 5b69 202b  ric_sequence[i +
+00007270: 2031 5d20 2d20 6e75 6d65 7269 635f 7365   1] - numeric_se
+00007280: 7175 656e 6365 5b69 5d20 666f 7220 6920  quence[i] for i 
+00007290: 696e 2072 616e 6765 286c 656e 286e 756d  in range(len(num
+000072a0: 6572 6963 5f73 6571 7565 6e63 6529 202d  eric_sequence) -
+000072b0: 2031 295d 0a20 2020 2020 2020 2067 6169   1)].        gai
+000072c0: 6e73 203d 205b 6d61 7828 6465 6c74 612c  ns = [max(delta,
+000072d0: 2030 2920 666f 7220 6465 6c74 6120 696e   0) for delta in
+000072e0: 2064 656c 7461 735d 0a20 2020 2020 2020   deltas].       
+000072f0: 206c 6f73 7365 7320 3d20 5b6d 6178 282d   losses = [max(-
+00007300: 6465 6c74 612c 2030 2920 666f 7220 6465  delta, 0) for de
+00007310: 6c74 6120 696e 2064 656c 7461 735d 0a0a  lta in deltas]..
+00007320: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
+00007330: 6c69 7a65 2045 4d41 2077 6974 6820 534d  lize EMA with SM
+00007340: 4120 666f 7220 7468 6520 6669 7273 7420  A for the first 
+00007350: 2770 6572 696f 6427 0a20 2020 2020 2020  'period'.       
+00007360: 2061 7667 5f67 6169 6e20 3d20 7375 6d28   avg_gain = sum(
+00007370: 6761 696e 735b 3a70 6572 696f 645d 2920  gains[:period]) 
+00007380: 2f20 7065 7269 6f64 0a20 2020 2020 2020  / period.       
+00007390: 2061 7667 5f6c 6f73 7320 3d20 7375 6d28   avg_loss = sum(
+000073a0: 6c6f 7373 6573 5b3a 7065 7269 6f64 5d29  losses[:period])
+000073b0: 202f 2070 6572 696f 640a 0a20 2020 2020   / period..     
+000073c0: 2020 2023 2041 7070 6c79 2045 4d41 2066     # Apply EMA f
+000073d0: 6f72 6d75 6c61 2066 6f72 2067 6169 6e73  ormula for gains
+000073e0: 2061 6e64 206c 6f73 7365 730a 2020 2020   and losses.    
+000073f0: 2020 2020 656d 615f 6661 6374 6f72 203d      ema_factor =
+00007400: 2032 202f 2028 7065 7269 6f64 202b 2031   2 / (period + 1
+00007410: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
+00007420: 696e 2072 616e 6765 2870 6572 696f 642c  in range(period,
+00007430: 206c 656e 2864 656c 7461 7329 293a 0a20   len(deltas)):. 
+00007440: 2020 2020 2020 2020 2020 2061 7667 5f67             avg_g
+00007450: 6169 6e20 3d20 2867 6169 6e73 5b69 5d20  ain = (gains[i] 
+00007460: 2a20 656d 615f 6661 6374 6f72 2920 2b20  * ema_factor) + 
+00007470: 2861 7667 5f67 6169 6e20 2a20 2831 202d  (avg_gain * (1 -
+00007480: 2065 6d61 5f66 6163 746f 7229 290a 2020   ema_factor)).  
+00007490: 2020 2020 2020 2020 2020 6176 675f 6c6f            avg_lo
+000074a0: 7373 203d 2028 6c6f 7373 6573 5b69 5d20  ss = (losses[i] 
+000074b0: 2a20 656d 615f 6661 6374 6f72 2920 2b20  * ema_factor) + 
+000074c0: 2861 7667 5f6c 6f73 7320 2a20 2831 202d  (avg_loss * (1 -
+000074d0: 2065 6d61 5f66 6163 746f 7229 290a 0a20   ema_factor)).. 
+000074e0: 2020 2020 2020 2072 7320 3d20 6176 675f         rs = avg_
+000074f0: 6761 696e 202f 2061 7667 5f6c 6f73 7320  gain / avg_loss 
+00007500: 6966 2061 7667 5f6c 6f73 7320 213d 2030  if avg_loss != 0
+00007510: 2065 6c73 6520 300a 2020 2020 2020 2020   else 0.        
+00007520: 7273 6920 3d20 3130 3020 2d20 2831 3030  rsi = 100 - (100
+00007530: 202f 2028 3120 2b20 7273 2929 2069 6620   / (1 + rs)) if 
+00007540: 6176 675f 6c6f 7373 2021 3d20 3020 656c  avg_loss != 0 el
+00007550: 7365 2031 3030 0a0a 2020 2020 2020 2020  se 100..        
+00007560: 7265 7475 726e 2072 7369 0a0a 2020 2020  return rsi..    
+00007570: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00007580: 2020 6465 6620 7365 6173 6f6e 616c 5f61    def seasonal_a
+00007590: 7574 6f72 6567 7265 7373 6976 655f 696e  utoregressive_in
+000075a0: 7465 6772 6174 6564 5f6d 6f76 696e 675f  tegrated_moving_
+000075b0: 6176 6572 6167 655f 6e65 7874 5f76 616c  average_next_val
+000075c0: 7565 286e 756d 6572 6963 5f73 6571 7565  ue(numeric_seque
+000075d0: 6e63 653a 204c 6973 745b 696e 745d 2920  nce: List[int]) 
+000075e0: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+000075f0: 2222 220a 2020 2020 2020 2020 4669 7420  """.        Fit 
+00007600: 6120 5365 6173 6f6e 616c 2041 7574 6f72  a Seasonal Autor
+00007610: 6567 7265 7373 6976 6520 496e 7465 6772  egressive Integr
+00007620: 6174 6564 204d 6f76 696e 6720 4176 6572  ated Moving Aver
+00007630: 6167 6520 2853 4152 494d 4129 206d 6f64  age (SARIMA) mod
+00007640: 656c 2074 6f0a 2020 2020 2020 2020 7468  el to.        th
+00007650: 6520 7072 6f76 6964 6564 2074 696d 6520  e provided time 
+00007660: 7365 7269 6573 2064 6174 6120 616e 6420  series data and 
+00007670: 7072 6564 6963 7420 7468 6520 6e65 7874  predict the next
+00007680: 2076 616c 7565 2069 6e20 7468 6520 7365   value in the se
+00007690: 7269 6573 2e0a 0a20 2020 2020 2020 2053  ries...        S
+000076a0: 4152 494d 4120 6d6f 6465 6c73 2061 7265  ARIMA models are
+000076b0: 2075 7365 6420 746f 2066 6f72 6563 6173   used to forecas
+000076c0: 7420 6675 7475 7265 2070 6f69 6e74 7320  t future points 
+000076d0: 696e 2061 2074 696d 6520 7365 7269 6573  in a time series
+000076e0: 2e20 5468 6579 2061 7265 0a20 2020 2020  . They are.     
+000076f0: 2020 2063 6170 6162 6c65 206f 6620 6d6f     capable of mo
+00007700: 6465 6c69 6e67 2063 6f6d 706c 6578 2073  deling complex s
+00007710: 6561 736f 6e61 6c20 7061 7474 6572 6e73  easonal patterns
+00007720: 2062 7920 696e 636f 7270 6f72 6174 696e   by incorporatin
+00007730: 6720 626f 7468 206e 6f6e 2d73 6561 736f  g both non-seaso
+00007740: 6e61 6c0a 2020 2020 2020 2020 2841 5249  nal.        (ARI
+00007750: 4d41 2920 616e 6420 7365 6173 6f6e 616c  MA) and seasonal
+00007760: 2065 6c65 6d65 6e74 732e 0a0a 2020 2020   elements...    
+00007770: 2020 2020 3a70 6172 616d 206e 756d 6572      :param numer
+00007780: 6963 5f73 6571 7565 6e63 653a 2041 206c  ic_sequence: A l
+00007790: 6973 7420 6f66 206e 756d 6572 6963 616c  ist of numerical
+000077a0: 2076 616c 7565 7320 7265 7072 6573 656e   values represen
+000077b0: 7469 6e67 2061 2074 696d 6520 7365 7269  ting a time seri
+000077c0: 6573 2e0a 2020 2020 2020 2020 3a72 6574  es..        :ret
+000077d0: 7572 6e3a 2054 6865 206e 6578 7420 696e  urn: The next in
+000077e0: 7465 6765 7220 7661 6c75 6520 7072 6564  teger value pred
+000077f0: 6963 7465 6420 6279 2074 6865 2053 4152  icted by the SAR
+00007800: 494d 4120 6d6f 6465 6c2e 0a20 2020 2020  IMA model..     
+00007810: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+00007820: 2043 6f6e 7665 7274 2074 6865 2064 6174   Convert the dat
+00007830: 6120 746f 2061 206e 756d 7079 2061 7272  a to a numpy arr
+00007840: 6179 2066 6f72 2074 696d 6520 7365 7269  ay for time seri
+00007850: 6573 2061 6e61 6c79 7369 730a 2020 2020  es analysis.    
+00007860: 2020 2020 7469 6d65 7365 7269 6573 203d      timeseries =
+00007870: 206e 702e 6172 7261 7928 6e75 6d65 7269   np.array(numeri
+00007880: 635f 7365 7175 656e 6365 290a 0a20 2020  c_sequence)..   
+00007890: 2020 2020 2023 2041 7574 6f6d 6174 6963       # Automatic
+000078a0: 616c 6c79 2064 6973 636f 7665 7220 7468  ally discover th
+000078b0: 6520 6f70 7469 6d61 6c20 6f72 6465 7220  e optimal order 
+000078c0: 666f 7220 7468 6520 5341 5249 4d41 206d  for the SARIMA m
+000078d0: 6f64 656c 0a20 2020 2020 2020 2073 7465  odel.        ste
+000078e0: 7077 6973 655f 6d6f 6465 6c20 3d20 6175  pwise_model = au
+000078f0: 746f 5f61 7269 6d61 2874 696d 6573 6572  to_arima(timeser
+00007900: 6965 732c 2073 7461 7274 5f70 3d32 2c20  ies, start_p=2, 
+00007910: 7374 6172 745f 713d 322c 0a20 2020 2020  start_q=2,.     
+00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007930: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00007940: 6178 5f70 3d33 2c20 6d61 785f 713d 332c  ax_p=3, max_q=3,
+00007950: 206d 3d31 322c 0a20 2020 2020 2020 2020   m=12,.         
+00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007970: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00007980: 5f50 3d31 2c20 7374 6172 745f 513d 312c  _P=1, start_Q=1,
+00007990: 206d 6178 5f50 3d33 2c20 6d61 785f 513d   max_P=3, max_Q=
+000079a0: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
+000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079c0: 2020 2020 2020 2073 6561 736f 6e61 6c3d         seasonal=
+000079d0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079f0: 2020 2020 2020 2020 2020 643d 312c 2044            d=1, D
+00007a00: 3d31 2c20 7472 6163 653d 4661 6c73 652c  =1, trace=False,
+00007a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a30: 2020 2020 2065 7272 6f72 5f61 6374 696f       error_actio
+00007a40: 6e3d 2769 676e 6f72 6527 2c0a 2020 2020  n='ignore',.    
+00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 7375 7070 7265 7373 5f77 6172 6e69 6e67  suppress_warning
+00007a80: 733d 5472 7565 2c0a 2020 2020 2020 2020  s=True,.        
+00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007aa0: 2020 2020 2020 2020 2020 2020 7374 6570              step
+00007ab0: 7769 7365 3d54 7275 6529 0a0a 2020 2020  wise=True)..    
+00007ac0: 2020 2020 2320 4669 7420 7468 6520 5341      # Fit the SA
+00007ad0: 5249 4d41 206d 6f64 656c 2074 6f20 7468  RIMA model to th
+00007ae0: 6520 7469 6d65 2073 6572 6965 7320 6461  e time series da
+00007af0: 7461 0a20 2020 2020 2020 206d 6f64 656c  ta.        model
+00007b00: 203d 2073 7465 7077 6973 655f 6d6f 6465   = stepwise_mode
+00007b10: 6c2e 6669 7428 7469 6d65 7365 7269 6573  l.fit(timeseries
+00007b20: 290a 0a20 2020 2020 2020 2023 2050 7265  )..        # Pre
+00007b30: 6469 6374 2074 6865 206e 6578 7420 7661  dict the next va
+00007b40: 6c75 6520 696e 2074 6865 2074 696d 6520  lue in the time 
+00007b50: 7365 7269 6573 0a20 2020 2020 2020 2066  series.        f
+00007b60: 6f72 6563 6173 7420 3d20 6d6f 6465 6c2e  orecast = model.
+00007b70: 7072 6564 6963 7428 6e5f 7065 7269 6f64  predict(n_period
+00007b80: 733d 3129 0a0a 2020 2020 2020 2020 2320  s=1)..        # 
+00007b90: 5265 7475 726e 2074 6865 2070 7265 6469  Return the predi
+00007ba0: 6374 6564 2076 616c 7565 2061 7320 616e  cted value as an
+00007bb0: 2069 6e74 6567 6572 0a20 2020 2020 2020   integer.       
+00007bc0: 2072 6574 7572 6e20 4361 6c63 756c 6174   return Calculat
+00007bd0: 6555 7469 6c2e 7265 616c 5f72 6f75 6e64  eUtil.real_round
+00007be0: 2866 6f72 6563 6173 745b 305d 290a 0a0a  (forecast[0])...
+00007bf0: 636c 6173 7320 5370 6964 6572 5574 696c  class SpiderUtil
+00007c00: 2841 4243 293a 0a20 2020 2022 2222 0a20  (ABC):.    """. 
+00007c10: 2020 204d 6f73 746c 7920 6372 6177 6c69     Mostly crawli
+00007c20: 6e67 2064 6174 610a 2020 2020 2222 220a  ng data.    """.
+00007c30: 2020 2020 7572 6c20 3d20 2768 7474 7073      url = 'https
+00007c40: 3a2f 2f77 7777 2e6c 6f74 7465 7279 2e67  ://www.lottery.g
+00007c50: 6f76 2e63 6e2f 6b6a 2f6b 6a6c 622e 6874  ov.cn/kj/kjlb.ht
+00007c60: 6d6c 3f64 6c74 270a 0a20 2020 2064 6566  ml?dlt'..    def
+00007c70: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00007c80: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00007c90: 2020 2022 2222 0a20 2020 2020 2020 2049     """.        I
+00007ca0: 6e69 7469 616c 697a 6520 7468 6520 5370  nitialize the Sp
+00007cb0: 6964 6572 5574 696c 206f 626a 6563 7420  iderUtil object 
+00007cc0: 7769 7468 2061 2055 524c 2e0a 0a20 2020  with a URL...   
+00007cd0: 2020 2020 203a 7061 7261 6d20 6b77 6172       :param kwar
+00007ce0: 6773 3a20 4120 6469 6374 696f 6e61 7279  gs: A dictionary
+00007cf0: 206f 6620 6b65 7977 6f72 6420 6172 6775   of keyword argu
+00007d00: 6d65 6e74 7320 7768 6572 653a 0a20 2020  ments where:.   
+00007d10: 2020 2020 2020 2020 202d 2027 7572 6c27           - 'url'
+00007d20: 3a20 7374 7220 6973 2074 6865 2055 524c  : str is the URL
+00007d30: 2074 6f20 6665 7463 6820 7468 6520 6461   to fetch the da
+00007d40: 7461 2066 726f 6d2e 2049 6620 6e6f 7420  ta from. If not 
+00007d50: 7072 6f76 6964 6564 2c20 6974 2064 6566  provided, it def
+00007d60: 6175 6c74 7320 746f 2061 6e20 656d 7074  aults to an empt
+00007d70: 7920 7374 7269 6e67 2e0a 2020 2020 2020  y string..      
+00007d80: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+00007d90: 6c66 2e75 726c 203d 206b 7761 7267 732e  lf.url = kwargs.
+00007da0: 6765 7428 2775 726c 272c 2027 2729 206f  get('url', '') o
+00007db0: 7220 7365 6c66 2e75 726c 0a0a 2020 2020  r self.url..    
+00007dc0: 6465 6620 7370 6964 6572 5f63 6872 6f6d  def spider_chrom
+00007dd0: 655f 6472 6976 6572 2873 656c 6629 202d  e_driver(self) -
+00007de0: 3e20 7765 6264 7269 7665 722e 4368 726f  > webdriver.Chro
+00007df0: 6d65 3a0a 2020 2020 2020 2020 2222 220a  me:.        """.
+00007e00: 2020 2020 2020 2020 496e 6974 6961 6c69          Initiali
+00007e10: 7a65 2061 2043 6872 6f6d 6520 5765 6244  ze a Chrome WebD
+00007e20: 7269 7665 7220 7769 7468 2068 6561 646c  river with headl
+00007e30: 6573 7320 6f70 7469 6f6e 2061 6e64 206e  ess option and n
+00007e40: 6176 6967 6174 6520 746f 2074 6865 2055  avigate to the U
+00007e50: 524c 2e0a 0a20 2020 2020 2020 203a 7265  RL...        :re
+00007e60: 7475 726e 3a20 416e 2069 6e73 7461 6e63  turn: An instanc
+00007e70: 6520 6f66 2043 6872 6f6d 6520 5765 6244  e of Chrome WebD
+00007e80: 7269 7665 722e 0a20 2020 2020 2020 2022  river..        "
+00007e90: 2222 0a20 2020 2020 2020 2023 2049 6d70  "".        # Imp
+00007ea0: 6f72 7420 6272 6f77 7365 7220 636f 6e66  ort browser conf
+00007eb0: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
+00007ec0: 2020 6f70 7469 6f6e 7320 3d20 7765 6264    options = webd
+00007ed0: 7269 7665 722e 4368 726f 6d65 4f70 7469  river.ChromeOpti
+00007ee0: 6f6e 7328 290a 2020 2020 2020 2020 2320  ons().        # 
+00007ef0: 5365 7420 6865 6164 6c65 7373 206d 6f64  Set headless mod
+00007f00: 650a 2020 2020 2020 2020 6f70 7469 6f6e  e.        option
+00007f10: 732e 6164 645f 6172 6775 6d65 6e74 2827  s.add_argument('
+00007f20: 2d2d 6865 6164 6c65 7373 2729 0a20 2020  --headless').   
+00007f30: 2020 2020 2064 7269 7665 7220 3d20 7765       driver = we
+00007f40: 6264 7269 7665 722e 4368 726f 6d65 286f  bdriver.Chrome(o
+00007f50: 7074 696f 6e73 3d6f 7074 696f 6e73 290a  ptions=options).
+00007f60: 2020 2020 2020 2020 6472 6976 6572 2e67          driver.g
+00007f70: 6574 2873 656c 662e 7572 6c29 0a20 2020  et(self.url).   
+00007f80: 2020 2020 2072 6574 7572 6e20 6472 6976       return driv
+00007f90: 6572 0a0a 2020 2020 4061 6273 7472 6163  er..    @abstrac
+00007fa0: 746d 6574 686f 640a 2020 2020 6465 6620  tmethod.    def 
+00007fb0: 7370 6964 6572 5f72 6563 656e 745f 6461  spider_recent_da
+00007fc0: 7461 2873 656c 6629 202d 3e20 4c69 7374  ta(self) -> List
+00007fd0: 5b4c 6973 745b 7374 725d 5d3a 0a20 2020  [List[str]]:.   
+00007fe0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007ff0: 2046 6574 6368 2074 6865 2072 6563 656e   Fetch the recen
+00008000: 7420 6461 7461 2066 726f 6d20 7468 6520  t data from the 
+00008010: 7765 6220 7061 6765 2e0a 0a20 2020 2020  web page...     
+00008020: 2020 203a 7265 7475 726e 3a20 4120 6c69     :return: A li
+00008030: 7374 206f 6620 6c69 7374 7320 636f 6e74  st of lists cont
+00008040: 6169 6e69 6e67 2072 6563 656e 7420 6461  aining recent da
+00008050: 7461 2065 6e74 7269 6573 2e0a 2020 2020  ta entries..    
+00008060: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008070: 6472 6976 6572 203d 2073 656c 662e 7370  driver = self.sp
+00008080: 6964 6572 5f63 6872 6f6d 655f 6472 6976  ider_chrome_driv
+00008090: 6572 2829 0a20 2020 2020 2020 2074 696d  er().        tim
+000080a0: 652e 736c 6565 7028 3129 2020 2320 416c  e.sleep(1)  # Al
+000080b0: 6c6f 7720 7469 6d65 2066 6f72 2074 6865  low time for the
+000080c0: 2070 6167 6520 746f 206c 6f61 640a 2020   page to load.  
+000080d0: 2020 2020 2020 6672 616d 6520 3d20 6472        frame = dr
+000080e0: 6976 6572 2e66 696e 645f 656c 656d 656e  iver.find_elemen
+000080f0: 7428 4279 2e58 5041 5448 2c20 272f 2f69  t(By.XPATH, '//i
+00008100: 6672 616d 655b 4069 643d 2269 4672 616d  frame[@id="iFram
+00008110: 6531 225d 2729 0a20 2020 2020 2020 2064  e1"]').        d
+00008120: 7269 7665 722e 7377 6974 6368 5f74 6f2e  river.switch_to.
+00008130: 6672 616d 6528 6672 616d 6529 0a20 2020  frame(frame).   
+00008140: 2020 2020 2063 6f6e 7465 6e74 203d 2064       content = d
+00008150: 7269 7665 722e 6669 6e64 5f65 6c65 6d65  river.find_eleme
+00008160: 6e74 2842 792e 5850 4154 482c 2027 2f2f  nt(By.XPATH, '//
+00008170: 7462 6f64 795b 4069 643d 2268 6973 746f  tbody[@id="histo
+00008180: 7279 4461 7461 225d 2729 0a20 2020 2020  ryData"]').     
+00008190: 2020 2072 6563 656e 745f 6461 7461 203d     recent_data =
+000081a0: 205b 782e 7370 6c69 7428 2720 2729 5b3a   [x.split(' ')[:
+000081b0: 395d 2066 6f72 2078 2069 6e20 636f 6e74  9] for x in cont
+000081c0: 656e 742e 7465 7874 2e73 706c 6974 2827  ent.text.split('
+000081d0: 5c6e 2729 5d0a 2020 2020 2020 2020 7265  \n')].        re
+000081e0: 7475 726e 2072 6563 656e 745f 6461 7461  turn recent_data
+000081f0: 0a0a 2020 2020 4061 6273 7472 6163 746d  ..    @abstractm
+00008200: 6574 686f 640a 2020 2020 6465 6620 7370  ethod.    def sp
+00008210: 6964 6572 5f6c 6174 6573 745f 6461 7461  ider_latest_data
+00008220: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
+00008230: 616c 5b4c 6973 745b 7374 725d 5d3a 0a20  al[List[str]]:. 
+00008240: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00008250: 2020 2046 6574 6368 2074 6865 206c 6174     Fetch the lat
+00008260: 6573 7420 7369 6e67 6c65 2064 6174 6120  est single data 
+00008270: 656e 7472 792e 0a0a 2020 2020 2020 2020  entry...        
+00008280: 3a72 6574 7572 6e3a 2041 206c 6973 7420  :return: A list 
+00008290: 636f 6e74 6169 6e69 6e67 2074 6865 206c  containing the l
+000082a0: 6174 6573 7420 6461 7461 2065 6e74 7279  atest data entry
+000082b0: 2c20 6f72 204e 6f6e 6520 6966 2074 6865  , or None if the
+000082c0: 7265 2069 7320 6e6f 2064 6174 612e 0a20  re is no data.. 
+000082d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000082e0: 2020 2072 6563 656e 745f 6461 7461 203d     recent_data =
+000082f0: 2073 656c 662e 7370 6964 6572 5f72 6563   self.spider_rec
+00008300: 656e 745f 6461 7461 2829 0a20 2020 2020  ent_data().     
+00008310: 2020 2072 6574 7572 6e20 7265 6365 6e74     return recent
+00008320: 5f64 6174 615b 305d 2069 6620 7265 6365  _data[0] if rece
+00008330: 6e74 5f64 6174 6120 656c 7365 204e 6f6e  nt_data else Non
+00008340: 650a 0a20 2020 2040 6162 7374 7261 6374  e..    @abstract
+00008350: 6d65 7468 6f64 0a20 2020 2064 6566 2073  method.    def s
+00008360: 7069 6465 725f 6675 6c6c 5f64 6174 6128  pider_full_data(
+00008370: 7365 6c66 2920 2d3e 204c 6973 745b 4c69  self) -> List[Li
+00008380: 7374 5b73 7472 5d5d 3a0a 2020 2020 2020  st[str]]:.      
+00008390: 2020 2222 220a 2020 2020 2020 2020 4c6f    """.        Lo
+000083a0: 6164 2074 6865 2066 756c 6c20 7365 7420  ad the full set 
+000083b0: 6f66 2064 6174 6120 6672 6f6d 2074 6865  of data from the
+000083c0: 2073 6f75 7263 652e 0a0a 2020 2020 2020   source...      
+000083d0: 2020 3a72 6574 7572 6e3a 2041 206c 6973    :return: A lis
+000083e0: 7420 6f66 206c 6973 7473 2063 6f6e 7461  t of lists conta
+000083f0: 696e 696e 6720 616c 6c20 6461 7461 2065  ining all data e
+00008400: 6e74 7269 6573 2e0a 2020 2020 2020 2020  ntries..        
+00008410: 2222 220a 2020 2020 2020 2020 2320 5468  """.        # Th
+00008420: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00008430: 2073 686f 756c 6420 6265 2070 726f 7669   should be provi
+00008440: 6465 6420 6279 2074 6865 2073 7562 636c  ded by the subcl
+00008450: 6173 732e 0a20 2020 2020 2020 2066 756c  ass..        ful
+00008460: 6c5f 6461 7461 203d 205b 5d0a 2020 2020  l_data = [].    
+00008470: 2020 2020 6472 6976 6572 203d 2073 656c      driver = sel
+00008480: 662e 7370 6964 6572 5f63 6872 6f6d 655f  f.spider_chrome_
+00008490: 6472 6976 6572 2829 0a20 2020 2020 2020  driver().       
+000084a0: 2074 696d 652e 736c 6565 7028 3129 2020   time.sleep(1)  
+000084b0: 2320 416c 6c6f 7720 7469 6d65 2066 6f72  # Allow time for
+000084c0: 2074 6865 2070 6167 6520 746f 206c 6f61   the page to loa
+000084d0: 640a 2020 2020 2020 2020 6672 616d 6520  d.        frame 
+000084e0: 3d20 6472 6976 6572 2e66 696e 645f 656c  = driver.find_el
+000084f0: 656d 656e 7428 4279 2e58 5041 5448 2c20  ement(By.XPATH, 
+00008500: 272f 2f69 6672 616d 655b 4069 643d 2269  '//iframe[@id="i
+00008510: 4672 616d 6531 225d 2729 0a20 2020 2020  Frame1"]').     
+00008520: 2020 2064 7269 7665 722e 7377 6974 6368     driver.switch
+00008530: 5f74 6f2e 6672 616d 6528 6672 616d 6529  _to.frame(frame)
+00008540: 0a20 2020 2020 2020 206d 6174 6368 6573  .        matches
+00008550: 203d 2072 652e 6669 6e64 616c 6c28 7227   = re.findall(r'
+00008560: 676f 4e65 7874 5061 6765 5c28 285c 642b  goNextPage\((\d+
+00008570: 295c 2927 2c20 6472 6976 6572 2e70 6167  )\)', driver.pag
+00008580: 655f 736f 7572 6365 290a 2020 2020 2020  e_source).      
+00008590: 2020 7061 6765 5f69 6e64 6578 203d 205b    page_index = [
+000085a0: 696e 7428 6d61 7463 6829 2066 6f72 206d  int(match) for m
+000085b0: 6174 6368 2069 6e20 6d61 7463 6865 735d  atch in matches]
+000085c0: 0a20 2020 2020 2020 2066 6f72 2069 6e64  .        for ind
+000085d0: 6578 2069 6e20 7261 6e67 6528 6d61 7828  ex in range(max(
+000085e0: 7061 6765 5f69 6e64 6578 2929 3a0a 2020  page_index)):.  
+000085f0: 2020 2020 2020 2020 2020 2320 7761 6974            # wait
+00008600: 2064 6174 6120 6c6f 6164 0a20 2020 2020   data load.     
+00008610: 2020 2020 2020 2057 6562 4472 6976 6572         WebDriver
+00008620: 5761 6974 2864 7269 7665 722c 2031 3029  Wait(driver, 10)
+00008630: 2e75 6e74 696c 280a 2020 2020 2020 2020  .until(.        
+00008640: 2020 2020 2020 2020 4543 2e70 7265 7365          EC.prese
+00008650: 6e63 655f 6f66 5f65 6c65 6d65 6e74 5f6c  nce_of_element_l
+00008660: 6f63 6174 6564 2828 4279 2e58 5041 5448  ocated((By.XPATH
+00008670: 2c20 272f 2f74 626f 6479 5b40 6964 3d22  , '//tbody[@id="
+00008680: 6869 7374 6f72 7944 6174 6122 5d27 2929  historyData"]'))
+00008690: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+000086a0: 2020 2020 2020 2020 2020 2020 2320 6578              # ex
+000086b0: 7472 6163 7420 6461 7461 0a20 2020 2020  tract data.     
+000086c0: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
+000086d0: 2064 7269 7665 722e 6669 6e64 5f65 6c65   driver.find_ele
+000086e0: 6d65 6e74 2842 792e 5850 4154 482c 2027  ment(By.XPATH, '
+000086f0: 2f2f 7462 6f64 795b 4069 643d 2268 6973  //tbody[@id="his
+00008700: 746f 7279 4461 7461 225d 2729 0a20 2020  toryData"]').   
+00008710: 2020 2020 2020 2020 2066 756c 6c5f 6461           full_da
+00008720: 7461 2e65 7874 656e 6428 5b78 2e73 706c  ta.extend([x.spl
+00008730: 6974 2829 5b3a 395d 2066 6f72 2078 2069  it()[:9] for x i
+00008740: 6e20 636f 6e74 656e 742e 7465 7874 2e73  n content.text.s
+00008750: 706c 6974 2827 5c6e 2729 2069 6620 6c65  plit('\n') if le
+00008760: 6e28 782e 7370 6c69 7428 2929 203e 3d20  n(x.split()) >= 
+00008770: 395d 290a 0a20 2020 2020 2020 2020 2020  9])..           
+00008780: 2023 2077 6169 7420 6e65 7874 2070 6167   # wait next pag
+00008790: 6520 6c6f 6164 0a20 2020 2020 2020 2020  e load.         
+000087a0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000087b0: 2020 2020 2020 2020 2320 7472 7920 746f          # try to
+000087c0: 2066 696e 6420 656c 656d 656e 7420 6f66   find element of
+000087d0: 2070 6f73 6974 696f 6e20 3d3d 2031 330a   position == 13.
+000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087f0: 6e65 7874 5f62 7574 746f 6e20 3d20 5765  next_button = We
+00008800: 6244 7269 7665 7257 6169 7428 6472 6976  bDriverWait(driv
+00008810: 6572 2c20 3130 292e 756e 7469 6c28 0a20  er, 10).until(. 
+00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008830: 2020 2045 432e 656c 656d 656e 745f 746f     EC.element_to
+00008840: 5f62 655f 636c 6963 6b61 626c 6528 2842  _be_clickable((B
+00008850: 792e 5850 4154 482c 2022 2f68 746d 6c2f  y.XPATH, "/html/
+00008860: 626f 6479 2f64 6976 2f64 6976 2f64 6976  body/div/div/div
+00008870: 5b33 5d2f 756c 2f6c 695b 706f 7369 7469  [3]/ul/li[positi
+00008880: 6f6e 2829 3d31 335d 2229 290a 2020 2020  on()=13]")).    
+00008890: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000088a0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+000088b0: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
+000088c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000088d0: 2020 2320 7472 7920 746f 2066 696e 6420    # try to find 
+000088e0: 656c 656d 656e 7420 6f66 2070 6f73 6974  element of posit
+000088f0: 696f 6e20 3d3d 2038 0a20 2020 2020 2020  ion == 8.       
+00008900: 2020 2020 2020 2020 206e 6578 745f 6275           next_bu
+00008910: 7474 6f6e 203d 2057 6562 4472 6976 6572  tton = WebDriver
+00008920: 5761 6974 2864 7269 7665 722c 2031 3029  Wait(driver, 10)
+00008930: 2e75 6e74 696c 280a 2020 2020 2020 2020  .until(.        
+00008940: 2020 2020 2020 2020 2020 2020 4543 2e65              EC.e
+00008950: 6c65 6d65 6e74 5f74 6f5f 6265 5f63 6c69  lement_to_be_cli
+00008960: 636b 6162 6c65 2828 4279 2e58 5041 5448  ckable((By.XPATH
+00008970: 2c20 222f 6874 6d6c 2f62 6f64 792f 6469  , "/html/body/di
+00008980: 762f 6469 762f 6469 765b 335d 2f75 6c2f  v/div/div[3]/ul/
+00008990: 6c69 5b70 6f73 6974 696f 6e28 293d 385d  li[position()=8]
+000089a0: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+000089b0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+000089c0: 2020 2023 2063 6c69 636b 2074 6f20 6e65     # click to ne
+000089d0: 7874 2070 6167 650a 2020 2020 2020 2020  xt page.        
+000089e0: 2020 2020 6e65 7874 5f62 7574 746f 6e2e      next_button.
+000089f0: 636c 6963 6b28 290a 2020 2020 2020 2020  click().        
+00008a00: 2020 2020 7469 6d65 2e73 6c65 6570 2833      time.sleep(3
+00008a10: 2920 2023 206c 6f61 6469 6e67 0a20 2020  )  # loading.   
+00008a20: 2020 2020 2064 7269 7665 722e 7175 6974       driver.quit
+00008a30: 2829 0a20 2020 2020 2020 2073 6f72 7465  ().        sorte
+00008a40: 645f 6675 6c6c 5f64 6174 6120 3d20 736f  d_full_data = so
+00008a50: 7274 6564 2866 756c 6c5f 6461 7461 2c20  rted(full_data, 
+00008a60: 6b65 793d 6c61 6d62 6461 2078 3a20 696e  key=lambda x: in
+00008a70: 7428 785b 305d 2929 0a0a 2020 2020 2020  t(x[0]))..      
+00008a80: 2020 7265 7475 726e 2073 6f72 7465 645f    return sorted_
+00008a90: 6675 6c6c 5f64 6174 610a 0a0a 636c 6173  full_data...clas
+00008aa0: 7320 4361 6c63 756c 6174 6555 7469 6c28  s CalculateUtil(
+00008ab0: 4142 4329 3a0a 2020 2020 2222 220a 2020  ABC):.    """.  
+00008ac0: 2020 436f 6d70 7574 6520 6665 6174 7572    Compute featur
+00008ad0: 6573 2062 6173 6564 206f 6e20 6120 7369  es based on a si
+00008ae0: 6e67 6c65 206f 7220 6d75 6c74 6920 6f66  ngle or multi of
+00008af0: 2064 6174 610a 2020 2020 2222 220a 2020   data.    """.  
+00008b00: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+00008b10: 2020 2020 6465 6620 7265 616c 5f72 6f75      def real_rou
+00008b20: 6e64 286e 293a 0a20 2020 2020 2020 2022  nd(n):.        "
+00008b30: 2222 0a20 2020 2020 2020 2043 7573 746f  "".        Custo
+00008b40: 6d20 726f 756e 6469 6e67 2066 756e 6374  m rounding funct
+00008b50: 696f 6e2e 0a0a 2020 2020 2020 2020 5061  ion...        Pa
+00008b60: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+00008b70: 2020 6e20 2866 6c6f 6174 293a 2054 6865    n (float): The
+00008b80: 206e 756d 6265 7220 746f 2072 6f75 6e64   number to round
+00008b90: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00008ba0: 6e73 3a0a 2020 2020 2020 2020 696e 743a  ns:.        int:
+00008bb0: 2054 6865 2072 6f75 6e64 6564 2072 6573   The rounded res
+00008bc0: 756c 742e 0a20 2020 2020 2020 2022 2222  ult..        """
+00008bd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008be0: 6d61 7468 2e66 6c6f 6f72 286e 202b 2030  math.floor(n + 0
+00008bf0: 2e35 290a 0a20 2020 2040 7374 6174 6963  .5)..    @static
+00008c00: 6d65 7468 6f64 0a20 2020 2064 6566 2069  method.    def i
+00008c10: 6e76 6572 745f 726f 756e 6428 6e29 3a0a  nvert_round(n):.
+00008c20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008c30: 2020 2020 4375 7374 6f6d 2072 6f75 6e64      Custom round
+00008c40: 696e 6720 6675 6e63 7469 6f6e 2077 6865  ing function whe
+00008c50: 7265 3a0a 2020 2020 2020 2020 2d20 5661  re:.        - Va
+00008c60: 6c75 6573 2077 6974 6820 6465 6369 6d61  lues with decima
+00008c70: 6c20 7061 7274 206c 6573 7320 7468 616e  l part less than
+00008c80: 2030 2e35 2061 7265 2072 6f75 6e64 6564   0.5 are rounded
+00008c90: 2075 702e 0a20 2020 2020 2020 202d 2056   up..        - V
+00008ca0: 616c 7565 7320 7769 7468 2064 6563 696d  alues with decim
+00008cb0: 616c 2070 6172 7420 6578 6163 746c 7920  al part exactly 
+00008cc0: 302e 3520 6172 6520 726f 756e 6465 6420  0.5 are rounded 
+00008cd0: 646f 776e 2e0a 0a20 2020 2020 2020 2050  down...        P
+00008ce0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+00008cf0: 2020 206e 2028 666c 6f61 7429 3a20 5468     n (float): Th
+00008d00: 6520 6e75 6d62 6572 2074 6f20 726f 756e  e number to roun
+00008d10: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
+00008d20: 726e 733a 0a20 2020 2020 2020 2069 6e74  rns:.        int
+00008d30: 3a20 5468 6520 726f 756e 6465 6420 7265  : The rounded re
+00008d40: 7375 6c74 2e0a 2020 2020 2020 2020 2222  sult..        ""
+00008d50: 220a 2020 2020 2020 2020 6966 206e 2025  ".        if n %
+00008d60: 2031 203e 3d20 302e 353a 0a20 2020 2020   1 >= 0.5:.     
+00008d70: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
+00008d80: 7468 2e66 6c6f 6f72 286e 290a 2020 2020  th.floor(n).    
+00008d90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008da0: 2020 2020 2020 7265 7475 726e 206d 6174        return mat
+00008db0: 682e 6365 696c 286e 290a 0a20 2020 2040  h.ceil(n)..    @
+00008dc0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+00008dd0: 2064 6566 206c 6f6e 6765 7374 5f69 6e63   def longest_inc
+00008de0: 7265 6173 696e 675f 7375 6273 6571 7565  reasing_subseque
+00008df0: 6e63 6528 6e75 6d65 7269 635f 7365 7175  nce(numeric_sequ
+00008e00: 656e 6365 3a20 4c69 7374 5b69 6e74 5d29  ence: List[int])
+00008e10: 202d 3e20 4c69 7374 5b69 6e74 5d3a 0a20   -> List[int]:. 
+00008e20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00008e30: 2020 2046 696e 6473 2074 6865 206c 6f6e     Finds the lon
+00008e40: 6765 7374 2069 6e63 7265 6173 696e 6720  gest increasing 
+00008e50: 7375 6273 6571 7565 6e63 6520 696e 2061  subsequence in a
+00008e60: 2067 6976 656e 206e 756d 6572 6963 2073   given numeric s
+00008e70: 6571 7565 6e63 652e 0a0a 2020 2020 2020  equence...      
+00008e80: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00008e90: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
+00008ea0: 2028 4c69 7374 5b69 6e74 5d29 3a20 5468   (List[int]): Th
+00008eb0: 6520 696e 7075 7420 6c69 7374 206f 6620  e input list of 
+00008ec0: 696e 7465 6765 7273 2e0a 0a20 2020 2020  integers...     
+00008ed0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00008ee0: 2020 2020 4c69 7374 5b69 6e74 5d3a 2054      List[int]: T
+00008ef0: 6865 206c 6f6e 6765 7374 2069 6e63 7265  he longest incre
+00008f00: 6173 696e 6720 7375 6273 6571 7565 6e63  asing subsequenc
+00008f10: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00008f20: 2020 2020 2020 206e 203d 206c 656e 286e         n = len(n
+00008f30: 756d 6572 6963 5f73 6571 7565 6e63 6529  umeric_sequence)
+00008f40: 0a20 2020 2020 2020 2064 7020 3d20 5b31  .        dp = [1
+00008f50: 5d20 2a20 6e0a 0a20 2020 2020 2020 2023  ] * n..        #
+00008f60: 2046 696c 6c20 6470 2061 7272 6179 2077   Fill dp array w
+00008f70: 6974 6820 6c65 6e67 7468 7320 6f66 204c  ith lengths of L
+00008f80: 4953 2065 6e64 696e 6720 6174 2065 6163  IS ending at eac
+00008f90: 6820 696e 6465 780a 2020 2020 2020 2020  h index.        
+00008fa0: 666f 7220 6920 696e 2072 616e 6765 2831  for i in range(1
+00008fb0: 2c20 6e29 3a0a 2020 2020 2020 2020 2020  , n):.          
+00008fc0: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+00008fd0: 2830 2c20 6929 3a0a 2020 2020 2020 2020  (0, i):.        
+00008fe0: 2020 2020 2020 2020 6966 206e 756d 6572          if numer
+00008ff0: 6963 5f73 6571 7565 6e63 655b 695d 203e  ic_sequence[i] >
+00009000: 206e 756d 6572 6963 5f73 6571 7565 6e63   numeric_sequenc
+00009010: 655b 6a5d 3a0a 2020 2020 2020 2020 2020  e[j]:.          
+00009020: 2020 2020 2020 2020 2020 6470 5b69 5d20            dp[i] 
+00009030: 3d20 6d61 7828 6470 5b69 5d2c 2064 705b  = max(dp[i], dp[
+00009040: 6a5d 202b 2031 290a 0a20 2020 2020 2020  j] + 1)..       
+00009050: 206c 6973 5f6c 656e 6774 6820 3d20 6d61   lis_length = ma
+00009060: 7828 6470 290a 2020 2020 2020 2020 6c69  x(dp).        li
+00009070: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
+00009080: 2320 4669 6e64 2074 6865 2069 6e64 6578  # Find the index
+00009090: 206f 6620 7468 6520 6d61 7869 6d75 6d20   of the maximum 
+000090a0: 7661 6c75 6520 696e 2064 7020 6172 7261  value in dp arra
+000090b0: 790a 2020 2020 2020 2020 6d61 785f 696e  y.        max_in
+000090c0: 6465 7820 3d20 6470 2e69 6e64 6578 286c  dex = dp.index(l
+000090d0: 6973 5f6c 656e 6774 6829 0a20 2020 2020  is_length).     
+000090e0: 2020 206c 6973 2e61 7070 656e 6428 6e75     lis.append(nu
+000090f0: 6d65 7269 635f 7365 7175 656e 6365 5b6d  meric_sequence[m
+00009100: 6178 5f69 6e64 6578 5d29 0a20 2020 2020  ax_index]).     
+00009110: 2020 2063 7572 7265 6e74 5f6c 656e 6774     current_lengt
+00009120: 6820 3d20 6c69 735f 6c65 6e67 7468 202d  h = lis_length -
+00009130: 2031 0a0a 2020 2020 2020 2020 2320 5472   1..        # Tr
+00009140: 6163 6520 6261 636b 2074 6865 2073 6571  ace back the seq
+00009150: 7565 6e63 6520 746f 2066 696e 6420 7468  uence to find th
+00009160: 6520 4c49 530a 2020 2020 2020 2020 666f  e LIS.        fo
+00009170: 7220 6920 696e 2072 616e 6765 286d 6178  r i in range(max
+00009180: 5f69 6e64 6578 202d 2031 2c20 2d31 2c20  _index - 1, -1, 
+00009190: 2d31 293a 0a20 2020 2020 2020 2020 2020  -1):.           
+000091a0: 2069 6620 6470 5b69 5d20 3d3d 2063 7572   if dp[i] == cur
+000091b0: 7265 6e74 5f6c 656e 6774 6820 616e 6420  rent_length and 
+000091c0: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
+000091d0: 5b69 5d20 3c20 6c69 735b 2d31 5d3a 0a20  [i] < lis[-1]:. 
+000091e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000091f0: 6973 2e61 7070 656e 6428 6e75 6d65 7269  is.append(numeri
+00009200: 635f 7365 7175 656e 6365 5b69 5d29 0a20  c_sequence[i]). 
+00009210: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009220: 7572 7265 6e74 5f6c 656e 6774 6820 2d3d  urrent_length -=
+00009230: 2031 0a0a 2020 2020 2020 2020 7265 7475   1..        retu
+00009240: 726e 206c 6973 7428 7265 7665 7273 6564  rn list(reversed
+00009250: 286c 6973 2929 0a0a 2020 2020 4073 7461  (lis))..    @sta
+00009260: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
+00009270: 6620 6c6f 6e67 6573 745f 6465 6372 6561  f longest_decrea
+00009280: 7369 6e67 5f73 7562 7365 7175 656e 6365  sing_subsequence
+00009290: 286e 756d 6572 6963 5f73 6571 7565 6e63  (numeric_sequenc
+000092a0: 653a 204c 6973 745b 696e 745d 2920 2d3e  e: List[int]) ->
+000092b0: 204c 6973 745b 696e 745d 3a0a 2020 2020   List[int]:.    
+000092c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000092d0: 4669 6e64 7320 7468 6520 6c6f 6e67 6573  Finds the longes
+000092e0: 7420 6465 6372 6561 7369 6e67 2073 7562  t decreasing sub
+000092f0: 7365 7175 656e 6365 2069 6e20 6120 6769  sequence in a gi
+00009300: 7665 6e20 6e75 6d65 7269 6320 7365 7175  ven numeric sequ
+00009310: 656e 6365 2e0a 0a20 2020 2020 2020 2041  ence...        A
+00009320: 7267 733a 0a20 2020 2020 2020 206e 756d  rgs:.        num
+00009330: 6572 6963 5f73 6571 7565 6e63 6520 284c  eric_sequence (L
+00009340: 6973 745b 696e 745d 293a 2054 6865 2069  ist[int]): The i
+00009350: 6e70 7574 206c 6973 7420 6f66 2069 6e74  nput list of int
+00009360: 6567 6572 732e 0a0a 2020 2020 2020 2020  egers...        
+00009370: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00009380: 204c 6973 745b 696e 745d 3a20 5468 6520   List[int]: The 
+00009390: 6c6f 6e67 6573 7420 6465 6372 6561 7369  longest decreasi
+000093a0: 6e67 2073 7562 7365 7175 656e 6365 2e0a  ng subsequence..
+000093b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000093c0: 2020 2020 6e20 3d20 6c65 6e28 6e75 6d65      n = len(nume
+000093d0: 7269 635f 7365 7175 656e 6365 290a 2020  ric_sequence).  
+000093e0: 2020 2020 2020 6470 203d 205b 315d 202a        dp = [1] *
+000093f0: 206e 0a0a 2020 2020 2020 2020 2320 4669   n..        # Fi
+00009400: 6c6c 2064 7020 6172 7261 7920 7769 7468  ll dp array with
+00009410: 206c 656e 6774 6873 206f 6620 4c44 5320   lengths of LDS 
+00009420: 656e 6469 6e67 2061 7420 6561 6368 2069  ending at each i
+00009430: 6e64 6578 0a20 2020 2020 2020 2066 6f72  ndex.        for
+00009440: 2069 2069 6e20 7261 6e67 6528 312c 206e   i in range(1, n
+00009450: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+00009460: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+00009470: 2069 293a 0a20 2020 2020 2020 2020 2020   i):.           
+00009480: 2020 2020 2069 6620 6e75 6d65 7269 635f       if numeric_
+00009490: 7365 7175 656e 6365 5b69 5d20 3c20 6e75  sequence[i] < nu
+000094a0: 6d65 7269 635f 7365 7175 656e 6365 5b6a  meric_sequence[j
+000094b0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+000094c0: 2020 2020 2020 2064 705b 695d 203d 206d         dp[i] = m
+000094d0: 6178 2864 705b 695d 2c20 6470 5b6a 5d20  ax(dp[i], dp[j] 
+000094e0: 2b20 3129 0a0a 2020 2020 2020 2020 6c64  + 1)..        ld
+000094f0: 735f 6c65 6e67 7468 203d 206d 6178 2864  s_length = max(d
+00009500: 7029 0a20 2020 2020 2020 206c 6473 203d  p).        lds =
+00009510: 205b 5d0a 0a20 2020 2020 2020 2023 2046   []..        # F
+00009520: 696e 6420 7468 6520 696e 6465 7820 6f66  ind the index of
+00009530: 2074 6865 206d 6178 696d 756d 2076 616c   the maximum val
+00009540: 7565 2069 6e20 6470 2061 7272 6179 0a20  ue in dp array. 
+00009550: 2020 2020 2020 206d 6178 5f69 6e64 6578         max_index
+00009560: 203d 2064 702e 696e 6465 7828 6c64 735f   = dp.index(lds_
+00009570: 6c65 6e67 7468 290a 2020 2020 2020 2020  length).        
+00009580: 6c64 732e 6170 7065 6e64 286e 756d 6572  lds.append(numer
+00009590: 6963 5f73 6571 7565 6e63 655b 6d61 785f  ic_sequence[max_
+000095a0: 696e 6465 785d 290a 2020 2020 2020 2020  index]).        
+000095b0: 6375 7272 656e 745f 6c65 6e67 7468 203d  current_length =
+000095c0: 206c 6473 5f6c 656e 6774 6820 2d20 310a   lds_length - 1.
+000095d0: 0a20 2020 2020 2020 2023 2054 7261 6365  .        # Trace
+000095e0: 2062 6163 6b20 7468 6520 7365 7175 656e   back the sequen
+000095f0: 6365 2074 6f20 6669 6e64 2074 6865 204c  ce to find the L
+00009600: 4453 0a20 2020 2020 2020 2066 6f72 2069  DS.        for i
+00009610: 2069 6e20 7261 6e67 6528 6d61 785f 696e   in range(max_in
+00009620: 6465 7820 2d20 312c 202d 312c 202d 3129  dex - 1, -1, -1)
+00009630: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00009640: 2064 705b 695d 203d 3d20 6375 7272 656e   dp[i] == curren
+00009650: 745f 6c65 6e67 7468 2061 6e64 206e 756d  t_length and num
+00009660: 6572 6963 5f73 6571 7565 6e63 655b 695d  eric_sequence[i]
+00009670: 203e 206c 6473 5b2d 315d 3a0a 2020 2020   > lds[-1]:.    
+00009680: 2020 2020 2020 2020 2020 2020 6c64 732e              lds.
+00009690: 6170 7065 6e64 286e 756d 6572 6963 5f73  append(numeric_s
+000096a0: 6571 7565 6e63 655b 695d 290a 2020 2020  equence[i]).    
+000096b0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000096c0: 656e 745f 6c65 6e67 7468 202d 3d20 310a  ent_length -= 1.
+000096d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000096e0: 6c69 7374 2872 6576 6572 7365 6428 6c64  list(reversed(ld
+000096f0: 7329 290a 0a20 2020 2040 7374 6174 6963  s))..    @static
+00009700: 6d65 7468 6f64 0a20 2020 2064 6566 2067  method.    def g
+00009710: 656e 6572 6174 655f 6461 7461 7365 7473  enerate_datasets
+00009720: 5f77 6974 685f 726f 6c6c 696e 675f 7369  _with_rolling_si
+00009730: 7a65 2864 6174 613a 204c 6973 745b 696e  ze(data: List[in
+00009740: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
+00009750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009770: 726f 6c6c 696e 675f 7369 7a65 3a20 696e  rolling_size: in
+00009780: 7420 3d20 352c 0a20 2020 2020 2020 2020  t = 5,.         
+00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097b0: 2020 2061 646a 7573 743a 2062 6f6f 6c20     adjust: bool 
+000097c0: 3d20 4661 6c73 6529 202d 3e20 5475 706c  = False) -> Tupl
+000097d0: 655b 4c69 7374 5b4c 6973 745b 696e 745d  e[List[List[int]
+000097e0: 5d2c 204c 6973 745b 696e 745d 5d3a 0a20  ], List[int]]:. 
+000097f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00009800: 2020 2047 656e 6572 6174 6573 2073 6571     Generates seq
+00009810: 7565 6e74 6961 6c20 7465 7374 2061 6e64  uential test and
+00009820: 2076 616c 6964 6174 696f 6e20 6461 7461   validation data
+00009830: 7365 7473 2066 726f 6d20 6120 6c69 7374  sets from a list
+00009840: 206f 6620 696e 7465 6765 7273 2e20 4974   of integers. It
+00009850: 206f 7074 696f 6e61 6c6c 7920 6164 6a75   optionally adju
+00009860: 7374 730a 2020 2020 2020 2020 7465 7374  sts.        test
+00009870: 2064 6174 6173 6574 7320 6279 2072 656d   datasets by rem
+00009880: 6f76 696e 6720 6578 7472 656d 6520 7661  oving extreme va
+00009890: 6c75 6573 2e0a 0a20 2020 2020 2020 2054  lues...        T
+000098a0: 6865 2066 756e 6374 696f 6e20 6974 6572  he function iter
+000098b0: 6174 6573 206f 7665 7220 7468 6520 6461  ates over the da
+000098c0: 7461 2074 6f20 6372 6561 7465 206f 7665  ta to create ove
+000098d0: 726c 6170 7069 6e67 2074 6573 7420 7365  rlapping test se
+000098e0: 7473 206f 6620 6120 7370 6563 6966 6965  ts of a specifie
+000098f0: 6420 7369 7a65 2e20 4561 6368 2074 6573  d size. Each tes
+00009900: 7420 7365 7420 6973 0a20 2020 2020 2020  t set is.       
+00009910: 2066 6f6c 6c6f 7765 6420 6279 2061 2076   followed by a v
+00009920: 616c 6964 6174 696f 6e20 7365 7420 7768  alidation set wh
+00009930: 6963 6820 6973 2074 6865 206e 6578 7420  ich is the next 
+00009940: 7369 6e67 6c65 2065 6c65 6d65 6e74 2069  single element i
+00009950: 6e20 7468 6520 6c69 7374 2e20 4966 2074  n the list. If t
+00009960: 6865 2027 6164 6a75 7374 2720 666c 6167  he 'adjust' flag
+00009970: 2069 7320 5472 7565 2c0a 2020 2020 2020   is True,.      
+00009980: 2020 7468 6520 6d61 7869 6d75 6d20 616e    the maximum an
+00009990: 6420 6d69 6e69 6d75 6d20 7661 6c75 6573  d minimum values
+000099a0: 2061 7265 2072 656d 6f76 6564 2066 726f   are removed fro
+000099b0: 6d20 6561 6368 2074 6573 7420 7365 742e  m each test set.
+000099c0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000099d0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000099e0: 2028 4c69 7374 5b69 6e74 5d29 3a20 5468   (List[int]): Th
+000099f0: 6520 696e 7075 7420 6461 7461 206c 6973  e input data lis
+00009a00: 7420 6672 6f6d 2077 6869 6368 2064 6174  t from which dat
+00009a10: 6173 6574 7320 6172 6520 6765 6e65 7261  asets are genera
+00009a20: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
+00009a30: 2072 6f6c 6c69 6e67 5f73 697a 6520 2869   rolling_size (i
+00009a40: 6e74 293a 2054 6865 206e 756d 6265 7220  nt): The number 
+00009a50: 6f66 2065 6c65 6d65 6e74 7320 696e 2065  of elements in e
+00009a60: 6163 6820 7465 7374 2073 6574 2e20 4465  ach test set. De
+00009a70: 6661 756c 7473 2074 6f20 352e 0a20 2020  faults to 5..   
+00009a80: 2020 2020 2020 2020 2061 646a 7573 7420           adjust 
+00009a90: 2862 6f6f 6c29 3a20 5768 6574 6865 7220  (bool): Whether 
+00009aa0: 746f 2072 656d 6f76 6520 7468 6520 6d61  to remove the ma
+00009ab0: 7869 6d75 6d20 616e 6420 6d69 6e69 6d75  ximum and minimu
+00009ac0: 6d20 7661 6c75 6573 2066 726f 6d20 6561  m values from ea
+00009ad0: 6368 2074 6573 7420 7365 742e 2044 6566  ch test set. Def
+00009ae0: 6175 6c74 7320 746f 2046 616c 7365 2e0a  aults to False..
+00009af0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00009b00: 3a0a 2020 2020 2020 2020 2020 2020 5475  :.            Tu
+00009b10: 706c 655b 4c69 7374 5b4c 6973 745b 696e  ple[List[List[in
+00009b20: 745d 5d2c 204c 6973 745b 696e 745d 5d3a  t]], List[int]]:
+00009b30: 2041 2074 7570 6c65 2063 6f6e 7461 696e   A tuple contain
+00009b40: 696e 6720 7477 6f20 6c69 7374 733a 0a20  ing two lists:. 
+00009b50: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00009b60: 2054 6865 2066 6972 7374 206c 6973 7420   The first list 
+00009b70: 636f 6e74 6169 6e73 2074 6865 2074 6573  contains the tes
+00009b80: 7420 7365 7473 2c20 706f 7373 6962 6c79  t sets, possibly
+00009b90: 2061 646a 7573 7465 642e 0a20 2020 2020   adjusted..     
+00009ba0: 2020 2020 2020 2020 2020 202d 2054 6865             - The
+00009bb0: 2073 6563 6f6e 6420 6c69 7374 2063 6f6e   second list con
+00009bc0: 7461 696e 7320 7468 6520 7369 6e67 6c65  tains the single
+00009bd0: 2d65 6c65 6d65 6e74 2076 616c 6964 6174  -element validat
+00009be0: 696f 6e20 7365 7473 2e0a 2020 2020 2020  ion sets..      
+00009bf0: 2020 2222 220a 2020 2020 2020 2020 785f    """.        x_
+00009c00: 7365 7473 203d 205b 5d20 2023 204c 6973  sets = []  # Lis
+00009c10: 7420 746f 2068 6f6c 6420 7468 6520 7465  t to hold the te
+00009c20: 7374 2073 6574 730a 2020 2020 2020 2020  st sets.        
+00009c30: 795f 7365 7473 203d 205b 5d20 2023 204c  y_sets = []  # L
+00009c40: 6973 7420 746f 2068 6f6c 6420 7468 6520  ist to hold the 
+00009c50: 7661 6c69 6461 7469 6f6e 2073 6574 730a  validation sets.
+00009c60: 0a20 2020 2020 2020 2023 2049 7465 7261  .        # Itera
+00009c70: 7465 206f 7665 7220 7468 6520 6461 7461  te over the data
+00009c80: 2074 6f20 666f 726d 2074 6573 7420 616e   to form test an
+00009c90: 6420 7661 6c69 6461 7469 6f6e 2073 6574  d validation set
+00009ca0: 730a 2020 2020 2020 2020 666f 7220 6920  s.        for i 
+00009cb0: 696e 2072 616e 6765 286c 656e 2864 6174  in range(len(dat
+00009cc0: 6129 202d 2072 6f6c 6c69 6e67 5f73 697a  a) - rolling_siz
+00009cd0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00009ce0: 7465 7374 5f73 6574 203d 2064 6174 615b  test_set = data[
+00009cf0: 693a 6920 2b20 726f 6c6c 696e 675f 7369  i:i + rolling_si
+00009d00: 7a65 5d20 2023 2045 7874 7261 6374 2073  ze]  # Extract s
+00009d10: 697a 6520 656c 656d 656e 7473 2066 6f72  ize elements for
+00009d20: 2074 6865 2074 6573 7420 7365 740a 2020   the test set.  
+00009d30: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
+00009d40: 7469 6f6e 5f73 6574 203d 2064 6174 615b  tion_set = data[
+00009d50: 6920 2b20 726f 6c6c 696e 675f 7369 7a65  i + rolling_size
+00009d60: 5d20 2023 2054 616b 6520 7468 6520 6e65  ]  # Take the ne
+00009d70: 7874 2065 6c65 6d65 6e74 2061 7320 7468  xt element as th
+00009d80: 6520 7661 6c69 6461 7469 6f6e 2073 6574  e validation set
+00009d90: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00009da0: 206c 656e 2874 6573 745f 7365 7429 203e   len(test_set) >
+00009db0: 2032 2061 6e64 2061 646a 7573 743a 0a20   2 and adjust:. 
+00009dc0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00009dd0: 2052 656d 6f76 6520 7468 6520 6d61 7869   Remove the maxi
+00009de0: 6d75 6d20 616e 6420 6d69 6e69 6d75 6d20  mum and minimum 
+00009df0: 7661 6c75 6573 2069 6620 6164 6a75 7374  values if adjust
+00009e00: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00009e10: 2020 2020 6d61 785f 7661 6c20 3d20 6d61      max_val = ma
+00009e20: 7828 7465 7374 5f73 6574 290a 2020 2020  x(test_set).    
+00009e30: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
+00009e40: 7661 6c20 3d20 6d69 6e28 7465 7374 5f73  val = min(test_s
+00009e50: 6574 290a 2020 2020 2020 2020 2020 2020  et).            
+00009e60: 2020 2020 6d61 785f 696e 6465 7820 3d20      max_index = 
+00009e70: 7465 7374 5f73 6574 2e69 6e64 6578 286d  test_set.index(m
+00009e80: 6178 5f76 616c 290a 2020 2020 2020 2020  ax_val).        
+00009e90: 2020 2020 2020 2020 6d69 6e5f 696e 6465          min_inde
+00009ea0: 7820 3d20 7465 7374 5f73 6574 2e69 6e64  x = test_set.ind
+00009eb0: 6578 286d 696e 5f76 616c 290a 2020 2020  ex(min_val).    
+00009ec0: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+00009ed0: 6572 6564 5f74 6573 745f 7365 7420 3d20  ered_test_set = 
+00009ee0: 5b78 2066 6f72 2069 6478 2c20 7820 696e  [x for idx, x in
+00009ef0: 2065 6e75 6d65 7261 7465 2874 6573 745f   enumerate(test_
+00009f00: 7365 7429 2069 6620 6964 7820 213d 206d  set) if idx != m
+00009f10: 6178 5f69 6e64 6578 2061 6e64 2069 6478  ax_index and idx
+00009f20: 2021 3d20 6d69 6e5f 696e 6465 785d 0a20   != min_index]. 
+00009f30: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00009f40: 5f73 6574 732e 6170 7065 6e64 2866 696c  _sets.append(fil
+00009f50: 7465 7265 645f 7465 7374 5f73 6574 290a  tered_test_set).
+00009f60: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00009f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009f80: 2020 785f 7365 7473 2e61 7070 656e 6428    x_sets.append(
+00009f90: 7465 7374 5f73 6574 2920 2023 2041 7070  test_set)  # App
+00009fa0: 656e 6420 7468 6520 7465 7374 2073 6574  end the test set
+00009fb0: 2061 7320 6973 2069 6620 6e6f 7420 6164   as is if not ad
+00009fc0: 6a75 7374 696e 670a 0a20 2020 2020 2020  justing..       
+00009fd0: 2020 2020 2079 5f73 6574 732e 6170 7065       y_sets.appe
+00009fe0: 6e64 2876 616c 6964 6174 696f 6e5f 7365  nd(validation_se
+00009ff0: 7429 2020 2320 4170 7065 6e64 2074 6865  t)  # Append the
+0000a000: 2076 616c 6964 6174 696f 6e20 656c 656d   validation elem
+0000a010: 656e 740a 0a20 2020 2020 2020 2072 6574  ent..        ret
+0000a020: 7572 6e20 785f 7365 7473 2c20 795f 7365  urn x_sets, y_se
+0000a030: 7473 0a0a 2020 2020 4073 7461 7469 636d  ts..    @staticm
+0000a040: 6574 686f 640a 2020 2020 6465 6620 6361  ethod.    def ca
+0000a050: 6c63 756c 6174 655f 6575 636c 6964 6561  lculate_euclidea
+0000a060: 6e5f 6469 7374 616e 6365 280a 2020 2020  n_distance(.    
+0000a070: 2020 2020 706f 696e 7431 3a20 4974 6572      point1: Iter
+0000a080: 6162 6c65 5b4f 7074 696f 6e61 6c5b 556e  able[Optional[Un
+0000a090: 696f 6e5b 696e 742c 2066 6c6f 6174 5d5d  ion[int, float]]
+0000a0a0: 5d2c 0a20 2020 2020 2020 2070 6f69 6e74  ],.        point
+0000a0b0: 323a 2049 7465 7261 626c 655b 4f70 7469  2: Iterable[Opti
+0000a0c0: 6f6e 616c 5b55 6e69 6f6e 5b69 6e74 2c20  onal[Union[int, 
+0000a0d0: 666c 6f61 745d 5d5d 0a20 2020 2029 202d  float]]].    ) -
+0000a0e0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+0000a0f0: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
+0000a100: 6c61 7465 2074 6865 2045 7563 6c69 6465  late the Euclide
+0000a110: 616e 2064 6973 7461 6e63 6520 6265 7477  an distance betw
+0000a120: 6565 6e20 7477 6f20 706f 696e 7473 2069  een two points i
+0000a130: 6e20 6e2d 6469 6d65 6e73 696f 6e61 6c20  n n-dimensional 
+0000a140: 7370 6163 652e 0a0a 2020 2020 2020 2020  space...        
+0000a150: 5468 6520 4575 636c 6964 6561 6e20 6469  The Euclidean di
+0000a160: 7374 616e 6365 2069 7320 7468 6520 7374  stance is the st
+0000a170: 7261 6967 6874 2d6c 696e 6520 6469 7374  raight-line dist
+0000a180: 616e 6365 2062 6574 7765 656e 2074 776f  ance between two
+0000a190: 2070 6f69 6e74 7320 696e 2045 7563 6c69   points in Eucli
+0000a1a0: 6465 616e 2073 7061 6365 2e0a 0a20 2020  dean space...   
+0000a1b0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000a1c0: 2020 2020 2020 2070 6f69 6e74 3120 2849         point1 (I
+0000a1d0: 7465 7261 626c 655b 4f70 7469 6f6e 616c  terable[Optional
+0000a1e0: 5b55 6e69 6f6e 5b69 6e74 2c20 666c 6f61  [Union[int, floa
+0000a1f0: 745d 5d5d 293a 2054 6865 2066 6972 7374  t]]]): The first
+0000a200: 2070 6f69 6e74 2061 7320 616e 2069 7465   point as an ite
+0000a210: 7261 626c 6520 6f66 2063 6f6f 7264 696e  rable of coordin
+0000a220: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
+0000a230: 2020 706f 696e 7432 2028 4974 6572 6162    point2 (Iterab
+0000a240: 6c65 5b4f 7074 696f 6e61 6c5b 556e 696f  le[Optional[Unio
+0000a250: 6e5b 696e 742c 2066 6c6f 6174 5d5d 5d29  n[int, float]]])
+0000a260: 3a20 5468 6520 7365 636f 6e64 2070 6f69  : The second poi
+0000a270: 6e74 2061 7320 616e 2069 7465 7261 626c  nt as an iterabl
+0000a280: 6520 6f66 2063 6f6f 7264 696e 6174 6573  e of coordinates
+0000a290: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000a2a0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000a2b0: 696e 743a 2054 6865 2045 7563 6c69 6465  int: The Euclide
+0000a2c0: 616e 2064 6973 7461 6e63 6520 6265 7477  an distance betw
+0000a2d0: 6565 6e20 706f 696e 7431 2061 6e64 2070  een point1 and p
+0000a2e0: 6f69 6e74 322e 0a0a 2020 2020 2020 2020  oint2...        
+0000a2f0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+0000a300: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
+0000a310: 4966 2070 6f69 6e74 3120 616e 6420 706f  If point1 and po
+0000a320: 696e 7432 2064 6f20 6e6f 7420 6861 7665  int2 do not have
+0000a330: 2074 6865 2073 616d 6520 6469 6d65 6e73   the same dimens
+0000a340: 696f 6e73 2e0a 2020 2020 2020 2020 2222  ions..        ""
+0000a350: 220a 2020 2020 2020 2020 6966 206c 656e  ".        if len
+0000a360: 2870 6f69 6e74 3129 2021 3d20 6c65 6e28  (point1) != len(
+0000a370: 706f 696e 7432 293a 0a20 2020 2020 2020  point2):.       
+0000a380: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0000a390: 4572 726f 7228 2242 6f74 6820 706f 696e  Error("Both poin
+0000a3a0: 7473 206d 7573 7420 6861 7665 2074 6865  ts must have the
+0000a3b0: 2073 616d 6520 6e75 6d62 6572 206f 6620   same number of 
+0000a3c0: 6469 6d65 6e73 696f 6e73 2e22 290a 0a20  dimensions.").. 
+0000a3d0: 2020 2020 2020 2070 3120 3d20 5b66 6c6f         p1 = [flo
+0000a3e0: 6174 2870 2920 6966 2070 2069 7320 6e6f  at(p) if p is no
+0000a3f0: 7420 4e6f 6e65 2065 6c73 6520 302e 3020  t None else 0.0 
+0000a400: 666f 7220 7020 696e 2070 6f69 6e74 315d  for p in point1]
+0000a410: 0a20 2020 2020 2020 2070 3220 3d20 5b66  .        p2 = [f
+0000a420: 6c6f 6174 2870 2920 6966 2070 2069 7320  loat(p) if p is 
+0000a430: 6e6f 7420 4e6f 6e65 2065 6c73 6520 302e  not None else 0.
+0000a440: 3020 666f 7220 7020 696e 2070 6f69 6e74  0 for p in point
+0000a450: 325d 0a0a 2020 2020 2020 2020 6575 636c  2]..        eucl
+0000a460: 6964 6561 6e5f 6469 7374 616e 6365 203d  idean_distance =
+0000a470: 206d 6174 682e 7371 7274 2873 756d 2828   math.sqrt(sum((
+0000a480: 7831 202d 2078 3229 202a 2a20 3220 666f  x1 - x2) ** 2 fo
+0000a490: 7220 7831 2c20 7832 2069 6e20 7a69 7028  r x1, x2 in zip(
+0000a4a0: 7031 2c20 7032 2929 290a 2020 2020 2020  p1, p2))).      
+0000a4b0: 2020 7265 7475 726e 2043 616c 6375 6c61    return Calcula
+0000a4c0: 7465 5574 696c 2e72 6561 6c5f 726f 756e  teUtil.real_roun
+0000a4d0: 6428 6575 636c 6964 6561 6e5f 6469 7374  d(euclidean_dist
+0000a4e0: 616e 6365 290a 0a20 2020 2040 7374 6174  ance)..    @stat
+0000a4f0: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0000a500: 2063 616c 6375 6c61 7465 5f73 616d 655f   calculate_same_
+0000a510: 6e75 6d62 6572 5f69 6e64 6578 2874 6172  number_index(tar
+0000a520: 6765 745f 6461 7461 3a20 4c69 7374 5b69  get_data: List[i
+0000a530: 6e74 5d2c 2069 6e70 7574 5f64 6174 613a  nt], input_data:
+0000a540: 204c 6973 745b 696e 745d 2920 2d3e 204c   List[int]) -> L
+0000a550: 6973 745b 696e 745d 3a0a 2020 2020 2020  ist[int]:.      
+0000a560: 2020 2222 220a 2020 2020 2020 2020 4669    """.        Fi
+0000a570: 6e64 7320 7468 6520 696e 6469 6365 7320  nds the indices 
+0000a580: 696e 2027 7461 7267 6574 5f64 6174 6127  in 'target_data'
+0000a590: 2077 6865 7265 2074 6865 206e 756d 6265   where the numbe
+0000a5a0: 7273 2061 7265 2070 7265 7365 6e74 2069  rs are present i
+0000a5b0: 6e20 2769 6e70 7574 5f64 6174 6127 2e0a  n 'input_data'..
+0000a5c0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000a5d0: 2020 2020 2020 2074 6172 6765 745f 6461         target_da
+0000a5e0: 7461 2028 4c69 7374 5b69 6e74 5d29 3a20  ta (List[int]): 
+0000a5f0: 5468 6520 6c69 7374 206f 6620 7461 7267  The list of targ
+0000a600: 6574 2069 6e74 6567 6572 732e 0a20 2020  et integers..   
+0000a610: 2020 2020 2069 6e70 7574 5f64 6174 6120       input_data 
+0000a620: 284c 6973 745b 696e 745d 293a 2054 6865  (List[int]): The
+0000a630: 206c 6973 7420 6f66 2069 6e70 7574 2069   list of input i
+0000a640: 6e74 6567 6572 7320 746f 2062 6520 6d61  ntegers to be ma
+0000a650: 7463 6865 6420 6167 6169 6e73 742e 0a0a  tched against...
+0000a660: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0000a670: 0a20 2020 2020 2020 204c 6973 745b 696e  .        List[in
+0000a680: 745d 3a20 4120 6c69 7374 206f 6620 696e  t]: A list of in
+0000a690: 6469 6365 7320 2831 2d62 6173 6564 2920  dices (1-based) 
+0000a6a0: 696e 2027 7461 7267 6574 5f64 6174 6127  in 'target_data'
+0000a6b0: 2077 6865 7265 206e 756d 6265 7273 2061   where numbers a
+0000a6c0: 7265 2066 6f75 6e64 2069 6e20 2769 6e70  re found in 'inp
+0000a6d0: 7574 5f64 6174 6127 2e0a 2020 2020 2020  ut_data'..      
+0000a6e0: 2020 2222 220a 2020 2020 2020 2020 7361    """.        sa
+0000a6f0: 6d65 5f6e 756d 6265 725f 696e 6465 7820  me_number_index 
+0000a700: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+0000a710: 2069 6e64 2c20 6e75 6d20 696e 2065 6e75   ind, num in enu
+0000a720: 6d65 7261 7465 2874 6172 6765 745f 6461  merate(target_da
+0000a730: 7461 293a 0a20 2020 2020 2020 2020 2020  ta):.           
+0000a740: 2069 6620 6e75 6d20 696e 2069 6e70 7574   if num in input
+0000a750: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
+0000a760: 2020 2020 2020 2073 616d 655f 6e75 6d62         same_numb
+0000a770: 6572 5f69 6e64 6578 2e61 7070 656e 6428  er_index.append(
+0000a780: 696e 6429 0a20 2020 2020 2020 2072 6574  ind).        ret
+0000a790: 7572 6e20 7361 6d65 5f6e 756d 6265 725f  urn same_number_
+0000a7a0: 696e 6465 780a 0a20 2020 2040 7374 6174  index..    @stat
+0000a7b0: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0000a7c0: 2063 616c 6375 6c61 7465 5f65 6467 655f   calculate_edge_
+0000a7d0: 6e75 6d62 6572 5f69 6e64 6578 2874 6172  number_index(tar
+0000a7e0: 6765 745f 6461 7461 3a20 4c69 7374 5b69  get_data: List[i
+0000a7f0: 6e74 5d2c 2069 6e70 7574 5f64 6174 613a  nt], input_data:
+0000a800: 204c 6973 745b 696e 745d 2920 2d3e 204c   List[int]) -> L
+0000a810: 6973 745b 696e 745d 3a0a 2020 2020 2020  ist[int]:.      
+0000a820: 2020 2222 220a 2020 2020 2020 2020 4669    """.        Fi
+0000a830: 6e64 7320 7468 6520 696e 6469 6365 7320  nds the indices 
+0000a840: 696e 2027 7461 7267 6574 5f64 6174 6127  in 'target_data'
+0000a850: 2077 6865 7265 2074 6865 206e 756d 6265   where the numbe
+0000a860: 7273 2061 7265 2061 646a 6163 656e 7420  rs are adjacent 
+0000a870: 746f 2061 6e79 206e 756d 6265 7220 696e  to any number in
+0000a880: 2027 696e 7075 745f 6461 7461 272e 0a20   'input_data'.. 
+0000a890: 2020 2020 2020 2041 206e 756d 6265 7220         A number 
+0000a8a0: 6973 2063 6f6e 7369 6465 7265 6420 6164  is considered ad
+0000a8b0: 6a61 6365 6e74 2069 6620 6974 2773 2065  jacent if it's e
+0000a8c0: 6974 6865 7220 6f6e 6520 736d 616c 6c65  ither one smalle
+0000a8d0: 7220 6f72 206f 6e65 206c 6172 6765 722e  r or one larger.
+0000a8e0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000a8f0: 2020 2020 2020 2020 7461 7267 6574 5f64          target_d
+0000a900: 6174 6120 284c 6973 745b 696e 745d 293a  ata (List[int]):
+0000a910: 2054 6865 206c 6973 7420 6f66 2074 6172   The list of tar
+0000a920: 6765 7420 696e 7465 6765 7273 2e0a 2020  get integers..  
+0000a930: 2020 2020 2020 696e 7075 745f 6461 7461        input_data
+0000a940: 2028 4c69 7374 5b69 6e74 5d29 3a20 5468   (List[int]): Th
+0000a950: 6520 6c69 7374 206f 6620 696e 7075 7420  e list of input 
+0000a960: 696e 7465 6765 7273 2074 6f20 6368 6563  integers to chec
+0000a970: 6b20 666f 7220 6164 6a61 6365 6e63 792e  k for adjacency.
+0000a980: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000a990: 733a 0a20 2020 2020 2020 204c 6973 745b  s:.        List[
+0000a9a0: 696e 745d 3a20 4120 6c69 7374 206f 6620  int]: A list of 
+0000a9b0: 696e 6469 6365 7320 2831 2d62 6173 6564  indices (1-based
+0000a9c0: 2920 696e 2027 7461 7267 6574 5f64 6174  ) in 'target_dat
+0000a9d0: 6127 2077 6865 7265 206e 756d 6265 7273  a' where numbers
+0000a9e0: 2061 7265 2061 646a 6163 656e 7420 746f   are adjacent to
+0000a9f0: 2061 6e79 2069 6e20 2769 6e70 7574 5f64   any in 'input_d
+0000aa00: 6174 6127 2e0a 2020 2020 2020 2020 2222  ata'..        ""
+0000aa10: 220a 2020 2020 2020 2020 6564 6765 5f69  ".        edge_i
+0000aa20: 6e66 6f20 3d20 5b5d 0a20 2020 2020 2020  nfo = [].       
+0000aa30: 2066 6f72 2069 6e64 2c20 6e75 6d20 696e   for ind, num in
+0000aa40: 2065 6e75 6d65 7261 7465 2874 6172 6765   enumerate(targe
+0000aa50: 745f 6461 7461 293a 0a20 2020 2020 2020  t_data):.       
+0000aa60: 2020 2020 2065 6467 655f 6e75 6d73 203d       edge_nums =
+0000aa70: 2073 6574 286e 756d 202b 2069 2066 6f72   set(num + i for
+0000aa80: 2069 2069 6e20 5b2d 312c 2031 5d29 0a20   i in [-1, 1]). 
+0000aa90: 2020 2020 2020 2020 2020 2070 6c65 6164             plead
+0000aaa0: 5f65 6467 6520 3d20 7365 7428 696e 7075  _edge = set(inpu
+0000aab0: 745f 6461 7461 292e 696e 7465 7273 6563  t_data).intersec
+0000aac0: 7469 6f6e 2865 6467 655f 6e75 6d73 290a  tion(edge_nums).
+0000aad0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+0000aae0: 656e 2870 6c65 6164 5f65 6467 6529 203e  en(plead_edge) >
+0000aaf0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000ab00: 2020 2020 6564 6765 5f69 6e66 6f2e 6170      edge_info.ap
+0000ab10: 7065 6e64 2869 6e64 290a 2020 2020 2020  pend(ind).      
+0000ab20: 2020 7265 7475 726e 2065 6467 655f 696e    return edge_in
+0000ab30: 666f 0a0a 2020 2020 4063 6c61 7373 6d65  fo..    @classme
+0000ab40: 7468 6f64 0a20 2020 2064 6566 2063 616c  thod.    def cal
+0000ab50: 6375 6c61 7465 5f7a 6f6e 655f 7261 7469  culate_zone_rati
+0000ab60: 6f28 0a20 2020 2020 2020 2020 2020 2063  o(.            c
+0000ab70: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+0000ab80: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
+0000ab90: 6f6e 3a20 4974 6572 6162 6c65 5b69 6e74  on: Iterable[int
+0000aba0: 5d2c 0a20 2020 2020 2020 2020 2020 207a  ],.            z
+0000abb0: 6f6e 655f 7261 6e67 6573 3a20 4c69 7374  one_ranges: List
+0000abc0: 5b54 7570 6c65 5b69 6e74 2c20 696e 745d  [Tuple[int, int]
+0000abd0: 5d2c 0a20 2020 2020 2020 2020 2020 202a  ],.            *
+0000abe0: 2a6b 7761 7267 733a 2041 6e79 0a20 2020  *kwargs: Any.   
+0000abf0: 2029 202d 3e20 5475 706c 655b 696e 742c   ) -> Tuple[int,
+0000ac00: 202e 2e2e 5d3a 0a20 2020 2020 2020 2022   ...]:.        "
+0000ac10: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
+0000ac20: 6c61 7465 2074 6865 2063 6f75 6e74 7320  late the counts 
+0000ac30: 6f66 206e 756d 6265 7273 2077 6974 6869  of numbers withi
+0000ac40: 6e20 7072 6564 6566 696e 6564 207a 6f6e  n predefined zon
+0000ac50: 6573 2066 6f72 2061 2067 6976 656e 2073  es for a given s
+0000ac60: 6571 7565 6e63 6520 6f66 206e 756d 6265  equence of numbe
+0000ac70: 7273 2e0a 2020 2020 2020 2020 5468 6973  rs..        This
+0000ac80: 2063 6c61 7373 206d 6574 686f 6420 6465   class method de
+0000ac90: 7465 726d 696e 6573 2074 6865 2064 6973  termines the dis
+0000aca0: 7472 6962 7574 696f 6e20 6f66 2074 6865  tribution of the
+0000acb0: 206e 756d 6265 7273 2069 6e20 7468 6520   numbers in the 
+0000acc0: 696e 7075 7420 7365 7175 656e 6365 2061  input sequence a
+0000acd0: 6372 6f73 7320 7370 6563 6966 6965 6420  cross specified 
+0000ace0: 7a6f 6e65 732e 0a20 2020 2020 2020 2045  zones..        E
+0000acf0: 6163 6820 7a6f 6e65 2069 7320 6465 6669  ach zone is defi
+0000ad00: 6e65 6420 6279 2061 2072 616e 6765 2c20  ned by a range, 
+0000ad10: 616e 6420 7468 6973 206d 6574 686f 6420  and this method 
+0000ad20: 636f 756e 7473 2068 6f77 206d 616e 7920  counts how many 
+0000ad30: 6e75 6d62 6572 7320 6661 6c6c 2069 6e74  numbers fall int
+0000ad40: 6f20 6561 6368 207a 6f6e 652e 0a0a 2020  o each zone...  
+0000ad50: 2020 2020 2020 3a70 6172 616d 206e 756d        :param num
+0000ad60: 6265 725f 636f 6d62 696e 6174 696f 6e3a  ber_combination:
+0000ad70: 2041 6e20 6974 6572 6162 6c65 206f 6620   An iterable of 
+0000ad80: 6e75 6d62 6572 7320 286c 696b 6520 6120  numbers (like a 
+0000ad90: 6c69 7374 206f 7220 7475 706c 6529 2066  list or tuple) f
+0000ada0: 726f 6d20 7768 6963 6820 7468 6520 6d65  rom which the me
+0000adb0: 7468 6f64 2077 696c 6c20 636f 756e 7420  thod will count 
+0000adc0: 686f 7720 6d61 6e79 0a20 2020 2020 2020  how many.       
+0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ade0: 2020 2020 2020 2020 2020 2020 206e 756d               num
+0000adf0: 6265 7273 2066 616c 6c20 696e 746f 2065  bers fall into e
+0000ae00: 6163 6820 7a6f 6e65 2e0a 2020 2020 2020  ach zone..      
+0000ae10: 2020 3a70 6172 616d 207a 6f6e 655f 7261    :param zone_ra
+0000ae20: 6e67 6573 3a20 4120 6c69 7374 206f 6620  nges: A list of 
+0000ae30: 7475 706c 6573 2077 6865 7265 2065 6163  tuples where eac
+0000ae40: 6820 7475 706c 6520 636f 6e74 6169 6e73  h tuple contains
+0000ae50: 2074 776f 206e 756d 6265 7273 2072 6570   two numbers rep
+0000ae60: 7265 7365 6e74 696e 6720 7468 6520 7374  resenting the st
+0000ae70: 6172 7420 616e 6420 656e 6420 6f66 2061  art and end of a
+0000ae80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ae90: 2020 2020 2020 2020 2020 2020 207a 6f6e               zon
+0000aea0: 6520 7261 6e67 652c 2072 6573 7065 6374  e range, respect
+0000aeb0: 6976 656c 792e 2054 6865 7365 2072 616e  ively. These ran
+0000aec0: 6765 7320 6465 6669 6e65 2074 6865 207a  ges define the z
+0000aed0: 6f6e 6573 2066 6f72 2063 6174 6567 6f72  ones for categor
+0000aee0: 697a 696e 6720 7468 6520 6e75 6d62 6572  izing the number
+0000aef0: 732e 0a20 2020 2020 2020 203a 7061 7261  s..        :para
+0000af00: 6d20 6b77 6172 6773 3a20 4164 6469 7469  m kwargs: Additi
+0000af10: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
+0000af20: 756d 656e 7473 2074 6861 7420 6d61 7920  uments that may 
+0000af30: 6265 2075 7365 6420 666f 7220 6675 7475  be used for futu
+0000af40: 7265 2065 7874 656e 7369 6f6e 7320 6f66  re extensions of
+0000af50: 2074 6865 206d 6574 686f 642e 0a20 2020   the method..   
+0000af60: 2020 2020 203a 7265 7475 726e 3a20 4120       :return: A 
+0000af70: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
+0000af80: 2074 6865 2063 6f75 6e74 206f 6620 6e75   the count of nu
+0000af90: 6d62 6572 7320 7468 6174 2066 616c 6c20  mbers that fall 
+0000afa0: 7769 7468 696e 2065 6163 6820 7370 6563  within each spec
+0000afb0: 6966 6965 6420 7a6f 6e65 2e0a 2020 2020  ified zone..    
+0000afc0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000afd0: 2023 2043 6865 636b 2069 6620 7a6f 6e65   # Check if zone
+0000afe0: 2072 616e 6765 7320 6172 6520 6465 6669   ranges are defi
+0000aff0: 6e65 642c 2069 6620 6e6f 742c 2072 6169  ned, if not, rai
+0000b000: 7365 2061 6e20 6578 6365 7074 696f 6e2e  se an exception.
+0000b010: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000b020: 7a6f 6e65 5f72 616e 6765 733a 0a20 2020  zone_ranges:.   
+0000b030: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000b040: 616c 7565 4572 726f 7228 275a 6f6e 6520  alueError('Zone 
+0000b050: 7261 6e67 6573 206d 7573 7420 6265 2070  ranges must be p
+0000b060: 726f 7669 6465 642e 2729 0a0a 2020 2020  rovided.')..    
+0000b070: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
+0000b080: 2063 6f75 6e74 6572 7320 666f 7220 6561   counters for ea
+0000b090: 6368 207a 6f6e 6520 746f 207a 6572 6f2e  ch zone to zero.
+0000b0a0: 0a20 2020 2020 2020 2072 6174 696f 203d  .        ratio =
+0000b0b0: 205b 305d 202a 206c 656e 287a 6f6e 655f   [0] * len(zone_
+0000b0c0: 7261 6e67 6573 290a 0a20 2020 2020 2020  ranges)..       
+0000b0d0: 2023 2049 7465 7261 7465 2074 6872 6f75   # Iterate throu
+0000b0e0: 6768 2065 6163 6820 6e75 6d62 6572 2061  gh each number a
+0000b0f0: 6e64 2063 6865 636b 2077 6869 6368 207a  nd check which z
+0000b100: 6f6e 6520 6974 2066 616c 6c73 2069 6e74  one it falls int
+0000b110: 6f2e 0a20 2020 2020 2020 2066 6f72 206e  o..        for n
+0000b120: 756d 2069 6e20 6d61 7028 696e 742c 206e  um in map(int, n
+0000b130: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
+0000b140: 6e29 3a20 2023 2043 6f6e 7665 7274 2065  n):  # Convert e
+0000b150: 6163 6820 6e75 6d62 6572 2074 6f20 616e  ach number to an
+0000b160: 2069 6e74 6567 6572 206f 6e63 6520 6265   integer once be
+0000b170: 666f 7265 2074 6865 206c 6f6f 702e 0a20  fore the loop.. 
+0000b180: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0000b190: 2c20 2873 7461 7274 2c20 656e 6429 2069  , (start, end) i
+0000b1a0: 6e20 656e 756d 6572 6174 6528 7a6f 6e65  n enumerate(zone
+0000b1b0: 5f72 616e 6765 7329 3a0a 2020 2020 2020  _ranges):.      
+0000b1c0: 2020 2020 2020 2020 2020 6966 2073 7461            if sta
+0000b1d0: 7274 203c 3d20 6e75 6d20 3c3d 2065 6e64  rt <= num <= end
+0000b1e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b1f0: 2020 2020 2020 7261 7469 6f5b 695d 202b        ratio[i] +
+0000b200: 3d20 3120 2023 2049 6e63 7265 6d65 6e74  = 1  # Increment
+0000b210: 2074 6865 2063 6f75 6e74 6572 2066 6f72   the counter for
+0000b220: 2074 6865 2063 7572 7265 6e74 207a 6f6e   the current zon
+0000b230: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000b240: 2020 2020 2020 2062 7265 616b 2020 2320         break  # 
+0000b250: 4966 2074 6865 206e 756d 6265 7220 6973  If the number is
+0000b260: 2077 6974 6869 6e20 7468 6520 6375 7272   within the curr
+0000b270: 656e 7420 7a6f 6e65 2c20 6e6f 206e 6565  ent zone, no nee
+0000b280: 6420 746f 2063 6865 636b 2066 7572 7468  d to check furth
+0000b290: 6572 207a 6f6e 6573 2e0a 0a20 2020 2020  er zones...     
+0000b2a0: 2020 2023 2052 6574 7572 6e20 7468 6520     # Return the 
+0000b2b0: 636f 756e 7473 2061 7320 6120 7475 706c  counts as a tupl
+0000b2c0: 652c 2077 6974 6820 6561 6368 2065 6c65  e, with each ele
+0000b2d0: 6d65 6e74 2072 6570 7265 7365 6e74 696e  ment representin
+0000b2e0: 6720 7468 6520 636f 756e 7420 666f 7220  g the count for 
+0000b2f0: 6120 7265 7370 6563 7469 7665 207a 6f6e  a respective zon
+0000b300: 652e 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+0000b310: 6e20 7475 706c 6528 7261 7469 6f29 0a0a  n tuple(ratio)..
+0000b320: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+0000b330: 0a20 2020 2064 6566 2063 616c 6375 6c61  .    def calcula
+0000b340: 7465 5f62 6967 5f73 6d61 6c6c 5f72 6174  te_big_small_rat
+0000b350: 696f 280a 2020 2020 2020 2020 2020 2020  io(.            
+0000b360: 636c 732c 0a20 2020 2020 2020 2020 2020  cls,.           
+0000b370: 206e 756d 6265 725f 636f 6d62 696e 6174   number_combinat
+0000b380: 696f 6e73 3a20 4974 6572 6162 6c65 5b69  ions: Iterable[i
+0000b390: 6e74 5d2c 0a20 2020 2020 2020 2020 2020  nt],.           
+0000b3a0: 2062 6967 5f73 6d61 6c6c 5f72 616e 6765   big_small_range
+0000b3b0: 733a 204c 6973 745b 5475 706c 655b 696e  s: List[Tuple[in
+0000b3c0: 742c 2069 6e74 5d5d 2c0a 2020 2020 2020  t, int]],.      
+0000b3d0: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
+0000b3e0: 416e 790a 2020 2020 2920 2d3e 2054 7570  Any.    ) -> Tup
+0000b3f0: 6c65 5b69 6e74 2c20 2e2e 2e5d 3a0a 2020  le[int, ...]:.  
+0000b400: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000b410: 2020 4361 6c63 756c 6174 6520 7468 6520    Calculate the 
+0000b420: 636f 756e 7473 206f 6620 6e75 6d62 6572  counts of number
+0000b430: 7320 7769 7468 696e 2070 7265 6465 6669  s within predefi
+0000b440: 6e65 6420 7369 7a65 2072 616e 6765 7320  ned size ranges 
+0000b450: 666f 7220 6120 7365 7175 656e 6365 206f  for a sequence o
+0000b460: 6620 6e75 6d62 6572 732e 0a20 2020 2020  f numbers..     
+0000b470: 2020 2054 6869 7320 636c 6173 7320 6d65     This class me
+0000b480: 7468 6f64 2061 7373 6573 7365 7320 686f  thod assesses ho
+0000b490: 7720 6d61 6e79 206e 756d 6265 7273 2066  w many numbers f
+0000b4a0: 726f 6d20 7468 6520 696e 7075 7420 7365  rom the input se
+0000b4b0: 7175 656e 6365 2066 616c 6c20 7769 7468  quence fall with
+0000b4c0: 696e 2065 6163 6820 6f66 2074 6865 2073  in each of the s
+0000b4d0: 7065 6369 6669 6564 2073 697a 6520 7261  pecified size ra
+0000b4e0: 6e67 6573 2e0a 2020 2020 2020 2020 4561  nges..        Ea
+0000b4f0: 6368 2072 616e 6765 2072 6570 7265 7365  ch range represe
+0000b500: 6e74 7320 6120 277a 6f6e 6527 2c20 7768  nts a 'zone', wh
+0000b510: 6963 6820 636f 756c 6420 636f 7272 6573  ich could corres
+0000b520: 706f 6e64 2074 6f20 6120 636f 6e63 6570  pond to a concep
+0000b530: 7420 6c69 6b65 2027 6269 6727 206f 7220  t like 'big' or 
+0000b540: 2773 6d61 6c6c 2720 6e75 6d62 6572 732e  'small' numbers.
+0000b550: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000b560: 206e 756d 6265 725f 636f 6d62 696e 6174   number_combinat
+0000b570: 696f 6e73 3a20 416e 2069 7465 7261 626c  ions: An iterabl
+0000b580: 6520 6f66 206e 756d 6265 7273 2028 6c69  e of numbers (li
+0000b590: 6b65 2061 206c 6973 7420 6f72 2074 7570  ke a list or tup
+0000b5a0: 6c65 2920 6672 6f6d 2077 6869 6368 2074  le) from which t
+0000b5b0: 6865 206d 6574 686f 6420 7769 6c6c 2063  he method will c
+0000b5c0: 6f75 6e74 2068 6f77 206d 616e 790a 2020  ount how many.  
+0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5f0: 2020 6e75 6d62 6572 7320 6661 6c6c 2069    numbers fall i
+0000b600: 6e74 6f20 6561 6368 2073 697a 6520 7261  nto each size ra
+0000b610: 6e67 652e 0a20 2020 2020 2020 203a 7061  nge..        :pa
+0000b620: 7261 6d20 6269 675f 736d 616c 6c5f 7261  ram big_small_ra
+0000b630: 6e67 6573 3a20 4120 6c69 7374 206f 6620  nges: A list of 
+0000b640: 7475 706c 6573 2077 6865 7265 2065 6163  tuples where eac
+0000b650: 6820 7475 706c 6520 636f 6e74 6169 6e73  h tuple contains
+0000b660: 2074 776f 206e 756d 6265 7273 2072 6570   two numbers rep
+0000b670: 7265 7365 6e74 696e 6720 7468 6520 7374  resenting the st
+0000b680: 6172 7420 616e 6420 656e 6420 6f66 2061  art and end of a
+0000b690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6b0: 2020 7261 6e67 652c 2072 6573 7065 6374    range, respect
+0000b6c0: 6976 656c 792e 2054 6865 7365 2072 616e  ively. These ran
+0000b6d0: 6765 7320 6465 6669 6e65 2074 6865 207a  ges define the z
+0000b6e0: 6f6e 6573 2066 6f72 2063 6174 6567 6f72  ones for categor
+0000b6f0: 697a 696e 6720 7468 6520 6e75 6d62 6572  izing the number
+0000b700: 732e 0a20 2020 2020 2020 203a 7061 7261  s..        :para
+0000b710: 6d20 6b77 6172 6773 3a20 4164 6469 7469  m kwargs: Additi
+0000b720: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
+0000b730: 756d 656e 7473 2074 6861 7420 6d61 7920  uments that may 
+0000b740: 6265 2075 7365 6420 666f 7220 6675 7475  be used for futu
+0000b750: 7265 2065 7874 656e 7369 6f6e 7320 6f66  re extensions of
+0000b760: 2074 6865 206d 6574 686f 642e 0a20 2020   the method..   
+0000b770: 2020 2020 203a 7265 7475 726e 3a20 4120       :return: A 
+0000b780: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
+0000b790: 2074 6865 2063 6f75 6e74 206f 6620 6e75   the count of nu
+0000b7a0: 6d62 6572 7320 7468 6174 2066 616c 6c20  mbers that fall 
+0000b7b0: 7769 7468 696e 2065 6163 6820 7370 6563  within each spec
+0000b7c0: 6966 6965 6420 7261 6e67 6520 6f72 2027  ified range or '
+0000b7d0: 7a6f 6e65 272e 0a20 2020 2020 2020 2022  zone'..        "
+0000b7e0: 2222 0a0a 2020 2020 2020 2020 2320 4368  ""..        # Ch
+0000b7f0: 6563 6b20 6966 2073 697a 6520 7261 6e67  eck if size rang
+0000b800: 6573 2061 7265 2064 6566 696e 6564 2c20  es are defined, 
+0000b810: 6966 206e 6f74 2c20 7261 6973 6520 616e  if not, raise an
+0000b820: 2065 7863 6570 7469 6f6e 2e0a 2020 2020   exception..    
+0000b830: 2020 2020 6966 206e 6f74 2062 6967 5f73      if not big_s
+0000b840: 6d61 6c6c 5f72 616e 6765 733a 0a20 2020  mall_ranges:.   
+0000b850: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000b860: 616c 7565 4572 726f 7228 2753 697a 6520  alueError('Size 
+0000b870: 7261 6e67 6573 2066 6f72 2062 6967 2061  ranges for big a
+0000b880: 6e64 2073 6d61 6c6c 206e 756d 6265 7273  nd small numbers
+0000b890: 206d 7573 7420 6265 2070 726f 7669 6465   must be provide
+0000b8a0: 642e 2729 0a0a 2020 2020 2020 2020 2320  d.')..        # 
+0000b8b0: 496e 6974 6961 6c69 7a65 2063 6f75 6e74  Initialize count
+0000b8c0: 6572 7320 666f 7220 6561 6368 2072 616e  ers for each ran
+0000b8d0: 6765 2074 6f20 7a65 726f 2e0a 2020 2020  ge to zero..    
+0000b8e0: 2020 2020 7261 7469 6f20 3d20 5b30 5d20      ratio = [0] 
+0000b8f0: 2a20 6c65 6e28 6269 675f 736d 616c 6c5f  * len(big_small_
+0000b900: 7261 6e67 6573 290a 0a20 2020 2020 2020  ranges)..       
+0000b910: 2023 2049 7465 7261 7465 2074 6872 6f75   # Iterate throu
+0000b920: 6768 2065 6163 6820 6e75 6d62 6572 2061  gh each number a
+0000b930: 6e64 2063 6865 636b 2077 6869 6368 2072  nd check which r
+0000b940: 616e 6765 2069 7420 6661 6c6c 7320 696e  ange it falls in
+0000b950: 746f 2e0a 2020 2020 2020 2020 666f 7220  to..        for 
+0000b960: 6e75 6d20 696e 206d 6170 2869 6e74 2c20  num in map(int, 
+0000b970: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
+0000b980: 6f6e 7329 3a20 2023 2043 6f6e 7665 7274  ons):  # Convert
+0000b990: 2065 6163 6820 6e75 6d62 6572 2074 6f20   each number to 
+0000b9a0: 616e 2069 6e74 6567 6572 206f 6e63 6520  an integer once 
+0000b9b0: 6265 666f 7265 2074 6865 206c 6f6f 702e  before the loop.
+0000b9c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000b9d0: 2069 2c20 2873 7461 7274 2c20 656e 6429   i, (start, end)
+0000b9e0: 2069 6e20 656e 756d 6572 6174 6528 6269   in enumerate(bi
+0000b9f0: 675f 736d 616c 6c5f 7261 6e67 6573 293a  g_small_ranges):
+0000ba00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ba10: 2069 6620 7374 6172 7420 3c3d 206e 756d   if start <= num
+0000ba20: 203c 3d20 656e 643a 0a20 2020 2020 2020   <= end:.       
+0000ba30: 2020 2020 2020 2020 2020 2020 2072 6174               rat
+0000ba40: 696f 5b69 5d20 2b3d 2031 2020 2320 496e  io[i] += 1  # In
+0000ba50: 6372 656d 656e 7420 7468 6520 636f 756e  crement the coun
+0000ba60: 7465 7220 666f 7220 7468 6520 6375 7272  ter for the curr
+0000ba70: 656e 7420 7261 6e67 652e 0a20 2020 2020  ent range..     
+0000ba80: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000ba90: 7265 616b 2020 2320 4966 2074 6865 206e  reak  # If the n
+0000baa0: 756d 6265 7220 6973 2077 6974 6869 6e20  umber is within 
+0000bab0: 7468 6520 6375 7272 656e 7420 7261 6e67  the current rang
+0000bac0: 652c 206e 6f20 6e65 6564 2074 6f20 6368  e, no need to ch
+0000bad0: 6563 6b20 6675 7274 6865 7220 7261 6e67  eck further rang
+0000bae0: 6573 2e0a 0a20 2020 2020 2020 2023 2052  es...        # R
+0000baf0: 6574 7572 6e20 7468 6520 636f 756e 7473  eturn the counts
+0000bb00: 2061 7320 6120 7475 706c 652c 2077 6974   as a tuple, wit
+0000bb10: 6820 6561 6368 2065 6c65 6d65 6e74 2072  h each element r
+0000bb20: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+0000bb30: 636f 756e 7420 666f 7220 6120 7265 7370  count for a resp
+0000bb40: 6563 7469 7665 2072 616e 6765 206f 7220  ective range or 
+0000bb50: 277a 6f6e 6527 2e0a 2020 2020 2020 2020  'zone'..        
+0000bb60: 7265 7475 726e 2074 7570 6c65 2872 6174  return tuple(rat
+0000bb70: 696f 290a 0a20 2020 2040 636c 6173 736d  io)..    @classm
+0000bb80: 6574 686f 640a 2020 2020 6465 6620 6361  ethod.    def ca
+0000bb90: 6c63 756c 6174 655f 726f 6164 5f30 3132  lculate_road_012
+0000bba0: 5f72 6174 696f 280a 2020 2020 2020 2020  _ratio(.        
+0000bbb0: 2020 2020 636c 732c 0a20 2020 2020 2020      cls,.       
+0000bbc0: 2020 2020 206e 756d 6265 725f 636f 6d62       number_comb
+0000bbd0: 696e 6174 696f 6e3a 2049 7465 7261 626c  ination: Iterabl
+0000bbe0: 655b 696e 745d 2c0a 2020 2020 2020 2020  e[int],.        
+0000bbf0: 2020 2020 726f 6164 5f30 3132 5f72 616e      road_012_ran
+0000bc00: 6765 733a 204c 6973 745b 7475 706c 655b  ges: List[tuple[
+0000bc10: 696e 742c 202e 2e2e 5d5d 2c0a 2020 2020  int, ...]],.    
+0000bc20: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0000bc30: 3a20 416e 790a 2020 2020 2920 2d3e 2054  : Any.    ) -> T
+0000bc40: 7570 6c65 5b69 6e74 2c20 2e2e 2e5d 3a0a  uple[int, ...]:.
+0000bc50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000bc60: 2020 2020 4361 6c63 756c 6174 6520 7468      Calculate th
+0000bc70: 6520 636f 756e 7420 6f66 206e 756d 6265  e count of numbe
+0000bc80: 7273 2077 6974 6869 6e20 7072 6564 6566  rs within predef
+0000bc90: 696e 6564 207a 6f6e 6573 2028 7265 6665  ined zones (refe
+0000bca0: 7272 6564 2074 6f20 6173 2027 726f 6164  rred to as 'road
+0000bcb0: 7327 2920 666f 7220 6120 6769 7665 6e20  s') for a given 
+0000bcc0: 7365 7175 656e 6365 206f 6620 6e75 6d62  sequence of numb
+0000bcd0: 6572 732e 0a20 2020 2020 2020 2054 6869  ers..        Thi
+0000bce0: 7320 636c 6173 7320 6d65 7468 6f64 2064  s class method d
+0000bcf0: 6574 6572 6d69 6e65 7320 686f 7720 6d61  etermines how ma
+0000bd00: 6e79 206e 756d 6265 7273 2066 726f 6d20  ny numbers from 
+0000bd10: 7468 6520 696e 7075 7420 6661 6c6c 2077  the input fall w
+0000bd20: 6974 6869 6e20 6561 6368 206f 6620 7468  ithin each of th
+0000bd30: 6520 7370 6563 6966 6965 6420 7261 6e67  e specified rang
+0000bd40: 6573 2e20 4561 6368 2072 616e 6765 0a20  es. Each range. 
+0000bd50: 2020 2020 2020 2072 6570 7265 7365 6e74         represent
+0000bd60: 7320 6120 2772 6f61 6427 2c20 7768 6963  s a 'road', whic
+0000bd70: 6820 6973 2061 2073 6567 6d65 6e74 206f  h is a segment o
+0000bd80: 6620 7468 6520 6f76 6572 616c 6c20 6461  f the overall da
+0000bd90: 7461 2073 6574 2e0a 0a20 2020 2020 2020  ta set...       
+0000bda0: 203a 7061 7261 6d20 6e75 6d62 6572 5f63   :param number_c
+0000bdb0: 6f6d 6269 6e61 7469 6f6e 3a20 4120 6c69  ombination: A li
+0000bdc0: 7374 2c20 7475 706c 652c 206f 7220 6f74  st, tuple, or ot
+0000bdd0: 6865 7220 6974 6572 6162 6c65 206f 6620  her iterable of 
+0000bde0: 6e75 6d62 6572 732e 2054 6865 206d 6574  numbers. The met
+0000bdf0: 686f 6420 7769 6c6c 2069 7465 7261 7465  hod will iterate
+0000be00: 2074 6872 6f75 6768 2074 6869 730a 2020   through this.  
+0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be30: 2063 6f6c 6c65 6374 696f 6e20 746f 2063   collection to c
+0000be40: 6f75 6e74 2068 6f77 206d 616e 7920 6e75  ount how many nu
+0000be50: 6d62 6572 7320 6661 6c6c 2069 6e74 6f20  mbers fall into 
+0000be60: 6561 6368 2027 726f 6164 2720 6173 2064  each 'road' as d
+0000be70: 6566 696e 6564 2062 7920 7468 6520 7261  efined by the ra
+0000be80: 6e67 6573 2e0a 2020 2020 2020 2020 3a70  nges..        :p
+0000be90: 6172 616d 2072 6f61 645f 3031 325f 7261  aram road_012_ra
+0000bea0: 6e67 6573 3a20 4120 6c69 7374 206f 6620  nges: A list of 
+0000beb0: 7261 6e67 6520 6f62 6a65 6374 7320 6f72  range objects or
+0000bec0: 2073 6571 7565 6e63 6573 2064 6566 696e   sequences defin
+0000bed0: 696e 6720 7468 6520 2772 6f61 6473 272e  ing the 'roads'.
+0000bee0: 2045 6163 6820 656c 656d 656e 7420 696e   Each element in
+0000bef0: 2074 6869 7320 6c69 7374 0a20 2020 2020   this list.     
+0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf10: 2020 2020 2020 2020 2020 2063 6f72 7265             corre
+0000bf20: 7370 6f6e 6473 2074 6f20 6120 6469 6666  sponds to a diff
+0000bf30: 6572 656e 7420 2772 6f61 6427 2c20 616e  erent 'road', an
+0000bf40: 6420 7468 6520 6e75 6d62 6572 7320 696e  d the numbers in
+0000bf50: 2027 6e75 6d62 6572 5f63 6f6d 6269 6e61   'number_combina
+0000bf60: 7469 6f6e 2720 6172 6520 6368 6563 6b65  tion' are checke
+0000bf70: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf90: 2020 6167 6169 6e73 7420 7468 6573 6520    against these 
+0000bfa0: 7261 6e67 6573 2074 6f20 6465 7465 726d  ranges to determ
+0000bfb0: 696e 6520 7468 6569 7220 636f 756e 7473  ine their counts
+0000bfc0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000bfd0: 206b 7761 7267 733a 2041 6464 6974 696f   kwargs: Additio
+0000bfe0: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+0000bff0: 6d65 6e74 7320 7468 6174 2061 7265 206e  ments that are n
+0000c000: 6f74 2075 7365 6420 696e 2074 6869 7320  ot used in this 
+0000c010: 6d65 7468 6f64 2062 7574 2061 7265 2069  method but are i
+0000c020: 6e63 6c75 6465 6420 666f 7220 706f 7465  ncluded for pote
+0000c030: 6e74 6961 6c0a 2020 2020 2020 2020 2020  ntial.          
+0000c040: 2020 2020 2020 2020 2020 2020 2066 7574               fut
+0000c050: 7572 6520 6578 7465 6e73 6962 696c 6974  ure extensibilit
+0000c060: 7920 6f66 2074 6865 206d 6574 686f 642e  y of the method.
+0000c070: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000c080: 3a20 4120 7475 706c 6520 636f 6e74 6169  : A tuple contai
+0000c090: 6e69 6e67 2074 6865 2063 6f75 6e74 206f  ning the count o
+0000c0a0: 6620 6e75 6d62 6572 7320 696e 2065 6163  f numbers in eac
+0000c0b0: 6820 2772 6f61 6427 2e0a 2020 2020 2020  h 'road'..      
+0000c0c0: 2020 2222 220a 0a20 2020 2020 2020 2023    """..        #
+0000c0d0: 2056 616c 6964 6174 6520 7468 6520 7072   Validate the pr
+0000c0e0: 6573 656e 6365 206f 6620 2772 6f61 645f  esence of 'road_
+0000c0f0: 3031 325f 7261 6e67 6573 272e 0a20 2020  012_ranges'..   
+0000c100: 2020 2020 2069 6620 6e6f 7420 726f 6164       if not road
+0000c110: 5f30 3132 5f72 616e 6765 733a 0a20 2020  _012_ranges:.   
+0000c120: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000c130: 616c 7565 4572 726f 7228 2752 6f61 6420  alueError('Road 
+0000c140: 3031 3220 7261 6e67 6573 206d 7573 7420  012 ranges must 
+0000c150: 6265 2070 726f 7669 6465 642e 2729 0a0a  be provided.')..
+0000c160: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
+0000c170: 6c69 7a65 2063 6f75 6e74 6572 7320 666f  lize counters fo
+0000c180: 7220 6561 6368 2027 726f 6164 2720 746f  r each 'road' to
+0000c190: 207a 6572 6f2e 0a20 2020 2020 2020 2072   zero..        r
+0000c1a0: 6174 696f 203d 205b 305d 202a 206c 656e  atio = [0] * len
+0000c1b0: 2872 6f61 645f 3031 325f 7261 6e67 6573  (road_012_ranges
+0000c1c0: 290a 0a20 2020 2020 2020 2023 2043 6f75  )..        # Cou
+0000c1d0: 6e74 2074 6865 206e 756d 6265 7273 2069  nt the numbers i
+0000c1e0: 6e20 6561 6368 2027 726f 6164 2720 6279  n each 'road' by
+0000c1f0: 2069 7465 7261 7469 6e67 2074 6872 6f75   iterating throu
+0000c200: 6768 2074 6865 2069 6e70 7574 206e 756d  gh the input num
+0000c210: 6265 7273 2061 6e64 2074 6865 2064 6566  bers and the def
+0000c220: 696e 6564 2072 616e 6765 732e 0a20 2020  ined ranges..   
+0000c230: 2020 2020 2066 6f72 206e 756d 2069 6e20       for num in 
+0000c240: 6d61 7028 696e 742c 206e 756d 6265 725f  map(int, number_
+0000c250: 636f 6d62 696e 6174 696f 6e29 3a20 2023  combination):  #
+0000c260: 2043 6f6e 7665 7274 2065 6163 6820 6e75   Convert each nu
+0000c270: 6d62 6572 2074 6f20 616e 2069 6e74 6567  mber to an integ
+0000c280: 6572 206f 6e63 652c 2062 6566 6f72 6520  er once, before 
+0000c290: 7468 6520 6c6f 6f70 2e0a 2020 2020 2020  the loop..      
+0000c2a0: 2020 2020 2020 666f 7220 692c 2076 616c        for i, val
+0000c2b0: 7320 696e 2065 6e75 6d65 7261 7465 2872  s in enumerate(r
+0000c2c0: 6f61 645f 3031 325f 7261 6e67 6573 293a  oad_012_ranges):
+0000c2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c2e0: 2069 6620 6e75 6d20 696e 2076 616c 733a   if num in vals:
+0000c2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c300: 2020 2020 2072 6174 696f 5b69 5d20 2b3d       ratio[i] +=
+0000c310: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+0000c320: 2020 2020 2020 2062 7265 616b 2020 2320         break  # 
+0000c330: 4f6e 6365 2074 6865 206e 756d 6265 7220  Once the number 
+0000c340: 6973 2066 6f75 6e64 2069 6e20 6120 2772  is found in a 'r
+0000c350: 6f61 6427 2c20 7374 6f70 2063 6865 636b  oad', stop check
+0000c360: 696e 6720 7468 6520 7265 6d61 696e 696e  ing the remainin
+0000c370: 6720 2772 6f61 6473 272e 0a0a 2020 2020  g 'roads'...    
+0000c380: 2020 2020 2320 5265 7475 726e 2074 6865      # Return the
+0000c390: 2063 6f75 6e74 7320 6173 2061 2074 7570   counts as a tup
+0000c3a0: 6c65 2c20 7769 7468 2065 6163 6820 656c  le, with each el
+0000c3b0: 656d 656e 7420 7265 7072 6573 656e 7469  ement representi
+0000c3c0: 6e67 2074 6865 2063 6f75 6e74 2066 6f72  ng the count for
+0000c3d0: 2061 2072 6573 7065 6374 6976 6520 2772   a respective 'r
+0000c3e0: 6f61 6427 2e0a 2020 2020 2020 2020 7265  oad'..        re
+0000c3f0: 7475 726e 2074 7570 6c65 2872 6174 696f  turn tuple(ratio
+0000c400: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
+0000c410: 686f 640a 2020 2020 6465 6620 6361 6c63  hod.    def calc
+0000c420: 756c 6174 655f 6f64 645f 6576 656e 5f72  ulate_odd_even_r
+0000c430: 6174 696f 280a 2020 2020 2020 2020 2020  atio(.          
+0000c440: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
+0000c450: 2020 206e 756d 6265 725f 636f 6d62 696e     number_combin
+0000c460: 6174 696f 6e3a 2049 7465 7261 626c 655b  ation: Iterable[
+0000c470: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
+0000c480: 2020 2a2a 6b77 6172 6773 3a20 416e 790a    **kwargs: Any.
+0000c490: 2020 2020 2920 2d3e 2054 7570 6c65 5b69      ) -> Tuple[i
+0000c4a0: 6e74 2c20 696e 745d 3a0a 2020 2020 2020  nt, int]:.      
+0000c4b0: 2020 2222 220a 2020 2020 2020 2020 4361    """.        Ca
+0000c4c0: 6c63 756c 6174 6520 7468 6520 7261 7469  lculate the rati
+0000c4d0: 6f20 6f66 206f 6464 2074 6f20 6576 656e  o of odd to even
+0000c4e0: 206e 756d 6265 7273 2077 6974 6869 6e20   numbers within 
+0000c4f0: 6120 6769 7665 6e20 7365 7175 656e 6365  a given sequence
+0000c500: 206f 6620 6e75 6d62 6572 732e 0a20 2020   of numbers..   
+0000c510: 2020 2020 2054 6869 7320 6d65 7468 6f64       This method
+0000c520: 2069 7320 6465 7369 676e 6564 2074 6f20   is designed to 
+0000c530: 6265 2063 616c 6c65 6420 6f6e 2074 6865  be called on the
+0000c540: 2063 6c61 7373 2069 7473 656c 6620 7261   class itself ra
+0000c550: 7468 6572 2074 6861 6e20 6f6e 2061 6e20  ther than on an 
+0000c560: 696e 7374 616e 6365 206f 6620 7468 6520  instance of the 
+0000c570: 636c 6173 732e 2049 7420 6361 6e20 6265  class. It can be
+0000c580: 0a20 2020 2020 2020 2075 7365 6420 746f  .        used to
+0000c590: 2061 6e61 6c79 7a65 2061 2063 6f6c 6c65   analyze a colle
+0000c5a0: 6374 696f 6e20 6f66 206e 756d 6265 7273  ction of numbers
+0000c5b0: 2028 6e75 6d62 6572 5f63 6f6d 6269 6e61   (number_combina
+0000c5c0: 7469 6f6e 2920 616e 6420 6465 7465 726d  tion) and determ
+0000c5d0: 696e 6520 7468 6520 636f 756e 7420 6f66  ine the count of
+0000c5e0: 206f 6464 2061 6e64 2065 7665 6e20 6e75   odd and even nu
+0000c5f0: 6d62 6572 732e 0a0a 2020 2020 2020 2020  mbers...        
+0000c600: 3a70 6172 616d 206e 756d 6265 725f 636f  :param number_co
+0000c610: 6d62 696e 6174 696f 6e3a 2041 206c 6973  mbination: A lis
+0000c620: 742c 2074 7570 6c65 2c20 6f72 206f 7468  t, tuple, or oth
+0000c630: 6572 2069 7465 7261 626c 6520 6f66 2069  er iterable of i
+0000c640: 6e74 6567 6572 732e 2054 6865 206d 6574  ntegers. The met
+0000c650: 686f 6420 7769 6c6c 2069 7465 7261 7465  hod will iterate
+0000c660: 2074 6872 6f75 6768 0a20 2020 2020 2020   through.       
+0000c670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c680: 2020 2020 2020 2020 2020 2020 7468 6973              this
+0000c690: 2063 6f6c 6c65 6374 696f 6e20 746f 2064   collection to d
+0000c6a0: 6574 6572 6d69 6e65 2074 6865 2063 6f75  etermine the cou
+0000c6b0: 6e74 206f 6620 6f64 6420 616e 6420 6576  nt of odd and ev
+0000c6c0: 656e 206e 756d 6265 7273 2e0a 2020 2020  en numbers..    
+0000c6d0: 2020 2020 3a70 6172 616d 206b 7761 7267      :param kwarg
+0000c6e0: 733a 2041 6464 6974 696f 6e61 6c20 6b65  s: Additional ke
+0000c6f0: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+0000c700: 7468 6174 2061 7265 206e 6f74 2075 7365  that are not use
+0000c710: 6420 696e 2074 6869 7320 6d65 7468 6f64  d in this method
+0000c720: 2062 7574 2061 7265 2069 6e63 6c75 6465   but are include
+0000c730: 6420 666f 7220 706f 7465 6e74 6961 6c0a  d for potential.
+0000c740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c750: 2020 2020 2020 2066 7574 7572 6520 6578         future ex
+0000c760: 7465 6e73 6962 696c 6974 7920 6f66 2074  tensibility of t
+0000c770: 6865 206d 6574 686f 642e 0a20 2020 2020  he method..     
+0000c780: 2020 203a 7265 7475 726e 3a20 4120 7475     :return: A tu
+0000c790: 706c 6520 636f 6e74 6169 6e69 6e67 2074  ple containing t
+0000c7a0: 776f 2065 6c65 6d65 6e74 733b 2074 6865  wo elements; the
+0000c7b0: 2066 6972 7374 2069 7320 7468 6520 636f   first is the co
+0000c7c0: 756e 7420 6f66 206f 6464 206e 756d 6265  unt of odd numbe
+0000c7d0: 7273 2061 6e64 2074 6865 2073 6563 6f6e  rs and the secon
+0000c7e0: 6420 6973 2074 6865 0a20 2020 2020 2020  d is the.       
+0000c7f0: 2020 2020 2020 2020 2020 636f 756e 7420            count 
+0000c800: 6f66 2065 7665 6e20 6e75 6d62 6572 7320  of even numbers 
+0000c810: 696e 2074 6865 206e 756d 6265 725f 636f  in the number_co
+0000c820: 6d62 696e 6174 696f 6e2e 0a20 2020 2020  mbination..     
+0000c830: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000c840: 2320 436f 756e 7420 7468 6520 6e75 6d62  # Count the numb
+0000c850: 6572 206f 6620 6f64 6420 6e75 6d62 6572  er of odd number
+0000c860: 7320 696e 2074 6865 206e 756d 6265 725f  s in the number_
+0000c870: 636f 6d62 696e 6174 696f 6e0a 2020 2020  combination.    
+0000c880: 2020 2020 2320 4120 6e75 6d62 6572 2069      # A number i
+0000c890: 7320 636f 6e73 6964 6572 6564 206f 6464  s considered odd
+0000c8a0: 2069 6620 7468 6520 7265 6d61 696e 6465   if the remainde
+0000c8b0: 7220 6f66 2074 6865 2064 6976 6973 696f  r of the divisio
+0000c8c0: 6e20 6279 2032 2069 7320 3120 286e 756d  n by 2 is 1 (num
+0000c8d0: 2025 2032 2065 7661 6c75 6174 6573 2074   % 2 evaluates t
+0000c8e0: 6f20 5472 7565 290a 2020 2020 2020 2020  o True).        
+0000c8f0: 6f64 645f 636f 756e 7420 3d20 7375 6d28  odd_count = sum(
+0000c900: 3120 666f 7220 6e75 6d20 696e 206e 756d  1 for num in num
+0000c910: 6265 725f 636f 6d62 696e 6174 696f 6e20  ber_combination 
+0000c920: 6966 206e 756d 2025 2032 290a 0a20 2020  if num % 2)..   
+0000c930: 2020 2020 2023 2043 6f75 6e74 2074 6865       # Count the
+0000c940: 206e 756d 6265 7220 6f66 2065 7665 6e20   number of even 
+0000c950: 6e75 6d62 6572 7320 696e 2074 6865 206e  numbers in the n
+0000c960: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
+0000c970: 6e0a 2020 2020 2020 2020 2320 4974 2773  n.        # It's
+0000c980: 2063 616c 6375 6c61 7465 6420 6279 2073   calculated by s
+0000c990: 7562 7472 6163 7469 6e67 2074 6865 206f  ubtracting the o
+0000c9a0: 6464 2063 6f75 6e74 2066 726f 6d20 7468  dd count from th
+0000c9b0: 6520 746f 7461 6c20 6c65 6e67 7468 206f  e total length o
+0000c9c0: 6620 7468 6520 6e75 6d62 6572 5f63 6f6d  f the number_com
+0000c9d0: 6269 6e61 7469 6f6e 0a20 2020 2020 2020  bination.       
+0000c9e0: 2065 7665 6e5f 636f 756e 7420 3d20 6c65   even_count = le
+0000c9f0: 6e28 6c69 7374 286e 756d 6265 725f 636f  n(list(number_co
+0000ca00: 6d62 696e 6174 696f 6e29 2920 2d20 6f64  mbination)) - od
+0000ca10: 645f 636f 756e 740a 0a20 2020 2020 2020  d_count..       
+0000ca20: 2023 2052 6574 7572 6e20 6120 7475 706c   # Return a tupl
+0000ca30: 6520 6f66 206f 6464 2061 6e64 2065 7665  e of odd and eve
+0000ca40: 6e20 636f 756e 7473 0a20 2020 2020 2020  n counts.       
+0000ca50: 2072 6574 7572 6e20 6f64 645f 636f 756e   return odd_coun
+0000ca60: 742c 2065 7665 6e5f 636f 756e 740a 0a20  t, even_count.. 
+0000ca70: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+0000ca80: 2020 2020 6465 6620 6361 6c63 756c 6174      def calculat
+0000ca90: 655f 7072 696d 655f 636f 6d70 6f73 6974  e_prime_composit
+0000caa0: 655f 7261 7469 6f28 0a20 2020 2020 2020  e_ratio(.       
+0000cab0: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
+0000cac0: 2020 2020 2020 6e75 6d62 6572 5f63 6f6d        number_com
+0000cad0: 6269 6e61 7469 6f6e 3a20 4974 6572 6162  bination: Iterab
+0000cae0: 6c65 5b69 6e74 5d2c 0a20 2020 2020 2020  le[int],.       
+0000caf0: 2020 2020 202a 2a6b 7761 7267 733a 2041       **kwargs: A
+0000cb00: 6e79 0a20 2020 2029 202d 3e20 5475 706c  ny.    ) -> Tupl
+0000cb10: 655b 696e 742c 2069 6e74 5d3a 0a20 2020  e[int, int]:.   
+0000cb20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000cb30: 2043 616c 6375 6c61 7465 2074 6865 2072   Calculate the r
+0000cb40: 6174 696f 206f 6620 7072 696d 6520 746f  atio of prime to
+0000cb50: 2063 6f6d 706f 7369 7465 206e 756d 6265   composite numbe
+0000cb60: 7273 2069 6e20 6120 7365 7175 656e 6365  rs in a sequence
+0000cb70: 206f 6620 6e75 6d62 6572 7320 7072 6f76   of numbers prov
+0000cb80: 6964 6564 2069 6e20 7468 6520 6e75 6d62  ided in the numb
+0000cb90: 6572 5f63 6f6d 6269 6e61 7469 6f6e 2e0a  er_combination..
+0000cba0: 2020 2020 2020 2020 496e 2074 6869 7320          In this 
+0000cbb0: 636f 6e74 6578 742c 2074 6865 206e 756d  context, the num
+0000cbc0: 6265 7220 3120 6973 2063 6f6e 7369 6465  ber 1 is conside
+0000cbd0: 7265 6420 6120 7072 696d 6520 6e75 6d62  red a prime numb
+0000cbe0: 6572 2e0a 0a20 2020 2020 2020 203a 7061  er...        :pa
+0000cbf0: 7261 6d20 6e75 6d62 6572 5f63 6f6d 6269  ram number_combi
+0000cc00: 6e61 7469 6f6e 3a20 4120 6c69 7374 206f  nation: A list o
+0000cc10: 7220 7475 706c 6520 6f66 206e 756d 6572  r tuple of numer
+0000cc20: 6963 616c 2076 616c 7565 732e 2054 6865  ical values. The
+0000cc30: 206d 6574 686f 6420 7769 6c6c 2064 6574   method will det
+0000cc40: 6572 6d69 6e65 2077 6869 6368 206e 756d  ermine which num
+0000cc50: 6265 7273 2061 7265 0a20 2020 2020 2020  bers are.       
+0000cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc70: 2020 2020 2020 2020 2020 2020 7072 696d              prim
+0000cc80: 6520 2869 6e63 6c75 6469 6e67 2031 2920  e (including 1) 
+0000cc90: 616e 6420 7768 6963 6820 6172 6520 636f  and which are co
+0000cca0: 6d70 6f73 6974 652c 2061 6e64 2063 6f6d  mposite, and com
+0000ccb0: 7075 7465 2074 6865 6972 2063 6f75 6e74  pute their count
+0000ccc0: 732e 0a20 2020 2020 2020 203a 7061 7261  s..        :para
+0000ccd0: 6d20 6b77 6172 6773 3a20 4164 6469 7469  m kwargs: Additi
+0000cce0: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
+0000ccf0: 756d 656e 7473 2c20 6e6f 7420 7573 6564  uments, not used
+0000cd00: 2069 6e20 7468 6973 2066 756e 6374 696f   in this functio
+0000cd10: 6e20 6275 7420 696e 636c 7564 6564 2066  n but included f
+0000cd20: 6f72 2070 6f74 656e 7469 616c 2066 7574  or potential fut
+0000cd30: 7572 650a 2020 2020 2020 2020 2020 2020  ure.            
+0000cd40: 2020 2020 2020 2020 2020 2065 7874 656e             exten
+0000cd50: 7369 6269 6c69 7479 206f 6620 7468 6520  sibility of the 
+0000cd60: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
+0000cd70: 3a72 6574 7572 6e3a 2041 2074 7570 6c65  :return: A tuple
+0000cd80: 2063 6f6e 7461 696e 696e 6720 7477 6f20   containing two 
+0000cd90: 656c 656d 656e 7473 3b20 7468 6520 6669  elements; the fi
+0000cda0: 7273 7420 6973 2074 6865 2063 6f75 6e74  rst is the count
+0000cdb0: 206f 6620 7072 696d 6520 6e75 6d62 6572   of prime number
+0000cdc0: 7320 2869 6e63 6c75 6469 6e67 2031 2920  s (including 1) 
+0000cdd0: 616e 6420 7468 650a 2020 2020 2020 2020  and the.        
+0000cde0: 2020 2020 2020 2020 2073 6563 6f6e 6420           second 
+0000cdf0: 6973 2074 6865 2063 6f75 6e74 206f 6620  is the count of 
+0000ce00: 636f 6d70 6f73 6974 6520 6e75 6d62 6572  composite number
+0000ce10: 7320 696e 2074 6865 206e 756d 6265 725f  s in the number_
+0000ce20: 636f 6d62 696e 6174 696f 6e2e 0a20 2020  combination..   
+0000ce30: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+0000ce40: 2020 6465 6620 6973 5f70 7269 6d65 286e    def is_prime(n
+0000ce50: 756d 3a20 696e 7429 202d 3e20 626f 6f6c  um: int) -> bool
+0000ce60: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000ce70: 436f 6e73 6964 6572 2031 2061 7320 6120  Consider 1 as a 
+0000ce80: 7072 696d 6520 6e75 6d62 6572 2066 6f72  prime number for
+0000ce90: 2074 6865 2070 7572 706f 7365 206f 6620   the purpose of 
+0000cea0: 7468 6973 2063 616c 6375 6c61 7469 6f6e  this calculation
+0000ceb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000cec0: 6e75 6d20 3d3d 2031 3a0a 2020 2020 2020  num == 1:.      
+0000ced0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000cee0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+0000cef0: 2020 2320 4578 636c 7564 6520 6e75 6d62    # Exclude numb
+0000cf00: 6572 7320 6c65 7373 2074 6861 6e20 3120  ers less than 1 
+0000cf10: 616e 6420 6576 656e 206e 756d 6265 7273  and even numbers
+0000cf20: 2067 7265 6174 6572 2074 6861 6e20 3220   greater than 2 
+0000cf30: 6173 2074 6865 7920 6172 6520 6e6f 7420  as they are not 
+0000cf40: 7072 696d 650a 2020 2020 2020 2020 2020  prime.          
+0000cf50: 2020 6966 206e 756d 203c 2031 206f 7220    if num < 1 or 
+0000cf60: 286e 756d 2025 2032 203d 3d20 3020 616e  (num % 2 == 0 an
+0000cf70: 6420 6e75 6d20 3e20 3229 3a0a 2020 2020  d num > 2):.    
+0000cf80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000cf90: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0000cfa0: 2020 2020 2023 2043 6865 636b 2066 6f72       # Check for
+0000cfb0: 2066 6163 746f 7273 2066 726f 6d20 3320   factors from 3 
+0000cfc0: 746f 2074 6865 2073 7175 6172 6520 726f  to the square ro
+0000cfd0: 6f74 206f 6620 6e75 6d0a 2020 2020 2020  ot of num.      
+0000cfe0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000cff0: 616e 6765 2833 2c20 696e 7428 6e75 6d20  ange(3, int(num 
+0000d000: 2a2a 2030 2e35 2920 2b20 312c 2032 293a  ** 0.5) + 1, 2):
+0000d010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d020: 2069 6620 6e75 6d20 2520 6920 3d3d 2030   if num % i == 0
+0000d030: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d040: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0000d050: 7365 0a20 2020 2020 2020 2020 2020 2072  se.            r
+0000d060: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+0000d070: 2020 2020 2320 436f 756e 7420 7072 696d      # Count prim
+0000d080: 6520 6e75 6d62 6572 7320 696e 2074 6865  e numbers in the
+0000d090: 206e 756d 6265 725f 636f 6d62 696e 6174   number_combinat
+0000d0a0: 696f 6e0a 2020 2020 2020 2020 7072 696d  ion.        prim
+0000d0b0: 655f 636f 756e 7420 3d20 7375 6d28 3120  e_count = sum(1 
+0000d0c0: 666f 7220 6e75 6d20 696e 206e 756d 6265  for num in numbe
+0000d0d0: 725f 636f 6d62 696e 6174 696f 6e20 6966  r_combination if
+0000d0e0: 2069 735f 7072 696d 6528 6e75 6d29 290a   is_prime(num)).
+0000d0f0: 2020 2020 2020 2020 2320 436f 756e 7420          # Count 
+0000d100: 636f 6d70 6f73 6974 6520 6e75 6d62 6572  composite number
+0000d110: 7320 6173 2074 6865 2072 656d 6169 6e69  s as the remaini
+0000d120: 6e67 206e 756d 6265 7273 2069 6e20 7468  ng numbers in th
+0000d130: 6520 6e75 6d62 6572 5f63 6f6d 6269 6e61  e number_combina
+0000d140: 7469 6f6e 0a20 2020 2020 2020 2063 6f6d  tion.        com
+0000d150: 706f 7369 7465 5f63 6f75 6e74 203d 206c  posite_count = l
+0000d160: 656e 286c 6973 7428 6e75 6d62 6572 5f63  en(list(number_c
+0000d170: 6f6d 6269 6e61 7469 6f6e 2929 202d 2070  ombination)) - p
+0000d180: 7269 6d65 5f63 6f75 6e74 0a0a 2020 2020  rime_count..    
+0000d190: 2020 2020 2320 5265 7475 726e 2061 2074      # Return a t
+0000d1a0: 7570 6c65 206f 6620 7072 696d 6520 616e  uple of prime an
+0000d1b0: 6420 636f 6d70 6f73 6974 6520 636f 756e  d composite coun
+0000d1c0: 7473 0a20 2020 2020 2020 2072 6574 7572  ts.        retur
+0000d1d0: 6e20 7072 696d 655f 636f 756e 742c 2063  n prime_count, c
+0000d1e0: 6f6d 706f 7369 7465 5f63 6f75 6e74 0a0a  omposite_count..
+0000d1f0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+0000d200: 0a20 2020 2064 6566 2063 616c 6375 6c61  .    def calcula
+0000d210: 7465 5f73 7061 6e28 0a20 2020 2020 2020  te_span(.       
+0000d220: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
+0000d230: 2020 2020 2020 6e75 6d62 6572 5f63 6f6d        number_com
+0000d240: 6269 6e61 7469 6f6e 3a0a 2020 2020 2020  bination:.      
+0000d250: 2020 2020 2020 4974 6572 6162 6c65 5b69        Iterable[i
+0000d260: 6e74 5d2c 0a20 2020 2020 2020 2020 2020  nt],.           
+0000d270: 202a 2a6b 7761 7267 733a 2041 6e79 0a20   **kwargs: Any. 
+0000d280: 2020 2029 202d 3e20 696e 743a 0a20 2020     ) -> int:.   
+0000d290: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d2a0: 2043 616c 6375 6c61 7465 2074 6865 2073   Calculate the s
+0000d2b0: 7061 6e20 6f66 2061 2073 6571 7565 6e63  pan of a sequenc
+0000d2c0: 6520 6f66 206e 756d 6265 7273 2070 726f  e of numbers pro
+0000d2d0: 7669 6465 6420 696e 2074 6865 206e 756d  vided in the num
+0000d2e0: 6265 725f 636f 6d62 696e 6174 696f 6e2e  ber_combination.
+0000d2f0: 2054 6865 2073 7061 6e20 6973 2064 6566   The span is def
+0000d300: 696e 6564 2061 7320 7468 650a 2020 2020  ined as the.    
+0000d310: 2020 2020 6469 6666 6572 656e 6365 2062      difference b
+0000d320: 6574 7765 656e 2074 6865 206d 6178 696d  etween the maxim
+0000d330: 756d 2061 6e64 206d 696e 696d 756d 2076  um and minimum v
+0000d340: 616c 7565 7320 696e 2074 6865 2073 6574  alues in the set
+0000d350: 206f 6620 6e75 6d62 6572 732e 0a0a 2020   of numbers...  
+0000d360: 2020 2020 2020 3a70 6172 616d 206e 756d        :param num
+0000d370: 6265 725f 636f 6d62 696e 6174 696f 6e3a  ber_combination:
+0000d380: 2041 206c 6973 7420 6f72 2074 7570 6c65   A list or tuple
+0000d390: 206f 6620 6e75 6d65 7269 6361 6c20 7661   of numerical va
+0000d3a0: 6c75 6573 2e20 5468 6520 6d65 7468 6f64  lues. The method
+0000d3b0: 2077 696c 6c20 6669 6e64 2074 6865 206d   will find the m
+0000d3c0: 6178 696d 756d 2061 6e64 206d 696e 696d  aximum and minim
+0000d3d0: 756d 0a20 2020 2020 2020 2020 2020 2020  um.             
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3f0: 2020 2020 2020 7661 6c75 6573 2069 6e20        values in 
+0000d400: 7468 6973 2063 6f6c 6c65 6374 696f 6e20  this collection 
+0000d410: 616e 6420 6361 6c63 756c 6174 6520 7468  and calculate th
+0000d420: 6520 6469 6666 6572 656e 6365 2028 7370  e difference (sp
+0000d430: 616e 2920 6265 7477 6565 6e20 7468 656d  an) between them
+0000d440: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000d450: 206b 7761 7267 733a 2041 6464 6974 696f   kwargs: Additio
+0000d460: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+0000d470: 6d65 6e74 732c 206e 6f74 2075 7365 6420  ments, not used 
+0000d480: 696e 2074 6869 7320 6675 6e63 7469 6f6e  in this function
+0000d490: 2062 7574 2069 6e63 6c75 6465 6420 666f   but included fo
+0000d4a0: 7220 706f 7465 6e74 6961 6c20 6675 7475  r potential futu
+0000d4b0: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
+0000d4c0: 2020 2020 2020 2020 2020 6578 7465 6e73            extens
+0000d4d0: 6962 696c 6974 7920 6f66 2074 6865 206d  ibility of the m
+0000d4e0: 6574 686f 642e 0a20 2020 2020 2020 203a  ethod..        :
+0000d4f0: 7265 7475 726e 3a20 5468 6520 7370 616e  return: The span
+0000d500: 206f 6620 7468 6520 6e75 6d62 6572 7320   of the numbers 
+0000d510: 696e 2074 6865 206e 756d 6265 725f 636f  in the number_co
+0000d520: 6d62 696e 6174 696f 6e20 6173 2061 6e20  mbination as an 
+0000d530: 696e 7465 6765 722e 2049 6620 7468 6520  integer. If the 
+0000d540: 696e 7075 7420 636f 6e74 6169 6e73 2066  input contains f
+0000d550: 6c6f 6174 696e 670a 2020 2020 2020 2020  loating.        
+0000d560: 2020 2020 2020 2020 2070 6f69 6e74 206e           point n
+0000d570: 756d 6265 7273 2c20 7468 6520 7370 616e  umbers, the span
+0000d580: 2069 7320 6361 7374 2074 6f20 616e 2069   is cast to an i
+0000d590: 6e74 6567 6572 2062 6566 6f72 6520 6265  nteger before be
+0000d5a0: 696e 6720 7265 7475 726e 6564 2e0a 2020  ing returned..  
+0000d5b0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000d5c0: 2020 2023 2046 696e 6420 7468 6520 6d61     # Find the ma
+0000d5d0: 7869 6d75 6d20 616e 6420 6d69 6e69 6d75  ximum and minimu
+0000d5e0: 6d20 7661 6c75 6573 2069 6e20 7468 6520  m values in the 
+0000d5f0: 6e75 6d62 6572 2063 6f6d 6269 6e61 7469  number combinati
+0000d600: 6f6e 0a20 2020 2020 2020 206d 6178 5f76  on.        max_v
+0000d610: 616c 7565 203d 206d 6178 286e 756d 6265  alue = max(numbe
+0000d620: 725f 636f 6d62 696e 6174 696f 6e29 0a20  r_combination). 
+0000d630: 2020 2020 2020 206d 696e 5f76 616c 7565         min_value
+0000d640: 203d 206d 696e 286e 756d 6265 725f 636f   = min(number_co
+0000d650: 6d62 696e 6174 696f 6e29 0a0a 2020 2020  mbination)..    
+0000d660: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
+0000d670: 7468 6520 7370 616e 2062 7920 7375 6274  the span by subt
+0000d680: 7261 6374 696e 6720 7468 6520 6d69 6e69  racting the mini
+0000d690: 6d75 6d20 7661 6c75 6520 6672 6f6d 2074  mum value from t
+0000d6a0: 6865 206d 6178 696d 756d 2076 616c 7565  he maximum value
+0000d6b0: 0a20 2020 2020 2020 2073 7061 6e20 3d20  .        span = 
+0000d6c0: 6d61 785f 7661 6c75 6520 2d20 6d69 6e5f  max_value - min_
+0000d6d0: 7661 6c75 650a 0a20 2020 2020 2020 2023  value..        #
+0000d6e0: 2043 6173 7420 7468 6520 7370 616e 2074   Cast the span t
+0000d6f0: 6f20 616e 2069 6e74 6567 6572 2061 6e64  o an integer and
+0000d700: 2072 6574 7572 6e20 6974 0a20 2020 2020   return it.     
+0000d710: 2020 2072 6574 7572 6e20 696e 7428 7370     return int(sp
+0000d720: 616e 290a 0a20 2020 2040 636c 6173 736d  an)..    @classm
+0000d730: 6574 686f 640a 2020 2020 6465 6620 6361  ethod.    def ca
+0000d740: 6c63 756c 6174 655f 7375 6d5f 746f 7461  lculate_sum_tota
+0000d750: 6c28 0a20 2020 2020 2020 2020 2020 2063  l(.            c
+0000d760: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+0000d770: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
+0000d780: 6f6e 3a20 4974 6572 6162 6c65 5b55 6e69  on: Iterable[Uni
+0000d790: 6f6e 5b69 6e74 2c20 666c 6f61 745d 5d2c  on[int, float]],
+0000d7a0: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+0000d7b0: 7761 7267 733a 2041 6e79 0a20 2020 2029  wargs: Any.    )
+0000d7c0: 202d 3e20 556e 696f 6e5b 696e 742c 2066   -> Union[int, f
+0000d7d0: 6c6f 6174 5d3a 0a20 2020 2020 2020 2022  loat]:.        "
+0000d7e0: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
+0000d7f0: 6c61 7465 2074 6865 2074 6f74 616c 2073  late the total s
+0000d800: 756d 206f 6620 6120 7365 7175 656e 6365  um of a sequence
+0000d810: 206f 6620 6e75 6d62 6572 7320 7072 6f76   of numbers prov
+0000d820: 6964 6564 2069 6e20 7468 6520 6e75 6d62  ided in the numb
+0000d830: 6572 5f63 6f6d 6269 6e61 7469 6f6e 2e20  er_combination. 
+0000d840: 5468 6973 206d 6574 686f 640a 2020 2020  This method.    
+0000d850: 2020 2020 6167 6772 6567 6174 6573 2061      aggregates a
+0000d860: 6c6c 2074 6865 206e 756d 6572 6963 616c  ll the numerical
+0000d870: 2076 616c 7565 7320 696e 2074 6865 206c   values in the l
+0000d880: 6973 7420 6f72 2074 7570 6c65 2070 6173  ist or tuple pas
+0000d890: 7365 6420 6173 2061 6e20 6172 6775 6d65  sed as an argume
+0000d8a0: 6e74 2061 6e64 2072 6574 7572 6e73 2074  nt and returns t
+0000d8b0: 6865 6972 2073 756d 2e0a 0a20 2020 2020  heir sum...     
+0000d8c0: 2020 203a 7061 7261 6d20 6e75 6d62 6572     :param number
+0000d8d0: 5f63 6f6d 6269 6e61 7469 6f6e 3a20 4120  _combination: A 
+0000d8e0: 6c69 7374 206f 7220 7475 706c 6520 6f66  list or tuple of
+0000d8f0: 206e 756d 6572 6963 616c 2076 616c 7565   numerical value
+0000d900: 732e 2054 6865 206d 6574 686f 6420 7769  s. The method wi
+0000d910: 6c6c 2073 756d 2074 6865 7365 2076 616c  ll sum these val
+0000d920: 7565 7320 616e 6420 7265 7475 726e 0a20  ues and return. 
+0000d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d950: 2020 7468 6520 7265 7375 6c74 2e0a 2020    the result..  
+0000d960: 2020 2020 2020 3a70 6172 616d 206b 7761        :param kwa
+0000d970: 7267 733a 2041 6464 6974 696f 6e61 6c20  rgs: Additional 
+0000d980: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+0000d990: 732c 206e 6f74 2075 7365 6420 696e 2074  s, not used in t
+0000d9a0: 6869 7320 6675 6e63 7469 6f6e 2062 7574  his function but
+0000d9b0: 2069 6e63 6c75 6465 6420 666f 7220 706f   included for po
+0000d9c0: 7465 6e74 6961 6c20 6675 7475 7265 0a20  tential future. 
+0000d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9e0: 2020 2020 2020 6578 7465 6e73 6962 696c        extensibil
+0000d9f0: 6974 7920 6f66 2074 6865 206d 6574 686f  ity of the metho
+0000da00: 642e 0a20 2020 2020 2020 203a 7265 7475  d..        :retu
+0000da10: 726e 3a20 5468 6520 7375 6d20 746f 7461  rn: The sum tota
+0000da20: 6c20 6f66 2074 6865 206e 756d 6265 7273  l of the numbers
+0000da30: 2069 6e20 7468 6520 6e75 6d62 6572 5f63   in the number_c
+0000da40: 6f6d 6269 6e61 7469 6f6e 2061 7320 616e  ombination as an
+0000da50: 2069 6e74 6567 6572 206f 7220 666c 6f61   integer or floa
+0000da60: 742c 2064 6570 656e 6469 6e67 206f 6e20  t, depending on 
+0000da70: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0000da80: 2020 2020 2069 6e70 7574 2076 616c 7565       input value
+0000da90: 732e 0a20 2020 2020 2020 2022 2222 0a0a  s..        """..
+0000daa0: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
+0000dab0: 6174 6520 7468 6520 7375 6d20 6f66 2074  ate the sum of t
+0000dac0: 6865 206e 756d 6265 7273 2069 6e20 7468  he numbers in th
+0000dad0: 6520 636f 6d62 696e 6174 696f 6e20 7573  e combination us
+0000dae0: 696e 6720 7468 6520 6275 696c 742d 696e  ing the built-in
+0000daf0: 2073 756d 2066 756e 6374 696f 6e0a 2020   sum function.  
+0000db00: 2020 2020 2020 746f 7461 6c5f 7375 6d20        total_sum 
+0000db10: 3d20 7375 6d28 6e75 6d62 6572 5f63 6f6d  = sum(number_com
+0000db20: 6269 6e61 7469 6f6e 290a 0a20 2020 2020  bination)..     
+0000db30: 2020 2023 2052 6574 7572 6e20 7468 6520     # Return the 
+0000db40: 7375 6d20 746f 7461 6c0a 2020 2020 2020  sum total.      
+0000db50: 2020 7265 7475 726e 2074 6f74 616c 5f73    return total_s
+0000db60: 756d 0a0a 2020 2020 4063 6c61 7373 6d65  um..    @classme
+0000db70: 7468 6f64 0a20 2020 2064 6566 2063 616c  thod.    def cal
+0000db80: 6375 6c61 7465 5f73 756d 5f74 6169 6c28  culate_sum_tail(
+0000db90: 0a20 2020 2020 2020 2020 2020 2063 6c73  .            cls
+0000dba0: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
+0000dbb0: 6d62 6572 5f63 6f6d 6269 6e61 7469 6f6e  mber_combination
+0000dbc0: 3a20 4974 6572 6162 6c65 5b69 6e74 5d2c  : Iterable[int],
+0000dbd0: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+0000dbe0: 7761 7267 733a 2041 6e79 0a20 2020 2029  wargs: Any.    )
+0000dbf0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+0000dc00: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+0000dc10: 6375 6c61 7465 2074 6865 206c 6173 7420  culate the last 
+0000dc20: 6469 6769 7420 2874 6169 6c29 206f 6620  digit (tail) of 
+0000dc30: 7468 6520 7375 6d20 6f66 2061 2067 6976  the sum of a giv
+0000dc40: 656e 206e 756d 6265 7220 636f 6d62 696e  en number combin
+0000dc50: 6174 696f 6e2e 2054 6865 2074 6169 6c20  ation. The tail 
+0000dc60: 6973 2074 6865 2075 6e69 7427 7320 706c  is the unit's pl
+0000dc70: 6163 650a 2020 2020 2020 2020 6f66 2074  ace.        of t
+0000dc80: 6865 2073 756d 2c20 7768 6963 6820 6361  he sum, which ca
+0000dc90: 6e20 6265 2075 7365 6675 6c20 666f 7220  n be useful for 
+0000dca0: 6365 7274 6169 6e20 7479 7065 7320 6f66  certain types of
+0000dcb0: 206e 756d 6572 6963 616c 2061 6e61 6c79   numerical analy
+0000dcc0: 7369 7320 6f72 2070 6174 7465 726e 2072  sis or pattern r
+0000dcd0: 6563 6f67 6e69 7469 6f6e 2e0a 0a20 2020  ecognition...   
+0000dce0: 2020 2020 203a 7061 7261 6d20 6e75 6d62       :param numb
+0000dcf0: 6572 5f63 6f6d 6269 6e61 7469 6f6e 3a20  er_combination: 
+0000dd00: 4120 6c69 7374 206f 7220 7475 706c 6520  A list or tuple 
+0000dd10: 6f66 206e 756d 6572 6963 616c 2076 616c  of numerical val
+0000dd20: 7565 732e 2054 6865 2073 756d 206f 6620  ues. The sum of 
+0000dd30: 7468 6573 6520 6e75 6d62 6572 7320 7769  these numbers wi
+0000dd40: 6c6c 2062 6520 6361 6c63 756c 6174 6564  ll be calculated
+0000dd50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd70: 2020 2020 2061 6e64 2074 6865 2074 6169       and the tai
+0000dd80: 6c20 6f66 2074 6869 7320 7375 6d20 286c  l of this sum (l
+0000dd90: 6173 7420 6469 6769 7429 2077 696c 6c20  ast digit) will 
+0000dda0: 6265 2072 6574 7572 6e65 642e 0a20 2020  be returned..   
+0000ddb0: 2020 2020 203a 7061 7261 6d20 6b77 6172       :param kwar
+0000ddc0: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
+0000ddd0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+0000dde0: 2c20 6e6f 7420 7573 6564 2069 6e20 7468  , not used in th
+0000ddf0: 6973 2066 756e 6374 696f 6e20 6275 7420  is function but 
+0000de00: 696e 636c 7564 6564 2066 6f72 2070 6f74  included for pot
+0000de10: 656e 7469 616c 2066 7574 7572 650a 2020  ential future.  
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2020 2020 2065 7874 656e 7369 6269 6c69       extensibili
+0000de40: 7479 206f 6620 7468 6520 6d65 7468 6f64  ty of the method
+0000de50: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+0000de60: 6e3a 2054 6865 206c 6173 7420 6469 6769  n: The last digi
+0000de70: 7420 6f66 2074 6865 2073 756d 206f 6620  t of the sum of 
+0000de80: 7468 6520 6e75 6d62 6572 2063 6f6d 6269  the number combi
+0000de90: 6e61 7469 6f6e 2061 7320 616e 2069 6e74  nation as an int
+0000dea0: 6567 6572 2e0a 2020 2020 2020 2020 2222  eger..        ""
+0000deb0: 220a 0a20 2020 2020 2020 2023 2043 616c  "..        # Cal
+0000dec0: 6375 6c61 7465 2074 6865 2073 756d 206f  culate the sum o
+0000ded0: 6620 7468 6520 6e75 6d62 6572 7320 696e  f the numbers in
+0000dee0: 2074 6865 2063 6f6d 6269 6e61 7469 6f6e   the combination
+0000def0: 0a20 2020 2020 2020 2074 6f74 616c 5f73  .        total_s
+0000df00: 756d 203d 2063 6c73 2e63 616c 6375 6c61  um = cls.calcula
+0000df10: 7465 5f73 756d 5f74 6f74 616c 286e 756d  te_sum_total(num
+0000df20: 6265 725f 636f 6d62 696e 6174 696f 6e29  ber_combination)
+0000df30: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
+0000df40: 726e 2074 6865 206c 6173 7420 6469 6769  rn the last digi
+0000df50: 7420 6f66 2074 6869 7320 7375 6d0a 2020  t of this sum.  
+0000df60: 2020 2020 2020 7265 7475 726e 2074 6f74        return tot
+0000df70: 616c 5f73 756d 2025 2031 300a 0a20 2020  al_sum % 10..   
+0000df80: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+0000df90: 2020 6465 6620 6361 6c63 756c 6174 655f    def calculate_
+0000dfa0: 7765 656b 6461 7928 0a20 2020 2020 2020  weekday(.       
+0000dfb0: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
+0000dfc0: 2020 2020 2020 6461 7465 3a20 7374 722c        date: str,
+0000dfd0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000dfe0: 655f 666f 726d 6174 3a20 7374 7220 3d20  e_format: str = 
+0000dff0: 2725 592d 256d 2d25 6427 2c0a 2020 2020  '%Y-%m-%d',.    
+0000e000: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0000e010: 3a20 416e 790a 2020 2020 2920 2d3e 2069  : Any.    ) -> i
+0000e020: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+0000e030: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
+0000e040: 6520 7468 6520 7765 656b 6461 7920 6e75  e the weekday nu
+0000e050: 6d62 6572 2066 726f 6d20 6120 6461 7465  mber from a date
+0000e060: 2073 7472 696e 672e 0a0a 2020 2020 2020   string...      
+0000e070: 2020 3a70 6172 616d 2064 6174 653a 2044    :param date: D
+0000e080: 6174 6520 7374 7269 6e67 2e0a 2020 2020  ate string..    
+0000e090: 2020 2020 3a70 6172 616d 2064 6174 655f      :param date_
+0000e0a0: 666f 726d 6174 3a20 6465 6661 756c 7420  format: default 
+0000e0b0: 2759 5959 592d 4d4d 2d44 4427 2066 6f72  'YYYY-MM-DD' for
+0000e0c0: 6d61 740a 2020 2020 2020 2020 3a72 6574  mat.        :ret
+0000e0d0: 7572 6e3a 2057 6565 6b64 6179 206e 756d  urn: Weekday num
+0000e0e0: 6265 7220 7768 6572 6520 3120 7265 7072  ber where 1 repr
+0000e0f0: 6573 656e 7473 204d 6f6e 6461 7920 616e  esents Monday an
+0000e100: 6420 3720 7265 7072 6573 656e 7473 2053  d 7 represents S
+0000e110: 756e 6461 792e 0a20 2020 2020 2020 2022  unday..        "
+0000e120: 2222 0a20 2020 2020 2020 2064 6174 6520  "".        date 
+0000e130: 3d20 6461 7465 7469 6d65 2e64 6174 6574  = datetime.datet
+0000e140: 696d 652e 7374 7270 7469 6d65 2864 6174  ime.strptime(dat
+0000e150: 652c 2064 6174 655f 666f 726d 6174 292e  e, date_format).
+0000e160: 6461 7465 2829 0a20 2020 2020 2020 2072  date().        r
+0000e170: 6574 7572 6e20 6461 7465 2e77 6565 6b64  eturn date.weekd
+0000e180: 6179 2829 202b 2031 0a0a 2020 2020 4063  ay() + 1..    @c
+0000e190: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+0000e1a0: 6566 2063 616c 6375 6c61 7465 5f61 6328  ef calculate_ac(
+0000e1b0: 0a20 2020 2020 2020 2020 2020 2063 6c73  .            cls
+0000e1c0: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
+0000e1d0: 6d62 6572 5f63 6f6d 6269 6e61 7469 6f6e  mber_combination
+0000e1e0: 3a20 4974 6572 6162 6c65 5b69 6e74 5d2c  : Iterable[int],
+0000e1f0: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+0000e200: 7761 7267 733a 2041 6e79 0a20 2020 2029  wargs: Any.    )
+0000e210: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+0000e220: 2022 2222 0a20 2020 2020 2020 2043 6f6d   """.        Com
+0000e230: 7075 7465 2074 6865 2063 6f6d 706c 6578  pute the complex
+0000e240: 6974 7920 6f66 2061 2067 6976 656e 206e  ity of a given n
+0000e250: 756d 6265 7220 636f 6d62 696e 6174 696f  umber combinatio
+0000e260: 6e2e 2043 6f6d 706c 6578 6974 7920 6973  n. Complexity is
+0000e270: 2064 6566 696e 6564 2061 7320 7468 6520   defined as the 
+0000e280: 6e75 6d62 6572 206f 6620 6469 7374 696e  number of distin
+0000e290: 6374 0a20 2020 2020 2020 2061 6273 6f6c  ct.        absol
+0000e2a0: 7574 6520 6469 6666 6572 656e 6365 7320  ute differences 
+0000e2b0: 6265 7477 6565 6e20 6561 6368 2070 6169  between each pai
+0000e2c0: 7220 6f66 206e 756d 6265 7273 2069 6e20  r of numbers in 
+0000e2d0: 7468 6520 636f 6d62 696e 6174 696f 6e2c  the combination,
+0000e2e0: 2065 7863 6c75 6469 6e67 2074 6865 206e   excluding the n
+0000e2f0: 756d 6265 7220 6f66 2065 6c65 6d65 6e74  umber of element
+0000e300: 7320 6d69 6e75 7320 6f6e 652e 0a0a 2020  s minus one...  
+0000e310: 2020 2020 2020 3a70 6172 616d 206e 756d        :param num
+0000e320: 6265 725f 636f 6d62 696e 6174 696f 6e3a  ber_combination:
+0000e330: 2041 206c 6973 7420 6f72 2074 7570 6c65   A list or tuple
+0000e340: 206f 6620 6e75 6d65 7269 6361 6c20 7661   of numerical va
+0000e350: 6c75 6573 2066 6f72 2077 6869 6368 2074  lues for which t
+0000e360: 6865 2063 6f6d 706c 6578 6974 7920 7769  he complexity wi
+0000e370: 6c6c 2062 6520 6361 6c63 756c 6174 6564  ll be calculated
+0000e380: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000e390: 206b 7761 7267 733a 2041 6464 6974 696f   kwargs: Additio
+0000e3a0: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+0000e3b0: 6d65 6e74 732c 206e 6f74 2075 7365 6420  ments, not used 
+0000e3c0: 696e 2074 6869 7320 6675 6e63 7469 6f6e  in this function
+0000e3d0: 2062 7574 2061 6c6c 6f77 7320 666f 7220   but allows for 
+0000e3e0: 6578 7465 6e73 6962 696c 6974 792e 0a20  extensibility.. 
+0000e3f0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+0000e400: 416e 2069 6e74 6567 6572 2072 6570 7265  An integer repre
+0000e410: 7365 6e74 696e 6720 7468 6520 636f 6d70  senting the comp
+0000e420: 6c65 7869 7479 206f 6620 7468 6520 6e75  lexity of the nu
+0000e430: 6d62 6572 2063 6f6d 6269 6e61 7469 6f6e  mber combination
+0000e440: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+0000e450: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
+0000e460: 697a 6520 6120 7365 7420 746f 2073 746f  ize a set to sto
+0000e470: 7265 2064 6973 7469 6e63 7420 6162 736f  re distinct abso
+0000e480: 6c75 7465 2064 6966 6665 7265 6e63 6573  lute differences
+0000e490: 0a20 2020 2020 2020 2064 6973 7469 6e63  .        distinc
+0000e4a0: 745f 6469 6666 7320 3d20 7365 7428 290a  t_diffs = set().
+0000e4b0: 0a20 2020 2020 2020 2023 2043 6f75 6e74  .        # Count
+0000e4c0: 2074 6865 206e 756d 6265 7220 6f66 2065   the number of e
+0000e4d0: 6c65 6d65 6e74 7320 696e 2074 6865 206e  lements in the n
+0000e4e0: 756d 6265 7220 636f 6d62 696e 6174 696f  umber combinatio
+0000e4f0: 6e0a 2020 2020 2020 2020 6e75 6d62 6572  n.        number
+0000e500: 5f63 6f6d 6269 6e61 7469 6f6e 5f6c 6973  _combination_lis
+0000e510: 7420 3d20 6c69 7374 286e 756d 6265 725f  t = list(number_
+0000e520: 636f 6d62 696e 6174 696f 6e29 0a20 2020  combination).   
+0000e530: 2020 2020 206e 756d 5f63 6f75 6e74 203d       num_count =
+0000e540: 206c 656e 286e 756d 6265 725f 636f 6d62   len(number_comb
+0000e550: 696e 6174 696f 6e5f 6c69 7374 290a 0a20  ination_list).. 
+0000e560: 2020 2020 2020 2023 2049 7465 7261 7465         # Iterate
+0000e570: 206f 7665 7220 6561 6368 2075 6e69 7175   over each uniqu
+0000e580: 6520 7061 6972 206f 6620 6e75 6d62 6572  e pair of number
+0000e590: 7320 746f 2063 616c 6375 6c61 7465 2061  s to calculate a
+0000e5a0: 6273 6f6c 7574 6520 6469 6666 6572 656e  bsolute differen
+0000e5b0: 6365 730a 2020 2020 2020 2020 666f 7220  ces.        for 
+0000e5c0: 6920 696e 2072 616e 6765 286e 756d 5f63  i in range(num_c
+0000e5d0: 6f75 6e74 293a 0a20 2020 2020 2020 2020  ount):.         
+0000e5e0: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+0000e5f0: 6528 6920 2b20 312c 206e 756d 5f63 6f75  e(i + 1, num_cou
+0000e600: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+0000e610: 2020 2020 2023 2043 616c 6375 6c61 7465       # Calculate
+0000e620: 2074 6865 2061 6273 6f6c 7574 6520 6469   the absolute di
+0000e630: 6666 6572 656e 6365 2062 6574 7765 656e  fference between
+0000e640: 2074 6865 2074 776f 206e 756d 6265 7273   the two numbers
+0000e650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e660: 2064 6966 6620 3d20 6162 7328 6e75 6d62   diff = abs(numb
+0000e670: 6572 5f63 6f6d 6269 6e61 7469 6f6e 5f6c  er_combination_l
+0000e680: 6973 745b 6a5d 202d 206e 756d 6265 725f  ist[j] - number_
+0000e690: 636f 6d62 696e 6174 696f 6e5f 6c69 7374  combination_list
+0000e6a0: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+0000e6b0: 2020 2020 2023 2041 6464 2074 6865 2061       # Add the a
+0000e6c0: 6273 6f6c 7574 6520 6469 6666 6572 656e  bsolute differen
+0000e6d0: 6365 2074 6f20 7468 6520 7365 7420 6f66  ce to the set of
+0000e6e0: 2064 6973 7469 6e63 7420 6469 6666 6572   distinct differ
+0000e6f0: 656e 6365 730a 2020 2020 2020 2020 2020  ences.          
+0000e700: 2020 2020 2020 6469 7374 696e 6374 5f64        distinct_d
+0000e710: 6966 6673 2e61 6464 2864 6966 6629 0a0a  iffs.add(diff)..
+0000e720: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+0000e730: 2074 6865 206e 756d 6265 7220 6f66 2064   the number of d
+0000e740: 6973 7469 6e63 7420 6469 6666 6572 656e  istinct differen
+0000e750: 6365 7320 6d69 6e75 7320 7468 6520 6e75  ces minus the nu
+0000e760: 6d62 6572 206f 6620 656c 656d 656e 7473  mber of elements
+0000e770: 206d 696e 7573 206f 6e65 0a20 2020 2020   minus one.     
+0000e780: 2020 2072 6574 7572 6e20 6c65 6e28 6469     return len(di
+0000e790: 7374 696e 6374 5f64 6966 6673 2920 2d20  stinct_diffs) - 
+0000e7a0: 286e 756d 5f63 6f75 6e74 202d 2031 290a  (num_count - 1).
+0000e7b0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+0000e7c0: 640a 2020 2020 6465 6620 6361 6c63 756c  d.    def calcul
+0000e7d0: 6174 655f 6176 6728 636c 732c 206e 756d  ate_avg(cls, num
+0000e7e0: 6265 725f 636f 6d62 696e 6174 696f 6e3a  ber_combination:
+0000e7f0: 2049 7465 7261 626c 655b 696e 745d 2c20   Iterable[int], 
+0000e800: 2a2a 6b77 6172 6773 3a20 416e 7929 202d  **kwargs: Any) -
+0000e810: 3e20 696e 743a 0a20 2020 2020 2020 2072  > int:.        r
+0000e820: 6574 7572 6e20 6d61 7468 2e66 6c6f 6f72  eturn math.floor
+0000e830: 2873 756d 286e 756d 6265 725f 636f 6d62  (sum(number_comb
+0000e840: 696e 6174 696f 6e29 202f 206c 656e 286c  ination) / len(l
+0000e850: 6973 7428 6e75 6d62 6572 5f63 6f6d 6269  ist(number_combi
+0000e860: 6e61 7469 6f6e 2929 290a 0a20 2020 2040  nation)))..    @
+0000e870: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+0000e880: 6465 6620 6361 6c63 756c 6174 655f 636f  def calculate_co
+0000e890: 6e73 6563 7574 6976 655f 6e75 6d62 6572  nsecutive_number
+0000e8a0: 7328 0a20 2020 2020 2020 2020 2020 2063  s(.            c
+0000e8b0: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+0000e8c0: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
+0000e8d0: 6f6e 3a20 4974 6572 6162 6c65 5b69 6e74  on: Iterable[int
+0000e8e0: 5d2c 0a20 2020 2020 2020 2020 2020 202a  ],.            *
+0000e8f0: 2a6b 7761 7267 733a 2041 6e79 0a20 2020  *kwargs: Any.   
+0000e900: 2029 202d 3e20 4c69 7374 5b4c 6973 745b   ) -> List[List[
+0000e910: 696e 745d 5d3a 0a20 2020 2020 2020 2022  int]]:.        "
+0000e920: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
+0000e930: 6c61 7465 2074 6865 2073 6571 7565 6e63  late the sequenc
+0000e940: 6573 206f 6620 636f 6e73 6563 7574 6976  es of consecutiv
+0000e950: 6520 6e75 6d62 6572 7320 696e 2061 2067  e numbers in a g
+0000e960: 6976 656e 2069 7465 7261 626c 6520 6f66  iven iterable of
+0000e970: 2069 6e74 6567 6572 732e 0a0a 2020 2020   integers...    
+0000e980: 2020 2020 3a70 6172 616d 206e 756d 6265      :param numbe
+0000e990: 725f 636f 6d62 696e 6174 696f 6e3a 2041  r_combination: A
+0000e9a0: 6e20 6974 6572 6162 6c65 206f 6620 696e  n iterable of in
+0000e9b0: 7465 6765 7273 2074 6f20 636f 6d70 7574  tegers to comput
+0000e9c0: 6520 636f 6e73 6563 7574 6976 6520 6e75  e consecutive nu
+0000e9d0: 6d62 6572 7320 6672 6f6d 2e0a 2020 2020  mbers from..    
+0000e9e0: 2020 2020 3a70 6172 616d 206b 7761 7267      :param kwarg
+0000e9f0: 733a 2041 6464 6974 696f 6e61 6c20 6b65  s: Additional ke
+0000ea00: 7977 6f72 6420 6172 6775 6d65 6e74 732e  yword arguments.
+0000ea10: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000ea20: 3a20 4120 6c69 7374 206f 6620 6c69 7374  : A list of list
+0000ea30: 732c 2065 6163 6820 636f 6e74 6169 6e69  s, each containi
+0000ea40: 6e67 2061 2073 6571 7565 6e63 6520 6f66  ng a sequence of
+0000ea50: 2063 6f6e 7365 6375 7469 7665 206e 756d   consecutive num
+0000ea60: 6265 7273 2e0a 2020 2020 2020 2020 2222  bers..        ""
+0000ea70: 220a 2020 2020 2020 2020 2320 436f 6e76  ".        # Conv
+0000ea80: 6572 7420 7468 6520 696e 7075 7420 6974  ert the input it
+0000ea90: 6572 6162 6c65 2074 6f20 6120 6c69 7374  erable to a list
+0000eaa0: 2074 6f20 7375 7070 6f72 7420 696e 6465   to support inde
+0000eab0: 7869 6e67 0a20 2020 2020 2020 206e 756d  xing.        num
+0000eac0: 6265 725f 636f 6d62 696e 6174 696f 6e5f  ber_combination_
+0000ead0: 6c69 7374 203d 206c 6973 7428 6e75 6d62  list = list(numb
+0000eae0: 6572 5f63 6f6d 6269 6e61 7469 6f6e 290a  er_combination).
+0000eaf0: 2020 2020 2020 2020 7365 7175 656e 6365          sequence
+0000eb00: 7320 3d20 5b5d 0a20 2020 2020 2020 2063  s = [].        c
+0000eb10: 7572 7265 6e74 5f73 6571 7565 6e63 6520  urrent_sequence 
+0000eb20: 3d20 5b6e 756d 6265 725f 636f 6d62 696e  = [number_combin
+0000eb30: 6174 696f 6e5f 6c69 7374 5b30 5d5d 2020  ation_list[0]]  
+0000eb40: 2320 496e 6974 6961 6c69 7a65 2077 6974  # Initialize wit
+0000eb50: 6820 7468 6520 6669 7273 7420 6e75 6d62  h the first numb
+0000eb60: 6572 0a0a 2020 2020 2020 2020 666f 7220  er..        for 
+0000eb70: 6920 696e 2072 616e 6765 2831 2c20 6c65  i in range(1, le
+0000eb80: 6e28 6e75 6d62 6572 5f63 6f6d 6269 6e61  n(number_combina
+0000eb90: 7469 6f6e 5f6c 6973 7429 293a 0a20 2020  tion_list)):.   
+0000eba0: 2020 2020 2020 2020 2069 6620 6e75 6d62           if numb
+0000ebb0: 6572 5f63 6f6d 6269 6e61 7469 6f6e 5f6c  er_combination_l
+0000ebc0: 6973 745b 695d 203d 3d20 6375 7272 656e  ist[i] == curren
+0000ebd0: 745f 7365 7175 656e 6365 5b2d 315d 202b  t_sequence[-1] +
+0000ebe0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000ebf0: 2020 2020 6375 7272 656e 745f 7365 7175      current_sequ
+0000ec00: 656e 6365 2e61 7070 656e 6428 6e75 6d62  ence.append(numb
+0000ec10: 6572 5f63 6f6d 6269 6e61 7469 6f6e 5f6c  er_combination_l
+0000ec20: 6973 745b 695d 290a 2020 2020 2020 2020  ist[i]).        
+0000ec30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ec40: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0000ec50: 2863 7572 7265 6e74 5f73 6571 7565 6e63  (current_sequenc
+0000ec60: 6529 203e 2031 3a0a 2020 2020 2020 2020  e) > 1:.        
+0000ec70: 2020 2020 2020 2020 2020 2020 7365 7175              sequ
+0000ec80: 656e 6365 732e 6170 7065 6e64 2863 7572  ences.append(cur
+0000ec90: 7265 6e74 5f73 6571 7565 6e63 6529 0a20  rent_sequence). 
+0000eca0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000ecb0: 7572 7265 6e74 5f73 6571 7565 6e63 6520  urrent_sequence 
+0000ecc0: 3d20 5b6e 756d 6265 725f 636f 6d62 696e  = [number_combin
+0000ecd0: 6174 696f 6e5f 6c69 7374 5b69 5d5d 0a0a  ation_list[i]]..
+0000ece0: 2020 2020 2020 2020 6966 206c 656e 2863          if len(c
+0000ecf0: 7572 7265 6e74 5f73 6571 7565 6e63 6529  urrent_sequence)
+0000ed00: 203e 2031 3a0a 2020 2020 2020 2020 2020   > 1:.          
+0000ed10: 2020 7365 7175 656e 6365 732e 6170 7065    sequences.appe
+0000ed20: 6e64 2863 7572 7265 6e74 5f73 6571 7565  nd(current_seque
+0000ed30: 6e63 6529 0a0a 2020 2020 2020 2020 7265  nce)..        re
+0000ed40: 7475 726e 2073 6571 7565 6e63 6573 0a0a  turn sequences..
+0000ed50: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+0000ed60: 0a20 2020 2064 6566 2063 616c 6375 6c61  .    def calcula
+0000ed70: 7465 5f72 6570 6561 7465 645f 6e75 6d62  te_repeated_numb
+0000ed80: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
+0000ed90: 2063 6c73 2c0a 2020 2020 2020 2020 2020   cls,.          
+0000eda0: 2020 6e75 6d62 6572 5f63 6f6d 6269 6e61    number_combina
+0000edb0: 7469 6f6e 733a 2049 7465 7261 626c 655b  tions: Iterable[
+0000edc0: 4974 6572 6162 6c65 5b69 6e74 5d5d 2c0a  Iterable[int]],.
+0000edd0: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
+0000ede0: 6f77 3a20 696e 7420 3d20 322c 0a20 2020  ow: int = 2,.   
+0000edf0: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+0000ee00: 733a 2041 6e79 0a20 2020 2029 202d 3e20  s: Any.    ) -> 
+0000ee10: 4c69 7374 5b69 6e74 5d3a 0a20 2020 2020  List[int]:.     
+0000ee20: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+0000ee30: 616c 6375 6c61 7465 2074 6865 206e 756d  alculate the num
+0000ee40: 6265 7273 2074 6861 7420 6170 7065 6172  bers that appear
+0000ee50: 2069 6e20 616c 6c20 6769 7665 6e20 6974   in all given it
+0000ee60: 6572 6162 6c65 206f 6620 696e 7465 6765  erable of intege
+0000ee70: 7273 2028 696e 7465 7273 6563 7469 6f6e  rs (intersection
+0000ee80: 292e 0a0a 2020 2020 2020 2020 3a70 6172  )...        :par
+0000ee90: 616d 206e 756d 6265 725f 636f 6d62 696e  am number_combin
+0000eea0: 6174 696f 6e73 3a20 416e 2069 7465 7261  ations: An itera
+0000eeb0: 626c 6520 6f66 2069 6e74 6567 6572 7320  ble of integers 
+0000eec0: 746f 2066 696e 6420 636f 6d6d 6f6e 206e  to find common n
+0000eed0: 756d 6265 7273 2e0a 2020 2020 2020 2020  umbers..        
+0000eee0: 3a70 6172 616d 2077 696e 646f 773a 2054  :param window: T
+0000eef0: 6865 206e 756d 6265 7220 6f66 2072 6563  he number of rec
+0000ef00: 656e 7420 7065 7269 6f64 7320 746f 2070  ent periods to p
+0000ef10: 726f 6365 7373 2e0a 2020 2020 2020 2020  rocess..        
+0000ef20: 3a70 6172 616d 206b 7761 7267 733a 2041  :param kwargs: A
+0000ef30: 6464 6974 696f 6e61 6c20 6b65 7977 6f72  dditional keywor
+0000ef40: 6420 6172 6775 6d65 6e74 732e 0a20 2020  d arguments..   
+0000ef50: 2020 2020 203a 7265 7475 726e 3a20 4120       :return: A 
+0000ef60: 6c69 7374 2063 6f6e 7461 696e 696e 6720  list containing 
+0000ef70: 7468 6520 6e75 6d62 6572 7320 7468 6174  the numbers that
+0000ef80: 2061 7265 2063 6f6d 6d6f 6e20 696e 2061   are common in a
+0000ef90: 6c6c 2067 6976 656e 2069 7465 7261 626c  ll given iterabl
+0000efa0: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+0000efb0: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
+0000efc0: 6c69 7a65 2074 6865 2073 6574 2077 6974  lize the set wit
+0000efd0: 6820 7468 6520 6669 7273 7420 6974 6572  h the first iter
+0000efe0: 6162 6c65 2074 6f20 7374 6172 7420 7468  able to start th
+0000eff0: 6520 696e 7465 7273 6563 7469 6f6e 2070  e intersection p
+0000f000: 726f 6365 7373 0a20 2020 2020 2020 2072  rocess.        r
+0000f010: 6570 6561 7465 645f 6e75 6d62 6572 733a  epeated_numbers:
+0000f020: 2053 6574 5b69 6e74 5d20 3d20 7365 7428   Set[int] = set(
+0000f030: 6e65 7874 2869 7465 7228 6e75 6d62 6572  next(iter(number
+0000f040: 5f63 6f6d 6269 6e61 7469 6f6e 735b 2d77  _combinations[-w
+0000f050: 696e 646f 773a 5d29 2c20 5b5d 2929 0a0a  indow:]), []))..
+0000f060: 2020 2020 2020 2020 2320 5065 7266 6f72          # Perfor
+0000f070: 6d20 696e 7465 7273 6563 7469 6f6e 2077  m intersection w
+0000f080: 6974 6820 7468 6520 7375 6273 6571 7565  ith the subseque
+0000f090: 6e74 2069 7465 7261 626c 6573 0a20 2020  nt iterables.   
+0000f0a0: 2020 2020 2066 6f72 206e 756d 6265 725f       for number_
+0000f0b0: 636f 6d62 696e 6174 696f 6e20 696e 206e  combination in n
+0000f0c0: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
+0000f0d0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000f0e0: 7265 7065 6174 6564 5f6e 756d 6265 7273  repeated_numbers
+0000f0f0: 2e69 6e74 6572 7365 6374 696f 6e5f 7570  .intersection_up
+0000f100: 6461 7465 2873 6574 286e 756d 6265 725f  date(set(number_
+0000f110: 636f 6d62 696e 6174 696f 6e29 290a 0a20  combination)).. 
+0000f120: 2020 2020 2020 2023 2052 6574 7572 6e20         # Return 
+0000f130: 7468 6520 7265 7375 6c74 2061 7320 6120  the result as a 
+0000f140: 6c69 7374 0a20 2020 2020 2020 2072 6574  list.        ret
+0000f150: 7572 6e20 6c69 7374 2872 6570 6561 7465  urn list(repeate
+0000f160: 645f 6e75 6d62 6572 7329 0a0a 2020 2020  d_numbers)..    
+0000f170: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+0000f180: 2064 6566 2063 616c 6375 6c61 7465 5f65   def calculate_e
+0000f190: 6467 655f 6e75 6d62 6572 7328 0a20 2020  dge_numbers(.   
+0000f1a0: 2020 2020 2020 2020 2063 6c73 2c0a 2020           cls,.  
+0000f1b0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+0000f1c0: 5f63 6f6d 6269 6e61 7469 6f6e 733a 2049  _combinations: I
+0000f1d0: 7465 7261 626c 655b 4974 6572 6162 6c65  terable[Iterable
+0000f1e0: 5b69 6e74 5d5d 2c0a 2020 2020 2020 2020  [int]],.        
+0000f1f0: 2020 2020 7769 6e64 6f77 3a20 696e 7420      window: int 
+0000f200: 3d20 322c 0a20 2020 2020 2020 2020 2020  = 2,.           
+0000f210: 202a 2a6b 7761 7267 733a 2041 6e79 0a20   **kwargs: Any. 
+0000f220: 2020 2029 202d 3e20 4c69 7374 5b69 6e74     ) -> List[int
+0000f230: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+0000f240: 2020 2020 2020 2043 616c 6375 6c61 7465         Calculate
+0000f250: 2027 6564 6765 206e 756d 6265 7273 2720   'edge numbers' 
+0000f260: 7768 6963 6820 6172 6520 7072 6573 656e  which are presen
+0000f270: 7420 696e 2063 6f6e 7365 6375 7469 7665  t in consecutive
+0000f280: 2069 7465 7261 626c 6573 2077 6865 7265   iterables where
+0000f290: 2065 6163 6820 6e75 6d62 6572 2066 726f   each number fro
+0000f2a0: 6d20 7468 6520 6669 7273 7420 6974 6572  m the first iter
+0000f2b0: 6162 6c65 0a20 2020 2020 2020 2069 7320  able.        is 
+0000f2c0: 6569 7468 6572 206f 6e65 206c 6573 7320  either one less 
+0000f2d0: 6f72 206f 6e65 206d 6f72 6520 7468 616e  or one more than
+0000f2e0: 2074 6865 206e 756d 6265 7273 2069 6e20   the numbers in 
+0000f2f0: 7468 6520 666f 6c6c 6f77 696e 6720 6974  the following it
+0000f300: 6572 6162 6c65 2e0a 0a20 2020 2020 2020  erable...       
+0000f310: 203a 7061 7261 6d20 6e75 6d62 6572 5f63   :param number_c
+0000f320: 6f6d 6269 6e61 7469 6f6e 733a 2041 6e20  ombinations: An 
+0000f330: 6974 6572 6162 6c65 206f 6620 6974 6572  iterable of iter
+0000f340: 6162 6c65 7320 6f66 2069 6e74 6567 6572  ables of integer
+0000f350: 7320 746f 2066 696e 6420 2765 6467 6520  s to find 'edge 
+0000f360: 6e75 6d62 6572 7327 2e0a 2020 2020 2020  numbers'..      
+0000f370: 2020 3a70 6172 616d 2077 696e 646f 773a    :param window:
+0000f380: 2054 6865 206e 756d 6265 7220 6f66 2072   The number of r
+0000f390: 6563 656e 7420 7065 7269 6f64 7320 746f  ecent periods to
+0000f3a0: 2070 726f 6365 7373 2e0a 2020 2020 2020   process..      
+0000f3b0: 2020 3a70 6172 616d 206b 7761 7267 733a    :param kwargs:
+0000f3c0: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
+0000f3d0: 6f72 6420 6172 6775 6d65 6e74 732e 0a20  ord arguments.. 
+0000f3e0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+0000f3f0: 4120 6c69 7374 2063 6f6e 7461 696e 696e  A list containin
+0000f400: 6720 7468 6520 2765 6467 6520 6e75 6d62  g the 'edge numb
+0000f410: 6572 7327 2e0a 2020 2020 2020 2020 2222  ers'..        ""
+0000f420: 220a 2020 2020 2020 2020 2320 436f 6e76  ".        # Conv
+0000f430: 6572 7420 7468 6520 696e 7075 7420 746f  ert the input to
+0000f440: 2061 206c 6973 7420 666f 7220 696e 6465   a list for inde
+0000f450: 7865 6420 6163 6365 7373 0a20 2020 2020  xed access.     
+0000f460: 2020 206e 756d 6265 725f 636f 6d62 696e     number_combin
+0000f470: 6174 696f 6e73 5f6c 6973 7420 3d20 6c69  ations_list = li
+0000f480: 7374 286e 756d 6265 725f 636f 6d62 696e  st(number_combin
+0000f490: 6174 696f 6e73 5b2d 7769 6e64 6f77 3a5d  ations[-window:]
+0000f4a0: 290a 0a20 2020 2020 2020 2023 2049 6e69  )..        # Ini
+0000f4b0: 7469 616c 697a 6520 616e 2065 6d70 7479  tialize an empty
+0000f4c0: 2073 6574 2066 6f72 2074 6865 2065 6467   set for the edg
+0000f4d0: 6520 6e75 6d62 6572 730a 2020 2020 2020  e numbers.      
+0000f4e0: 2020 6564 6765 5f6e 756d 6265 7273 3a20    edge_numbers: 
+0000f4f0: 5365 745b 696e 745d 203d 2073 6574 2829  Set[int] = set()
+0000f500: 0a0a 2020 2020 2020 2020 2320 4974 6572  ..        # Iter
+0000f510: 6174 6520 6f76 6572 2065 6163 6820 6e75  ate over each nu
+0000f520: 6d62 6572 2063 6f6d 6269 6e61 7469 6f6e  mber combination
+0000f530: 2c20 7374 6172 7469 6e67 2066 726f 6d20  , starting from 
+0000f540: 7468 6520 7365 636f 6e64 206f 6e65 0a20  the second one. 
+0000f550: 2020 2020 2020 2066 6f72 2069 6e64 6578         for index
+0000f560: 2069 6e20 7261 6e67 6528 312c 206c 656e   in range(1, len
+0000f570: 286e 756d 6265 725f 636f 6d62 696e 6174  (number_combinat
+0000f580: 696f 6e73 5f6c 6973 7429 293a 0a20 2020  ions_list)):.   
+0000f590: 2020 2020 2020 2020 2023 2043 7265 6174           # Creat
+0000f5a0: 6520 6120 7365 7420 6f66 2070 6f74 656e  e a set of poten
+0000f5b0: 7469 616c 2065 6467 6520 6e75 6d62 6572  tial edge number
+0000f5c0: 7320 6672 6f6d 2074 6865 2070 7265 7669  s from the previ
+0000f5d0: 6f75 7320 636f 6d62 696e 6174 696f 6e0a  ous combination.
+0000f5e0: 2020 2020 2020 2020 2020 2020 6c61 7374              last
+0000f5f0: 5f6e 756d 6265 725f 7365 7420 3d20 7365  _number_set = se
+0000f600: 7428 6e75 6d20 2b20 6920 666f 7220 6920  t(num + i for i 
+0000f610: 696e 205b 2d31 2c20 302c 2031 5d0a 2020  in [-1, 0, 1].  
+0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 666f 7220 6e75 6d20 696e 206e 756d 6265  for num in numbe
+0000f650: 725f 636f 6d62 696e 6174 696f 6e73 5f6c  r_combinations_l
+0000f660: 6973 745b 696e 6465 7820 2d20 315d 0a20  ist[index - 1]. 
+0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f690: 2069 6620 286e 756d 202b 2069 2920 3e20   if (num + i) > 
+0000f6a0: 3029 0a20 2020 2020 2020 2020 2020 2023  0).            #
+0000f6b0: 2043 7265 6174 6520 6120 7365 7420 6672   Create a set fr
+0000f6c0: 6f6d 2074 6865 2063 7572 7265 6e74 2063  om the current c
+0000f6d0: 6f6d 6269 6e61 7469 6f6e 0a20 2020 2020  ombination.     
+0000f6e0: 2020 2020 2020 2063 7572 7265 6e74 5f6e         current_n
+0000f6f0: 756d 6265 725f 7365 7420 3d20 7365 7428  umber_set = set(
+0000f700: 6e75 6d62 6572 5f63 6f6d 6269 6e61 7469  number_combinati
+0000f710: 6f6e 735f 6c69 7374 5b69 6e64 6578 5d29  ons_list[index])
+0000f720: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0000f730: 696e 6420 7468 6520 696e 7465 7273 6563  ind the intersec
+0000f740: 7469 6f6e 206f 6620 7468 6520 7477 6f20  tion of the two 
+0000f750: 7365 7473 0a20 2020 2020 2020 2020 2020  sets.           
+0000f760: 2069 6e74 6572 7365 6374 696f 6e20 3d20   intersection = 
+0000f770: 6375 7272 656e 745f 6e75 6d62 6572 5f73  current_number_s
+0000f780: 6574 2e69 6e74 6572 7365 6374 696f 6e28  et.intersection(
+0000f790: 6c61 7374 5f6e 756d 6265 725f 7365 7429  last_number_set)
+0000f7a0: 0a20 2020 2020 2020 2020 2020 2023 2055  .            # U
+0000f7b0: 7064 6174 6520 7468 6520 6564 6765 206e  pdate the edge n
+0000f7c0: 756d 6265 7273 2073 6574 2077 6974 6820  umbers set with 
+0000f7d0: 7468 6520 696e 7465 7273 6563 7469 6f6e  the intersection
+0000f7e0: 0a20 2020 2020 2020 2020 2020 2065 6467  .            edg
+0000f7f0: 655f 6e75 6d62 6572 732e 7570 6461 7465  e_numbers.update
+0000f800: 2869 6e74 6572 7365 6374 696f 6e29 0a0a  (intersection)..
+0000f810: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+0000f820: 2074 6865 2072 6573 756c 7420 6173 2061   the result as a
+0000f830: 2073 6f72 7465 6420 6c69 7374 2074 6f20   sorted list to 
+0000f840: 6d61 696e 7461 696e 2061 2063 6f6e 7369  maintain a consi
+0000f850: 7374 656e 7420 6f72 6465 720a 2020 2020  stent order.    
+0000f860: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
+0000f870: 6428 6564 6765 5f6e 756d 6265 7273 290a  d(edge_numbers).
+0000f880: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+0000f890: 640a 2020 2020 6465 6620 6361 6c63 756c  d.    def calcul
+0000f8a0: 6174 655f 636f 6c64 5f68 6f74 5f6e 756d  ate_cold_hot_num
+0000f8b0: 6265 7273 280a 2020 2020 2020 2020 2020  bers(.          
+0000f8c0: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
+0000f8d0: 2020 206e 756d 6265 725f 636f 6d62 696e     number_combin
+0000f8e0: 6174 696f 6e73 3a20 4974 6572 6162 6c65  ations: Iterable
+0000f8f0: 5b49 7465 7261 626c 655b 696e 745d 5d2c  [Iterable[int]],
+0000f900: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+0000f910: 5f6e 756d 6265 7273 3a20 4974 6572 6162  _numbers: Iterab
+0000f920: 6c65 5b69 6e74 5d2c 0a20 2020 2020 2020  le[int],.       
+0000f930: 2020 2020 2077 696e 646f 773a 2069 6e74       window: int
+0000f940: 203d 2035 2c0a 2020 2020 2020 2020 2020   = 5,.          
+0000f950: 2020 2a2a 6b77 6172 6773 3a20 416e 790a    **kwargs: Any.
+0000f960: 2020 2020 2920 2d3e 2054 7570 6c65 5b4c      ) -> Tuple[L
+0000f970: 6973 745b 696e 745d 2c20 4c69 7374 5b69  ist[int], List[i
+0000f980: 6e74 5d5d 3a0a 2020 2020 2020 2020 2222  nt]]:.        ""
+0000f990: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
+0000f9a0: 6174 6520 616e 6420 7265 7475 726e 2027  ate and return '
+0000f9b0: 636f 6c64 206e 756d 6265 7273 2720 616e  cold numbers' an
+0000f9c0: 6420 2768 6f74 206e 756d 6265 7273 2720  d 'hot numbers' 
+0000f9d0: 6672 6f6d 2061 2073 6572 6965 7320 6f66  from a series of
+0000f9e0: 206e 756d 6265 7220 636f 6d62 696e 6174   number combinat
+0000f9f0: 696f 6e73 2e0a 2020 2020 2020 2020 2743  ions..        'C
+0000fa00: 6f6c 6420 6e75 6d62 6572 7327 2061 7265  old numbers' are
+0000fa10: 2074 686f 7365 2074 6861 7420 6469 6420   those that did 
+0000fa20: 6e6f 7420 6170 7065 6172 2069 6e20 7468  not appear in th
+0000fa30: 6520 6c61 7374 2035 2069 7465 7261 7469  e last 5 iterati
+0000fa40: 6f6e 732c 0a20 2020 2020 2020 2061 6e64  ons,.        and
+0000fa50: 2027 686f 7420 6e75 6d62 6572 7327 2061   'hot numbers' a
+0000fa60: 7265 2074 686f 7365 2074 6861 7420 6170  re those that ap
+0000fa70: 7065 6172 6564 2061 7420 6c65 6173 7420  peared at least 
+0000fa80: 6f6e 6365 2069 6e20 7468 6520 6c61 7374  once in the last
+0000fa90: 2035 2069 7465 7261 7469 6f6e 732e 0a0a   5 iterations...
+0000faa0: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
+0000fab0: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
+0000fac0: 6e73 3a20 416e 2069 7465 7261 626c 6520  ns: An iterable 
+0000fad0: 6f66 2069 7465 7261 626c 6573 206f 6620  of iterables of 
+0000fae0: 696e 7465 6765 7273 2074 6f20 616e 616c  integers to anal
+0000faf0: 797a 6520 6e75 6d62 6572 732e 0a20 2020  yze numbers..   
+0000fb00: 2020 2020 203a 7061 7261 6d20 616c 6c5f       :param all_
+0000fb10: 6e75 6d62 6572 733a 2041 6e20 6974 6572  numbers: An iter
+0000fb20: 6162 6c65 206f 6620 616c 6c20 706f 7373  able of all poss
+0000fb30: 6962 6c65 206e 756d 6265 7273 2074 6861  ible numbers tha
+0000fb40: 7420 636f 756c 6420 6170 7065 6172 2e0a  t could appear..
+0000fb50: 2020 2020 2020 2020 3a70 6172 616d 2077          :param w
+0000fb60: 696e 646f 773a 2064 6566 6175 6c74 2035  indow: default 5
+0000fb70: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000fb80: 6b77 6172 6773 3a20 4164 6469 7469 6f6e  kwargs: Addition
+0000fb90: 616c 206b 6579 776f 7264 2061 7267 756d  al keyword argum
+0000fba0: 656e 7473 2e0a 2020 2020 2020 2020 3a72  ents..        :r
+0000fbb0: 6574 7572 6e3a 2041 2074 7570 6c65 2063  eturn: A tuple c
+0000fbc0: 6f6e 7461 696e 696e 6720 7477 6f20 6c69  ontaining two li
+0000fbd0: 7374 7320 2d20 7468 6520 6669 7273 7420  sts - the first 
+0000fbe0: 7769 7468 2027 636f 6c64 206e 756d 6265  with 'cold numbe
+0000fbf0: 7273 2720 616e 6420 7468 6520 7365 636f  rs' and the seco
+0000fc00: 6e64 2077 6974 6820 2768 6f74 206e 756d  nd with 'hot num
+0000fc10: 6265 7273 272e 0a20 2020 2020 2020 2022  bers'..        "
+0000fc20: 2222 0a20 2020 2020 2020 2023 2043 6f6e  "".        # Con
+0000fc30: 7665 7274 2074 6865 2069 6e70 7574 2074  vert the input t
+0000fc40: 6f20 6120 6c69 7374 2066 6f72 2069 6e64  o a list for ind
+0000fc50: 6578 6564 2061 6363 6573 730a 2020 2020  exed access.    
+0000fc60: 2020 2020 6e75 6d62 6572 5f63 6f6d 6269      number_combi
+0000fc70: 6e61 7469 6f6e 735f 6c69 7374 203d 206c  nations_list = l
+0000fc80: 6973 7428 6e75 6d62 6572 5f63 6f6d 6269  ist(number_combi
+0000fc90: 6e61 7469 6f6e 735b 2d77 696e 646f 773a  nations[-window:
+0000fca0: 5d29 0a0a 2020 2020 2020 2020 2320 4465  ])..        # De
+0000fcb0: 7465 726d 696e 6520 7468 6520 7261 6e67  termine the rang
+0000fcc0: 6520 666f 7220 7468 6520 6c61 7374 2035  e for the last 5
+0000fcd0: 2070 6572 696f 6473 0a20 2020 2020 2020   periods.       
+0000fce0: 206c 6173 745f 6669 7665 5f70 6572 696f   last_five_perio
+0000fcf0: 6473 203d 206e 756d 6265 725f 636f 6d62  ds = number_comb
+0000fd00: 696e 6174 696f 6e73 5f6c 6973 7420 6966  inations_list if
+0000fd10: 206c 656e 280a 2020 2020 2020 2020 2020   len(.          
+0000fd20: 2020 6e75 6d62 6572 5f63 6f6d 6269 6e61    number_combina
+0000fd30: 7469 6f6e 735f 6c69 7374 2920 3e3d 2077  tions_list) >= w
+0000fd40: 696e 646f 7720 656c 7365 206e 756d 6265  indow else numbe
+0000fd50: 725f 636f 6d62 696e 6174 696f 6e73 5f6c  r_combinations_l
+0000fd60: 6973 740a 0a20 2020 2020 2020 2023 2046  ist..        # F
+0000fd70: 6c61 7474 656e 2074 6865 206c 6973 7420  latten the list 
+0000fd80: 6f66 206c 6173 7420 6669 7665 2070 6572  of last five per
+0000fd90: 696f 6473 2061 6e64 2063 6f6e 7665 7274  iods and convert
+0000fda0: 2074 6f20 6120 7365 7420 746f 2072 656d   to a set to rem
+0000fdb0: 6f76 6520 6475 706c 6963 6174 6573 0a20  ove duplicates. 
+0000fdc0: 2020 2020 2020 206e 756d 6265 7273 5f69         numbers_i
+0000fdd0: 6e5f 6c61 7374 5f66 6976 655f 7065 7269  n_last_five_peri
+0000fde0: 6f64 733a 2053 6574 5b69 6e74 5d20 3d20  ods: Set[int] = 
+0000fdf0: 7365 7428 6e75 6d20 666f 7220 7065 7269  set(num for peri
+0000fe00: 6f64 2069 6e20 6c61 7374 5f66 6976 655f  od in last_five_
+0000fe10: 7065 7269 6f64 7320 666f 7220 6e75 6d20  periods for num 
+0000fe20: 696e 2070 6572 696f 6429 0a0a 2020 2020  in period)..    
+0000fe30: 2020 2020 2320 436f 6e76 6572 7420 616c      # Convert al
+0000fe40: 6c5f 6e75 6d62 6572 7320 746f 2061 2073  l_numbers to a s
+0000fe50: 6574 2066 6f72 2065 6666 6963 6965 6e74  et for efficient
+0000fe60: 206c 6f6f 6b75 700a 2020 2020 2020 2020   lookup.        
+0000fe70: 616c 6c5f 6e75 6d62 6572 735f 7365 743a  all_numbers_set:
+0000fe80: 2053 6574 5b69 6e74 5d20 3d20 7365 7428   Set[int] = set(
+0000fe90: 616c 6c5f 6e75 6d62 6572 7329 0a0a 2020  all_numbers)..  
+0000fea0: 2020 2020 2020 2320 2743 6f6c 6420 6e75        # 'Cold nu
+0000feb0: 6d62 6572 7327 2061 7265 2074 686f 7365  mbers' are those
+0000fec0: 2074 6861 7420 6172 6520 6e6f 7420 696e   that are not in
+0000fed0: 2074 6865 206c 6173 7420 6669 7665 2070   the last five p
+0000fee0: 6572 696f 6473 0a20 2020 2020 2020 2063  eriods.        c
+0000fef0: 6f6c 645f 6e75 6d62 6572 733a 204c 6973  old_numbers: Lis
+0000ff00: 745b 696e 745d 203d 2073 6f72 7465 6428  t[int] = sorted(
+0000ff10: 6c69 7374 2861 6c6c 5f6e 756d 6265 7273  list(all_numbers
+0000ff20: 5f73 6574 202d 206e 756d 6265 7273 5f69  _set - numbers_i
+0000ff30: 6e5f 6c61 7374 5f66 6976 655f 7065 7269  n_last_five_peri
+0000ff40: 6f64 7329 290a 0a20 2020 2020 2020 2023  ods))..        #
+0000ff50: 2027 486f 7420 6e75 6d62 6572 7327 2061   'Hot numbers' a
+0000ff60: 7265 2074 686f 7365 2074 6861 7420 6172  re those that ar
+0000ff70: 6520 696e 2074 6865 206c 6173 7420 6669  e in the last fi
+0000ff80: 7665 2070 6572 696f 6473 0a20 2020 2020  ve periods.     
+0000ff90: 2020 2068 6f74 5f6e 756d 6265 7273 3a20     hot_numbers: 
+0000ffa0: 4c69 7374 5b69 6e74 5d20 3d20 736f 7274  List[int] = sort
+0000ffb0: 6564 286c 6973 7428 6e75 6d62 6572 735f  ed(list(numbers_
+0000ffc0: 696e 5f6c 6173 745f 6669 7665 5f70 6572  in_last_five_per
+0000ffd0: 696f 6473 2929 0a0a 2020 2020 2020 2020  iods))..        
+0000ffe0: 2320 5265 7475 726e 2074 6865 2063 6f6c  # Return the col
+0000fff0: 6420 6e75 6d62 6572 7320 616e 6420 686f  d numbers and ho
+00010000: 7420 6e75 6d62 6572 730a 2020 2020 2020  t numbers.      
+00010010: 2020 7265 7475 726e 2063 6f6c 645f 6e75    return cold_nu
+00010020: 6d62 6572 732c 2068 6f74 5f6e 756d 6265  mbers, hot_numbe
+00010030: 7273 0a0a 2020 2020 4063 6c61 7373 6d65  rs..    @classme
+00010040: 7468 6f64 0a20 2020 2064 6566 2063 616c  thod.    def cal
+00010050: 6375 6c61 7465 5f6f 6d69 7474 6564 5f6e  culate_omitted_n
+00010060: 756d 6265 7273 280a 2020 2020 2020 2020  umbers(.        
+00010070: 2020 2020 636c 732c 0a20 2020 2020 2020      cls,.       
+00010080: 2020 2020 206e 756d 6265 725f 636f 6d62       number_comb
+00010090: 696e 6174 696f 6e73 3a20 4974 6572 6162  inations: Iterab
+000100a0: 6c65 5b49 7465 7261 626c 655b 696e 745d  le[Iterable[int]
+000100b0: 5d2c 0a20 2020 2020 2020 2020 2020 2061  ],.            a
+000100c0: 6c6c 5f6e 756d 6265 7273 3a20 4974 6572  ll_numbers: Iter
+000100d0: 6162 6c65 5b69 6e74 5d2c 0a20 2020 2020  able[int],.     
+000100e0: 2020 2020 2020 2077 696e 646f 773a 2069         window: i
+000100f0: 6e74 203d 2031 302c 0a20 2020 2020 2020  nt = 10,.       
+00010100: 2020 2020 202a 2a6b 7761 7267 733a 2041       **kwargs: A
+00010110: 6e79 0a20 2020 2029 202d 3e20 4469 6374  ny.    ) -> Dict
+00010120: 5b69 6e74 2c20 696e 745d 3a0a 2020 2020  [int, int]:.    
+00010130: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010140: 5570 6461 7465 2061 6e64 2072 6574 7572  Update and retur
+00010150: 6e20 7468 6520 6f6d 6973 7369 6f6e 2076  n the omission v
+00010160: 616c 7565 7320 666f 7220 6561 6368 206e  alues for each n
+00010170: 756d 6265 7220 696e 2061 6c6c 5f6e 756d  umber in all_num
+00010180: 6265 7273 2e0a 0a20 2020 2020 2020 203a  bers...        :
+00010190: 7061 7261 6d20 6e75 6d62 6572 5f63 6f6d  param number_com
+000101a0: 6269 6e61 7469 6f6e 733a 2041 206c 6973  binations: A lis
+000101b0: 7420 6f66 206c 6973 7473 206f 6620 696e  t of lists of in
+000101c0: 7465 6765 7273 2072 6570 7265 7365 6e74  tegers represent
+000101d0: 696e 6720 7061 7374 206e 756d 6265 7220  ing past number 
+000101e0: 6472 6177 732e 0a20 2020 2020 2020 203a  draws..        :
+000101f0: 7061 7261 6d20 616c 6c5f 6e75 6d62 6572  param all_number
+00010200: 733a 2041 206c 6973 7420 6f66 2061 6c6c  s: A list of all
+00010210: 2070 6f73 7369 626c 6520 6e75 6d62 6572   possible number
+00010220: 7320 7468 6174 2063 6f75 6c64 2061 7070  s that could app
+00010230: 6561 722e 0a20 2020 2020 2020 203a 7061  ear..        :pa
+00010240: 7261 6d20 7769 6e64 6f77 3a20 6465 6661  ram window: defa
+00010250: 756c 7420 3130 0a20 2020 2020 2020 203a  ult 10.        :
+00010260: 7265 7475 726e 3a20 4120 6469 6374 696f  return: A dictio
+00010270: 6e61 7279 2077 6974 6820 6e75 6d62 6572  nary with number
+00010280: 7320 6173 206b 6579 7320 616e 6420 7468  s as keys and th
+00010290: 6569 7220 6f6d 6973 7369 6f6e 2076 616c  eir omission val
+000102a0: 7565 7320 6173 2076 616c 7565 732e 0a20  ues as values.. 
+000102b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000102c0: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
+000102d0: 7468 6520 6f6d 6973 7369 6f6e 2076 616c  the omission val
+000102e0: 7565 7320 666f 7220 6561 6368 206e 756d  ues for each num
+000102f0: 6265 7220 746f 2030 0a20 2020 2020 2020  ber to 0.       
+00010300: 206f 6d69 7373 696f 6e5f 7661 6c75 6573   omission_values
+00010310: 3a20 4469 6374 5b69 6e74 2c20 696e 745d  : Dict[int, int]
+00010320: 203d 207b 6e75 6d62 6572 3a20 2d31 2066   = {number: -1 f
+00010330: 6f72 206e 756d 6265 7220 696e 2061 6c6c  or number in all
+00010340: 5f6e 756d 6265 7273 7d0a 0a20 2020 2020  _numbers}..     
+00010350: 2020 2023 2043 6f6e 7665 7274 2074 6865     # Convert the
+00010360: 2069 6e70 7574 2074 6f20 6120 6c69 7374   input to a list
+00010370: 2066 6f72 2069 6e64 6578 6564 2061 6363   for indexed acc
+00010380: 6573 730a 2020 2020 2020 2020 6e75 6d62  ess.        numb
+00010390: 6572 5f63 6f6d 6269 6e61 7469 6f6e 735f  er_combinations_
+000103a0: 6c69 7374 203d 206c 6973 7428 6e75 6d62  list = list(numb
+000103b0: 6572 5f63 6f6d 6269 6e61 7469 6f6e 735b  er_combinations[
+000103c0: 2d77 696e 646f 773a 5d29 0a0a 2020 2020  -window:])..    
+000103d0: 2020 2020 2320 4465 7465 726d 696e 6520      # Determine 
+000103e0: 7468 6520 7261 6e67 6520 666f 7220 7468  the range for th
+000103f0: 6520 6c61 7374 2035 2070 6572 696f 6473  e last 5 periods
+00010400: 0a20 2020 2020 2020 206c 6173 745f 7465  .        last_te
+00010410: 6e5f 7065 7269 6f64 7320 3d20 6e75 6d62  n_periods = numb
+00010420: 6572 5f63 6f6d 6269 6e61 7469 6f6e 735f  er_combinations_
+00010430: 6c69 7374 2069 6620 6c65 6e28 0a20 2020  list if len(.   
+00010440: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+00010450: 636f 6d62 696e 6174 696f 6e73 5f6c 6973  combinations_lis
+00010460: 7429 203e 3d20 7769 6e64 6f77 2065 6c73  t) >= window els
+00010470: 6520 6e75 6d62 6572 5f63 6f6d 6269 6e61  e number_combina
+00010480: 7469 6f6e 735f 6c69 7374 0a0a 2020 2020  tions_list..    
+00010490: 2020 2020 2320 5468 6520 6e75 6d62 6572      # The number
+000104a0: 206f 6620 6472 6177 7320 7369 6e63 6520   of draws since 
+000104b0: 7468 6520 6c61 7374 2061 7070 6561 7261  the last appeara
+000104c0: 6e63 650a 2020 2020 2020 2020 6472 6177  nce.        draw
+000104d0: 735f 7369 6e63 655f 6c61 7374 5f61 7070  s_since_last_app
+000104e0: 6561 7261 6e63 6520 3d20 300a 0a20 2020  earance = 0..   
+000104f0: 2020 2020 2023 2049 7465 7261 7465 206f       # Iterate o
+00010500: 7665 7220 7468 6520 7061 7374 2064 7261  ver the past dra
+00010510: 7773 2069 6e20 7265 7665 7273 6520 6f72  ws in reverse or
+00010520: 6465 7220 286d 6f73 7420 7265 6365 6e74  der (most recent
+00010530: 2066 6972 7374 290a 2020 2020 2020 2020   first).        
+00010540: 666f 7220 6472 6177 2069 6e20 7265 7665  for draw in reve
+00010550: 7273 6564 286c 6173 745f 7465 6e5f 7065  rsed(last_ten_pe
+00010560: 7269 6f64 7329 3a0a 2020 2020 2020 2020  riods):.        
+00010570: 2020 2020 2320 4368 6563 6b20 6561 6368      # Check each
+00010580: 206e 756d 6265 7220 696e 2061 6c6c 5f6e   number in all_n
+00010590: 756d 6265 7273 0a20 2020 2020 2020 2020  umbers.         
+000105a0: 2020 2066 6f72 206e 756d 6265 7220 696e     for number in
+000105b0: 2061 6c6c 5f6e 756d 6265 7273 3a0a 2020   all_numbers:.  
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000105d0: 4966 2074 6865 206e 756d 6265 7220 6973  If the number is
+000105e0: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+000105f0: 6472 6177 2061 6e64 2069 7473 206f 6d69  draw and its omi
+00010600: 7373 696f 6e20 7661 6c75 6520 6973 202d  ssion value is -
+00010610: 3120 2868 6173 6e27 7420 6170 7065 6172  1 (hasn't appear
+00010620: 6564 2079 6574 290a 2020 2020 2020 2020  ed yet).        
+00010630: 2020 2020 2020 2020 6966 206e 756d 6265          if numbe
+00010640: 7220 696e 2064 7261 7720 616e 6420 6f6d  r in draw and om
+00010650: 6973 7369 6f6e 5f76 616c 7565 735b 6e75  ission_values[nu
+00010660: 6d62 6572 5d20 3d3d 202d 313a 0a20 2020  mber] == -1:.   
+00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010680: 2023 2053 6574 2074 6865 206f 6d69 7373   # Set the omiss
+00010690: 696f 6e20 7661 6c75 6520 746f 2074 6865  ion value to the
+000106a0: 206e 756d 6265 7220 6f66 2064 7261 7773   number of draws
+000106b0: 2073 696e 6365 2069 7420 6c61 7374 2061   since it last a
+000106c0: 7070 6561 7265 640a 2020 2020 2020 2020  ppeared.        
+000106d0: 2020 2020 2020 2020 2020 2020 6f6d 6973              omis
+000106e0: 7369 6f6e 5f76 616c 7565 735b 6e75 6d62  sion_values[numb
+000106f0: 6572 5d20 3d20 6472 6177 735f 7369 6e63  er] = draws_sinc
+00010700: 655f 6c61 7374 5f61 7070 6561 7261 6e63  e_last_appearanc
+00010710: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
+00010720: 496e 6372 656d 656e 7420 7468 6520 636f  Increment the co
+00010730: 756e 7420 6f66 2064 7261 7773 2073 696e  unt of draws sin
+00010740: 6365 2074 6865 206c 6173 7420 6170 7065  ce the last appe
+00010750: 6172 616e 6365 0a20 2020 2020 2020 2020  arance.         
+00010760: 2020 2064 7261 7773 5f73 696e 6365 5f6c     draws_since_l
+00010770: 6173 745f 6170 7065 6172 616e 6365 202b  ast_appearance +
+00010780: 3d20 310a 0a20 2020 2020 2020 2023 2046  = 1..        # F
+00010790: 6f72 2061 6e79 206e 756d 6265 7220 7468  or any number th
+000107a0: 6174 2068 6173 6e27 7420 6170 7065 6172  at hasn't appear
+000107b0: 6564 2079 6574 2c20 7365 7420 6974 7320  ed yet, set its 
+000107c0: 6f6d 6973 7369 6f6e 2076 616c 7565 2074  omission value t
+000107d0: 6f20 7468 6520 746f 7461 6c20 6e75 6d62  o the total numb
+000107e0: 6572 206f 6620 6472 6177 730a 2020 2020  er of draws.    
+000107f0: 2020 2020 666f 7220 6e75 6d62 6572 2069      for number i
+00010800: 6e20 616c 6c5f 6e75 6d62 6572 733a 0a20  n all_numbers:. 
+00010810: 2020 2020 2020 2020 2020 2069 6620 6f6d             if om
+00010820: 6973 7369 6f6e 5f76 616c 7565 735b 6e75  ission_values[nu
+00010830: 6d62 6572 5d20 3d3d 202d 313a 0a20 2020  mber] == -1:.   
+00010840: 2020 2020 2020 2020 2020 2020 206f 6d69               omi
+00010850: 7373 696f 6e5f 7661 6c75 6573 5b6e 756d  ssion_values[num
+00010860: 6265 725d 203d 2064 7261 7773 5f73 696e  ber] = draws_sin
+00010870: 6365 5f6c 6173 745f 6170 7065 6172 616e  ce_last_appearan
+00010880: 6365 0a0a 2020 2020 2020 2020 7265 7475  ce..        retu
+00010890: 726e 206f 6d69 7373 696f 6e5f 7661 6c75  rn omission_valu
+000108a0: 6573 0a0a 2020 2020 4073 7461 7469 636d  es..    @staticm
+000108b0: 6574 686f 640a 2020 2020 6465 6620 6361  ethod.    def ca
+000108c0: 6c63 756c 6174 655f 7374 616e 6461 7264  lculate_standard
+000108d0: 5f64 6576 6961 7469 6f6e 5f77 656c 666f  _deviation_welfo
+000108e0: 7264 286e 756d 6572 6963 5f73 6571 7565  rd(numeric_seque
+000108f0: 6e63 653a 204c 6973 745b 556e 696f 6e5b  nce: List[Union[
+00010900: 696e 742c 2066 6c6f 6174 5d5d 2c0a 2020  int, float]],.  
+00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 2020 2020 2020 2020 2064 6563 6179             decay
+00010940: 5f66 6163 746f 723a 2055 6e69 6f6e 5b69  _factor: Union[i
+00010950: 6e74 2c20 666c 6f61 745d 203d 2030 2e39  nt, float] = 0.9
+00010960: 3529 202d 3e20 556e 696f 6e5b 696e 742c  5) -> Union[int,
+00010970: 2066 6c6f 6174 5d3a 0a20 2020 2020 2020   float]:.       
+00010980: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+00010990: 6375 6c61 7465 7320 7468 6520 7374 616e  culates the stan
+000109a0: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
+000109b0: 6620 6120 6e75 6d65 7269 6320 7365 7175  f a numeric sequ
+000109c0: 656e 6365 2075 7369 6e67 2057 656c 666f  ence using Welfo
+000109d0: 7264 2773 206d 6574 686f 642e 0a0a 2020  rd's method...  
+000109e0: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
+000109f0: 6420 6973 2061 6e20 6f6e 6c69 6e65 2061  d is an online a
+00010a00: 6c67 6f72 6974 686d 2064 6573 6967 6e65  lgorithm designe
+00010a10: 6420 746f 2063 6f6d 7075 7465 2074 6865  d to compute the
+00010a20: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+00010a30: 696f 6e20 6f66 2061 2073 6571 7565 6e63  ion of a sequenc
+00010a40: 6520 6f66 206e 756d 6265 7273 0a20 2020  e of numbers.   
+00010a50: 2020 2020 2069 7465 7261 7469 7665 6c79       iteratively
+00010a60: 2c20 7768 6963 6820 6361 6e20 6265 2075  , which can be u
+00010a70: 7365 6675 6c20 666f 7220 6c61 7267 6520  seful for large 
+00010a80: 6461 7461 7365 7473 2077 6865 7265 2061  datasets where a
+00010a90: 6c6c 2064 6174 6120 6361 6e6e 6f74 2062  ll data cannot b
+00010aa0: 6520 6c6f 6164 6564 2069 6e74 6f20 6d65  e loaded into me
+00010ab0: 6d6f 7279 2061 7420 6f6e 6365 2e0a 0a20  mory at once... 
+00010ac0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00010ad0: 2020 2020 2020 2020 206e 756d 6572 6963           numeric
+00010ae0: 5f73 6571 7565 6e63 6520 284c 6973 745b  _sequence (List[
+00010af0: 556e 696f 6e5b 696e 742c 2066 6c6f 6174  Union[int, float
+00010b00: 5d5d 293a 2054 6865 2073 6571 7565 6e63  ]]): The sequenc
+00010b10: 6520 6f66 206e 756d 6265 7273 2028 696e  e of numbers (in
+00010b20: 7465 6765 7273 206f 7220 666c 6f61 7473  tegers or floats
+00010b30: 2920 666f 7220 7768 6963 6820 7468 6520  ) for which the 
+00010b40: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+00010b50: 6f6e 2069 7320 746f 2062 6520 6361 6c63  on is to be calc
+00010b60: 756c 6174 6564 2e0a 2020 2020 2020 2020  ulated..        
+00010b70: 2020 2020 6465 6361 795f 6661 6374 6f72      decay_factor
+00010b80: 2028 556e 696f 6e5b 696e 742c 2066 6c6f   (Union[int, flo
+00010b90: 6174 5d29 3a20 5468 6520 6465 6361 7920  at]): The decay 
+00010ba0: 6661 6374 6f72 2066 6f72 2077 6569 6768  factor for weigh
+00010bb0: 7469 6e67 2072 6563 656e 7420 7661 6c75  ting recent valu
+00010bc0: 6573 206d 6f72 6520 6865 6176 696c 792e  es more heavily.
+00010bd0: 2044 6566 6175 6c74 7320 746f 2030 2e39   Defaults to 0.9
+00010be0: 352e 0a0a 2020 2020 2020 2020 5265 7475  5...        Retu
+00010bf0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00010c00: 2066 6c6f 6174 3a20 5468 6520 7374 616e   float: The stan
+00010c10: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
+00010c20: 6620 7468 6520 7365 7175 656e 6365 2e20  f the sequence. 
+00010c30: 5265 7475 726e 7320 3020 6966 2074 6865  Returns 0 if the
+00010c40: 2073 6571 7565 6e63 6520 636f 6e74 6169   sequence contai
+00010c50: 6e73 2066 6577 6572 2074 6861 6e20 7477  ns fewer than tw
+00010c60: 6f20 656c 656d 656e 7473 2e0a 0a20 2020  o elements...   
+00010c70: 2020 2020 204e 6f74 6573 3a0a 2020 2020       Notes:.    
+00010c80: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
+00010c90: 6374 696f 6e20 7573 6573 2061 6e20 6578  ction uses an ex
+00010ca0: 706f 6e65 6e74 6961 6c20 6465 6361 7920  ponential decay 
+00010cb0: 746f 2077 6569 6768 7420 7265 6365 6e74  to weight recent
+00010cc0: 206f 6273 6572 7661 7469 6f6e 7320 6d6f   observations mo
+00010cd0: 7265 2068 6561 7669 6c79 2069 6e20 7468  re heavily in th
+00010ce0: 6520 6361 6c63 756c 6174 696f 6e0a 2020  e calculation.  
+00010cf0: 2020 2020 2020 2020 2020 6f66 2074 6865            of the
+00010d00: 206d 6561 6e20 616e 6420 7661 7269 616e   mean and varian
+00010d10: 6365 2c20 7768 6963 6820 6d61 6b65 7320  ce, which makes 
+00010d20: 6974 2073 656e 7369 7469 7665 2074 6f20  it sensitive to 
+00010d30: 7265 6365 6e74 2063 6861 6e67 6573 2069  recent changes i
+00010d40: 6e20 7468 6520 7365 7175 656e 6365 2e0a  n the sequence..
+00010d50: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00010d60: 2020 2020 2069 6620 6c65 6e28 6e75 6d65       if len(nume
+00010d70: 7269 635f 7365 7175 656e 6365 2920 3d3d  ric_sequence) ==
+00010d80: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00010d90: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00010da0: 2822 5468 6520 6e75 6d65 7269 6320 7365  ("The numeric se
+00010db0: 7175 656e 6365 2063 616e 6e6f 7420 6265  quence cannot be
+00010dc0: 2065 6d70 7479 2e22 290a 2020 2020 2020   empty.").      
+00010dd0: 2020 6e20 3d20 300a 2020 2020 2020 2020    n = 0.        
+00010de0: 6d65 616e 203d 2030 2e30 0a20 2020 2020  mean = 0.0.     
+00010df0: 2020 204d 3220 3d20 302e 300a 2020 2020     M2 = 0.0.    
+00010e00: 2020 2020 7765 6967 6874 6564 5f6e 203d      weighted_n =
+00010e10: 2030 2e30 2020 2320 5765 6967 6874 6564   0.0  # Weighted
+00010e20: 2073 616d 706c 6520 636f 756e 740a 0a20   sample count.. 
+00010e30: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
+00010e40: 6e75 6d65 7269 635f 7365 7175 656e 6365  numeric_sequence
+00010e50: 3a0a 2020 2020 2020 2020 2020 2020 6e20  :.            n 
+00010e60: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
+00010e70: 2077 6569 6768 7420 3d20 6465 6361 795f   weight = decay_
+00010e80: 6661 6374 6f72 202a 2a20 286c 656e 286e  factor ** (len(n
+00010e90: 756d 6572 6963 5f73 6571 7565 6e63 6529  umeric_sequence)
+00010ea0: 202d 206e 2920 2023 2043 6f6d 7075 7465   - n)  # Compute
+00010eb0: 2077 6569 6768 742c 206e 6577 6572 2064   weight, newer d
+00010ec0: 6174 6120 6861 7320 6869 6768 6572 2077  ata has higher w
+00010ed0: 6569 6768 740a 2020 2020 2020 2020 2020  eight.          
+00010ee0: 2020 6465 6c74 6120 3d20 7820 2d20 6d65    delta = x - me
+00010ef0: 616e 0a20 2020 2020 2020 2020 2020 2077  an.            w
+00010f00: 6569 6768 7465 645f 6e20 2b3d 2077 6569  eighted_n += wei
+00010f10: 6768 740a 2020 2020 2020 2020 2020 2020  ght.            
+00010f20: 6d65 616e 202b 3d20 2864 656c 7461 202a  mean += (delta *
+00010f30: 2077 6569 6768 7429 202f 2077 6569 6768   weight) / weigh
+00010f40: 7465 645f 6e0a 2020 2020 2020 2020 2020  ted_n.          
+00010f50: 2020 6465 6c74 6132 203d 2078 202d 206d    delta2 = x - m
+00010f60: 6561 6e0a 2020 2020 2020 2020 2020 2020  ean.            
+00010f70: 4d32 202b 3d20 6465 6c74 6120 2a20 6465  M2 += delta * de
+00010f80: 6c74 6132 202a 2077 6569 6768 740a 0a20  lta2 * weight.. 
+00010f90: 2020 2020 2020 2069 6620 7765 6967 6874         if weight
+00010fa0: 6564 5f6e 203c 2032 3a0a 2020 2020 2020  ed_n < 2:.      
+00010fb0: 2020 2020 2020 7265 7475 726e 2030 2e30        return 0.0
+00010fc0: 2020 2320 4e6f 7420 656e 6f75 6768 2073    # Not enough s
+00010fd0: 616d 706c 6573 2074 6f20 636f 6d70 7574  amples to comput
+00010fe0: 6520 7374 616e 6461 7264 2064 6576 6961  e standard devia
+00010ff0: 7469 6f6e 0a20 2020 2020 2020 2076 6172  tion.        var
+00011000: 6961 6e63 6520 3d20 4d32 202f 2077 6569  iance = M2 / wei
+00011010: 6768 7465 645f 6e20 2023 2043 6f6d 7075  ghted_n  # Compu
+00011020: 7465 2076 6172 6961 6e63 6520 7573 696e  te variance usin
+00011030: 6720 7765 6967 6874 6564 2073 616d 706c  g weighted sampl
+00011040: 6520 636f 756e 740a 2020 2020 2020 2020  e count.        
+00011050: 7265 7475 726e 206d 6174 682e 7371 7274  return math.sqrt
+00011060: 2876 6172 6961 6e63 6529 0a0a 2020 2020  (variance)..    
+00011070: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00011080: 2020 6465 6620 6361 6c63 756c 6174 655f    def calculate_
+00011090: 7374 616e 6461 7264 5f64 6576 6961 7469  standard_deviati
+000110a0: 6f6e 286e 756d 6572 6963 5f73 6571 7565  on(numeric_seque
+000110b0: 6e63 653a 204c 6973 745b 556e 696f 6e5b  nce: List[Union[
+000110c0: 696e 742c 2066 6c6f 6174 5d5d 2920 2d3e  int, float]]) ->
+000110d0: 2055 6e69 6f6e 5b69 6e74 2c20 666c 6f61   Union[int, floa
+000110e0: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
+000110f0: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
+00011100: 6573 2074 6865 2073 7461 6e64 6172 6420  es the standard 
+00011110: 6465 7669 6174 696f 6e20 6f66 2061 206e  deviation of a n
+00011120: 756d 6572 6963 2073 6571 7565 6e63 652e  umeric sequence.
+00011130: 0a0a 2020 2020 2020 2020 5468 6973 206d  ..        This m
+00011140: 6574 686f 6420 636f 6d70 7574 6573 2074  ethod computes t
+00011150: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
+00011160: 6174 696f 6e20 6279 2066 6972 7374 2063  ation by first c
+00011170: 616c 6375 6c61 7469 6e67 2074 6865 206d  alculating the m
+00011180: 6561 6e20 6f66 2074 6865 206e 756d 6265  ean of the numbe
+00011190: 7273 2c0a 2020 2020 2020 2020 7468 656e  rs,.        then
+000111a0: 2074 6865 2076 6172 6961 6e63 6520 6173   the variance as
+000111b0: 2074 6865 2061 7665 7261 6765 206f 6620   the average of 
+000111c0: 7468 6520 7371 7561 7265 6420 6469 6666  the squared diff
+000111d0: 6572 656e 6365 7320 6672 6f6d 2074 6865  erences from the
+000111e0: 206d 6561 6e2c 2061 6e64 2066 696e 616c   mean, and final
+000111f0: 6c79 0a20 2020 2020 2020 2074 616b 696e  ly.        takin
+00011200: 6720 7468 6520 7371 7561 7265 2072 6f6f  g the square roo
+00011210: 7420 6f66 2074 6865 2076 6172 6961 6e63  t of the varianc
+00011220: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
+00011230: 3a0a 2020 2020 2020 2020 2020 2020 6e75  :.            nu
+00011240: 6d65 7269 635f 7365 7175 656e 6365 2028  meric_sequence (
+00011250: 4c69 7374 5b55 6e69 6f6e 5b69 6e74 2c20  List[Union[int, 
+00011260: 666c 6f61 745d 5d29 3a20 5468 6520 7365  float]]): The se
+00011270: 7175 656e 6365 206f 6620 6e75 6d62 6572  quence of number
+00011280: 7320 2869 6e74 6567 6572 7320 6f72 2066  s (integers or f
+00011290: 6c6f 6174 7329 2066 6f72 2077 6869 6368  loats) for which
+000112a0: 2074 6865 2073 7461 6e64 6172 6420 6465   the standard de
+000112b0: 7669 6174 696f 6e20 6973 2074 6f20 6265  viation is to be
+000112c0: 2063 616c 6375 6c61 7465 642e 0a0a 2020   calculated...  
+000112d0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+000112e0: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+000112f0: 3a20 5468 6520 7374 616e 6461 7264 2064  : The standard d
+00011300: 6576 6961 7469 6f6e 206f 6620 7468 6520  eviation of the 
+00011310: 7365 7175 656e 6365 2e0a 0a20 2020 2020  sequence...     
+00011320: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+00011330: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
+00011340: 723a 2049 6620 7468 6520 6e75 6d65 7269  r: If the numeri
+00011350: 635f 7365 7175 656e 6365 2069 7320 656d  c_sequence is em
+00011360: 7074 792c 2061 7320 7374 616e 6461 7264  pty, as standard
+00011370: 2064 6576 6961 7469 6f6e 2063 616e 6e6f   deviation canno
+00011380: 7420 6265 2063 616c 6375 6c61 7465 642e  t be calculated.
+00011390: 0a20 2020 2020 2020 204e 6f74 6573 3a0a  .        Notes:.
+000113a0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+000113b0: 2066 756e 6374 696f 6e20 7573 6573 2061   function uses a
+000113c0: 6e20 6578 706f 6e65 6e74 6961 6c20 6465  n exponential de
+000113d0: 6361 7920 746f 2077 6569 6768 7420 7265  cay to weight re
+000113e0: 6365 6e74 206f 6273 6572 7661 7469 6f6e  cent observation
+000113f0: 7320 6d6f 7265 2068 6561 7669 6c79 2069  s more heavily i
+00011400: 6e20 7468 6520 6361 6c63 756c 6174 696f  n the calculatio
+00011410: 6e0a 2020 2020 2020 2020 2020 2020 6f66  n.            of
+00011420: 2074 6865 206d 6561 6e20 616e 6420 7661   the mean and va
+00011430: 7269 616e 6365 2c20 7768 6963 6820 6d61  riance, which ma
+00011440: 6b65 7320 6974 2073 656e 7369 7469 7665  kes it sensitive
+00011450: 2074 6f20 7265 6365 6e74 2063 6861 6e67   to recent chang
+00011460: 6573 2069 6e20 7468 6520 7365 7175 656e  es in the sequen
+00011470: 6365 2e0a 2020 2020 2020 2020 2222 220a  ce..        """.
+00011480: 2020 2020 2020 2020 6966 206c 656e 286e          if len(n
+00011490: 756d 6572 6963 5f73 6571 7565 6e63 6529  umeric_sequence)
+000114a0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+000114b0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000114c0: 726f 7228 2254 6865 206e 756d 6572 6963  ror("The numeric
+000114d0: 2073 6571 7565 6e63 6520 6361 6e6e 6f74   sequence cannot
+000114e0: 2062 6520 656d 7074 792e 2229 0a0a 2020   be empty.")..  
+000114f0: 2020 2020 2020 2320 4361 6c63 756c 6174        # Calculat
+00011500: 6520 7468 6520 6d65 616e 206f 6620 7468  e the mean of th
+00011510: 6520 7365 7175 656e 6365 0a20 2020 2020  e sequence.     
+00011520: 2020 206d 6561 6e20 3d20 7375 6d28 6e75     mean = sum(nu
+00011530: 6d65 7269 635f 7365 7175 656e 6365 2920  meric_sequence) 
+00011540: 2f20 6c65 6e28 6e75 6d65 7269 635f 7365  / len(numeric_se
+00011550: 7175 656e 6365 290a 0a20 2020 2020 2020  quence)..       
+00011560: 2023 2043 616c 6375 6c61 7465 2074 6865   # Calculate the
+00011570: 2073 7175 6172 6564 2064 6966 6665 7265   squared differe
+00011580: 6e63 6573 2066 726f 6d20 7468 6520 6d65  nces from the me
+00011590: 616e 0a20 2020 2020 2020 2073 7175 6172  an.        squar
+000115a0: 6564 5f64 6966 6673 203d 205b 2878 202d  ed_diffs = [(x -
+000115b0: 206d 6561 6e29 202a 2a20 3220 666f 7220   mean) ** 2 for 
+000115c0: 7820 696e 206e 756d 6572 6963 5f73 6571  x in numeric_seq
+000115d0: 7565 6e63 655d 0a0a 2020 2020 2020 2020  uence]..        
+000115e0: 2320 4361 6c63 756c 6174 6520 7468 6520  # Calculate the 
+000115f0: 7661 7269 616e 6365 0a20 2020 2020 2020  variance.       
+00011600: 2076 6172 6961 6e63 6520 3d20 7375 6d28   variance = sum(
+00011610: 7371 7561 7265 645f 6469 6666 7329 202f  squared_diffs) /
+00011620: 206c 656e 286e 756d 6572 6963 5f73 6571   len(numeric_seq
+00011630: 7565 6e63 6529 0a0a 2020 2020 2020 2020  uence)..        
+00011640: 2320 4361 6c63 756c 6174 6520 616e 6420  # Calculate and 
+00011650: 7265 7475 726e 2074 6865 2073 7461 6e64  return the stand
+00011660: 6172 6420 6465 7669 6174 696f 6e0a 2020  ard deviation.  
+00011670: 2020 2020 2020 7374 616e 6461 7264 5f64        standard_d
+00011680: 6576 6961 7469 6f6e 203d 206d 6174 682e  eviation = math.
+00011690: 7371 7274 2876 6172 6961 6e63 6529 0a20  sqrt(variance). 
+000116a0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+000116b0: 616e 6461 7264 5f64 6576 6961 7469 6f6e  andard_deviation
+000116c0: 0a0a 2020 2020 4061 6273 7472 6163 746d  ..    @abstractm
+000116d0: 6574 686f 640a 2020 2020 6465 6620 6361  ethod.    def ca
+000116e0: 6c63 756c 6174 655f 7769 6e6e 696e 675f  lculate_winning_
+000116f0: 616d 6f75 6e74 280a 2020 2020 2020 2020  amount(.        
+00011700: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00011710: 2020 2020 2020 7769 6e6e 696e 675f 6e75        winning_nu
+00011720: 6d62 6572 5f63 6f6d 6269 6e61 7469 6f6e  mber_combination
+00011730: 3a20 4c69 7374 5b69 6e74 5d2c 0a20 2020  : List[int],.   
+00011740: 2020 2020 2020 2020 2070 7572 6368 6173           purchas
+00011750: 655f 6e75 6d62 6572 5f63 6f6d 6269 6e61  e_number_combina
+00011760: 7469 6f6e 733a 204c 6973 745b 4c69 7374  tions: List[List
+00011770: 5b69 6e74 5d5d 2c0a 2020 2020 2020 2020  [int]],.        
+00011780: 2020 2020 2a2a 6b77 6172 6773 3a20 416e      **kwargs: An
+00011790: 790a 2020 2020 2920 2d3e 2054 7570 6c65  y.    ) -> Tuple
+000117a0: 5b66 6c6f 6174 2c20 696e 745d 3a0a 2020  [float, int]:.  
+000117b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000117c0: 2020 4361 6c63 756c 6174 6520 7468 6520    Calculate the 
+000117d0: 7769 6e6e 696e 6720 616d 6f75 6e74 2062  winning amount b
+000117e0: 6173 6564 206f 6e20 6d61 7463 6869 6e67  ased on matching
+000117f0: 2063 6f6d 6269 6e61 7469 6f6e 732e 0a0a   combinations...
+00011800: 2020 2020 2020 2020 3a70 6172 616d 2077          :param w
+00011810: 696e 6e69 6e67 5f6e 756d 6265 725f 636f  inning_number_co
+00011820: 6d62 696e 6174 696f 6e3a 2057 696e 6e69  mbination: Winni
+00011830: 6e67 206e 756d 6265 7220 636f 6d62 696e  ng number combin
+00011840: 6174 696f 6e2e 0a20 2020 2020 2020 203a  ation..        :
+00011850: 7061 7261 6d20 7075 7263 6861 7365 5f6e  param purchase_n
+00011860: 756d 6265 725f 636f 6d62 696e 6174 696f  umber_combinatio
+00011870: 6e73 3a20 5075 7263 6861 7365 206e 756d  ns: Purchase num
+00011880: 6265 7220 636f 6d62 696e 6174 696f 6e73  ber combinations
+00011890: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000118a0: 206b 7761 7267 733a 2041 6464 6974 696f   kwargs: Additio
+000118b0: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+000118c0: 6d65 6e74 732e 0a20 2020 2020 2020 203a  ments..        :
+000118d0: 7265 7475 726e 3a20 5468 6520 746f 7461  return: The tota
+000118e0: 6c20 7769 6e6e 696e 6720 616d 6f75 6e74  l winning amount
+000118f0: 2061 6e64 2074 6865 2063 6f75 6e74 206f   and the count o
+00011900: 6620 7769 6e6e 696e 6720 636f 6d62 696e  f winning combin
+00011910: 6174 696f 6e73 0a20 2020 2020 2020 2022  ations.        "
+00011920: 2222 0a20 2020 2020 2020 2070 6173 730a  "".        pass.
+00011930: 0a0a 636c 6173 7320 416e 616c 797a 6555  ..class AnalyzeU
+00011940: 7469 6c28 4142 4329 3a0a 2020 2020 2222  til(ABC):.    ""
+00011950: 220a 2020 2020 416e 616c 797a 6520 6261  ".    Analyze ba
+00011960: 7365 6420 6f6e 206d 756c 7469 706c 6520  sed on multiple 
+00011970: 6461 7461 0a20 2020 2022 2222 0a0a 2020  data.    """..  
+00011980: 2020 4061 6273 7472 6163 746d 6574 686f    @abstractmetho
+00011990: 640a 2020 2020 6465 6620 616e 616c 797a  d.    def analyz
+000119a0: 655f 7361 6d65 5f70 6572 696f 645f 6e75  e_same_period_nu
+000119b0: 6d62 6572 7328 7365 6c66 2c20 2a2a 6b77  mbers(self, **kw
+000119c0: 6172 6773 3a20 416e 7929 202d 3e20 4e6f  args: Any) -> No
+000119d0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+000119e0: 2020 2020 2020 2020 416e 616c 797a 6520          Analyze 
+000119f0: 7361 6d65 2070 6572 696f 6420 6e75 6d62  same period numb
+00011a00: 6572 2069 6e20 7468 6520 6c61 7374 2070  er in the last p
+00011a10: 6572 696f 642e 0a20 2020 2020 2020 2022  eriod..        "
+00011a20: 2222 0a20 2020 2020 2020 2070 6173 730a  "".        pass.
+00011a30: 0a20 2020 2040 6162 7374 7261 6374 6d65  .    @abstractme
+00011a40: 7468 6f64 0a20 2020 2064 6566 2061 6e61  thod.    def ana
+00011a50: 6c79 7a65 5f73 616d 655f 7765 656b 6461  lyze_same_weekda
+00011a60: 795f 6e75 6d62 6572 7328 7365 6c66 2c20  y_numbers(self, 
+00011a70: 2a2a 6b77 6172 6773 3a20 416e 7929 202d  **kwargs: Any) -
+00011a80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00011a90: 2222 220a 2020 2020 2020 2020 416e 616c  """.        Anal
+00011aa0: 797a 6520 7361 6d65 2077 6565 6b64 6179  yze same weekday
+00011ab0: 206e 756d 6265 7220 696e 2074 6865 206c   number in the l
+00011ac0: 6173 7420 7065 7269 6f64 2e0a 2020 2020  ast period..    
+00011ad0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011ae0: 7061 7373 0a0a 2020 2020 4061 6273 7472  pass..    @abstr
+00011af0: 6163 746d 6574 686f 640a 2020 2020 6465  actmethod.    de
+00011b00: 6620 616e 616c 797a 655f 7265 7065 6174  f analyze_repeat
+00011b10: 6564 5f6e 756d 6265 7273 2873 656c 662c  ed_numbers(self,
+00011b20: 202a 2a6b 7761 7267 733a 2041 6e79 2920   **kwargs: Any) 
+00011b30: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00011b40: 2022 2222 0a20 2020 2020 2020 2041 6e61   """.        Ana
+00011b50: 6c79 7a65 2074 6865 206e 756d 6265 7220  lyze the number 
+00011b60: 7468 6174 2061 7070 6561 7265 6420 7477  that appeared tw
+00011b70: 6963 6520 696e 2074 6865 206c 6173 7420  ice in the last 
+00011b80: 7477 6f20 7065 7269 6f64 2e0a 2020 2020  two period..    
+00011b90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011ba0: 7061 7373 0a0a 2020 2020 4061 6273 7472  pass..    @abstr
+00011bb0: 6163 746d 6574 686f 640a 2020 2020 6465  actmethod.    de
+00011bc0: 6620 616e 616c 797a 655f 6564 6765 5f6e  f analyze_edge_n
+00011bd0: 756d 6265 7273 2873 656c 662c 202a 2a6b  umbers(self, **k
+00011be0: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
+00011bf0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00011c00: 0a20 2020 2020 2020 2041 6e61 6c79 7a65  .        Analyze
+00011c10: 2041 6c73 6f20 6361 6c6c 6564 2061 646a   Also called adj
+00011c20: 6163 656e 7420 6e75 6d62 6572 2c20 706c  acent number, pl
+00011c30: 7573 206f 7220 6d69 6e75 7320 3120 7769  us or minus 1 wi
+00011c40: 7468 2074 6865 2077 696e 6e69 6e67 206e  th the winning n
+00011c50: 756d 6265 7220 6973 7375 6564 2069 6e20  umber issued in 
+00011c60: 7468 6520 7072 6576 696f 7573 2070 6572  the previous per
+00011c70: 696f 640a 2020 2020 2020 2020 2222 220a  iod.        """.
+00011c80: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00011c90: 2020 4061 6273 7472 6163 746d 6574 686f    @abstractmetho
+00011ca0: 640a 2020 2020 6465 6620 616e 616c 797a  d.    def analyz
+00011cb0: 655f 636f 6c64 5f68 6f74 5f6e 756d 6265  e_cold_hot_numbe
+00011cc0: 7273 2873 656c 662c 202a 2a6b 7761 7267  rs(self, **kwarg
+00011cd0: 733a 2041 6e79 2920 2d3e 204e 6f6e 653a  s: Any) -> None:
+00011ce0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011cf0: 2020 2020 2041 6e61 6c79 7a65 204e 756d       Analyze Num
+00011d00: 6265 7273 2074 6861 7420 6861 7665 2061  bers that have a
+00011d10: 7070 6561 7265 6420 696e 2074 6865 206c  ppeared in the l
+00011d20: 6173 7420 7065 7269 6f64 0a20 2020 2020  ast period.     
+00011d30: 2020 2041 6e61 6c79 7a65 204e 756d 6265     Analyze Numbe
+00011d40: 7273 2074 6861 7420 6861 7665 206e 6f74  rs that have not
+00011d50: 2061 7070 6561 7265 6420 696e 2074 6865   appeared in the
+00011d60: 206c 6173 7420 7065 7269 6f64 0a20 2020   last period.   
+00011d70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011d80: 2070 6173 730a 0a20 2020 2040 6162 7374   pass..    @abst
+00011d90: 7261 6374 6d65 7468 6f64 0a20 2020 2064  ractmethod.    d
+00011da0: 6566 2061 6e61 6c79 7a65 5f6f 6d69 7474  ef analyze_omitt
+00011db0: 6564 5f6e 756d 6265 7273 2873 656c 662c  ed_numbers(self,
+00011dc0: 202a 2a6b 7761 7267 733a 2041 6e79 2920   **kwargs: Any) 
+00011dd0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00011de0: 2022 2222 0a20 2020 2020 2020 2041 6e61   """.        Ana
+00011df0: 6c79 7a65 2e0a 2020 2020 2020 2020 4f6d  lyze..        Om
+00011e00: 6973 7369 6f6e 3a20 5468 6520 6e75 6d62  ission: The numb
+00011e10: 6572 206f 6620 7065 7269 6f64 7320 7369  er of periods si
+00011e20: 6e63 6520 7468 6520 7072 6576 696f 7573  nce the previous
+00011e30: 206f 7065 6e69 6e67 2074 6f20 7468 6520   opening to the 
+00011e40: 6375 7272 656e 7420 7065 7269 6f64 2e0a  current period..
+00011e50: 2020 2020 2020 2020 4176 6572 6167 6520          Average 
+00011e60: 6f6d 6973 7369 6f6e 3a20 5468 6520 6176  omission: The av
+00011e70: 6572 6167 6520 6e75 6d62 6572 206f 6620  erage number of 
+00011e80: 6f6d 6973 7369 6f6e 7320 696e 2074 6865  omissions in the
+00011e90: 2073 7461 7469 7374 6963 616c 2070 6572   statistical per
+00011ea0: 696f 640a 2020 2020 2020 2020 2020 2020  iod.            
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+00011ec0: 616c 6375 6c61 7469 6f6e 2066 6f72 6d75  alculation formu
+00011ed0: 6c61 3a20 4176 6572 6167 6520 6f6d 6973  la: Average omis
+00011ee0: 7369 6f6e 203d 0a20 2020 2020 2020 2020  sion =.         
+00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f00: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
+00011f10: 206f 6d69 7373 696f 6e73 2069 6e20 7468   omissions in th
+00011f20: 6520 7374 6174 6973 7469 6361 6c20 7065  e statistical pe
+00011f30: 7269 6f64 202f 2028 6e75 6d62 6572 206f  riod / (number o
+00011f40: 6620 6f63 6375 7272 656e 6365 7320 2b31  f occurrences +1
+00011f50: 2929 0a20 2020 2020 2020 204d 6178 696d  )).        Maxim
+00011f60: 756d 206d 6973 7365 6420 7661 6c75 653a  um missed value:
+00011f70: 2049 6e64 6963 6174 6573 2074 6865 206d   Indicates the m
+00011f80: 6178 696d 756d 2076 616c 7565 206f 6620  aximum value of 
+00011f90: 616c 6c20 6d69 7373 6564 2076 616c 7565  all missed value
+00011fa0: 7320 696e 2074 6865 2073 7461 7469 7374  s in the statist
+00011fb0: 6963 616c 2070 6572 696f 642e 0a20 2020  ical period..   
+00011fc0: 2020 2020 2043 7572 7265 6e74 206f 6d69       Current omi
+00011fd0: 7373 696f 6e3a 2054 6865 206e 756d 6265  ssion: The numbe
+00011fe0: 7220 6f66 2070 6572 696f 6473 2062 6574  r of periods bet
+00011ff0: 7765 656e 2074 6865 206c 6173 7420 6f63  ween the last oc
+00012000: 6375 7272 656e 6365 2061 6e64 2074 6865  currence and the
+00012010: 2070 7265 7365 6e74 2c20 6966 2074 6865   present, if the
+00012020: 206d 6973 7369 6e67 206f 626a 6563 740a   missing object.
+00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012040: 2020 2020 2020 2020 2020 6170 7065 6172            appear
+00012050: 6564 2069 6e20 7468 6520 6375 7272 656e  ed in the curren
+00012060: 7420 7065 7269 6f64 2c20 7468 6520 6375  t period, the cu
+00012070: 7272 656e 7420 6f6d 6973 7369 6f6e 2076  rrent omission v
+00012080: 616c 7565 2069 7320 300a 2020 2020 2020  alue is 0.      
+00012090: 2020 5072 6576 696f 7573 2070 6572 696f    Previous perio
+000120a0: 6420 6f6d 6973 7369 6f6e 3a20 5468 6520  d omission: The 
+000120b0: 696e 7465 7276 616c 2062 6574 7765 656e  interval between
+000120c0: 2074 6865 206c 6173 7420 7477 6f20 7065   the last two pe
+000120d0: 7269 6f64 7320 2865 7863 6c75 6469 6e67  riods (excluding
+000120e0: 2074 6865 2063 7572 7265 6e74 2070 6572   the current per
+000120f0: 696f 6429 0a20 2020 2020 2020 2054 6865  iod).        The
+00012100: 6f72 6574 6963 616c 206e 756d 6265 723a  oretical number:
+00012110: 2054 6865 2074 6865 6f72 6574 6963 616c   The theoretical
+00012120: 206e 756d 6265 7220 7265 6665 7273 2074   number refers t
+00012130: 6f20 7468 6520 6e75 6d62 6572 206f 6620  o the number of 
+00012140: 7469 6d65 7320 7468 6520 6d69 7373 696e  times the missin
+00012150: 6720 6f62 6a65 6374 2073 686f 756c 640a  g object should.
+00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012170: 2020 2020 2020 2020 2020 2020 7468 656f              theo
+00012180: 7265 7469 6361 6c6c 7920 6170 7065 6172  retically appear
+00012190: 2c20 3d20 7468 6520 746f 7461 6c20 6e75  , = the total nu
+000121a0: 6d62 6572 206f 6620 7420 7469 6d65 7320  mber of t times 
+000121b0: 2a20 7468 656f 7265 7469 6361 6c20 7072  * theoretical pr
+000121c0: 6f62 6162 696c 6974 790a 2020 2020 2020  obability.      
+000121d0: 2020 4465 7369 7265 6420 7072 6f62 6162    Desired probab
+000121e0: 696c 6974 793a 2044 6573 6972 6564 2070  ility: Desired p
+000121f0: 726f 6261 6269 6c69 7479 2072 6566 6c65  robability refle
+00012200: 6374 7320 7468 6520 6964 6561 6c20 6f63  cts the ideal oc
+00012210: 6375 7272 656e 6365 2070 726f 6261 6269  currence probabi
+00012220: 6c69 7479 206f 6620 7468 6520 6d69 7373  lity of the miss
+00012230: 696e 6720 6f62 6a65 6374 2e0a 2020 2020  ing object..    
+00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012250: 2020 2020 2020 2020 2054 6865 2066 6f72           The for
+00012260: 6d75 6c61 2069 7320 2863 7572 7265 6e74  mula is (current
+00012270: 206f 6d69 7373 696f 6e2f 6176 6572 6167   omission/averag
+00012280: 6520 6f6d 6973 7369 6f6e 202a 2074 6865  e omission * the
+00012290: 6f72 6574 6963 616c 2070 726f 6261 6269  oretical probabi
+000122a0: 6c69 7479 290a 2020 2020 2020 2020 2222  lity).        ""
+000122b0: 220a 2020 2020 2020 2020 7061 7373 0a0a  ".        pass..
+000122c0: 0a63 6c61 7373 2047 656e 6574 6963 7355  .class GeneticsU
+000122d0: 7469 6c3a 0a20 2020 2064 6566 205f 5f69  til:.    def __i
+000122e0: 6e69 745f 5f28 7365 6c66 2c20 7265 6665  nit__(self, refe
+000122f0: 7273 3a20 6c69 7374 2c20 6461 7461 3a20  rs: list, data: 
+00012300: 6c69 7374 2c20 6d69 6e5f 6e75 6d3a 2069  list, min_num: i
+00012310: 6e74 2c20 6d61 785f 6e75 6d3a 2069 6e74  nt, max_num: int
+00012320: 2c20 6669 746e 6573 735f 7061 7261 6d73  , fitness_params
+00012330: 3a20 6469 6374 2c0a 2020 2020 2020 2020  : dict,.        
+00012340: 2020 2020 2020 2020 2070 6f70 756c 6174           populat
+00012350: 696f 6e5f 7369 7a65 3a20 696e 7420 3d20  ion_size: int = 
+00012360: 3130 302c 206e 756d 5f67 656e 6573 3a20  100, num_genes: 
+00012370: 696e 7420 3d20 352c 2074 6f75 726e 616d  int = 5, tournam
+00012380: 656e 745f 7369 7a65 3a20 696e 7420 3d20  ent_size: int = 
+00012390: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
+000123a0: 2020 2020 6d75 7461 7469 6f6e 5f72 6174      mutation_rat
+000123b0: 653a 2066 6c6f 6174 203d 2030 2e31 2c20  e: float = 0.1, 
+000123c0: 6570 6f63 685f 636f 756e 743a 2069 6e74  epoch_count: int
+000123d0: 203d 2031 3030 293a 0a20 2020 2020 2020   = 100):.       
+000123e0: 2022 2222 0a20 2020 2020 2020 2049 6e69   """.        Ini
+000123f0: 7469 616c 697a 6573 2074 6865 2047 656e  tializes the Gen
+00012400: 6574 6963 7355 7469 6c20 636c 6173 7320  eticsUtil class 
+00012410: 7769 7468 2074 6865 206e 6563 6573 7361  with the necessa
+00012420: 7279 2070 6172 616d 6574 6572 7320 666f  ry parameters fo
+00012430: 7220 7468 6520 6765 6e65 7469 6320 616c  r the genetic al
+00012440: 676f 7269 7468 6d2e 0a0a 2020 2020 2020  gorithm...      
+00012450: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00012460: 7265 6665 7273 2028 6c69 7374 293a 2052  refers (list): R
+00012470: 6566 6572 656e 6365 206d 6174 7269 7820  eference matrix 
+00012480: 6f72 2064 6174 6120 7573 6564 2066 6f72  or data used for
+00012490: 2063 7265 6174 696e 6720 7468 6520 7265   creating the re
+000124a0: 6665 7265 6e63 6520 6d61 7472 6978 2e0a  ference matrix..
+000124b0: 2020 2020 2020 2020 6461 7461 2028 6c69          data (li
+000124c0: 7374 293a 2044 6174 6173 6574 2066 726f  st): Dataset fro
+000124d0: 6d20 7768 6963 6820 6765 6e65 7320 6172  m which genes ar
+000124e0: 6520 7365 6c65 6374 6564 2e0a 2020 2020  e selected..    
+000124f0: 2020 2020 6d69 6e5f 6e75 6d20 2869 6e74      min_num (int
+00012500: 293a 204d 696e 696d 756d 2061 6c6c 6f77  ): Minimum allow
+00012510: 6162 6c65 2076 616c 7565 2066 6f72 2061  able value for a
+00012520: 2067 656e 652e 0a20 2020 2020 2020 206d   gene..        m
+00012530: 6178 5f6e 756d 2028 696e 7429 3a20 4d61  ax_num (int): Ma
+00012540: 7869 6d75 6d20 616c 6c6f 7761 626c 6520  ximum allowable 
+00012550: 7661 6c75 6520 666f 7220 6120 6765 6e65  value for a gene
+00012560: 2e0a 2020 2020 2020 2020 6669 746e 6573  ..        fitnes
+00012570: 735f 7061 7261 6d73 2028 6469 6374 293a  s_params (dict):
+00012580: 2050 6172 616d 6574 6572 7320 7573 6564   Parameters used
+00012590: 2066 6f72 2063 616c 6375 6c61 7469 6e67   for calculating
+000125a0: 2066 6974 6e65 7373 2e0a 2020 2020 2020   fitness..      
+000125b0: 2020 706f 7075 6c61 7469 6f6e 5f73 697a    population_siz
+000125c0: 6520 2869 6e74 293a 204e 756d 6265 7220  e (int): Number 
+000125d0: 6f66 2069 6e64 6976 6964 7561 6c73 2069  of individuals i
+000125e0: 6e20 7468 6520 706f 7075 6c61 7469 6f6e  n the population
+000125f0: 2e0a 2020 2020 2020 2020 6e75 6d5f 6765  ..        num_ge
+00012600: 6e65 7320 2869 6e74 293a 204e 756d 6265  nes (int): Numbe
+00012610: 7220 6f66 2067 656e 6573 2069 6e20 6561  r of genes in ea
+00012620: 6368 2069 6e64 6976 6964 7561 6c2e 0a20  ch individual.. 
+00012630: 2020 2020 2020 2074 6f75 726e 616d 656e         tournamen
+00012640: 745f 7369 7a65 2028 696e 7429 3a20 5369  t_size (int): Si
+00012650: 7a65 206f 6620 7468 6520 746f 7572 6e61  ze of the tourna
+00012660: 6d65 6e74 2066 6f72 2073 656c 6563 7469  ment for selecti
+00012670: 6f6e 2070 726f 6365 7373 2e0a 2020 2020  on process..    
+00012680: 2020 2020 6d75 7461 7469 6f6e 5f72 6174      mutation_rat
+00012690: 6520 2866 6c6f 6174 293a 2050 726f 6261  e (float): Proba
+000126a0: 6269 6c69 7479 206f 6620 6d75 7461 7469  bility of mutati
+000126b0: 6f6e 2070 6572 2067 656e 652e 0a20 2020  on per gene..   
+000126c0: 2020 2020 2065 706f 6368 5f63 6f75 6e74       epoch_count
+000126d0: 2028 696e 7429 3a20 4e75 6d62 6572 206f   (int): Number o
+000126e0: 6620 6765 6e65 7261 7469 6f6e 7320 6f72  f generations or
+000126f0: 2065 706f 6368 7320 7468 6520 616c 676f   epochs the algo
+00012700: 7269 7468 6d20 7769 6c6c 2072 756e 2e0a  rithm will run..
+00012710: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012720: 2020 2020 7365 6c66 2e72 6566 6572 7320      self.refers 
+00012730: 3d20 7265 6665 7273 0a20 2020 2020 2020  = refers.       
+00012740: 2073 656c 662e 6461 7461 203d 2064 6174   self.data = dat
+00012750: 610a 2020 2020 2020 2020 7365 6c66 2e6d  a.        self.m
+00012760: 696e 5f6e 756d 203d 206d 696e 5f6e 756d  in_num = min_num
+00012770: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+00012780: 785f 6e75 6d20 3d20 6d61 785f 6e75 6d0a  x_num = max_num.
+00012790: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
+000127a0: 6e65 7373 5f70 6172 616d 7320 3d20 6669  ness_params = fi
+000127b0: 746e 6573 735f 7061 7261 6d73 0a20 2020  tness_params.   
+000127c0: 2020 2020 2073 656c 662e 706f 7075 6c61       self.popula
+000127d0: 7469 6f6e 5f73 697a 6520 3d20 706f 7075  tion_size = popu
+000127e0: 6c61 7469 6f6e 5f73 697a 650a 2020 2020  lation_size.    
+000127f0: 2020 2020 7365 6c66 2e6e 756d 5f67 656e      self.num_gen
+00012800: 6573 203d 206e 756d 5f67 656e 6573 0a20  es = num_genes. 
+00012810: 2020 2020 2020 2073 656c 662e 746f 7572         self.tour
+00012820: 6e61 6d65 6e74 5f73 697a 6520 3d20 746f  nament_size = to
+00012830: 7572 6e61 6d65 6e74 5f73 697a 650a 2020  urnament_size.  
+00012840: 2020 2020 2020 7365 6c66 2e6d 7574 6174        self.mutat
+00012850: 696f 6e5f 7261 7465 203d 206d 7574 6174  ion_rate = mutat
+00012860: 696f 6e5f 7261 7465 0a20 2020 2020 2020  ion_rate.       
+00012870: 2073 656c 662e 6570 6f63 685f 636f 756e   self.epoch_coun
+00012880: 7420 3d20 6570 6f63 685f 636f 756e 740a  t = epoch_count.
+00012890: 2020 2020 2020 2020 7365 6c66 2e70 6f70          self.pop
+000128a0: 756c 6174 696f 6e20 3d20 7365 6c66 2e69  ulation = self.i
+000128b0: 6e69 745f 706f 7075 6c61 7469 6f6e 2829  nit_population()
+000128c0: 2020 2320 496e 6974 6961 6c69 7a65 7320    # Initializes 
+000128d0: 7468 6520 706f 7075 6c61 7469 6f6e 0a20  the population. 
+000128e0: 2020 2020 2020 2073 656c 662e 7265 6665         self.refe
+000128f0: 7273 5f6d 6174 7269 7820 3d20 7365 6c66  rs_matrix = self
+00012900: 2e63 7265 6174 655f 7265 6665 7273 5f6d  .create_refers_m
+00012910: 6174 7269 7828 2920 2023 2043 7265 6174  atrix()  # Creat
+00012920: 6573 2061 206d 6174 7269 7820 6672 6f6d  es a matrix from
+00012930: 2072 6566 6572 656e 6365 2064 6174 610a   reference data.
+00012940: 0a20 2020 2064 6566 2069 6e69 745f 706f  .    def init_po
+00012950: 7075 6c61 7469 6f6e 2873 656c 6629 202d  pulation(self) -
+00012960: 3e20 6c69 7374 3a0a 2020 2020 2020 2020  > list:.        
+00012970: 2222 220a 2020 2020 2020 2020 496e 6974  """.        Init
+00012980: 6961 6c69 7a65 7320 7468 6520 706f 7075  ializes the popu
+00012990: 6c61 7469 6f6e 2077 6974 6820 7261 6e64  lation with rand
+000129a0: 6f6d 6c79 2073 656c 6563 7465 642c 206e  omly selected, n
+000129b0: 6f6e 2d72 6570 6561 7469 6e67 2067 656e  on-repeating gen
+000129c0: 6573 2066 726f 6d20 7468 6520 6461 7461  es from the data
+000129d0: 2073 6574 2e0a 0a20 2020 2020 2020 2052   set...        R
+000129e0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+000129f0: 6c69 7374 3a20 4120 6c69 7374 206f 6620  list: A list of 
+00012a00: 696e 6469 7669 6475 616c 732c 2065 6163  individuals, eac
+00012a10: 6820 7265 7072 6573 656e 7465 6420 6173  h represented as
+00012a20: 2061 2073 6f72 7465 6420 6c69 7374 206f   a sorted list o
+00012a30: 6620 6765 6e65 732e 0a20 2020 2020 2020  f genes..       
+00012a40: 2022 2222 0a20 2020 2020 2020 2070 6f70   """.        pop
+00012a50: 756c 6174 696f 6e20 3d20 5b6e 702e 7261  ulation = [np.ra
+00012a60: 6e64 6f6d 2e63 686f 6963 6528 7365 6c66  ndom.choice(self
+00012a70: 2e64 6174 612c 2073 656c 662e 6e75 6d5f  .data, self.num_
+00012a80: 6765 6e65 732c 2072 6570 6c61 6365 3d46  genes, replace=F
+00012a90: 616c 7365 2920 666f 7220 5f20 696e 2072  alse) for _ in r
+00012aa0: 616e 6765 2873 656c 662e 706f 7075 6c61  ange(self.popula
+00012ab0: 7469 6f6e 5f73 697a 6529 5d0a 2020 2020  tion_size)].    
+00012ac0: 2020 2020 736f 7274 6564 5f70 6f70 756c      sorted_popul
+00012ad0: 6174 696f 6e20 3d20 5b6e 702e 736f 7274  ation = [np.sort
+00012ae0: 2872 6f77 2920 666f 7220 726f 7720 696e  (row) for row in
+00012af0: 2070 6f70 756c 6174 696f 6e5d 0a20 2020   population].   
+00012b00: 2020 2020 2072 6574 7572 6e20 736f 7274       return sort
+00012b10: 6564 5f70 6f70 756c 6174 696f 6e0a 0a20  ed_population.. 
+00012b20: 2020 2064 6566 2063 7265 6174 655f 7265     def create_re
+00012b30: 6665 7273 5f6d 6174 7269 7828 7365 6c66  fers_matrix(self
+00012b40: 2920 2d3e 206c 6973 743a 0a20 2020 2020  ) -> list:.     
+00012b50: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00012b60: 7265 6174 6573 2061 206d 6174 7269 7820  reates a matrix 
+00012b70: 6261 7365 6420 6f6e 2074 6865 2072 6566  based on the ref
+00012b80: 6572 656e 6365 2064 6174 6120 7072 6f76  erence data prov
+00012b90: 6964 6564 2064 7572 696e 6720 696e 6974  ided during init
+00012ba0: 6961 6c69 7a61 7469 6f6e 2e0a 0a20 2020  ialization...   
+00012bb0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00012bc0: 2020 2020 2020 6c69 7374 3a20 4120 6d61        list: A ma
+00012bd0: 7472 6978 2077 6865 7265 2065 6163 6820  trix where each 
+00012be0: 726f 7720 636f 7272 6573 706f 6e64 7320  row corresponds 
+00012bf0: 746f 2061 6e20 6974 656d 2069 6e20 7468  to an item in th
+00012c00: 6520 7265 6665 7265 6e63 6520 6461 7461  e reference data
+00012c10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012c20: 7769 7468 2062 696e 6172 7920 656e 636f  with binary enco
+00012c30: 6469 6e67 2062 6173 6564 206f 6e20 7468  ding based on th
+00012c40: 6520 7072 6573 656e 6365 206f 6620 656c  e presence of el
+00012c50: 656d 656e 7473 2077 6974 6869 6e20 7468  ements within th
+00012c60: 6520 7370 6563 6966 6965 6420 7261 6e67  e specified rang
+00012c70: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00012c80: 2020 2020 2020 2072 6566 6572 735f 6d61         refers_ma
+00012c90: 7472 6978 203d 205b 5d0a 2020 2020 2020  trix = [].      
+00012ca0: 2020 666f 7220 726f 7720 696e 2073 656c    for row in sel
+00012cb0: 662e 7265 6665 7273 3a0a 2020 2020 2020  f.refers:.      
+00012cc0: 2020 2020 2020 7665 6374 6f72 203d 205b        vector = [
+00012cd0: 305d 202a 2073 656c 662e 6d61 785f 6e75  0] * self.max_nu
+00012ce0: 6d20 2023 2049 6e69 7469 616c 697a 6520  m  # Initialize 
+00012cf0: 7665 6374 6f72 206f 6620 6c65 6e67 7468  vector of length
+00012d00: 206d 6178 5f6e 756d 2077 6974 6820 7a65   max_num with ze
+00012d10: 726f 730a 2020 2020 2020 2020 2020 2020  ros.            
+00012d20: 666f 7220 6e75 6d20 696e 2072 6f77 3a0a  for num in row:.
+00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d40: 6966 2073 656c 662e 6d69 6e5f 6e75 6d20  if self.min_num 
+00012d50: 3c3d 206e 756d 203c 3d20 7365 6c66 2e6d  <= num <= self.m
+00012d60: 6178 5f6e 756d 3a0a 2020 2020 2020 2020  ax_num:.        
+00012d70: 2020 2020 2020 2020 2020 2020 7665 6374              vect
+00012d80: 6f72 5b6e 756d 202d 2031 5d20 3d20 3120  or[num - 1] = 1 
+00012d90: 2023 2053 6574 2074 6865 2063 6f72 7265   # Set the corre
+00012da0: 7370 6f6e 6469 6e67 2070 6f73 6974 696f  sponding positio
+00012db0: 6e20 746f 2031 0a20 2020 2020 2020 2020  n to 1.         
+00012dc0: 2020 2072 6566 6572 735f 6d61 7472 6978     refers_matrix
+00012dd0: 2e61 7070 656e 6428 7665 6374 6f72 290a  .append(vector).
+00012de0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00012df0: 6566 6572 735f 6d61 7472 6978 0a0a 2020  efers_matrix..  
+00012e00: 2020 6465 6620 6368 6563 6b5f 6469 6167    def check_diag
+00012e10: 6f6e 616c 2873 656c 662c 2069 6e64 6976  onal(self, indiv
+00012e20: 6964 7561 6c3a 206c 6973 742c 2064 6673  idual: list, dfs
+00012e30: 5f73 697a 653a 2074 7570 6c65 203d 2028  _size: tuple = (
+00012e40: 332c 2033 2929 202d 3e20 666c 6f61 743a  3, 3)) -> float:
+00012e50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012e60: 2020 2020 2043 6865 636b 7320 6469 6167       Checks diag
+00012e70: 6f6e 616c 2061 6c69 676e 6d65 6e74 7320  onal alignments 
+00012e80: 696e 2061 2064 796e 616d 6963 616c 6c79  in a dynamically
+00012e90: 2075 7064 6174 6564 206d 6174 7269 7820   updated matrix 
+00012ea0: 6261 7365 6420 6f6e 2074 6865 2069 6e64  based on the ind
+00012eb0: 6976 6964 7561 6c27 7320 6765 6e65 730a  ividual's genes.
+00012ec0: 2020 2020 2020 2020 616e 6420 6576 616c          and eval
+00012ed0: 7561 7465 7320 7468 6569 7220 6669 746e  uates their fitn
+00012ee0: 6573 7320 6261 7365 6420 6f6e 2074 6865  ess based on the
+00012ef0: 2061 6c69 676e 6d65 6e74 2e0a 0a20 2020   alignment...   
+00012f00: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00012f10: 2020 2069 6e64 6976 6964 7561 6c20 286c     individual (l
+00012f20: 6973 7429 3a20 4c69 7374 206f 6620 6765  ist): List of ge
+00012f30: 6e65 2069 6e64 6963 6573 2072 6570 7265  ne indices repre
+00012f40: 7365 6e74 696e 6720 616e 2069 6e64 6976  senting an indiv
+00012f50: 6964 7561 6c20 696e 2074 6865 2070 6f70  idual in the pop
+00012f60: 756c 6174 696f 6e2e 0a20 2020 2020 2020  ulation..       
+00012f70: 2064 6673 5f73 697a 6520 2874 7570 6c65   dfs_size (tuple
+00012f80: 293a 2053 697a 6520 6f66 2074 6865 206d  ): Size of the m
+00012f90: 6174 7269 7820 7265 6769 6f6e 2074 6f20  atrix region to 
+00012fa0: 6368 6563 6b20 666f 7220 6469 6167 6f6e  check for diagon
+00012fb0: 616c 2061 6c69 676e 6d65 6e74 7320 2872  al alignments (r
+00012fc0: 6f77 732c 2063 6f6c 7329 2e0a 0a20 2020  ows, cols)...   
+00012fd0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00012fe0: 2020 2020 2020 666c 6f61 743a 2041 2066        float: A f
+00012ff0: 6974 6e65 7373 2076 616c 7565 206d 6f64  itness value mod
+00013000: 6966 6965 6420 6261 7365 6420 6f6e 2074  ified based on t
+00013010: 6865 2070 7265 7365 6e63 6520 6f66 2064  he presence of d
+00013020: 6961 676f 6e61 6c20 616c 6967 6e6d 656e  iagonal alignmen
+00013030: 7473 2e0a 2020 2020 2020 2020 2222 220a  ts..        """.
+00013040: 2020 2020 2020 2020 6669 746e 6573 735f          fitness_
+00013050: 7661 6c75 6520 3d20 310a 2020 2020 2020  value = 1.      
+00013060: 2020 7072 655f 696e 6465 7820 3d20 696e    pre_index = in
+00013070: 6469 7669 6475 616c 5b30 5d20 2d20 3120  dividual[0] - 1 
+00013080: 2023 2050 7265 7669 6f75 7320 696e 6465   # Previous inde
+00013090: 7820 666f 7220 6469 6167 6f6e 616c 2063  x for diagonal c
+000130a0: 6865 636b 696e 670a 0a20 2020 2020 2020  hecking..       
+000130b0: 2066 6f72 2069 6e64 6920 696e 2069 6e64   for indi in ind
+000130c0: 6976 6964 7561 6c3a 0a20 2020 2020 2020  ividual:.       
+000130d0: 2020 2020 2069 6620 6e6f 7420 2873 656c       if not (sel
+000130e0: 662e 6d69 6e5f 6e75 6d20 3c3d 2069 6e64  f.min_num <= ind
+000130f0: 6920 3c3d 2073 656c 662e 6d61 785f 6e75  i <= self.max_nu
+00013100: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+00013110: 2020 2020 7265 7475 726e 2031 2020 2320      return 1  # 
+00013120: 5265 7475 726e 2061 2064 6566 6175 6c74  Return a default
+00013130: 2066 6974 6e65 7373 2076 616c 7565 2069   fitness value i
+00013140: 6620 6765 6e65 2069 7320 6f75 7420 6f66  f gene is out of
+00013150: 2076 616c 6964 2072 616e 6765 0a0a 2020   valid range..  
+00013160: 2020 2020 2020 2020 2020 6e75 6d5f 696e            num_in
+00013170: 6465 7820 3d20 696e 6469 202d 2031 0a20  dex = indi - 1. 
+00013180: 2020 2020 2020 2020 2020 2072 6f77 7320             rows 
+00013190: 3d20 6c65 6e28 7365 6c66 2e72 6566 6572  = len(self.refer
+000131a0: 735f 6d61 7472 6978 290a 2020 2020 2020  s_matrix).      
+000131b0: 2020 2020 2020 636f 6c73 203d 2073 656c        cols = sel
+000131c0: 662e 6d61 785f 6e75 6d0a 2020 2020 2020  f.max_num.      
+000131d0: 2020 2020 2020 6466 735f 726f 772c 2064        dfs_row, d
+000131e0: 6673 5f63 6f6c 203d 2064 6673 5f73 697a  fs_col = dfs_siz
+000131f0: 650a 2020 2020 2020 2020 2020 2020 6973  e.            is
+00013200: 5f62 616c 616e 6365 203d 2064 6673 5f72  _balance = dfs_r
+00013210: 6f77 203d 3d20 6466 735f 636f 6c20 2023  ow == dfs_col  #
+00013220: 2043 6865 636b 2069 6620 7468 6520 6172   Check if the ar
+00013230: 6561 2074 6f20 6265 2063 6865 636b 6564  ea to be checked
+00013240: 2069 7320 6120 7371 7561 7265 0a20 2020   is a square.   
+00013250: 2020 2020 2020 2020 2074 6172 6765 7420           target 
+00013260: 3d20 6d69 6e28 6466 735f 7369 7a65 290a  = min(dfs_size).
+00013270: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013280: 6466 735f 726f 7720 3e20 726f 7773 206f  dfs_row > rows o
+00013290: 7220 6466 735f 636f 6c20 3e20 636f 6c73  r dfs_col > cols
+000132a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000132b0: 2020 636f 6e74 696e 7565 2020 2320 536b    continue  # Sk
+000132c0: 6970 2069 6620 7468 6520 6d61 7472 6978  ip if the matrix
+000132d0: 2069 7320 736d 616c 6c65 7220 7468 616e   is smaller than
+000132e0: 2074 6865 2064 6673 2073 697a 650a 0a20   the dfs size.. 
+000132f0: 2020 2020 2020 2020 2020 2023 2043 7265             # Cre
+00013300: 6174 6520 6120 6e65 7720 6d61 7472 6978  ate a new matrix
+00013310: 2069 6e63 6c75 6469 6e67 2061 206e 6577   including a new
+00013320: 2072 6f77 2066 6f72 2074 6865 2063 7572   row for the cur
+00013330: 7265 6e74 2067 656e 650a 2020 2020 2020  rent gene.      
+00013340: 2020 2020 2020 6e65 775f 6d61 7472 6978        new_matrix
+00013350: 203d 205b 726f 775b 3a5d 2066 6f72 2072   = [row[:] for r
+00013360: 6f77 2069 6e20 7365 6c66 2e72 6566 6572  ow in self.refer
+00013370: 735f 6d61 7472 6978 5d20 2023 2043 6f70  s_matrix]  # Cop
+00013380: 7920 7468 6520 6578 6973 7469 6e67 206d  y the existing m
+00013390: 6174 7269 780a 2020 2020 2020 2020 2020  atrix.          
+000133a0: 2020 6e65 775f 726f 7720 3d20 5b30 5d20    new_row = [0] 
+000133b0: 2a20 7365 6c66 2e6d 6178 5f6e 756d 0a20  * self.max_num. 
+000133c0: 2020 2020 2020 2020 2020 206e 6577 5f72             new_r
+000133d0: 6f77 5b6e 756d 5f69 6e64 6578 5d20 3d20  ow[num_index] = 
+000133e0: 310a 2020 2020 2020 2020 2020 2020 6e65  1.            ne
+000133f0: 775f 6d61 7472 6978 2e61 7070 656e 6428  w_matrix.append(
+00013400: 6e65 775f 726f 7729 2020 2320 4164 6420  new_row)  # Add 
+00013410: 7468 6520 6e65 7720 726f 7720 636f 7272  the new row corr
+00013420: 6563 746c 790a 0a20 2020 2020 2020 2020  ectly..         
+00013430: 2020 2023 2043 6865 636b 2064 6961 676f     # Check diago
+00013440: 6e61 6c73 2c20 6f6e 6c79 2075 7077 6172  nals, only upwar
+00013450: 6473 0a20 2020 2020 2020 2020 2020 2066  ds.            f
+00013460: 6f72 2064 7220 696e 205b 2d31 5d3a 2020  or dr in [-1]:  
+00013470: 2320 4f6e 6c79 206e 6565 6420 746f 2063  # Only need to c
+00013480: 6865 636b 2074 6865 2075 7070 6572 2064  heck the upper d
+00013490: 6961 676f 6e61 6c73 0a20 2020 2020 2020  iagonals.       
+000134a0: 2020 2020 2020 2020 206d 6f76 655f 7220           move_r 
+000134b0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+000134c0: 2020 2020 2020 2020 6d6f 7665 5f72 5f63          move_r_c
+000134d0: 6f75 6e74 203d 2030 0a20 2020 2020 2020  ount = 0.       
+000134e0: 2020 2020 2020 2020 206d 6f76 655f 635f           move_c_
+000134f0: 636f 756e 7420 3d20 300a 2020 2020 2020  count = 0.      
+00013500: 2020 2020 2020 2020 2020 666f 7220 6463            for dc
+00013510: 2069 6e20 5b2d 312c 2031 5d3a 2020 2320   in [-1, 1]:  # 
+00013520: 4368 6563 6b20 626f 7468 206c 6566 7420  Check both left 
+00013530: 616e 6420 7269 6768 7420 6469 6167 6f6e  and right diagon
+00013540: 616c 730a 2020 2020 2020 2020 2020 2020  als.            
+00013550: 2020 2020 2020 2020 636f 756e 7420 3d20          count = 
+00013560: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00013570: 2020 2020 2020 722c 2063 203d 2072 6f77        r, c = row
+00013580: 732c 206e 756d 5f69 6e64 6578 0a20 2020  s, num_index.   
 00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135a0: 2020 2023 2041 646a 7573 7420 6669 746e     # Adjust fitn
-000135b0: 6573 7320 6261 7365 6420 6f6e 2074 6865  ess based on the
-000135c0: 2063 6f75 6e74 206f 6620 6469 6167 6f6e   count of diagon
-000135d0: 616c 2061 6c69 676e 6d65 6e74 730a 2020  al alignments.  
-000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135f0: 2020 6966 2064 6673 5f72 6f77 203d 3d20    if dfs_row == 
-00013600: 6466 735f 636f 6c20 616e 6420 636f 756e  dfs_col and coun
-00013610: 7420 3d3d 2074 6172 6765 743a 0a20 2020  t == target:.   
-00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013630: 2020 2020 2066 6974 6e65 7373 5f76 616c       fitness_val
-00013640: 7565 202a 3d20 7365 6c66 2e66 6974 6e65  ue *= self.fitne
-00013650: 7373 5f70 6172 616d 735b 305d 0a20 2020  ss_params[0].   
-00013660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013670: 2065 6c69 6620 6e6f 7420 6466 735f 726f   elif not dfs_ro
-00013680: 7720 3d3d 2064 6673 5f63 6f6c 2061 6e64  w == dfs_col and
-00013690: 206d 6178 286d 6f76 655f 725f 636f 756e   max(move_r_coun
-000136a0: 742c 206d 6f76 655f 635f 636f 756e 7429  t, move_c_count)
-000136b0: 203d 3d20 7461 7267 6574 202d 2031 3a0a   == target - 1:.
-000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136d0: 2020 2020 2020 2020 6669 746e 6573 735f          fitness_
-000136e0: 7661 6c75 6520 2a3d 2073 656c 662e 6669  value *= self.fi
-000136f0: 746e 6573 735f 7061 7261 6d73 5b31 5d0a  tness_params[1].
-00013700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013710: 2023 2043 6865 636b 2076 6572 7469 6361   # Check vertica
-00013720: 6c20 616c 6967 6e6d 656e 740a 2020 2020  l alignment.    
-00013730: 2020 2020 2020 2020 2020 2020 636f 756e              coun
-00013740: 7420 3d20 300a 2020 2020 2020 2020 2020  t = 0.          
-00013750: 2020 2020 2020 722c 2063 203d 2072 6f77        r, c = row
-00013760: 732c 206e 756d 5f69 6e64 6578 0a20 2020  s, num_index.   
-00013770: 2020 2020 2020 2020 2020 2020 2077 6869               whi
-00013780: 6c65 2030 203c 3d20 7220 3c20 6c65 6e28  le 0 <= r < len(
-00013790: 6e65 775f 6d61 7472 6978 293a 0a20 2020  new_matrix):.   
-000137a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137b0: 2069 6620 6e65 775f 6d61 7472 6978 5b72   if new_matrix[r
-000137c0: 5d5b 635d 203d 3d20 313a 0a20 2020 2020  ][c] == 1:.     
+000135a0: 2077 6869 6c65 2072 6f77 7320 2d20 6466   while rows - df
+000135b0: 735f 726f 7720 3c3d 2072 203c 3d20 726f  s_row <= r <= ro
+000135c0: 7773 202b 2031 2061 6e64 2070 7265 5f69  ws + 1 and pre_i
+000135d0: 6e64 6578 202d 2064 6673 5f63 6f6c 203c  ndex - dfs_col <
+000135e0: 3d20 6320 3c3d 206e 756d 5f69 6e64 6578  = c <= num_index
+000135f0: 202b 2064 6673 5f63 6f6c 3a0a 2020 2020   + dfs_col:.    
+00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013610: 2020 2020 6966 206e 6577 5f6d 6174 7269      if new_matri
+00013620: 785b 725d 5b63 5d20 3d3d 2031 3a0a 2020  x[r][c] == 1:.  
+00013630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013640: 2020 2020 2020 2020 2020 636f 756e 7420            count 
+00013650: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
+00013660: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00013670: 6973 5f62 616c 616e 6365 3a0a 2020 2020  is_balance:.    
+00013680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013690: 2020 2020 2020 2020 7220 2b3d 2064 720a          r += dr.
+000136a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136b0: 2020 2020 2020 2020 2020 2020 6320 2b3d              c +=
+000136c0: 2064 630a 2020 2020 2020 2020 2020 2020   dc.            
+000136d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000136e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000136f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00013700: 206d 6f76 655f 723a 0a20 2020 2020 2020   move_r:.       
+00013710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013720: 2020 2020 2020 2020 2069 6620 6e65 775f           if new_
+00013730: 6d61 7472 6978 5b72 5d5b 635d 203d 3d20  matrix[r][c] == 
+00013740: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013760: 2020 2020 2020 206d 6f76 655f 635f 636f         move_c_co
+00013770: 756e 7420 2b3d 2031 0a20 2020 2020 2020  unt += 1.       
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 2020 2020 2020 2020 2072 202b 3d20 6472           r += dr
+000137a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000137b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137c0: 206d 6f76 655f 7220 3d20 4661 6c73 650a   move_r = False.
 000137d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137e0: 2020 2063 6f75 6e74 202b 3d20 310a 2020     count += 1.  
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013820: 2320 4368 6563 6b20 6966 2074 6865 7265  # Check if there
-00013830: 2061 7265 206e 6f20 6765 6e65 7320 696e   are no genes in
-00013840: 2074 6865 2063 7572 7265 6e74 2063 6f6c   the current col
-00013850: 756d 6e20 696e 2074 6865 206f 7269 6769  umn in the origi
-00013860: 6e61 6c20 6d61 7472 6978 0a20 2020 2020  nal matrix.     
+000137e0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000137f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013810: 2020 6966 206e 6577 5f6d 6174 7269 785b    if new_matrix[
+00013820: 725d 5b63 5d20 3d3d 2031 3a0a 2020 2020  r][c] == 1:.    
+00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013850: 6d6f 7665 5f72 5f63 6f75 6e74 202b 3d20  move_r_count += 
+00013860: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
 00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013880: 2020 2069 6620 7375 6d28 6e65 775f 6d61     if sum(new_ma
-00013890: 7472 6978 5b72 6f77 5d5b 635d 2066 6f72  trix[row][c] for
-000138a0: 2072 6f77 2069 6e20 7261 6e67 6528 726f   row in range(ro
-000138b0: 7773 2929 203d 3d20 303a 0a20 2020 2020  ws)) == 0:.     
-000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138d0: 2020 2020 2020 2066 6974 6e65 7373 5f76         fitness_v
-000138e0: 616c 7565 202a 3d20 7365 6c66 2e66 6974  alue *= self.fit
-000138f0: 6e65 7373 5f70 6172 616d 735b 325d 0a20  ness_params[2]. 
-00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013910: 2020 2020 2020 2065 6c69 6620 636f 756e         elif coun
-00013920: 7420 3e20 313a 0a20 2020 2020 2020 2020  t > 1:.         
-00013930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013940: 2020 2066 6974 6e65 7373 5f76 616c 7565     fitness_value
-00013950: 202a 3d20 7365 6c66 2e66 6974 6e65 7373   *= self.fitness
-00013960: 5f70 6172 616d 735b 335d 0a20 2020 2020  _params[3].     
-00013970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013980: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139a0: 2020 2020 2066 6974 6e65 7373 5f76 616c       fitness_val
-000139b0: 7565 203d 2073 656c 662e 6669 746e 6573  ue = self.fitnes
-000139c0: 735f 7061 7261 6d73 5b34 5d0a 2020 2020  s_params[4].    
-000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139e0: 7220 2b3d 2064 720a 0a20 2020 2020 2020  r += dr..       
-000139f0: 2020 2020 2020 2020 2023 2041 646a 7573           # Adjus
-00013a00: 7420 6669 746e 6573 7320 6261 7365 6420  t fitness based 
-00013a10: 6f6e 2074 6865 2063 6f75 6e74 206f 6620  on the count of 
-00013a20: 7665 7274 6963 616c 2061 6c69 676e 6d65  vertical alignme
-00013a30: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00013a40: 2020 2020 6966 2063 6f75 6e74 2069 6e20      if count in 
-00013a50: 7261 6e67 6528 312c 2033 293a 0a20 2020  range(1, 3):.   
-00013a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a70: 2066 6974 6e65 7373 5f76 616c 7565 202a   fitness_value *
-00013a80: 3d20 7365 6c66 2e66 6974 6e65 7373 5f70  = self.fitness_p
-00013a90: 6172 616d 735b 355d 0a20 2020 2020 2020  arams[5].       
-00013aa0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00013ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ac0: 2020 2066 6974 6e65 7373 5f76 616c 7565     fitness_value
-00013ad0: 202a 3d20 7365 6c66 2e66 6974 6e65 7373   *= self.fitness
-00013ae0: 5f70 6172 616d 735b 365d 0a0a 2020 2020  _params[6]..    
-00013af0: 2020 2020 2020 2020 7072 655f 696e 6465          pre_inde
-00013b00: 7820 3d20 6e75 6d5f 696e 6465 7820 2023  x = num_index  #
-00013b10: 2055 7064 6174 6520 7072 6576 696f 7573   Update previous
-00013b20: 2069 6e64 6578 2066 6f72 2074 6865 206e   index for the n
-00013b30: 6578 7420 6765 6e65 0a0a 2020 2020 2020  ext gene..      
-00013b40: 2020 7265 7475 726e 2066 6974 6e65 7373    return fitness
-00013b50: 5f76 616c 7565 0a0a 2020 2020 6465 6620  _value..    def 
-00013b60: 746f 7572 6e61 6d65 6e74 5f73 656c 6563  tournament_selec
-00013b70: 7469 6f6e 2873 656c 6629 202d 3e20 6e70  tion(self) -> np
-00013b80: 2e6e 6461 7272 6179 3a0a 2020 2020 2020  .ndarray:.      
-00013b90: 2020 2222 220a 2020 2020 2020 2020 546f    """.        To
-00013ba0: 7572 6e61 6d65 6e74 2073 656c 6563 7469  urnament selecti
-00013bb0: 6f6e 206d 6574 686f 642e 2052 616e 646f  on method. Rando
-00013bc0: 6d6c 7920 7365 6c65 6374 7320 6b20 696e  mly selects k in
-00013bd0: 6469 7669 6475 616c 7320 6672 6f6d 2074  dividuals from t
-00013be0: 6865 2070 6f70 756c 6174 696f 6e0a 2020  he population.  
-00013bf0: 2020 2020 2020 616e 6420 7265 7475 726e        and return
-00013c00: 7320 7468 6520 696e 6469 7669 6475 616c  s the individual
-00013c10: 2077 6974 6820 7468 6520 6869 6768 6573   with the highes
-00013c20: 7420 6669 746e 6573 732e 0a0a 2020 2020  t fitness...    
-00013c30: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00013c40: 2020 2020 206e 702e 6e64 6172 7261 793a       np.ndarray:
-00013c50: 2054 6865 2069 6e64 6976 6964 7561 6c20   The individual 
-00013c60: 7769 7468 2074 6865 2068 6967 6865 7374  with the highest
-00013c70: 2066 6974 6e65 7373 2066 726f 6d20 7468   fitness from th
-00013c80: 6520 7365 6c65 6374 6564 2073 616d 706c  e selected sampl
-00013c90: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00013ca0: 2020 2020 2020 2023 2053 656c 6563 7420         # Select 
-00013cb0: 7468 6520 696e 6469 7669 6475 616c 2077  the individual w
-00013cc0: 6974 6820 7468 6520 6869 6768 6573 7420  ith the highest 
-00013cd0: 6669 746e 6573 7320 6672 6f6d 2061 2072  fitness from a r
-00013ce0: 616e 646f 6d20 7361 6d70 6c65 0a20 2020  andom sample.   
-00013cf0: 2020 2020 2073 656c 6563 7465 6420 3d20       selected = 
-00013d00: 6d61 7828 7261 6e64 6f6d 2e73 616d 706c  max(random.sampl
-00013d10: 6528 7365 6c66 2e70 6f70 756c 6174 696f  e(self.populatio
-00013d20: 6e2c 2073 656c 662e 746f 7572 6e61 6d65  n, self.tourname
-00013d30: 6e74 5f73 697a 6529 2c20 6b65 793d 6c61  nt_size), key=la
-00013d40: 6d62 6461 2069 6e64 3a20 3120 2f20 7365  mbda ind: 1 / se
-00013d50: 6c66 2e66 6974 6e65 7373 2869 6e64 2929  lf.fitness(ind))
-00013d60: 0a20 2020 2020 2020 2023 2053 6f72 7420  .        # Sort 
-00013d70: 7468 6520 7365 6c65 6374 6564 2069 6e64  the selected ind
-00013d80: 6976 6964 7561 6c20 666f 7220 636f 6e73  ividual for cons
-00013d90: 6973 7465 6e63 790a 2020 2020 2020 2020  istency.        
-00013da0: 736f 7274 6564 5f73 656c 6563 7465 6420  sorted_selected 
-00013db0: 3d20 6e70 2e73 6f72 7428 7365 6c65 6374  = np.sort(select
-00013dc0: 6564 290a 2020 2020 2020 2020 7265 7475  ed).        retu
-00013dd0: 726e 2073 6f72 7465 645f 7365 6c65 6374  rn sorted_select
-00013de0: 6564 0a0a 2020 2020 6465 6620 6372 6f73  ed..    def cros
-00013df0: 736f 7665 7228 7365 6c66 2c20 7061 7265  sover(self, pare
-00013e00: 6e74 313a 206e 702e 6e64 6172 7261 792c  nt1: np.ndarray,
-00013e10: 2070 6172 656e 7432 3a20 6e70 2e6e 6461   parent2: np.nda
-00013e20: 7272 6179 2920 2d3e 206e 702e 6e64 6172  rray) -> np.ndar
-00013e30: 7261 793a 0a20 2020 2020 2020 2022 2222  ray:.        """
-00013e40: 0a20 2020 2020 2020 2054 776f 2d70 6f69  .        Two-poi
-00013e50: 6e74 2063 726f 7373 6f76 6572 2e20 5261  nt crossover. Ra
-00013e60: 6e64 6f6d 6c79 2073 656c 6563 7473 2074  ndomly selects t
-00013e70: 776f 2070 6f69 6e74 7320 616e 6420 7377  wo points and sw
-00013e80: 6170 7320 7468 6520 6765 6e65 7320 6265  aps the genes be
-00013e90: 7477 6565 6e20 7468 6520 7477 6f20 7061  tween the two pa
-00013ea0: 7265 6e74 730a 2020 2020 2020 2020 746f  rents.        to
-00013eb0: 2063 7265 6174 6520 6120 6368 696c 642e   create a child.
-00013ec0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00013ed0: 2020 2020 2020 2020 7061 7265 6e74 3120          parent1 
-00013ee0: 286e 702e 6e64 6172 7261 7929 3a20 5468  (np.ndarray): Th
-00013ef0: 6520 6669 7273 7420 7061 7265 6e74 2e0a  e first parent..
-00013f00: 2020 2020 2020 2020 7061 7265 6e74 3220          parent2 
-00013f10: 286e 702e 6e64 6172 7261 7929 3a20 5468  (np.ndarray): Th
-00013f20: 6520 7365 636f 6e64 2070 6172 656e 742e  e second parent.
-00013f30: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00013f40: 733a 0a20 2020 2020 2020 206e 702e 6e64  s:.        np.nd
-00013f50: 6172 7261 793a 2054 6865 2063 6869 6c64  array: The child
-00013f60: 2063 7265 6174 6564 2062 7920 6372 6f73   created by cros
-00013f70: 736f 7665 722e 0a20 2020 2020 2020 2022  sover..        "
-00013f80: 2222 0a20 2020 2020 2020 2023 2052 616e  "".        # Ran
-00013f90: 646f 6d6c 7920 7365 6c65 6374 2074 776f  domly select two
-00013fa0: 2070 6f69 6e74 7320 666f 7220 6372 6f73   points for cros
-00013fb0: 736f 7665 720a 2020 2020 2020 2020 706f  sover.        po
-00013fc0: 696e 7473 203d 2073 6f72 7465 6428 7261  ints = sorted(ra
-00013fd0: 6e64 6f6d 2e73 616d 706c 6528 7261 6e67  ndom.sample(rang
-00013fe0: 6528 302c 2073 656c 662e 6e75 6d5f 6765  e(0, self.num_ge
-00013ff0: 6e65 7329 2c20 3229 290a 2020 2020 2020  nes), 2)).      
-00014000: 2020 2320 4372 6561 7465 206e 6577 2063    # Create new c
-00014010: 6869 6c64 2062 7920 636f 6d62 696e 696e  hild by combinin
-00014020: 6720 7061 7274 7320 6f66 2062 6f74 6820  g parts of both 
-00014030: 7061 7265 6e74 730a 2020 2020 2020 2020  parents.        
-00014040: 7265 7475 726e 206e 702e 636f 6e63 6174  return np.concat
-00014050: 656e 6174 6528 5b70 6172 656e 7431 5b3a  enate([parent1[:
-00014060: 706f 696e 7473 5b30 5d5d 2c20 7061 7265  points[0]], pare
-00014070: 6e74 325b 706f 696e 7473 5b30 5d3a 706f  nt2[points[0]:po
-00014080: 696e 7473 5b31 5d5d 2c20 7061 7265 6e74  ints[1]], parent
-00014090: 315b 706f 696e 7473 5b31 5d3a 5d5d 290a  1[points[1]:]]).
-000140a0: 0a20 2020 2064 6566 206d 7574 6174 6528  .    def mutate(
-000140b0: 7365 6c66 2c20 696e 6469 7669 6475 616c  self, individual
-000140c0: 3a20 6e70 2e6e 6461 7272 6179 2920 2d3e  : np.ndarray) ->
-000140d0: 206e 702e 6e64 6172 7261 793a 0a20 2020   np.ndarray:.   
-000140e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000140f0: 204d 7574 6174 696f 6e20 6f70 6572 6174   Mutation operat
-00014100: 696f 6e2e 204d 7574 6174 6573 2061 6e20  ion. Mutates an 
-00014110: 696e 6469 7669 6475 616c 2773 2067 656e  individual's gen
-00014120: 6520 7769 7468 2061 2063 6572 7461 696e  e with a certain
-00014130: 2070 726f 6261 6269 6c69 7479 2e0a 0a20   probability... 
-00014140: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00014150: 2020 2020 2069 6e64 6976 6964 7561 6c20       individual 
-00014160: 286e 702e 6e64 6172 7261 7929 3a20 5468  (np.ndarray): Th
-00014170: 6520 696e 6469 7669 6475 616c 2074 6f20  e individual to 
-00014180: 6d75 7461 7465 2e0a 0a20 2020 2020 2020  mutate...       
-00014190: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-000141a0: 2020 6e70 2e6e 6461 7272 6179 3a20 5468    np.ndarray: Th
-000141b0: 6520 6d75 7461 7465 6420 696e 6469 7669  e mutated indivi
-000141c0: 6475 616c 2e0a 2020 2020 2020 2020 2222  dual..        ""
-000141d0: 220a 2020 2020 2020 2020 2320 4d75 7461  ".        # Muta
-000141e0: 7465 2061 2067 656e 6520 7769 7468 2061  te a gene with a
-000141f0: 2067 6976 656e 2070 726f 6261 6269 6c69   given probabili
-00014200: 7479 0a20 2020 2020 2020 2069 6620 7261  ty.        if ra
-00014210: 6e64 6f6d 2e72 616e 646f 6d28 2920 3c20  ndom.random() < 
-00014220: 7365 6c66 2e6d 7574 6174 696f 6e5f 7261  self.mutation_ra
-00014230: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
-00014240: 696e 6465 7820 3d20 7261 6e64 6f6d 2e72  index = random.r
-00014250: 616e 6469 6e74 2830 2c20 6c65 6e28 696e  andint(0, len(in
-00014260: 6469 7669 6475 616c 2920 2d20 3129 0a20  dividual) - 1). 
-00014270: 2020 2020 2020 2020 2020 2069 6e64 6976             indiv
-00014280: 6964 7561 6c5b 696e 6465 785d 203d 2072  idual[index] = r
-00014290: 616e 646f 6d2e 6368 6f69 6365 2873 656c  andom.choice(sel
-000142a0: 662e 6461 7461 290a 2020 2020 2020 2020  f.data).        
-000142b0: 2320 5265 7475 726e 2074 6865 2073 6f72  # Return the sor
-000142c0: 7465 6420 696e 6469 7669 6475 616c 0a20  ted individual. 
-000142d0: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
-000142e0: 2e73 6f72 7428 696e 6469 7669 6475 616c  .sort(individual
-000142f0: 290a 0a20 2020 2064 6566 2067 656e 6574  )..    def genet
-00014300: 6963 2873 656c 6629 202d 3e20 6c69 7374  ic(self) -> list
-00014310: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00014320: 2020 2020 2020 4d61 696e 206c 6f6f 7020        Main loop 
-00014330: 6f66 2074 6865 2067 656e 6574 6963 2061  of the genetic a
-00014340: 6c67 6f72 6974 686d 2e20 5065 7266 6f72  lgorithm. Perfor
-00014350: 6d73 2067 656e 6574 6963 206f 7065 7261  ms genetic opera
-00014360: 7469 6f6e 7320 6f76 6572 206d 756c 7469  tions over multi
-00014370: 706c 6520 6765 6e65 7261 7469 6f6e 730a  ple generations.
-00014380: 2020 2020 2020 2020 746f 2066 696e 6420          to find 
-00014390: 7468 6520 6f70 7469 6d61 6c20 736f 6c75  the optimal solu
-000143a0: 7469 6f6e 2e0a 0a20 2020 2020 2020 2052  tion...        R
-000143b0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000143c0: 6e70 2e6e 6461 7272 6179 3a20 5468 6520  np.ndarray: The 
-000143d0: 6265 7374 2069 6e64 6976 6964 7561 6c20  best individual 
-000143e0: 666f 756e 6420 6166 7465 7220 616c 6c20  found after all 
-000143f0: 6765 6e65 7261 7469 6f6e 732e 0a20 2020  generations..   
-00014400: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014410: 2023 2049 7465 7261 7465 206f 7665 7220   # Iterate over 
-00014420: 6d75 6c74 6970 6c65 2067 656e 6572 6174  multiple generat
-00014430: 696f 6e73 0a20 2020 2020 2020 2066 6f72  ions.        for
-00014440: 205f 2069 6e20 7261 6e67 6528 7365 6c66   _ in range(self
-00014450: 2e65 706f 6368 5f63 6f75 6e74 293a 0a20  .epoch_count):. 
-00014460: 2020 2020 2020 2020 2020 206e 6577 5f70             new_p
-00014470: 6f70 756c 6174 696f 6e20 3d20 5b5d 0a20  opulation = []. 
-00014480: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
-00014490: 2069 6e20 7261 6e67 6528 7365 6c66 2e70   in range(self.p
-000144a0: 6f70 756c 6174 696f 6e5f 7369 7a65 202f  opulation_size /
-000144b0: 2f20 3229 3a0a 2020 2020 2020 2020 2020  / 2):.          
-000144c0: 2020 2020 2020 2320 5365 6c65 6374 2070        # Select p
-000144d0: 6172 656e 7473 2061 6e64 2063 7265 6174  arents and creat
-000144e0: 6520 6368 696c 6472 656e 0a20 2020 2020  e children.     
-000144f0: 2020 2020 2020 2020 2020 2070 6172 656e             paren
-00014500: 7431 203d 2073 656c 662e 746f 7572 6e61  t1 = self.tourna
-00014510: 6d65 6e74 5f73 656c 6563 7469 6f6e 2829  ment_selection()
-00014520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014530: 2070 6172 656e 7432 203d 2073 656c 662e   parent2 = self.
-00014540: 746f 7572 6e61 6d65 6e74 5f73 656c 6563  tournament_selec
-00014550: 7469 6f6e 2829 0a20 2020 2020 2020 2020  tion().         
-00014560: 2020 2020 2020 2063 6869 6c64 3120 3d20         child1 = 
-00014570: 7365 6c66 2e63 726f 7373 6f76 6572 2870  self.crossover(p
-00014580: 6172 656e 7431 2c20 7061 7265 6e74 3229  arent1, parent2)
-00014590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000145a0: 2063 6869 6c64 3220 3d20 7365 6c66 2e63   child2 = self.c
-000145b0: 726f 7373 6f76 6572 2870 6172 656e 7431  rossover(parent1
-000145c0: 2c20 7061 7265 6e74 3229 0a20 2020 2020  , parent2).     
-000145d0: 2020 2020 2020 2020 2020 2023 204d 7574             # Mut
-000145e0: 6174 6520 6368 696c 6472 656e 2061 6e64  ate children and
-000145f0: 2061 6464 2074 6f20 6e65 7720 706f 7075   add to new popu
-00014600: 6c61 7469 6f6e 0a20 2020 2020 2020 2020  lation.         
-00014610: 2020 2020 2020 206e 6577 5f70 6f70 756c         new_popul
-00014620: 6174 696f 6e2e 6578 7465 6e64 285b 7365  ation.extend([se
-00014630: 6c66 2e6d 7574 6174 6528 6368 696c 6431  lf.mutate(child1
-00014640: 292c 2073 656c 662e 6d75 7461 7465 2863  ), self.mutate(c
-00014650: 6869 6c64 3229 5d29 0a20 2020 2020 2020  hild2)]).       
-00014660: 2020 2020 2023 2055 7064 6174 6520 706f       # Update po
-00014670: 7075 6c61 7469 6f6e 0a20 2020 2020 2020  pulation.       
-00014680: 2020 2020 2073 656c 662e 706f 7075 6c61       self.popula
-00014690: 7469 6f6e 203d 206e 6577 5f70 6f70 756c  tion = new_popul
-000146a0: 6174 696f 6e0a 0a20 2020 2020 2020 2023  ation..        #
-000146b0: 2046 696e 6420 616e 6420 7265 7475 726e   Find and return
-000146c0: 2074 6865 2062 6573 7420 696e 6469 7669   the best indivi
-000146d0: 6475 616c 2062 6173 6564 206f 6e20 6669  dual based on fi
-000146e0: 746e 6573 730a 2020 2020 2020 2020 6265  tness.        be
-000146f0: 7374 5f69 6e64 6976 6964 7561 6c20 3d20  st_individual = 
-00014700: 6d69 6e28 5b6c 6973 7428 6974 656d 2920  min([list(item) 
-00014710: 666f 7220 6974 656d 2069 6e20 7365 6c66  for item in self
-00014720: 2e70 6f70 756c 6174 696f 6e5d 2c20 6b65  .population], ke
-00014730: 793d 7365 6c66 2e66 6974 6e65 7373 290a  y=self.fitness).
-00014740: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-00014750: 6573 745f 696e 6469 7669 6475 616c 0a0a  est_individual..
-00014760: 0a63 6c61 7373 2052 616e 646f 6d46 6f72  .class RandomFor
-00014770: 6573 7452 6567 7265 7373 6f72 5472 616e  estRegressorTran
-00014780: 7366 6f72 6d65 7228 4261 7365 4573 7469  sformer(BaseEsti
-00014790: 6d61 746f 722c 2054 7261 6e73 666f 726d  mator, Transform
-000147a0: 6572 4d69 7869 6e29 3a0a 2020 2020 6465  erMixin):.    de
-000147b0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-000147c0: 206d 6f64 656c 3a20 5261 6e64 6f6d 466f   model: RandomFo
-000147d0: 7265 7374 5265 6772 6573 736f 7229 3a0a  restRegressor):.
-000147e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000147f0: 2020 2020 496e 6974 6961 6c69 7a65 2074      Initialize t
-00014800: 6865 2074 7261 6e73 666f 726d 6572 2077  he transformer w
-00014810: 6974 6820 6120 5261 6e64 6f6d 466f 7265  ith a RandomFore
-00014820: 7374 5265 6772 6573 736f 7220 6d6f 6465  stRegressor mode
-00014830: 6c20 616e 6420 6120 5374 616e 6461 7264  l and a Standard
-00014840: 5363 616c 6572 2066 6f72 2066 6561 7475  Scaler for featu
-00014850: 7265 2073 6361 6c69 6e67 2e0a 0a20 2020  re scaling...   
-00014860: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
-00014870: 0a20 2020 2020 2020 206d 6f64 656c 2028  .        model (
-00014880: 5261 6e64 6f6d 466f 7265 7374 5265 6772  RandomForestRegr
-00014890: 6573 736f 7229 3a20 5468 6520 5261 6e64  essor): The Rand
-000148a0: 6f6d 466f 7265 7374 5265 6772 6573 736f  omForestRegresso
-000148b0: 7220 6d6f 6465 6c20 746f 2062 6520 7573  r model to be us
-000148c0: 6564 2066 6f72 2070 7265 6469 6374 696f  ed for predictio
-000148d0: 6e73 2e0a 2020 2020 2020 2020 2222 220a  ns..        """.
-000148e0: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-000148f0: 6375 6c61 7465 5f75 7469 6c20 3d20 4361  culate_util = Ca
-00014900: 6c63 756c 6174 6555 7469 6c0a 2020 2020  lculateUtil.    
-00014910: 2020 2020 7365 6c66 2e6d 6f64 656c 5f75      self.model_u
-00014920: 7469 6c20 3d20 4d6f 6465 6c55 7469 6c0a  til = ModelUtil.
-00014930: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
-00014940: 656c 203d 206d 6f64 656c 0a20 2020 2020  el = model.     
-00014950: 2020 2073 656c 662e 7363 616c 6572 203d     self.scaler =
-00014960: 2053 7461 6e64 6172 6453 6361 6c65 7228   StandardScaler(
-00014970: 290a 0a20 2020 2064 6566 2066 6974 2873  )..    def fit(s
-00014980: 656c 662c 2058 3a20 6e70 2e6e 6461 7272  elf, X: np.ndarr
-00014990: 6179 2c20 793a 204f 7074 696f 6e61 6c5b  ay, y: Optional[
-000149a0: 6e70 2e6e 6461 7272 6179 5d20 3d20 4e6f  np.ndarray] = No
-000149b0: 6e65 2920 2d3e 2027 5261 6e64 6f6d 466f  ne) -> 'RandomFo
-000149c0: 7265 7374 5265 6772 6573 736f 7254 7261  restRegressorTra
-000149d0: 6e73 666f 726d 6572 273a 0a20 2020 2020  nsformer':.     
-000149e0: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
-000149f0: 6974 2074 6865 2052 616e 646f 6d46 6f72  it the RandomFor
-00014a00: 6573 7420 6d6f 6465 6c20 616e 6420 7468  est model and th
-00014a10: 6520 7363 616c 6572 206f 6e20 7468 6520  e scaler on the 
-00014a20: 7472 6169 6e69 6e67 2064 6174 612e 0a0a  training data...
-00014a30: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00014a40: 7273 3a0a 2020 2020 2020 2020 5820 286e  rs:.        X (n
-00014a50: 702e 6e64 6172 7261 7929 3a20 5472 6169  p.ndarray): Trai
-00014a60: 6e69 6e67 2064 6174 6120 6665 6174 7572  ning data featur
-00014a70: 6573 2e0a 2020 2020 2020 2020 7920 284f  es..        y (O
-00014a80: 7074 696f 6e61 6c5b 6e70 2e6e 6461 7272  ptional[np.ndarr
-00014a90: 6179 5d29 3a20 5472 6169 6e69 6e67 2064  ay]): Training d
-00014aa0: 6174 6120 6c61 6265 6c73 2e0a 0a20 2020  ata labels...   
-00014ab0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00014ac0: 2020 2020 2020 5261 6e64 6f6d 466f 7265        RandomFore
-00014ad0: 7374 5265 6772 6573 736f 7254 7261 6e73  stRegressorTrans
-00014ae0: 666f 726d 6572 3a20 5468 6520 696e 7374  former: The inst
-00014af0: 616e 6365 206f 6620 7468 6973 2074 7261  ance of this tra
-00014b00: 6e73 666f 726d 6572 2e0a 2020 2020 2020  nsformer..      
-00014b10: 2020 2222 220a 2020 2020 2020 2020 585f    """.        X_
-00014b20: 7363 616c 6564 203d 2073 656c 662e 7363  scaled = self.sc
-00014b30: 616c 6572 2e66 6974 5f74 7261 6e73 666f  aler.fit_transfo
-00014b40: 726d 2858 290a 2020 2020 2020 2020 7365  rm(X).        se
-00014b50: 6c66 2e6d 6f64 656c 2e66 6974 2858 5f73  lf.model.fit(X_s
-00014b60: 6361 6c65 642c 2079 290a 2020 2020 2020  caled, y).      
-00014b70: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
-00014b80: 2020 2064 6566 2074 7261 6e73 666f 726d     def transform
-00014b90: 2873 656c 662c 2058 3a20 6e70 2e6e 6461  (self, X: np.nda
-00014ba0: 7272 6179 2920 2d3e 206e 702e 6e64 6172  rray) -> np.ndar
-00014bb0: 7261 793a 0a20 2020 2020 2020 2022 2222  ray:.        """
-00014bc0: 0a20 2020 2020 2020 2054 7261 6e73 666f  .        Transfo
-00014bd0: 726d 2074 6865 2069 6e70 7574 2064 6174  rm the input dat
-00014be0: 6120 6279 2073 6361 6c69 6e67 2c20 6d61  a by scaling, ma
-00014bf0: 6b69 6e67 2070 7265 6469 6374 696f 6e73  king predictions
-00014c00: 2c20 616e 6420 6361 6c63 756c 6174 696e  , and calculatin
-00014c10: 6720 7065 722d 726f 7720 7374 6174 6973  g per-row statis
-00014c20: 7469 6373 2e0a 0a20 2020 2020 2020 2050  tics...        P
-00014c30: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-00014c40: 2020 2058 2028 6e70 2e6e 6461 7272 6179     X (np.ndarray
-00014c50: 293a 2044 6174 6120 746f 2074 7261 6e73  ): Data to trans
-00014c60: 666f 726d 2e0a 0a20 2020 2020 2020 2052  form...        R
-00014c70: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00014c80: 6e70 2e6e 6461 7272 6179 3a20 5472 616e  np.ndarray: Tran
-00014c90: 7366 6f72 6d65 6420 6461 7461 2069 6e63  sformed data inc
-00014ca0: 6c75 6469 6e67 206c 6173 7420 656c 656d  luding last elem
-00014cb0: 656e 7473 2c20 7072 6564 6963 7469 6f6e  ents, prediction
-00014cc0: 732c 2073 7461 6e64 6172 6420 6465 7669  s, standard devi
-00014cd0: 6174 696f 6e73 2c20 616e 6420 5253 4920  ations, and RSI 
-00014ce0: 7661 6c75 6573 2e0a 2020 2020 2020 2020  values..        
-00014cf0: 2222 220a 2020 2020 2020 2020 585f 7363  """.        X_sc
-00014d00: 616c 6564 203d 2073 656c 662e 7363 616c  aled = self.scal
-00014d10: 6572 2e74 7261 6e73 666f 726d 2858 290a  er.transform(X).
-00014d20: 2020 2020 2020 2020 7072 6564 6963 7469          predicti
-00014d30: 6f6e 7320 3d20 7365 6c66 2e6d 6f64 656c  ons = self.model
-00014d40: 2e70 7265 6469 6374 2858 5f73 6361 6c65  .predict(X_scale
-00014d50: 6429 0a0a 2020 2020 2020 2020 2320 4361  d)..        # Ca
-00014d60: 6c63 756c 6174 6520 7374 616e 6461 7264  lculate standard
-00014d70: 2064 6576 6961 7469 6f6e 2061 6e64 2052   deviation and R
-00014d80: 5349 2066 6f72 2065 6163 6820 726f 770a  SI for each row.
-00014d90: 2020 2020 2020 2020 7364 5f70 6572 5f72          sd_per_r
-00014da0: 6f77 203d 206e 702e 6172 7261 7928 5b73  ow = np.array([s
-00014db0: 656c 662e 6361 6c63 756c 6174 655f 7574  elf.calculate_ut
-00014dc0: 696c 2e63 616c 6375 6c61 7465 5f73 7461  il.calculate_sta
-00014dd0: 6e64 6172 645f 6465 7669 6174 696f 6e5f  ndard_deviation_
-00014de0: 7765 6c66 6f72 6428 726f 7729 2066 6f72  welford(row) for
-00014df0: 2072 6f77 2069 6e20 585d 290a 2020 2020   row in X]).    
-00014e00: 2020 2020 7273 695f 7065 725f 726f 7720      rsi_per_row 
-00014e10: 3d20 6e70 2e61 7272 6179 285b 7365 6c66  = np.array([self
-00014e20: 2e6d 6f64 656c 5f75 7469 6c2e 7265 6c61  .model_util.rela
-00014e30: 7469 7665 5f73 7472 656e 6774 685f 696e  tive_strength_in
-00014e40: 6465 7828 726f 772c 2070 6572 696f 643d  dex(row, period=
-00014e50: 6c65 6e28 726f 7729 202f 2f20 3229 2066  len(row) // 2) f
-00014e60: 6f72 2072 6f77 2069 6e20 585d 290a 0a20  or row in X]).. 
-00014e70: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
-00014e80: 2074 6865 206c 6173 7420 656c 656d 656e   the last elemen
-00014e90: 7420 6672 6f6d 2065 6163 6820 726f 770a  t from each row.
-00014ea0: 2020 2020 2020 2020 6c61 7374 5f65 6c65          last_ele
-00014eb0: 6d65 6e74 7320 3d20 585b 3a2c 202d 315d  ments = X[:, -1]
-00014ec0: 0a0a 2020 2020 2020 2020 2320 436f 6d62  ..        # Comb
-00014ed0: 696e 6520 616c 6c20 7468 6520 636f 6d70  ine all the comp
-00014ee0: 7574 6564 2066 6561 7475 7265 7320 696e  uted features in
-00014ef0: 746f 2061 2073 696e 676c 6520 6172 7261  to a single arra
-00014f00: 790a 2020 2020 2020 2020 7472 616e 7366  y.        transf
-00014f10: 6f72 6d65 645f 6461 7461 203d 206e 702e  ormed_data = np.
-00014f20: 635f 5b6c 6173 745f 656c 656d 656e 7473  c_[last_elements
-00014f30: 2c20 7072 6564 6963 7469 6f6e 732c 2073  , predictions, s
-00014f40: 645f 7065 725f 726f 772c 2072 7369 5f70  d_per_row, rsi_p
-00014f50: 6572 5f72 6f77 5d0a 2020 2020 2020 2020  er_row].        
-00014f60: 7265 7475 726e 2074 7261 6e73 666f 726d  return transform
-00014f70: 6564 5f64 6174 610a 0a0a 6966 205f 5f6e  ed_data...if __n
-00014f80: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-00014f90: 5f5f 273a 0a20 2020 2070 6173 730a       __':.    pass.
+00013880: 2020 6320 2b3d 2064 630a 2020 2020 2020    c += dc.      
+00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138a0: 2020 2020 2020 2020 2020 6d6f 7665 5f72            move_r
+000138b0: 203d 2054 7275 650a 0a20 2020 2020 2020   = True..       
+000138c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000138d0: 6973 5f62 616c 616e 6365 2061 6e64 2063  is_balance and c
+000138e0: 6f75 6e74 203d 3d20 7461 7267 6574 3a0a  ount == target:.
+000138f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013900: 2020 2020 2020 2020 6669 746e 6573 735f          fitness_
+00013910: 7661 6c75 6520 2a3d 2030 2e31 2020 2320  value *= 0.1  # 
+00013920: 4465 6372 6561 7365 2066 6974 6e65 7373  Decrease fitness
+00013930: 2069 6620 6120 6261 6c61 6e63 6564 2064   if a balanced d
+00013940: 6961 676f 6e61 6c20 6973 2066 6f75 6e64  iagonal is found
+00013950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013960: 2020 2020 2065 6c69 6620 6e6f 7420 6973       elif not is
+00013970: 5f62 616c 616e 6365 2061 6e64 206d 6178  _balance and max
+00013980: 286d 6f76 655f 725f 636f 756e 742c 206d  (move_r_count, m
+00013990: 6f76 655f 635f 636f 756e 7429 203d 3d20  ove_c_count) == 
+000139a0: 7461 7267 6574 202d 2031 3a0a 2020 2020  target - 1:.    
+000139b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139c0: 2020 2020 6669 746e 6573 735f 7661 6c75      fitness_valu
+000139d0: 6520 2a3d 2030 2e33 2020 2320 4465 6372  e *= 0.3  # Decr
+000139e0: 6561 7365 2066 6974 6e65 7373 2069 6620  ease fitness if 
+000139f0: 616e 2075 6e62 616c 616e 6365 6420 6469  an unbalanced di
+00013a00: 6167 6f6e 616c 2069 7320 666f 756e 640a  agonal is found.
+00013a10: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
+00013a20: 5f69 6e64 6578 203d 206e 756d 5f69 6e64  _index = num_ind
+00013a30: 6578 2020 2320 5570 6461 7465 2070 7265  ex  # Update pre
+00013a40: 7669 6f75 7320 696e 6465 7820 666f 7220  vious index for 
+00013a50: 7468 6520 6e65 7874 2067 656e 650a 0a20  the next gene.. 
+00013a60: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
+00013a70: 746e 6573 735f 7661 6c75 650a 0a20 2020  tness_value..   
+00013a80: 2064 6566 2063 6865 636b 5f76 6572 7469   def check_verti
+00013a90: 6361 6c28 7365 6c66 2c20 696e 6469 7669  cal(self, indivi
+00013aa0: 6475 616c 3a20 6c69 7374 2920 2d3e 2066  dual: list) -> f
+00013ab0: 6c6f 6174 3a0a 2020 2020 2020 2020 2222  loat:.        ""
+00013ac0: 220a 2020 2020 2020 2020 4368 6563 6b73  ".        Checks
+00013ad0: 2076 6572 7469 6361 6c20 616c 6967 6e6d   vertical alignm
+00013ae0: 656e 7473 2069 6e20 6120 6479 6e61 6d69  ents in a dynami
+00013af0: 6361 6c6c 7920 7570 6461 7465 6420 6d61  cally updated ma
+00013b00: 7472 6978 2062 6173 6564 206f 6e20 7468  trix based on th
+00013b10: 6520 696e 6469 7669 6475 616c 2773 2067  e individual's g
+00013b20: 656e 6573 0a20 2020 2020 2020 2061 6e64  enes.        and
+00013b30: 2065 7661 6c75 6174 6573 2074 6865 6972   evaluates their
+00013b40: 2066 6974 6e65 7373 2062 6173 6564 206f   fitness based o
+00013b50: 6e20 7468 6520 616c 6967 6e6d 656e 742e  n the alignment.
+00013b60: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00013b70: 2020 2020 2020 2020 696e 6469 7669 6475          individu
+00013b80: 616c 2028 6c69 7374 293a 204c 6973 7420  al (list): List 
+00013b90: 6f66 2067 656e 6520 696e 6469 6365 7320  of gene indices 
+00013ba0: 7265 7072 6573 656e 7469 6e67 2061 6e20  representing an 
+00013bb0: 696e 6469 7669 6475 616c 2069 6e20 7468  individual in th
+00013bc0: 6520 706f 7075 6c61 7469 6f6e 2e0a 0a20  e population... 
+00013bd0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00013be0: 2020 2020 2020 2020 666c 6f61 743a 2041          float: A
+00013bf0: 2066 6974 6e65 7373 2076 616c 7565 206d   fitness value m
+00013c00: 6f64 6966 6965 6420 6261 7365 6420 6f6e  odified based on
+00013c10: 2074 6865 2070 7265 7365 6e63 6520 6f66   the presence of
+00013c20: 2076 6572 7469 6361 6c20 616c 6967 6e6d   vertical alignm
+00013c30: 656e 7473 2e0a 2020 2020 2020 2020 2222  ents..        ""
+00013c40: 220a 2020 2020 2020 2020 6669 746e 6573  ".        fitnes
+00013c50: 735f 7661 6c75 6520 3d20 310a 2020 2020  s_value = 1.    
+00013c60: 2020 2020 7072 655f 696e 6465 7820 3d20      pre_index = 
+00013c70: 696e 6469 7669 6475 616c 5b30 5d20 2d20  individual[0] - 
+00013c80: 3120 2023 2050 7265 7669 6f75 7320 696e  1  # Previous in
+00013c90: 6465 782c 2075 6e75 7365 6420 696e 2076  dex, unused in v
+00013ca0: 6572 7469 6361 6c20 6368 6563 6b69 6e67  ertical checking
+00013cb0: 0a0a 2020 2020 2020 2020 666f 7220 696e  ..        for in
+00013cc0: 6469 2069 6e20 696e 6469 7669 6475 616c  di in individual
+00013cd0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00013ce0: 206e 6f74 2028 7365 6c66 2e6d 696e 5f6e   not (self.min_n
+00013cf0: 756d 203c 3d20 696e 6469 203c 3d20 7365  um <= indi <= se
+00013d00: 6c66 2e6d 6178 5f6e 756d 293a 0a20 2020  lf.max_num):.   
+00013d10: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00013d20: 7572 6e20 3120 2023 2052 6574 7572 6e20  urn 1  # Return 
+00013d30: 6120 6465 6661 756c 7420 6669 746e 6573  a default fitnes
+00013d40: 7320 7661 6c75 6520 6966 2067 656e 6520  s value if gene 
+00013d50: 6973 206f 7574 206f 6620 7661 6c69 6420  is out of valid 
+00013d60: 7261 6e67 650a 0a20 2020 2020 2020 2020  range..         
+00013d70: 2020 206e 756d 5f69 6e64 6578 203d 2069     num_index = i
+00013d80: 6e64 6920 2d20 310a 2020 2020 2020 2020  ndi - 1.        
+00013d90: 2020 2020 726f 7773 203d 206c 656e 2873      rows = len(s
+00013da0: 656c 662e 7265 6665 7273 5f6d 6174 7269  elf.refers_matri
+00013db0: 7829 0a0a 2020 2020 2020 2020 2020 2020  x)..            
+00013dc0: 2320 4372 6561 7465 2061 206e 6577 206d  # Create a new m
+00013dd0: 6174 7269 7820 696e 636c 7564 696e 6720  atrix including 
+00013de0: 6120 6e65 7720 726f 7720 666f 7220 7468  a new row for th
+00013df0: 6520 6375 7272 656e 7420 6765 6e65 0a20  e current gene. 
+00013e00: 2020 2020 2020 2020 2020 206e 6577 5f6d             new_m
+00013e10: 6174 7269 7820 3d20 5b72 6f77 5b3a 5d20  atrix = [row[:] 
+00013e20: 666f 7220 726f 7720 696e 2073 656c 662e  for row in self.
+00013e30: 7265 6665 7273 5f6d 6174 7269 785d 2020  refers_matrix]  
+00013e40: 2320 436f 7079 2074 6865 2065 7869 7374  # Copy the exist
+00013e50: 696e 6720 6d61 7472 6978 0a20 2020 2020  ing matrix.     
+00013e60: 2020 2020 2020 206e 6577 5f72 6f77 203d         new_row =
+00013e70: 205b 305d 202a 2073 656c 662e 6d61 785f   [0] * self.max_
+00013e80: 6e75 6d0a 2020 2020 2020 2020 2020 2020  num.            
+00013e90: 6e65 775f 726f 775b 6e75 6d5f 696e 6465  new_row[num_inde
+00013ea0: 785d 203d 2031 0a20 2020 2020 2020 2020  x] = 1.         
+00013eb0: 2020 206e 6577 5f6d 6174 7269 782e 6170     new_matrix.ap
+00013ec0: 7065 6e64 286e 6577 5f72 6f77 2920 2023  pend(new_row)  #
+00013ed0: 2041 6464 2074 6865 206e 6577 2072 6f77   Add the new row
+00013ee0: 2063 6f72 7265 6374 6c79 0a0a 2020 2020   correctly..    
+00013ef0: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+00013f00: 7665 7274 6963 616c 2061 6c69 676e 6d65  vertical alignme
+00013f10: 6e74 0a20 2020 2020 2020 2020 2020 2066  nt.            f
+00013f20: 6f72 2064 7220 696e 205b 2d31 5d3a 2020  or dr in [-1]:  
+00013f30: 2320 4f6e 6c79 206e 6565 6420 746f 2063  # Only need to c
+00013f40: 6865 636b 2074 6865 2075 7077 6172 6420  heck the upward 
+00013f50: 7665 7274 6963 616c 206c 696e 650a 2020  vertical line.  
+00013f60: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00013f70: 756e 7420 3d20 300a 2020 2020 2020 2020  unt = 0.        
+00013f80: 2020 2020 2020 2020 722c 2063 203d 2072          r, c = r
+00013f90: 6f77 732c 206e 756d 5f69 6e64 6578 0a20  ows, num_index. 
+00013fa0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00013fb0: 6869 6c65 2030 203c 3d20 7220 3c20 6c65  hile 0 <= r < le
+00013fc0: 6e28 6e65 775f 6d61 7472 6978 293a 0a20  n(new_matrix):. 
+00013fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fe0: 2020 2069 6620 6e65 775f 6d61 7472 6978     if new_matrix
+00013ff0: 5b72 5d5b 635d 203d 3d20 313a 0a20 2020  [r][c] == 1:.   
+00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014010: 2020 2020 2063 6f75 6e74 202b 3d20 310a       count += 1.
+00014020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014030: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014050: 2020 2320 4368 6563 6b20 6966 2074 6865    # Check if the
+00014060: 7265 2061 7265 206e 6f20 6765 6e65 7320  re are no genes 
+00014070: 696e 2074 6865 2063 7572 7265 6e74 2063  in the current c
+00014080: 6f6c 756d 6e20 696e 2074 6865 206f 7269  olumn in the ori
+00014090: 6769 6e61 6c20 6d61 7472 6978 0a20 2020  ginal matrix.   
+000140a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140b0: 2020 2020 2069 6620 7375 6d28 6e65 775f       if sum(new_
+000140c0: 6d61 7472 6978 5b72 6f77 5d5b 635d 2066  matrix[row][c] f
+000140d0: 6f72 2072 6f77 2069 6e20 7261 6e67 6528  or row in range(
+000140e0: 726f 7773 2929 203d 3d20 303a 0a20 2020  rows)) == 0:.   
+000140f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014100: 2020 2020 2020 2020 2066 6974 6e65 7373           fitness
+00014110: 5f76 616c 7565 202a 3d20 302e 350a 2020  _value *= 0.5.  
+00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014130: 2020 2020 2020 656c 6966 2063 6f75 6e74        elif count
+00014140: 203e 2031 3a0a 2020 2020 2020 2020 2020   > 1:.          
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 2020 6669 746e 6573 735f 7661 6c75 6520    fitness_value 
+00014170: 2a3d 2030 2e34 0a20 2020 2020 2020 2020  *= 0.4.         
+00014180: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00014190: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000141a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141b0: 2066 6974 6e65 7373 5f76 616c 7565 203d   fitness_value =
+000141c0: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+000141d0: 2020 2020 2020 2072 202b 3d20 6472 0a0a         r += dr..
+000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141f0: 2320 4164 6a75 7374 2066 6974 6e65 7373  # Adjust fitness
+00014200: 2062 6173 6564 206f 6e20 7468 6520 636f   based on the co
+00014210: 756e 7420 6f66 2076 6572 7469 6361 6c20  unt of vertical 
+00014220: 616c 6967 6e6d 656e 7473 0a20 2020 2020  alignments.     
+00014230: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00014240: 756e 7420 696e 2072 616e 6765 2831 2c20  unt in range(1, 
+00014250: 3329 3a0a 2020 2020 2020 2020 2020 2020  3):.            
+00014260: 2020 2020 2020 2020 6669 746e 6573 735f          fitness_
+00014270: 7661 6c75 6520 2a3d 2030 2e31 0a20 2020  value *= 0.1.   
+00014280: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00014290: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000142a0: 2020 2020 2020 2066 6974 6e65 7373 5f76         fitness_v
+000142b0: 616c 7565 202a 3d20 302e 370a 0a20 2020  alue *= 0.7..   
+000142c0: 2020 2020 2020 2020 2070 7265 5f69 6e64           pre_ind
+000142d0: 6578 203d 206e 756d 5f69 6e64 6578 2020  ex = num_index  
+000142e0: 2320 5570 6461 7465 2070 7265 7669 6f75  # Update previou
+000142f0: 7320 696e 6465 7820 666f 7220 7468 6520  s index for the 
+00014300: 6e65 7874 2067 656e 650a 0a20 2020 2020  next gene..     
+00014310: 2020 2072 6574 7572 6e20 6669 746e 6573     return fitnes
+00014320: 735f 7661 6c75 650a 0a20 2020 2064 6566  s_value..    def
+00014330: 2066 6974 6e65 7373 2873 656c 662c 2069   fitness(self, i
+00014340: 6e64 6976 6964 7561 6c3a 206c 6973 742c  ndividual: list,
+00014350: 2064 6673 5f73 697a 653a 2074 7570 6c65   dfs_size: tuple
+00014360: 203d 2028 322c 2032 2929 202d 3e20 666c   = (2, 2)) -> fl
+00014370: 6f61 743a 0a20 2020 2020 2020 2022 2222  oat:.        """
+00014380: 0a20 2020 2020 2020 2043 616c 6375 6c61  .        Calcula
+00014390: 7465 7320 7468 6520 6669 746e 6573 7320  tes the fitness 
+000143a0: 6f66 2061 6e20 696e 6469 7669 6475 616c  of an individual
+000143b0: 2062 6173 6564 206f 6e20 7468 6520 616c   based on the al
+000143c0: 6967 6e6d 656e 7420 6f66 2067 656e 6573  ignment of genes
+000143d0: 2069 6e20 6120 6479 6e61 6d69 6361 6c6c   in a dynamicall
+000143e0: 790a 2020 2020 2020 2020 7570 6461 7465  y.        update
+000143f0: 6420 6d61 7472 6978 2e20 4669 746e 6573  d matrix. Fitnes
+00014400: 7320 6973 2065 7661 6c75 6174 6564 2062  s is evaluated b
+00014410: 6173 6564 206f 6e20 7370 6563 6966 6963  ased on specific
+00014420: 2061 6c69 676e 6d65 6e74 2070 6174 7465   alignment patte
+00014430: 726e 7320 616e 6420 7061 7261 6d65 7465  rns and paramete
+00014440: 7273 2e0a 0a20 2020 2020 2020 2041 7267  rs...        Arg
+00014450: 733a 0a20 2020 2020 2020 2069 6e64 6976  s:.        indiv
+00014460: 6964 7561 6c20 286c 6973 7429 3a20 4c69  idual (list): Li
+00014470: 7374 206f 6620 6765 6e65 2069 6e64 6963  st of gene indic
+00014480: 6573 2072 6570 7265 7365 6e74 696e 6720  es representing 
+00014490: 616e 2069 6e64 6976 6964 7561 6c20 696e  an individual in
+000144a0: 2074 6865 2070 6f70 756c 6174 696f 6e2e   the population.
+000144b0: 0a20 2020 2020 2020 2064 6673 5f73 697a  .        dfs_siz
+000144c0: 6520 2874 7570 6c65 293a 2053 697a 6520  e (tuple): Size 
+000144d0: 6f66 2074 6865 206d 6174 7269 7820 7265  of the matrix re
+000144e0: 6769 6f6e 2074 6f20 6368 6563 6b20 666f  gion to check fo
+000144f0: 7220 616c 6967 6e6d 656e 7473 2028 726f  r alignments (ro
+00014500: 7773 2c20 636f 6c73 292e 0a0a 2020 2020  ws, cols)...    
+00014510: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00014520: 2020 2020 2066 6c6f 6174 3a20 4120 6669       float: A fi
+00014530: 746e 6573 7320 7661 6c75 6520 6d6f 6469  tness value modi
+00014540: 6669 6564 2062 6173 6564 206f 6e20 7468  fied based on th
+00014550: 6520 7072 6573 656e 6365 206f 6620 7370  e presence of sp
+00014560: 6563 6966 6963 2061 6c69 676e 6d65 6e74  ecific alignment
+00014570: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00014580: 2020 2020 2020 2023 2072 6574 7572 6e20         # return 
+00014590: 6e70 2e6c 696e 616c 672e 6e6f 726d 2869  np.linalg.norm(i
+000145a0: 6e64 6976 6964 7561 6c20 2d20 7461 7267  ndividual - targ
+000145b0: 6574 290a 2020 2020 2020 2020 2320 4368  et).        # Ch
+000145c0: 6563 6b20 666f 7220 6475 706c 6963 6174  eck for duplicat
+000145d0: 6520 6765 6e65 732c 2077 6869 6368 2061  e genes, which a
+000145e0: 7265 206e 6f74 2061 6c6c 6f77 6564 0a20  re not allowed. 
+000145f0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+00014600: 7428 696e 6469 7669 6475 616c 2929 203c  t(individual)) <
+00014610: 2073 656c 662e 6e75 6d5f 6765 6e65 733a   self.num_genes:
+00014620: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00014630: 7572 6e20 3130 3030 3020 2023 2048 6967  urn 10000  # Hig
+00014640: 6820 7065 6e61 6c74 7920 666f 7220 6475  h penalty for du
+00014650: 706c 6963 6174 6520 6765 6e65 730a 0a20  plicate genes.. 
+00014660: 2020 2020 2020 2066 6974 6e65 7373 5f76         fitness_v
+00014670: 616c 7565 203d 2031 0a20 2020 2020 2020  alue = 1.       
+00014680: 2070 7265 5f69 6e64 6578 203d 2069 6e64   pre_index = ind
+00014690: 6976 6964 7561 6c5b 305d 202d 2031 2020  ividual[0] - 1  
+000146a0: 2320 5072 6576 696f 7573 2069 6e64 6578  # Previous index
+000146b0: 2066 6f72 2061 6c69 676e 6d65 6e74 2063   for alignment c
+000146c0: 6865 636b 696e 670a 0a20 2020 2020 2020  hecking..       
+000146d0: 2066 6f72 2069 6e64 6920 696e 2069 6e64   for indi in ind
+000146e0: 6976 6964 7561 6c3a 0a20 2020 2020 2020  ividual:.       
+000146f0: 2020 2020 2023 2043 6865 636b 2069 6620       # Check if 
+00014700: 7468 6520 6765 6e65 2069 7320 7769 7468  the gene is with
+00014710: 696e 2074 6865 2076 616c 6964 2072 616e  in the valid ran
+00014720: 6765 0a20 2020 2020 2020 2020 2020 2069  ge.            i
+00014730: 6620 6e6f 7420 2873 656c 662e 6d69 6e5f  f not (self.min_
+00014740: 6e75 6d20 3c3d 2069 6e64 6920 3c3d 2073  num <= indi <= s
+00014750: 656c 662e 6d61 785f 6e75 6d29 3a0a 2020  elf.max_num):.  
+00014760: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00014770: 7475 726e 2031 3030 3030 2020 2320 4869  turn 10000  # Hi
+00014780: 6768 2070 656e 616c 7479 2066 6f72 206f  gh penalty for o
+00014790: 7574 2d6f 662d 7261 6e67 6520 6765 6e65  ut-of-range gene
+000147a0: 730a 0a20 2020 2020 2020 2020 2020 206e  s..            n
+000147b0: 756d 5f69 6e64 6578 203d 2069 6e64 6920  um_index = indi 
+000147c0: 2d20 310a 2020 2020 2020 2020 2020 2020  - 1.            
+000147d0: 726f 7773 2c20 636f 6c73 203d 206c 656e  rows, cols = len
+000147e0: 2873 656c 662e 7265 6665 7273 5f6d 6174  (self.refers_mat
+000147f0: 7269 7829 2c20 7365 6c66 2e6d 6178 5f6e  rix), self.max_n
+00014800: 756d 0a20 2020 2020 2020 2020 2020 2028  um.            (
+00014810: 6466 735f 726f 772c 2064 6673 5f63 6f6c  dfs_row, dfs_col
+00014820: 292c 2074 6172 6765 7420 3d20 6466 735f  ), target = dfs_
+00014830: 7369 7a65 2c20 6d69 6e28 6466 735f 7369  size, min(dfs_si
+00014840: 7a65 290a 0a20 2020 2020 2020 2020 2020  ze)..           
+00014850: 2023 2043 6865 636b 2069 6620 7468 6520   # Check if the 
+00014860: 6466 735f 7369 7a65 2069 7320 6c61 7267  dfs_size is larg
+00014870: 6572 2074 6861 6e20 7468 6520 6d61 7472  er than the matr
+00014880: 6978 2064 696d 656e 7369 6f6e 730a 2020  ix dimensions.  
+00014890: 2020 2020 2020 2020 2020 6966 2064 6673            if dfs
+000148a0: 5f72 6f77 203e 2072 6f77 7320 6f72 2064  _row > rows or d
+000148b0: 6673 5f63 6f6c 203e 2063 6f6c 733a 0a20  fs_col > cols:. 
+000148c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000148d0: 6574 7572 6e20 3120 2023 2052 6574 7572  eturn 1  # Retur
+000148e0: 6e20 6465 6661 756c 7420 6669 746e 6573  n default fitnes
+000148f0: 7320 6966 2074 6865 2064 6673 2073 697a  s if the dfs siz
+00014900: 6520 6973 2074 6f6f 206c 6172 6765 0a0a  e is too large..
+00014910: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+00014920: 6561 7465 2061 206e 6577 206d 6174 7269  eate a new matri
+00014930: 7820 696e 636c 7564 696e 6720 6120 6e65  x including a ne
+00014940: 7720 726f 7720 666f 7220 7468 6520 6375  w row for the cu
+00014950: 7272 656e 7420 6765 6e65 0a20 2020 2020  rrent gene.     
+00014960: 2020 2020 2020 206e 6577 5f6d 6174 7269         new_matri
+00014970: 7820 3d20 5b72 6f77 5b3a 5d20 666f 7220  x = [row[:] for 
+00014980: 726f 7720 696e 2073 656c 662e 7265 6665  row in self.refe
+00014990: 7273 5f6d 6174 7269 785d 2020 2320 436f  rs_matrix]  # Co
+000149a0: 7079 2074 6865 2065 7869 7374 696e 6720  py the existing 
+000149b0: 6d61 7472 6978 0a20 2020 2020 2020 2020  matrix.         
+000149c0: 2020 206e 6577 5f72 6f77 203d 205b 305d     new_row = [0]
+000149d0: 202a 2073 656c 662e 6d61 785f 6e75 6d0a   * self.max_num.
+000149e0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+000149f0: 726f 775b 6e75 6d5f 696e 6465 785d 203d  row[num_index] =
+00014a00: 2031 0a20 2020 2020 2020 2020 2020 206e   1.            n
+00014a10: 6577 5f6d 6174 7269 782e 6170 7065 6e64  ew_matrix.append
+00014a20: 286e 6577 5f72 6f77 2920 2023 2041 6464  (new_row)  # Add
+00014a30: 2074 6865 206e 6577 2072 6f77 2063 6f72   the new row cor
+00014a40: 7265 6374 6c79 0a0a 2020 2020 2020 2020  rectly..        
+00014a50: 2020 2020 2320 4368 6563 6b20 616c 6967      # Check alig
+00014a60: 6e6d 656e 7473 206f 6e6c 7920 7570 7761  nments only upwa
+00014a70: 7264 730a 2020 2020 2020 2020 2020 2020  rds.            
+00014a80: 666f 7220 6472 2069 6e20 5b2d 315d 3a20  for dr in [-1]: 
+00014a90: 2023 204f 6e6c 7920 6e65 6564 2074 6f20   # Only need to 
+00014aa0: 6368 6563 6b20 7468 6520 7570 7761 7264  check the upward
+00014ab0: 2064 6972 6563 7469 6f6e 0a20 2020 2020   direction.     
+00014ac0: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
+00014ad0: 636b 2064 6961 676f 6e61 6c73 0a20 2020  ck diagonals.   
+00014ae0: 2020 2020 2020 2020 2020 2020 206d 6f76               mov
+00014af0: 655f 7220 3d20 4661 6c73 650a 2020 2020  e_r = False.    
+00014b00: 2020 2020 2020 2020 2020 2020 6d6f 7665              move
+00014b10: 5f72 5f63 6f75 6e74 203d 2030 0a20 2020  _r_count = 0.   
+00014b20: 2020 2020 2020 2020 2020 2020 206d 6f76               mov
+00014b30: 655f 635f 636f 756e 7420 3d20 300a 2020  e_c_count = 0.  
+00014b40: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00014b50: 7220 6463 2069 6e20 5b2d 312c 2031 5d3a  r dc in [-1, 1]:
+00014b60: 2020 2320 4368 6563 6b20 626f 7468 206c    # Check both l
+00014b70: 6566 7420 616e 6420 7269 6768 7420 6469  eft and right di
+00014b80: 6167 6f6e 616c 730a 2020 2020 2020 2020  agonals.        
+00014b90: 2020 2020 2020 2020 2020 2020 636f 756e              coun
+00014ba0: 7420 3d20 300a 2020 2020 2020 2020 2020  t = 0.          
+00014bb0: 2020 2020 2020 2020 2020 722c 2063 203d            r, c =
+00014bc0: 2072 6f77 732c 206e 756d 5f69 6e64 6578   rows, num_index
+00014bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014be0: 2020 2020 2077 6869 6c65 2072 6f77 7320       while rows 
+00014bf0: 2d20 6466 735f 726f 7720 3c3d 2072 203c  - dfs_row <= r <
+00014c00: 3d20 726f 7773 202b 2031 2061 6e64 2070  = rows + 1 and p
+00014c10: 7265 5f69 6e64 6578 202d 2064 6673 5f63  re_index - dfs_c
+00014c20: 6f6c 203c 3d20 6320 3c3d 206d 696e 286e  ol <= c <= min(n
+00014c30: 756d 5f69 6e64 6578 202b 2064 6673 5f63  um_index + dfs_c
+00014c40: 6f6c 2c0a 2020 2020 2020 2020 2020 2020  ol,.            
+00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ca0: 2020 636f 6c73 202d 2031 293a 0a20 2020    cols - 1):.   
+00014cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cc0: 2020 2020 2069 6620 6e65 775f 6d61 7472       if new_matr
+00014cd0: 6978 5b72 5d5b 635d 203d 3d20 313a 0a20  ix[r][c] == 1:. 
+00014ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cf0: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
+00014d00: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
+00014d10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014d20: 2064 6673 5f72 6f77 203d 3d20 6466 735f   dfs_row == dfs_
+00014d30: 636f 6c3a 0a20 2020 2020 2020 2020 2020  col:.           
+00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d50: 2072 202b 3d20 6472 0a20 2020 2020 2020   r += dr.       
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d70: 2020 2020 2063 202b 3d20 6463 0a20 2020       c += dc.   
+00014d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014db0: 2020 2020 2020 2069 6620 6d6f 7665 5f72         if move_r
+00014dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014de0: 2020 6966 206e 6577 5f6d 6174 7269 785b    if new_matrix[
+00014df0: 725d 5b63 5d20 3d3d 2031 3a0a 2020 2020  r][c] == 1:.    
+00014e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e20: 6d6f 7665 5f63 5f63 6f75 6e74 202b 3d20  move_c_count += 
+00014e30: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00014e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e50: 2020 7220 2b3d 2064 720a 2020 2020 2020    r += dr.      
+00014e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e70: 2020 2020 2020 2020 2020 6d6f 7665 5f72            move_r
+00014e80: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ea0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00014eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ec0: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
+00014ed0: 775f 6d61 7472 6978 5b72 5d5b 635d 203d  w_matrix[r][c] =
+00014ee0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00014ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f00: 2020 2020 2020 2020 206d 6f76 655f 725f           move_r_
+00014f10: 636f 756e 7420 2b3d 2031 0a20 2020 2020  count += 1.     
+00014f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f30: 2020 2020 2020 2020 2020 2063 202b 3d20             c += 
+00014f40: 6463 0a20 2020 2020 2020 2020 2020 2020  dc.             
+00014f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f60: 2020 206d 6f76 655f 7220 3d20 5472 7565     move_r = True
+00014f70: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014f80: 2020 2020 2020 2320 4164 6a75 7374 2066        # Adjust f
+00014f90: 6974 6e65 7373 2062 6173 6564 206f 6e20  itness based on 
+00014fa0: 7468 6520 636f 756e 7420 6f66 2064 6961  the count of dia
+00014fb0: 676f 6e61 6c20 616c 6967 6e6d 656e 7473  gonal alignments
+00014fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014fd0: 2020 2020 2069 6620 6466 735f 726f 7720       if dfs_row 
+00014fe0: 3d3d 2064 6673 5f63 6f6c 2061 6e64 2063  == dfs_col and c
+00014ff0: 6f75 6e74 203d 3d20 7461 7267 6574 3a0a  ount == target:.
+00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015010: 2020 2020 2020 2020 6669 746e 6573 735f          fitness_
+00015020: 7661 6c75 6520 2a3d 2073 656c 662e 6669  value *= self.fi
+00015030: 746e 6573 735f 7061 7261 6d73 5b30 5d0a  tness_params[0].
+00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015050: 2020 2020 656c 6966 206e 6f74 2064 6673      elif not dfs
+00015060: 5f72 6f77 203d 3d20 6466 735f 636f 6c20  _row == dfs_col 
+00015070: 616e 6420 6d61 7828 6d6f 7665 5f72 5f63  and max(move_r_c
+00015080: 6f75 6e74 2c20 6d6f 7665 5f63 5f63 6f75  ount, move_c_cou
+00015090: 6e74 2920 3d3d 2074 6172 6765 7420 2d20  nt) == target - 
+000150a0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+000150b0: 2020 2020 2020 2020 2020 2066 6974 6e65             fitne
+000150c0: 7373 5f76 616c 7565 202a 3d20 7365 6c66  ss_value *= self
+000150d0: 2e66 6974 6e65 7373 5f70 6172 616d 735b  .fitness_params[
+000150e0: 315d 0a0a 2020 2020 2020 2020 2020 2020  1]..            
+000150f0: 2020 2020 2320 4368 6563 6b20 7665 7274      # Check vert
+00015100: 6963 616c 2061 6c69 676e 6d65 6e74 0a20  ical alignment. 
+00015110: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00015120: 6f75 6e74 203d 2030 0a20 2020 2020 2020  ount = 0.       
+00015130: 2020 2020 2020 2020 2072 2c20 6320 3d20           r, c = 
+00015140: 726f 7773 2c20 6e75 6d5f 696e 6465 780a  rows, num_index.
+00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015160: 7768 696c 6520 3020 3c3d 2072 203c 206c  while 0 <= r < l
+00015170: 656e 286e 6577 5f6d 6174 7269 7829 3a0a  en(new_matrix):.
+00015180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015190: 2020 2020 6966 206e 6577 5f6d 6174 7269      if new_matri
+000151a0: 785b 725d 5b63 5d20 3d3d 2031 3a0a 2020  x[r][c] == 1:.  
+000151b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151c0: 2020 2020 2020 636f 756e 7420 2b3d 2031        count += 1
+000151d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000151e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000151f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015200: 2020 2023 2043 6865 636b 2069 6620 7468     # Check if th
+00015210: 6572 6520 6172 6520 6e6f 2067 656e 6573  ere are no genes
+00015220: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00015230: 636f 6c75 6d6e 2069 6e20 7468 6520 6f72  column in the or
+00015240: 6967 696e 616c 206d 6174 7269 780a 2020  iginal matrix.  
+00015250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015260: 2020 2020 2020 6966 2073 756d 286e 6577        if sum(new
+00015270: 5f6d 6174 7269 785b 726f 775d 5b63 5d20  _matrix[row][c] 
+00015280: 666f 7220 726f 7720 696e 2072 616e 6765  for row in range
+00015290: 2872 6f77 7329 2920 3d3d 2030 3a0a 2020  (rows)) == 0:.  
+000152a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152b0: 2020 2020 2020 2020 2020 6669 746e 6573            fitnes
+000152c0: 735f 7661 6c75 6520 2a3d 2073 656c 662e  s_value *= self.
+000152d0: 6669 746e 6573 735f 7061 7261 6d73 5b32  fitness_params[2
+000152e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000152f0: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
+00015300: 6f75 6e74 203e 2031 3a0a 2020 2020 2020  ount > 1:.      
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 2020 2020 2020 6669 746e 6573 735f 7661        fitness_va
+00015330: 6c75 6520 2a3d 2073 656c 662e 6669 746e  lue *= self.fitn
+00015340: 6573 735f 7061 7261 6d73 5b33 5d0a 2020  ess_params[3].  
+00015350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015360: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00015370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015380: 2020 2020 2020 2020 6669 746e 6573 735f          fitness_
+00015390: 7661 6c75 6520 3d20 7365 6c66 2e66 6974  value = self.fit
+000153a0: 6e65 7373 5f70 6172 616d 735b 345d 0a20  ness_params[4]. 
+000153b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153c0: 2020 2072 202b 3d20 6472 0a0a 2020 2020     r += dr..    
+000153d0: 2020 2020 2020 2020 2020 2020 2320 4164              # Ad
+000153e0: 6a75 7374 2066 6974 6e65 7373 2062 6173  just fitness bas
+000153f0: 6564 206f 6e20 7468 6520 636f 756e 7420  ed on the count 
+00015400: 6f66 2076 6572 7469 6361 6c20 616c 6967  of vertical alig
+00015410: 6e6d 656e 7473 0a20 2020 2020 2020 2020  nments.         
+00015420: 2020 2020 2020 2069 6620 636f 756e 7420         if count 
+00015430: 696e 2072 616e 6765 2831 2c20 3329 3a0a  in range(1, 3):.
+00015440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015450: 2020 2020 6669 746e 6573 735f 7661 6c75      fitness_valu
+00015460: 6520 2a3d 2073 656c 662e 6669 746e 6573  e *= self.fitnes
+00015470: 735f 7061 7261 6d73 5b35 5d0a 2020 2020  s_params[5].    
+00015480: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00015490: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000154a0: 2020 2020 2020 6669 746e 6573 735f 7661        fitness_va
+000154b0: 6c75 6520 2a3d 2073 656c 662e 6669 746e  lue *= self.fitn
+000154c0: 6573 735f 7061 7261 6d73 5b36 5d0a 0a20  ess_params[6].. 
+000154d0: 2020 2020 2020 2020 2020 2070 7265 5f69             pre_i
+000154e0: 6e64 6578 203d 206e 756d 5f69 6e64 6578  ndex = num_index
+000154f0: 2020 2320 5570 6461 7465 2070 7265 7669    # Update previ
+00015500: 6f75 7320 696e 6465 7820 666f 7220 7468  ous index for th
+00015510: 6520 6e65 7874 2067 656e 650a 0a20 2020  e next gene..   
+00015520: 2020 2020 2072 6574 7572 6e20 6669 746e       return fitn
+00015530: 6573 735f 7661 6c75 650a 0a20 2020 2064  ess_value..    d
+00015540: 6566 2074 6f75 726e 616d 656e 745f 7365  ef tournament_se
+00015550: 6c65 6374 696f 6e28 7365 6c66 2920 2d3e  lection(self) ->
+00015560: 206e 702e 6e64 6172 7261 793a 0a20 2020   np.ndarray:.   
+00015570: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00015580: 2054 6f75 726e 616d 656e 7420 7365 6c65   Tournament sele
+00015590: 6374 696f 6e20 6d65 7468 6f64 2e20 5261  ction method. Ra
+000155a0: 6e64 6f6d 6c79 2073 656c 6563 7473 206b  ndomly selects k
+000155b0: 2069 6e64 6976 6964 7561 6c73 2066 726f   individuals fro
+000155c0: 6d20 7468 6520 706f 7075 6c61 7469 6f6e  m the population
+000155d0: 0a20 2020 2020 2020 2061 6e64 2072 6574  .        and ret
+000155e0: 7572 6e73 2074 6865 2069 6e64 6976 6964  urns the individ
+000155f0: 7561 6c20 7769 7468 2074 6865 2068 6967  ual with the hig
+00015600: 6865 7374 2066 6974 6e65 7373 2e0a 0a20  hest fitness... 
+00015610: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00015620: 2020 2020 2020 2020 6e70 2e6e 6461 7272          np.ndarr
+00015630: 6179 3a20 5468 6520 696e 6469 7669 6475  ay: The individu
+00015640: 616c 2077 6974 6820 7468 6520 6869 6768  al with the high
+00015650: 6573 7420 6669 746e 6573 7320 6672 6f6d  est fitness from
+00015660: 2074 6865 2073 656c 6563 7465 6420 7361   the selected sa
+00015670: 6d70 6c65 2e0a 2020 2020 2020 2020 2222  mple..        ""
+00015680: 220a 2020 2020 2020 2020 2320 5365 6c65  ".        # Sele
+00015690: 6374 2074 6865 2069 6e64 6976 6964 7561  ct the individua
+000156a0: 6c20 7769 7468 2074 6865 2068 6967 6865  l with the highe
+000156b0: 7374 2066 6974 6e65 7373 2066 726f 6d20  st fitness from 
+000156c0: 6120 7261 6e64 6f6d 2073 616d 706c 650a  a random sample.
+000156d0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+000156e0: 203d 206d 6178 2872 616e 646f 6d2e 7361   = max(random.sa
+000156f0: 6d70 6c65 2873 656c 662e 706f 7075 6c61  mple(self.popula
+00015700: 7469 6f6e 2c20 7365 6c66 2e74 6f75 726e  tion, self.tourn
+00015710: 616d 656e 745f 7369 7a65 292c 206b 6579  ament_size), key
+00015720: 3d6c 616d 6264 6120 696e 643a 2031 202f  =lambda ind: 1 /
+00015730: 2073 656c 662e 6669 746e 6573 7328 696e   self.fitness(in
+00015740: 6429 290a 2020 2020 2020 2020 2320 536f  d)).        # So
+00015750: 7274 2074 6865 2073 656c 6563 7465 6420  rt the selected 
+00015760: 696e 6469 7669 6475 616c 2066 6f72 2063  individual for c
+00015770: 6f6e 7369 7374 656e 6379 0a20 2020 2020  onsistency.     
+00015780: 2020 2073 6f72 7465 645f 7365 6c65 6374     sorted_select
+00015790: 6564 203d 206e 702e 736f 7274 2873 656c  ed = np.sort(sel
+000157a0: 6563 7465 6429 0a20 2020 2020 2020 2072  ected).        r
+000157b0: 6574 7572 6e20 736f 7274 6564 5f73 656c  eturn sorted_sel
+000157c0: 6563 7465 640a 0a20 2020 2064 6566 2063  ected..    def c
+000157d0: 726f 7373 6f76 6572 2873 656c 662c 2070  rossover(self, p
+000157e0: 6172 656e 7431 3a20 6e70 2e6e 6461 7272  arent1: np.ndarr
+000157f0: 6179 2c20 7061 7265 6e74 323a 206e 702e  ay, parent2: np.
+00015800: 6e64 6172 7261 7929 202d 3e20 6e70 2e6e  ndarray) -> np.n
+00015810: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
+00015820: 2222 220a 2020 2020 2020 2020 5477 6f2d  """.        Two-
+00015830: 706f 696e 7420 6372 6f73 736f 7665 722e  point crossover.
+00015840: 2052 616e 646f 6d6c 7920 7365 6c65 6374   Randomly select
+00015850: 7320 7477 6f20 706f 696e 7473 2061 6e64  s two points and
+00015860: 2073 7761 7073 2074 6865 2067 656e 6573   swaps the genes
+00015870: 2062 6574 7765 656e 2074 6865 2074 776f   between the two
+00015880: 2070 6172 656e 7473 0a20 2020 2020 2020   parents.       
+00015890: 2074 6f20 6372 6561 7465 2061 2063 6869   to create a chi
+000158a0: 6c64 2e0a 0a20 2020 2020 2020 2041 7267  ld...        Arg
+000158b0: 733a 0a20 2020 2020 2020 2070 6172 656e  s:.        paren
+000158c0: 7431 2028 6e70 2e6e 6461 7272 6179 293a  t1 (np.ndarray):
+000158d0: 2054 6865 2066 6972 7374 2070 6172 656e   The first paren
+000158e0: 742e 0a20 2020 2020 2020 2070 6172 656e  t..        paren
+000158f0: 7432 2028 6e70 2e6e 6461 7272 6179 293a  t2 (np.ndarray):
+00015900: 2054 6865 2073 6563 6f6e 6420 7061 7265   The second pare
+00015910: 6e74 2e0a 0a20 2020 2020 2020 2052 6574  nt...        Ret
+00015920: 7572 6e73 3a0a 2020 2020 2020 2020 6e70  urns:.        np
+00015930: 2e6e 6461 7272 6179 3a20 5468 6520 6368  .ndarray: The ch
+00015940: 696c 6420 6372 6561 7465 6420 6279 2063  ild created by c
+00015950: 726f 7373 6f76 6572 2e0a 2020 2020 2020  rossover..      
+00015960: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+00015970: 5261 6e64 6f6d 6c79 2073 656c 6563 7420  Randomly select 
+00015980: 7477 6f20 706f 696e 7473 2066 6f72 2063  two points for c
+00015990: 726f 7373 6f76 6572 0a20 2020 2020 2020  rossover.       
+000159a0: 2070 6f69 6e74 7320 3d20 736f 7274 6564   points = sorted
+000159b0: 2872 616e 646f 6d2e 7361 6d70 6c65 2872  (random.sample(r
+000159c0: 616e 6765 2830 2c20 7365 6c66 2e6e 756d  ange(0, self.num
+000159d0: 5f67 656e 6573 292c 2032 2929 0a20 2020  _genes), 2)).   
+000159e0: 2020 2020 2023 2043 7265 6174 6520 6e65       # Create ne
+000159f0: 7720 6368 696c 6420 6279 2063 6f6d 6269  w child by combi
+00015a00: 6e69 6e67 2070 6172 7473 206f 6620 626f  ning parts of bo
+00015a10: 7468 2070 6172 656e 7473 0a20 2020 2020  th parents.     
+00015a20: 2020 2072 6574 7572 6e20 6e70 2e63 6f6e     return np.con
+00015a30: 6361 7465 6e61 7465 285b 7061 7265 6e74  catenate([parent
+00015a40: 315b 3a70 6f69 6e74 735b 305d 5d2c 2070  1[:points[0]], p
+00015a50: 6172 656e 7432 5b70 6f69 6e74 735b 305d  arent2[points[0]
+00015a60: 3a70 6f69 6e74 735b 315d 5d2c 2070 6172  :points[1]], par
+00015a70: 656e 7431 5b70 6f69 6e74 735b 315d 3a5d  ent1[points[1]:]
+00015a80: 5d29 0a0a 2020 2020 6465 6620 6d75 7461  ])..    def muta
+00015a90: 7465 2873 656c 662c 2069 6e64 6976 6964  te(self, individ
+00015aa0: 7561 6c3a 206e 702e 6e64 6172 7261 7929  ual: np.ndarray)
+00015ab0: 202d 3e20 6e70 2e6e 6461 7272 6179 3a0a   -> np.ndarray:.
+00015ac0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015ad0: 2020 2020 4d75 7461 7469 6f6e 206f 7065      Mutation ope
+00015ae0: 7261 7469 6f6e 2e20 4d75 7461 7465 7320  ration. Mutates 
+00015af0: 616e 2069 6e64 6976 6964 7561 6c27 7320  an individual's 
+00015b00: 6765 6e65 2077 6974 6820 6120 6365 7274  gene with a cert
+00015b10: 6169 6e20 7072 6f62 6162 696c 6974 792e  ain probability.
+00015b20: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00015b30: 2020 2020 2020 2020 696e 6469 7669 6475          individu
+00015b40: 616c 2028 6e70 2e6e 6461 7272 6179 293a  al (np.ndarray):
+00015b50: 2054 6865 2069 6e64 6976 6964 7561 6c20   The individual 
+00015b60: 746f 206d 7574 6174 652e 0a0a 2020 2020  to mutate...    
+00015b70: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00015b80: 2020 2020 206e 702e 6e64 6172 7261 793a       np.ndarray:
+00015b90: 2054 6865 206d 7574 6174 6564 2069 6e64   The mutated ind
+00015ba0: 6976 6964 7561 6c2e 0a20 2020 2020 2020  ividual..       
+00015bb0: 2022 2222 0a20 2020 2020 2020 2023 204d   """.        # M
+00015bc0: 7574 6174 6520 6120 6765 6e65 2077 6974  utate a gene wit
+00015bd0: 6820 6120 6769 7665 6e20 7072 6f62 6162  h a given probab
+00015be0: 696c 6974 790a 2020 2020 2020 2020 6966  ility.        if
+00015bf0: 2072 616e 646f 6d2e 7261 6e64 6f6d 2829   random.random()
+00015c00: 203c 2073 656c 662e 6d75 7461 7469 6f6e   < self.mutation
+00015c10: 5f72 6174 653a 0a20 2020 2020 2020 2020  _rate:.         
+00015c20: 2020 2069 6e64 6578 203d 2072 616e 646f     index = rando
+00015c30: 6d2e 7261 6e64 696e 7428 302c 206c 656e  m.randint(0, len
+00015c40: 2869 6e64 6976 6964 7561 6c29 202d 2031  (individual) - 1
+00015c50: 290a 2020 2020 2020 2020 2020 2020 696e  ).            in
+00015c60: 6469 7669 6475 616c 5b69 6e64 6578 5d20  dividual[index] 
+00015c70: 3d20 7261 6e64 6f6d 2e63 686f 6963 6528  = random.choice(
+00015c80: 7365 6c66 2e64 6174 6129 0a20 2020 2020  self.data).     
+00015c90: 2020 2023 2052 6574 7572 6e20 7468 6520     # Return the 
+00015ca0: 736f 7274 6564 2069 6e64 6976 6964 7561  sorted individua
+00015cb0: 6c0a 2020 2020 2020 2020 7265 7475 726e  l.        return
+00015cc0: 206e 702e 736f 7274 2869 6e64 6976 6964   np.sort(individ
+00015cd0: 7561 6c29 0a0a 2020 2020 6465 6620 6765  ual)..    def ge
+00015ce0: 6e65 7469 6328 7365 6c66 2920 2d3e 206c  netic(self) -> l
+00015cf0: 6973 743a 0a20 2020 2020 2020 2022 2222  ist:.        """
+00015d00: 0a20 2020 2020 2020 204d 6169 6e20 6c6f  .        Main lo
+00015d10: 6f70 206f 6620 7468 6520 6765 6e65 7469  op of the geneti
+00015d20: 6320 616c 676f 7269 7468 6d2e 2050 6572  c algorithm. Per
+00015d30: 666f 726d 7320 6765 6e65 7469 6320 6f70  forms genetic op
+00015d40: 6572 6174 696f 6e73 206f 7665 7220 6d75  erations over mu
+00015d50: 6c74 6970 6c65 2067 656e 6572 6174 696f  ltiple generatio
+00015d60: 6e73 0a20 2020 2020 2020 2074 6f20 6669  ns.        to fi
+00015d70: 6e64 2074 6865 206f 7074 696d 616c 2073  nd the optimal s
+00015d80: 6f6c 7574 696f 6e2e 0a0a 2020 2020 2020  olution...      
+00015d90: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00015da0: 2020 206e 702e 6e64 6172 7261 793a 2054     np.ndarray: T
+00015db0: 6865 2062 6573 7420 696e 6469 7669 6475  he best individu
+00015dc0: 616c 2066 6f75 6e64 2061 6674 6572 2061  al found after a
+00015dd0: 6c6c 2067 656e 6572 6174 696f 6e73 2e0a  ll generations..
+00015de0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015df0: 2020 2020 2320 4974 6572 6174 6520 6f76      # Iterate ov
+00015e00: 6572 206d 756c 7469 706c 6520 6765 6e65  er multiple gene
+00015e10: 7261 7469 6f6e 730a 2020 2020 2020 2020  rations.        
+00015e20: 666f 7220 5f20 696e 2072 616e 6765 2873  for _ in range(s
+00015e30: 656c 662e 6570 6f63 685f 636f 756e 7429  elf.epoch_count)
+00015e40: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00015e50: 775f 706f 7075 6c61 7469 6f6e 203d 205b  w_population = [
+00015e60: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00015e70: 7220 5f20 696e 2072 616e 6765 2873 656c  r _ in range(sel
+00015e80: 662e 706f 7075 6c61 7469 6f6e 5f73 697a  f.population_siz
+00015e90: 6520 2f2f 2032 293a 0a20 2020 2020 2020  e // 2):.       
+00015ea0: 2020 2020 2020 2020 2023 2053 656c 6563           # Selec
+00015eb0: 7420 7061 7265 6e74 7320 616e 6420 6372  t parents and cr
+00015ec0: 6561 7465 2063 6869 6c64 7265 6e0a 2020  eate children.  
+00015ed0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00015ee0: 7265 6e74 3120 3d20 7365 6c66 2e74 6f75  rent1 = self.tou
+00015ef0: 726e 616d 656e 745f 7365 6c65 6374 696f  rnament_selectio
+00015f00: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
+00015f10: 2020 2020 7061 7265 6e74 3220 3d20 7365      parent2 = se
+00015f20: 6c66 2e74 6f75 726e 616d 656e 745f 7365  lf.tournament_se
+00015f30: 6c65 6374 696f 6e28 290a 2020 2020 2020  lection().      
+00015f40: 2020 2020 2020 2020 2020 6368 696c 6431            child1
+00015f50: 203d 2073 656c 662e 6372 6f73 736f 7665   = self.crossove
+00015f60: 7228 7061 7265 6e74 312c 2070 6172 656e  r(parent1, paren
+00015f70: 7432 290a 2020 2020 2020 2020 2020 2020  t2).            
+00015f80: 2020 2020 6368 696c 6432 203d 2073 656c      child2 = sel
+00015f90: 662e 6372 6f73 736f 7665 7228 7061 7265  f.crossover(pare
+00015fa0: 6e74 312c 2070 6172 656e 7432 290a 2020  nt1, parent2).  
+00015fb0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00015fc0: 4d75 7461 7465 2063 6869 6c64 7265 6e20  Mutate children 
+00015fd0: 616e 6420 6164 6420 746f 206e 6577 2070  and add to new p
+00015fe0: 6f70 756c 6174 696f 6e0a 2020 2020 2020  opulation.      
+00015ff0: 2020 2020 2020 2020 2020 6e65 775f 706f            new_po
+00016000: 7075 6c61 7469 6f6e 2e65 7874 656e 6428  pulation.extend(
+00016010: 5b73 656c 662e 6d75 7461 7465 2863 6869  [self.mutate(chi
+00016020: 6c64 3129 2c20 7365 6c66 2e6d 7574 6174  ld1), self.mutat
+00016030: 6528 6368 696c 6432 295d 290a 2020 2020  e(child2)]).    
+00016040: 2020 2020 2020 2020 2320 5570 6461 7465          # Update
+00016050: 2070 6f70 756c 6174 696f 6e0a 2020 2020   population.    
+00016060: 2020 2020 2020 2020 7365 6c66 2e70 6f70          self.pop
+00016070: 756c 6174 696f 6e20 3d20 6e65 775f 706f  ulation = new_po
+00016080: 7075 6c61 7469 6f6e 0a0a 2020 2020 2020  pulation..      
+00016090: 2020 2320 4669 6e64 2061 6e64 2072 6574    # Find and ret
+000160a0: 7572 6e20 7468 6520 6265 7374 2069 6e64  urn the best ind
+000160b0: 6976 6964 7561 6c20 6261 7365 6420 6f6e  ividual based on
+000160c0: 2066 6974 6e65 7373 0a20 2020 2020 2020   fitness.       
+000160d0: 2062 6573 745f 696e 6469 7669 6475 616c   best_individual
+000160e0: 203d 206d 696e 285b 6c69 7374 2869 7465   = min([list(ite
+000160f0: 6d29 2066 6f72 2069 7465 6d20 696e 2073  m) for item in s
+00016100: 656c 662e 706f 7075 6c61 7469 6f6e 5d2c  elf.population],
+00016110: 206b 6579 3d73 656c 662e 6669 746e 6573   key=self.fitnes
+00016120: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+00016130: 6e20 6265 7374 5f69 6e64 6976 6964 7561  n best_individua
+00016140: 6c0a 0a0a 636c 6173 7320 4465 6e6f 6973  l...class Denois
+00016150: 6572 5574 696c 3a0a 2020 2020 4073 7461  erUtil:.    @sta
+00016160: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
+00016170: 6620 6d6f 7669 6e67 5f61 7665 7261 6765  f moving_average
+00016180: 2873 6571 7565 6e63 652c 2077 696e 646f  (sequence, windo
+00016190: 775f 7369 7a65 3d33 293a 0a20 2020 2020  w_size=3):.     
+000161a0: 2020 2072 6574 7572 6e20 6e70 2e63 6f6e     return np.con
+000161b0: 766f 6c76 6528 7365 7175 656e 6365 2c20  volve(sequence, 
+000161c0: 6e70 2e6f 6e65 7328 7769 6e64 6f77 5f73  np.ones(window_s
+000161d0: 697a 6529 2f77 696e 646f 775f 7369 7a65  ize)/window_size
+000161e0: 2c20 6d6f 6465 3d27 7661 6c69 6427 290a  , mode='valid').
+000161f0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00016200: 6f64 0a20 2020 2064 6566 206d 6564 6961  od.    def media
+00016210: 6e5f 6669 6c74 6572 2873 6571 7565 6e63  n_filter(sequenc
+00016220: 652c 206b 6572 6e65 6c5f 7369 7a65 3d33  e, kernel_size=3
+00016230: 293a 0a20 2020 2020 2020 2066 696c 7465  ):.        filte
+00016240: 7265 645f 7365 7175 656e 6365 203d 205b  red_sequence = [
+00016250: 5d0a 2020 2020 2020 2020 666f 7220 6920  ].        for i 
+00016260: 696e 2072 616e 6765 286c 656e 2873 6571  in range(len(seq
+00016270: 7565 6e63 6529 293a 0a20 2020 2020 2020  uence)):.       
+00016280: 2020 2020 2073 7461 7274 203d 206d 6178       start = max
+00016290: 2830 2c20 6920 2d20 6b65 726e 656c 5f73  (0, i - kernel_s
+000162a0: 697a 6520 2f2f 2032 290a 2020 2020 2020  ize // 2).      
+000162b0: 2020 2020 2020 656e 6420 3d20 6d69 6e28        end = min(
+000162c0: 6c65 6e28 7365 7175 656e 6365 292c 2069  len(sequence), i
+000162d0: 202b 206b 6572 6e65 6c5f 7369 7a65 202f   + kernel_size /
+000162e0: 2f20 3220 2b20 3129 0a20 2020 2020 2020  / 2 + 1).       
+000162f0: 2020 2020 206d 6564 6961 6e5f 7661 6c20       median_val 
+00016300: 3d20 6e70 2e6d 6564 6961 6e28 7365 7175  = np.median(sequ
+00016310: 656e 6365 5b73 7461 7274 3a65 6e64 5d29  ence[start:end])
+00016320: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00016330: 7465 7265 645f 7365 7175 656e 6365 2e61  tered_sequence.a
+00016340: 7070 656e 6428 6d65 6469 616e 5f76 616c  ppend(median_val
+00016350: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00016360: 2066 696c 7465 7265 645f 7365 7175 656e   filtered_sequen
+00016370: 6365 0a0a 2020 2020 4073 7461 7469 636d  ce..    @staticm
+00016380: 6574 686f 640a 2020 2020 6465 6620 7265  ethod.    def re
+00016390: 6d6f 7665 5f6f 7574 6c69 6572 7328 7365  move_outliers(se
+000163a0: 7175 656e 6365 2c20 7468 7265 7368 6f6c  quence, threshol
+000163b0: 643d 3229 3a0a 2020 2020 2020 2020 6d65  d=2):.        me
+000163c0: 616e 203d 206e 702e 6d65 616e 2873 6571  an = np.mean(seq
+000163d0: 7565 6e63 6529 0a20 2020 2020 2020 2073  uence).        s
+000163e0: 7464 5f64 6576 203d 206e 702e 7374 6428  td_dev = np.std(
+000163f0: 7365 7175 656e 6365 290a 2020 2020 2020  sequence).      
+00016400: 2020 6669 6c74 6572 6564 5f73 6571 7565    filtered_seque
+00016410: 6e63 6520 3d20 5b78 2066 6f72 2078 2069  nce = [x for x i
+00016420: 6e20 7365 7175 656e 6365 2069 6620 6e70  n sequence if np
+00016430: 2e61 6273 2878 202d 206d 6561 6e29 203c  .abs(x - mean) <
+00016440: 3d20 7468 7265 7368 6f6c 6420 2a20 7374  = threshold * st
+00016450: 645f 6465 765d 0a20 2020 2020 2020 2072  d_dev].        r
+00016460: 6574 7572 6e20 6669 6c74 6572 6564 5f73  eturn filtered_s
+00016470: 6571 7565 6e63 650a 0a20 2020 2040 7374  equence..    @st
+00016480: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00016490: 6566 2064 656e 6f69 7365 5f77 6176 656c  ef denoise_wavel
+000164a0: 6574 2873 6571 7565 6e63 652c 2077 6176  et(sequence, wav
+000164b0: 656c 6574 3d27 6462 3127 2c20 6c65 7665  elet='db1', leve
+000164c0: 6c3d 3129 3a0a 2020 2020 2020 2020 636f  l=1):.        co
+000164d0: 6566 6673 203d 2070 7977 742e 7761 7665  effs = pywt.wave
+000164e0: 6465 6328 7365 7175 656e 6365 2c20 7761  dec(sequence, wa
+000164f0: 7665 6c65 742c 206c 6576 656c 3d6c 6576  velet, level=lev
+00016500: 656c 290a 2020 2020 2020 2020 2320 e4bd  el).        # ..
+00016510: bfe7 94a8 e8bd afe9 9888 e580 bce5 8ebb  ................
+00016520: e599 aa0a 2020 2020 2020 2020 7369 676d  ....        sigm
+00016530: 6120 3d20 6e70 2e6d 6564 6961 6e28 6e70  a = np.median(np
+00016540: 2e61 6273 2863 6f65 6666 735b 2d6c 6576  .abs(coeffs[-lev
+00016550: 656c 5d29 2920 2f20 302e 3637 3435 0a20  el])) / 0.6745. 
+00016560: 2020 2020 2020 2075 7468 7265 7368 203d         uthresh =
+00016570: 2073 6967 6d61 202a 206e 702e 7371 7274   sigma * np.sqrt
+00016580: 2832 202a 206e 702e 6c6f 6728 6c65 6e28  (2 * np.log(len(
+00016590: 7365 7175 656e 6365 2929 290a 2020 2020  sequence))).    
+000165a0: 2020 2020 636f 6566 6673 5b31 3a5d 203d      coeffs[1:] =
+000165b0: 2028 7079 7774 2e74 6872 6573 686f 6c64   (pywt.threshold
+000165c0: 2869 2c20 7661 6c75 653d 7574 6872 6573  (i, value=uthres
+000165d0: 682c 206d 6f64 653d 2773 6f66 7427 2920  h, mode='soft') 
+000165e0: 666f 7220 6920 696e 2063 6f65 6666 735b  for i in coeffs[
+000165f0: 313a 5d29 0a20 2020 2020 2020 2072 6574  1:]).        ret
+00016600: 7572 6e20 7079 7774 2e77 6176 6572 6563  urn pywt.waverec
+00016610: 2863 6f65 6666 732c 2077 6176 656c 6574  (coeffs, wavelet
+00016620: 290a 0a0a 636c 6173 7320 5261 6e64 6f6d  )...class Random
+00016630: 466f 7265 7374 5265 6772 6573 736f 7254  ForestRegressorT
+00016640: 7261 6e73 666f 726d 6572 2842 6173 6545  ransformer(BaseE
+00016650: 7374 696d 6174 6f72 2c20 5472 616e 7366  stimator, Transf
+00016660: 6f72 6d65 724d 6978 696e 293a 0a20 2020  ormerMixin):.   
+00016670: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00016680: 6c66 2c20 6d6f 6465 6c3a 2052 616e 646f  lf, model: Rando
+00016690: 6d46 6f72 6573 7452 6567 7265 7373 6f72  mForestRegressor
+000166a0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000166b0: 2020 2020 2020 2049 6e69 7469 616c 697a         Initializ
+000166c0: 6520 7468 6520 7472 616e 7366 6f72 6d65  e the transforme
+000166d0: 7220 7769 7468 2061 2052 616e 646f 6d46  r with a RandomF
+000166e0: 6f72 6573 7452 6567 7265 7373 6f72 206d  orestRegressor m
+000166f0: 6f64 656c 2061 6e64 2061 2053 7461 6e64  odel and a Stand
+00016700: 6172 6453 6361 6c65 7220 666f 7220 6665  ardScaler for fe
+00016710: 6174 7572 6520 7363 616c 696e 672e 0a0a  ature scaling...
+00016720: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00016730: 7273 3a0a 2020 2020 2020 2020 6d6f 6465  rs:.        mode
+00016740: 6c20 2852 616e 646f 6d46 6f72 6573 7452  l (RandomForestR
+00016750: 6567 7265 7373 6f72 293a 2054 6865 2052  egressor): The R
+00016760: 616e 646f 6d46 6f72 6573 7452 6567 7265  andomForestRegre
+00016770: 7373 6f72 206d 6f64 656c 2074 6f20 6265  ssor model to be
+00016780: 2075 7365 6420 666f 7220 7072 6564 6963   used for predic
+00016790: 7469 6f6e 732e 0a20 2020 2020 2020 2022  tions..        "
+000167a0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+000167b0: 6361 6c63 756c 6174 655f 7574 696c 203d  calculate_util =
+000167c0: 2043 616c 6375 6c61 7465 5574 696c 0a20   CalculateUtil. 
+000167d0: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+000167e0: 6c5f 7574 696c 203d 204d 6f64 656c 5574  l_util = ModelUt
+000167f0: 696c 0a20 2020 2020 2020 2073 656c 662e  il.        self.
+00016800: 6d6f 6465 6c20 3d20 6d6f 6465 6c0a 2020  model = model.  
+00016810: 2020 2020 2020 7365 6c66 2e73 6361 6c65        self.scale
+00016820: 7220 3d20 5374 616e 6461 7264 5363 616c  r = StandardScal
+00016830: 6572 2829 0a0a 2020 2020 6465 6620 6669  er()..    def fi
+00016840: 7428 7365 6c66 2c20 583a 206e 702e 6e64  t(self, X: np.nd
+00016850: 6172 7261 792c 2079 3a20 4f70 7469 6f6e  array, y: Option
+00016860: 616c 5b6e 702e 6e64 6172 7261 795d 203d  al[np.ndarray] =
+00016870: 204e 6f6e 6529 202d 3e20 2752 616e 646f   None) -> 'Rando
+00016880: 6d46 6f72 6573 7452 6567 7265 7373 6f72  mForestRegressor
+00016890: 5472 616e 7366 6f72 6d65 7227 3a0a 2020  Transformer':.  
+000168a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000168b0: 2020 4669 7420 7468 6520 5261 6e64 6f6d    Fit the Random
+000168c0: 466f 7265 7374 206d 6f64 656c 2061 6e64  Forest model and
+000168d0: 2074 6865 2073 6361 6c65 7220 6f6e 2074   the scaler on t
+000168e0: 6865 2074 7261 696e 696e 6720 6461 7461  he training data
+000168f0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00016900: 6574 6572 733a 0a20 2020 2020 2020 2058  eters:.        X
+00016910: 2028 6e70 2e6e 6461 7272 6179 293a 2054   (np.ndarray): T
+00016920: 7261 696e 696e 6720 6461 7461 2066 6561  raining data fea
+00016930: 7475 7265 732e 0a20 2020 2020 2020 2079  tures..        y
+00016940: 2028 4f70 7469 6f6e 616c 5b6e 702e 6e64   (Optional[np.nd
+00016950: 6172 7261 795d 293a 2054 7261 696e 696e  array]): Trainin
+00016960: 6720 6461 7461 206c 6162 656c 732e 0a0a  g data labels...
+00016970: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00016980: 0a20 2020 2020 2020 2052 616e 646f 6d46  .        RandomF
+00016990: 6f72 6573 7452 6567 7265 7373 6f72 5472  orestRegressorTr
+000169a0: 616e 7366 6f72 6d65 723a 2054 6865 2069  ansformer: The i
+000169b0: 6e73 7461 6e63 6520 6f66 2074 6869 7320  nstance of this 
+000169c0: 7472 616e 7366 6f72 6d65 722e 0a20 2020  transformer..   
+000169d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000169e0: 2058 5f73 6361 6c65 6420 3d20 7365 6c66   X_scaled = self
+000169f0: 2e73 6361 6c65 722e 6669 745f 7472 616e  .scaler.fit_tran
+00016a00: 7366 6f72 6d28 5829 0a20 2020 2020 2020  sform(X).       
+00016a10: 2073 656c 662e 6d6f 6465 6c2e 6669 7428   self.model.fit(
+00016a20: 585f 7363 616c 6564 2c20 7929 0a20 2020  X_scaled, y).   
+00016a30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00016a40: 0a0a 2020 2020 6465 6620 7472 616e 7366  ..    def transf
+00016a50: 6f72 6d28 7365 6c66 2c20 583a 206e 702e  orm(self, X: np.
+00016a60: 6e64 6172 7261 7929 202d 3e20 6e70 2e6e  ndarray) -> np.n
+00016a70: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
+00016a80: 2222 220a 2020 2020 2020 2020 5472 616e  """.        Tran
+00016a90: 7366 6f72 6d20 7468 6520 696e 7075 7420  sform the input 
+00016aa0: 6461 7461 2062 7920 7363 616c 696e 672c  data by scaling,
+00016ab0: 206d 616b 696e 6720 7072 6564 6963 7469   making predicti
+00016ac0: 6f6e 732c 2061 6e64 2063 616c 6375 6c61  ons, and calcula
+00016ad0: 7469 6e67 2070 6572 2d72 6f77 2073 7461  ting per-row sta
+00016ae0: 7469 7374 6963 732e 0a0a 2020 2020 2020  tistics...      
+00016af0: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+00016b00: 2020 2020 2020 5820 286e 702e 6e64 6172        X (np.ndar
+00016b10: 7261 7929 3a20 4461 7461 2074 6f20 7472  ray): Data to tr
+00016b20: 616e 7366 6f72 6d2e 0a0a 2020 2020 2020  ansform...      
+00016b30: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00016b40: 2020 206e 702e 6e64 6172 7261 793a 2054     np.ndarray: T
+00016b50: 7261 6e73 666f 726d 6564 2064 6174 6120  ransformed data 
+00016b60: 696e 636c 7564 696e 6720 6c61 7374 2065  including last e
+00016b70: 6c65 6d65 6e74 732c 2070 7265 6469 6374  lements, predict
+00016b80: 696f 6e73 2c20 7374 616e 6461 7264 2064  ions, standard d
+00016b90: 6576 6961 7469 6f6e 732c 2061 6e64 2052  eviations, and R
+00016ba0: 5349 2076 616c 7565 732e 0a20 2020 2020  SI values..     
+00016bb0: 2020 2022 2222 0a20 2020 2020 2020 2058     """.        X
+00016bc0: 5f73 6361 6c65 6420 3d20 7365 6c66 2e73  _scaled = self.s
+00016bd0: 6361 6c65 722e 7472 616e 7366 6f72 6d28  caler.transform(
+00016be0: 5829 0a20 2020 2020 2020 2070 7265 6469  X).        predi
+00016bf0: 6374 696f 6e73 203d 2073 656c 662e 6d6f  ctions = self.mo
+00016c00: 6465 6c2e 7072 6564 6963 7428 585f 7363  del.predict(X_sc
+00016c10: 616c 6564 290a 0a20 2020 2020 2020 2023  aled)..        #
+00016c20: 2043 616c 6375 6c61 7465 2073 7461 6e64   Calculate stand
+00016c30: 6172 6420 6465 7669 6174 696f 6e20 616e  ard deviation an
+00016c40: 6420 5253 4920 666f 7220 6561 6368 2072  d RSI for each r
+00016c50: 6f77 0a20 2020 2020 2020 2073 645f 7065  ow.        sd_pe
+00016c60: 725f 726f 7720 3d20 6e70 2e61 7272 6179  r_row = np.array
+00016c70: 285b 7365 6c66 2e63 616c 6375 6c61 7465  ([self.calculate
+00016c80: 5f75 7469 6c2e 6361 6c63 756c 6174 655f  _util.calculate_
+00016c90: 7374 616e 6461 7264 5f64 6576 6961 7469  standard_deviati
+00016ca0: 6f6e 5f77 656c 666f 7264 2872 6f77 2920  on_welford(row) 
+00016cb0: 666f 7220 726f 7720 696e 2058 5d29 0a20  for row in X]). 
+00016cc0: 2020 2020 2020 2072 7369 5f70 6572 5f72         rsi_per_r
+00016cd0: 6f77 203d 206e 702e 6172 7261 7928 5b73  ow = np.array([s
+00016ce0: 656c 662e 6d6f 6465 6c5f 7574 696c 2e72  elf.model_util.r
+00016cf0: 656c 6174 6976 655f 7374 7265 6e67 7468  elative_strength
+00016d00: 5f69 6e64 6578 2872 6f77 2c20 7065 7269  _index(row, peri
+00016d10: 6f64 3d6c 656e 2872 6f77 2920 2f2f 2032  od=len(row) // 2
+00016d20: 2920 666f 7220 726f 7720 696e 2058 5d29  ) for row in X])
+00016d30: 0a0a 2020 2020 2020 2020 2320 4578 7472  ..        # Extr
+00016d40: 6163 7420 7468 6520 6c61 7374 2065 6c65  act the last ele
+00016d50: 6d65 6e74 2066 726f 6d20 6561 6368 2072  ment from each r
+00016d60: 6f77 0a20 2020 2020 2020 206c 6173 745f  ow.        last_
+00016d70: 656c 656d 656e 7473 203d 2058 5b3a 2c20  elements = X[:, 
+00016d80: 2d31 5d0a 0a20 2020 2020 2020 2023 2043  -1]..        # C
+00016d90: 6f6d 6269 6e65 2061 6c6c 2074 6865 2063  ombine all the c
+00016da0: 6f6d 7075 7465 6420 6665 6174 7572 6573  omputed features
+00016db0: 2069 6e74 6f20 6120 7369 6e67 6c65 2061   into a single a
+00016dc0: 7272 6179 0a20 2020 2020 2020 2074 7261  rray.        tra
+00016dd0: 6e73 666f 726d 6564 5f64 6174 6120 3d20  nsformed_data = 
+00016de0: 6e70 2e63 5f5b 6c61 7374 5f65 6c65 6d65  np.c_[last_eleme
+00016df0: 6e74 732c 2070 7265 6469 6374 696f 6e73  nts, predictions
+00016e00: 2c20 7364 5f70 6572 5f72 6f77 2c20 7273  , sd_per_row, rs
+00016e10: 695f 7065 725f 726f 775d 0a20 2020 2020  i_per_row].     
+00016e20: 2020 2072 6574 7572 6e20 7472 616e 7366     return transf
+00016e30: 6f72 6d65 645f 6461 7461 0a0a 0a69 6620  ormed_data...if 
+00016e40: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00016e50: 6169 6e5f 5f27 3a0a 2020 2020 7061 7373  ain__':.    pass
+00016e60: 0a                                       .
```

### Comparing `lottokit-1.2/lottokit.egg-info/PKG-INFO` & `lottokit-1.3/lottokit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 1.2
+Version: 1.3
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.9
```

### Comparing `lottokit-1.2/setup.py` & `lottokit-1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lottokit',
-    version='1.2',
+    version='1.3',
     keywords=['lottokit', 'lottery'],
     packages=find_packages(),
     package_data={"": ["LICENSE", "NOTICE"]},
     include_package_data=True,
     author="nickdecodes",
     author_email="nickdecodes@163.com",
     description="Lotto Kit Package",
@@ -33,14 +33,15 @@
         'webdriver_manager>=4.0.0',
         'pandas>=2.0.3',
         'numpy>=1.24.3',
         'statsmodels>=0.14.0',
         'Pillow>=9.5.0',
         'scikit-learn>=1.3.2',
         'pmdarima>=2.0.4',
+        'pywavelets>=1.6.0',
         'requests',
         'twine'
     ],
     project_urls={
         "Documentation": "http://python-lottokit.readthedocs.io",
         "Source": "https://github.com/nickdecodes/python-lottokit",
     },
```

