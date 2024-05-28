# Comparing `tmp/timelined_array-0.0.5.tar.gz` & `tmp/timelined_array-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelined_array-0.0.5.tar", last modified: Mon May 27 23:43:09 2024, max compression
+gzip compressed data, was "timelined_array-0.0.6.tar", last modified: Tue May 28 14:29:52 2024, max compression
```

## Comparing `timelined_array-0.0.5.tar` & `timelined_array-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-27 23:42:56.507636 timelined_array-0.0.5/LICENSE
--rw-r--r--   0        0        0     2859 2024-05-27 23:42:56.507636 timelined_array-0.0.5/README.md
--rw-r--r--   0        0        0      613 2024-05-27 23:43:09.927599 timelined_array-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       97 2024-05-27 23:42:56.507636 timelined_array-0.0.5/src/timelined_array/__init__.py
--rw-r--r--   0        0        0    50908 2024-05-27 23:42:56.511636 timelined_array-0.0.5/src/timelined_array/time.py
--rw-r--r--   0        0        0        0 2024-05-27 23:42:56.511636 timelined_array-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 timelined_array-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 14:29:37.323919 timelined_array-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2859 2024-05-28 14:29:37.323919 timelined_array-0.0.6/README.md
+-rw-r--r--   0        0        0      613 2024-05-28 14:29:52.311951 timelined_array-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-05-28 14:29:37.323919 timelined_array-0.0.6/src/timelined_array/__init__.py
+-rw-r--r--   0        0        0    52532 2024-05-28 14:29:37.323919 timelined_array-0.0.6/src/timelined_array/time.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:29:37.323919 timelined_array-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 timelined_array-0.0.6/PKG-INFO
```

### Comparing `timelined_array-0.0.5/LICENSE` & `timelined_array-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `timelined_array-0.0.5/README.md` & `timelined_array-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `timelined_array-0.0.5/pyproject.toml` & `timelined_array-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 dependencies = [
     "numpy",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dynamic = []
-version = "0.0.5"
+version = "0.0.6"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `timelined_array-0.0.5/src/timelined_array/time.py` & `timelined_array-0.0.6/src/timelined_array/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     timeline: "Timeline"
 
     def __getitem__(self, index) -> np.ndarray: ...
 
     def __array__(self) -> np.ndarray: ...
 
     @property
-    def shape(self) -> Tuple[int]: ...
+    def shape(self) -> Tuple[int, ...]: ...
 
     @property
     def ndim(self) -> int: ...
 
     @property
     def itime(self) -> "TimeIndexer": ...
 
@@ -343,19 +343,19 @@
 
 
 class TimeMixin:
 
     time_dimension: int
     timeline: Timeline
 
-    def _time_dimension_in_axis(self, axis: int | Tuple[int] | None) -> bool:
+    def _time_dimension_in_axis(self, axis: int | Tuple[int, ...] | None) -> bool:
         """Check if the time dimension is present in the specified axis.
 
         Args:
-            axis (int | Tuple[int] | None): The axis to check for the time dimension.
+            axis (int | Tuple[int, ...] | None): The axis to check for the time dimension.
 
         Returns:
             bool: True if the time dimension is present in the axis, False otherwise.
         """
 
         if (
             axis is None
@@ -498,19 +498,19 @@
 
         final_timeline = (
             self.timeline[index[time_dimension_in_index]] if len(index) > time_dimension_in_index else self.timeline
         )
 
         return index, final_timeline, final_time_dimension
 
-    def _get_indexed_times(self, index: int | Tuple[int] | slice | Tuple[slice] | List | np.ndarray):
+    def _get_indexed_times(self, index: int | Tuple[int, ...] | slice | Tuple[slice] | List | np.ndarray):
         """Get indexed times based on the provided index.
 
         Args:
-            index (int | Tuple[int] | slice | Tuple[slice] | List | np.ndarray): The index to retrieve times from.
+            index (int | Tuple[int, ...] | slice | Tuple[slice] | List | np.ndarray): The index to retrieve times from.
 
         Returns:
             np.ndarray: The indexed times based on the provided index.
         """
 
         # if index is an array or a list, we do advanced indexing.
         if isinstance(index, (np.ndarray, list)):
@@ -527,28 +527,28 @@
 
         Returns:
             bool: True if the input object is a single element, False otherwise.
         """
 
         return obj.shape == ()
 
-    def _finish_axis_removing_operation(self, result: TimeCompatibleProtocol, axis: int | Tuple[int] | None):
+    def _finish_axis_removing_operation(self, result: TimeCompatibleProtocol, axis: int | Tuple[int, ...] | None):
         """Finish axis removing operation.
 
         Args:
             result (TimeCompatibleProtocol): The result of the operation.
-            axis (int | Tuple[int] | None): The axis or axes to remove.
+            axis (int | Tuple[int, ...] | None): The axis or axes to remove.
 
         Returns:
             TimeCompatibleProtocol: The result after finishing the axis removing operation.
         """
 
         if not isinstance(result, np.ndarray):
             return result
-        if not self._is_single_element(result):
+        if self._is_single_element(result):
             return result.item()
         if self._time_dimension_in_axis(axis):
             return np.asarray(result)
         result.time_dimension = self._get_time_dimension_after_axis_removal(axis)
         return result
 
     # # REDUCE and SETSTATE are used to instanciate the array from and to a pickled serialized object.
@@ -637,14 +637,48 @@
 
         Returns:
             TimelinedArray: The synchronized and cut arrray.
         """
 
         return self.itime[start:][:element_nb]  # type: ignore
 
+    def shift_values(
+        self,
+        period: int | Tuple[int, ...] | slice | Tuple[slice, ...] | List | np.ndarray = 0,
+        axis=None,
+        time_period=True,
+    ):
+        """Shifts the values of the array along the specified axis by the given period.
+
+        Args:
+            period (int): The period by which to shift the values.
+            axis (int, optional): The axis along which to shift the values. Defaults to None.
+            time_period (bool, optional): If True, the shift is applied based on time. Defaults to True.
+
+        Returns:
+            numpy.ndarray: The array with shifted values.
+        """
+
+        if axis is None:
+            axis = self.time_dimension
+
+        indexer = []
+        for dim in range(len(self.shape)):
+            if dim == axis:
+                # make a new axis to account fo the axis loss of the .mean later
+                indexer.append(np.newaxis)
+            else:
+                # select all with slice(None) equivalent to ":"
+                indexer.append(slice(None))
+        indexer = tuple(indexer)
+
+        shift_area = self.itime.__getitem__(period) if time_period else self.__getitem__(period)
+
+        return self - np.repeat(shift_area.mean(axis=axis).__getitem__(tuple(indexer)), self.shape[axis], axis=axis)
+
     def swapaxes(self: TimeCompatibleProtocol, axis1: int, axis2: int):
         """Swap the two specified axes of the TimelinedArray.
 
         Args:
             axis1 (int): The first axis to be swapped.
             axis2 (int): The second axis to be swapped.
 
@@ -697,20 +731,20 @@
 
     @property
     def T(self: TimeCompatibleProtocol):
         """Transposes the object using the transpose method."""
 
         return self.transpose()
 
-    def moveaxis(self: TimeCompatibleProtocol, source: int | Tuple[int], destination: int | Tuple[int]):
+    def moveaxis(self: TimeCompatibleProtocol, source: int | Tuple[int, ...], destination: int | Tuple[int, ...]):
         """Move the axis of the array to new positions.
 
         Args:
-            source (int or Tuple[int]): The source position(s) of the axis to move.
-            destination (int or Tuple[int]): The destination position(s) to move the axis to.
+            source (int or Tuple[int, ...]): The source position(s) of the axis to move.
+            destination (int or Tuple[int, ...]): The destination position(s) to move the axis to.
 
         Returns:
             TimeCompatibleProtocol: A new array with the axis moved to the specified destination.
 
         Note:
             This method re-instantiates a TimelinedArray with a view instead of the full
             constructor for faster performance.
@@ -773,36 +807,41 @@
                 rolled_array.time_dimension -= 1
             elif start > self.time_dimension:
                 rolled_array.time_dimension += 1
 
         # TimelinedArray.time_dimension and TimelinedArray.timeline are set. good to go
         return rolled_array
 
-    def mean(self: TimeCompatibleProtocol, axis: int | Tuple[int] | None = None, dtype=None, out=None, keepdims=False):
+    def mean(
+        self: TimeCompatibleProtocol, axis: int | Tuple[int, ...] | None = None, dtype=None, out=None, keepdims=False
+    ):
         """Calculates the mean along the specified axis.
 
         Args:
-            axis (int | Tuple[int] | None): Axis or axes along which to perform the mean operation. Default is None.
+            axis (int | Tuple[int, ...] | None): Axis or axes along which to perform the mean operation.
+                Default is None.
             dtype: Data-type to use in the computation.
             out: Output array where the result is stored.
             keepdims (bool): If True, the reduced dimensions are retained in the output array.
 
         Returns:
             ndarray: Mean of the input array along the specified axis.
         """
 
         result = super().mean(axis=axis, dtype=dtype, out=out, keepdims=keepdims)
         return self._finish_axis_removing_operation(result, axis)
 
     # Override other reduction methods similarly if needed
-    def sum(self: TimeCompatibleProtocol, axis: int | Tuple[int] | None = None, dtype=None, out=None, keepdims=False):
+    def sum(
+        self: TimeCompatibleProtocol, axis: int | Tuple[int, ...] | None = None, dtype=None, out=None, keepdims=False
+    ):
         """Calculate the sum along the specified axis.
 
         Args:
-            axis (int | Tuple[int] | None): Axis or axes along which a sum is performed.
+            axis (int | Tuple[int, ...] | None): Axis or axes along which a sum is performed.
                 The default is to sum over all the dimensions of the input array.
             dtype: The type of the returned array and of the accumulator in which the elements are summed.
                 If dtype is not specified, it defaults to the dtype of a, unless a has an integer dtype
                 with a precision less than that of the default platform integer.
                 In that case, the default platform integer is used.
             out: Alternative output array in which to place the result. It must have the same shape
                 as the expected output, but the type of the output values will be cast if necessary.
@@ -814,20 +853,25 @@
             The sum of the input array along the specified axis.
         """
 
         result = super().sum(axis=axis, dtype=dtype, out=out, keepdims=keepdims)
         return self._finish_axis_removing_operation(result, axis)
 
     def std(
-        self: TimeCompatibleProtocol, axis: int | Tuple[int] | None = None, dtype=None, out=None, ddof=0, keepdims=False
+        self: TimeCompatibleProtocol,
+        axis: int | Tuple[int, ...] | None = None,
+        dtype=None,
+        out=None,
+        ddof=0,
+        keepdims=False,
     ):
         """Calculate the standard deviation along the specified axis.
 
         Args:
-            axis (int or Tuple[int] or None): Axis or axes along which the standard deviation is computed.
+            axis (int or Tuple[int, ...] or None): Axis or axes along which the standard deviation is computed.
                 The default is to compute the standard deviation of the flattened array.
             dtype: Data-type of the result. If not provided, the data-type of the input is used.
             out: Output array with the same shape as input array, placed with the result.
             ddof (int): Delta degrees of freedom. The divisor used in calculations is N - ddof,
                 where N represents the number of elements along the specified axis.
             keepdims (bool): If this is set to True, the axes which are reduced
                 are left in the result as dimensions with size one.
@@ -837,21 +881,26 @@
                 of elements along the specified axis after removing the axis.
         """
 
         result = super().std(axis=axis, dtype=dtype, out=out, ddof=ddof, keepdims=keepdims)
         return self._finish_axis_removing_operation(result, axis)
 
     def var(
-        self: TimeCompatibleProtocol, axis: int | Tuple[int] | None = None, dtype=None, out=None, ddof=0, keepdims=False
+        self: TimeCompatibleProtocol,
+        axis: int | Tuple[int, ...] | None = None,
+        dtype=None,
+        out=None,
+        ddof=0,
+        keepdims=False,
     ):
         """Calculate the variance along the specified axis.
 
         Args:
             self (TimeCompatibleProtocol): The input data.
-            axis (int | Tuple[int] | None): Axis or axes along which the variance is computed.
+            axis (int | Tuple[int, ...] | None): Axis or axes along which the variance is computed.
                 The default is to compute the variance of the flattened array.
             dtype: Data-type of the result. If not provided, the data-type of the input is used.
             out: Alternative output array in which to place the result.
                 It must have the same shape as the expected output but the type will be cast if necessary.
             ddof (int): Delta degrees of freedom. The divisor used in calculations is N - ddof,
                 where N represents the number of elements along the specified axis.
             keepdims (bool): If this is set to True, the axes which are reduced
@@ -1110,20 +1159,20 @@
             The result of calling the function on the array.
         """
 
         logger.debug(f"intercepting array before function {func.__name__}")
         return super().__array_function__(func, types, args, kwargs)
 
     def __getitem__(
-        self, index: int | Tuple[int] | slice | Tuple[slice] | List | np.ndarray
+        self, index: int | Tuple[int, ...] | slice | Tuple[slice, ...] | List | np.ndarray
     ) -> "TimelinedArray | np.ndarray":
         """Get item from TimelinedArray based on index or slice.
 
         Args:
-            index (int | Tuple[int] | slice | Tuple[slice] | List | np.ndarray): Index or slice to retrieve item.
+            index (int | Tuple[int, ...] | slice | Tuple[slice] | List | np.ndarray): Index or slice to retrieve item.
 
         Returns:
             TimelinedArray | np.ndarray: Indexed result based on the provided index.
         """
 
         index, final_timeline, final_time_dimension = self._get_indexed_times(index)
 
@@ -1141,21 +1190,22 @@
         return TimelinedArray(indexed_result, timeline=final_timeline, time_dimension=final_time_dimension)
 
     # __repr__ and __str__ ARE OVERRIDEN TO AVOID HORRIBLE PERFORMANCE WHEN PRINTING
     # DUE TO CUSTOM __GETITEM__ PRE-CHECKS WITH RECURSIVE NATIVE NUMPY REPR
     def __repr__(self):
         """Return a string representation of the object with the class name and the array representation."""
 
-        return type(self).__name__ + np.array(self).__repr__()[5:]
+        # [5:] serves to remove the 'array' part for the original array repr string
+        return type(self).__name__ + np.asarray(self).__repr__()[5:]
 
     def __str__(self):
         """Return a string representation of the object by concatenating the class name with the string
         representation of the object as a NumPy array."""
 
-        return type(self).__name__ + np.array(self).__str__()
+        return type(self).__name__ + np.asarray(self).__str__()
 
     @staticmethod
     def align_from_iterable(iterable) -> "TimelinedArray":
         """Aligns arrays from an iterable based on their timelines.
 
         Args:
             iterable: An iterable containing TimelinedArray objects to align.
@@ -1245,20 +1295,20 @@
         super().__array_finalize__(obj)
         if obj is None:
             return
         self.timeline = getattr(obj, "timeline", Timeline([]))
         self.time_dimension = getattr(obj, "time_dimension", 0)
 
     def __getitem__(
-        self, index: int | Tuple[int] | slice | Tuple[slice] | List | np.ndarray
+        self, index: int | Tuple[int, ...] | slice | Tuple[slice] | List | np.ndarray
     ) -> "MaskedTimelinedArray | np.ma.MaskedArray":
         """Get item from the MaskedTimelinedArray based on the provided index.
 
         Args:
-            index (int | Tuple[int] | slice | Tuple[slice] | List | np.ndarray): The index or slice to retrieve.
+            index (int | Tuple[int, ...] | slice | Tuple[slice] | List | np.ndarray): The index or slice to retrieve.
 
         Returns:
             MaskedTimelinedArray | np.ma.MaskedArray: The masked array or MaskedTimelinedArray based on the index.
         """
 
         index, final_timeline, final_time_dimension = self._get_indexed_times(index)
```

### Comparing `timelined_array-0.0.5/PKG-INFO` & `timelined_array-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timelined_array
-Version: 0.0.5
+Version: 0.0.6
 Summary: Manage easily 1 or multidimensionnal samples numpy arrays that are time related. Extends numpy without removing any of it's abilities on such arrays.
 Author-Email: Timothe Jost <timothe.jost@wanadoo.fr>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
```

