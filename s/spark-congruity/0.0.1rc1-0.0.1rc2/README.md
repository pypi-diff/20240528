# Comparing `tmp/spark_congruity-0.0.1rc1.tar.gz` & `tmp/spark_congruity-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_congruity-0.0.1rc1.tar", max compression
+gzip compressed data, was "spark_congruity-0.0.1rc2.tar", max compression
```

## Comparing `spark_congruity-0.0.1rc1.tar` & `spark_congruity-0.0.1rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-05-16 15:30:11.346106 spark_congruity-0.0.1rc1/LICENSE
--rw-r--r--   0        0        0     1150 2024-05-16 15:30:11.346106 spark_congruity-0.0.1rc1/NOTICE
--rw-r--r--   0        0        0    14765 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/README.md
--rw-r--r--   0        0        0     2146 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/congruity/__init__.py
--rw-r--r--   0        0        0     1594 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/congruity/json_conversion.py
--rw-r--r--   0        0        0     8890 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/congruity/rdd_adapter.py
--rw-r--r--   0        0        0     1544 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/congruity/spark_context_adapter.py
--rw-r--r--   0        0        0     2206 2024-05-16 15:30:11.350106 spark_congruity-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0    15699 1970-01-01 00:00:00.000000 spark_congruity-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 20:50:14.666148 spark_congruity-0.0.1rc2/LICENSE
+-rw-r--r--   0        0        0     1150 2024-05-28 20:50:14.666148 spark_congruity-0.0.1rc2/NOTICE
+-rw-r--r--   0        0        0    15808 2024-05-28 20:50:14.666148 spark_congruity-0.0.1rc2/README.md
+-rw-r--r--   0        0        0     2146 2024-05-28 20:50:14.666148 spark_congruity-0.0.1rc2/congruity/__init__.py
+-rw-r--r--   0        0        0     1594 2024-05-28 20:50:14.666148 spark_congruity-0.0.1rc2/congruity/json_conversion.py
+-rw-r--r--   0        0        0    18998 2024-05-28 20:50:14.666148 spark_congruity-0.0.1rc2/congruity/rdd_adapter.py
+-rw-r--r--   0        0        0     1720 2024-05-28 20:50:14.666148 spark_congruity-0.0.1rc2/congruity/spark_context_adapter.py
+-rw-r--r--   0        0        0     2206 2024-05-28 20:50:14.666148 spark_congruity-0.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0    16742 1970-01-01 00:00:00.000000 spark_congruity-0.0.1rc2/PKG-INFO
```

### Comparing `spark_congruity-0.0.1rc1/LICENSE` & `spark_congruity-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc1/NOTICE` & `spark_congruity-0.0.1rc2/NOTICE`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc1/README.md` & `spark_congruity-0.0.1rc2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # congruity
 
+[![GitHub Actions Build](https://github.com/databricks/congruity/actions/workflows/main.yml/badge.svg)](https://github.com/databricks/congruity/actions/workflows/main.yml)
+[![PyPI Downloads](https://static.pepy.tech/personalized-badge/spark-congruity?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads)](https://pypi.org/project/spark-congruity/)
+
 In many ways, the migration from using classic Spark applications using the full
 power and flexibility to be using only the Spark Connect compatible DataFrame API
 can be challenging.
 
 The goal of this library is to provide a compatibility layer that makes it easier to
 adopt Spark Connect. The library is designed to be simply imported in your application
 and will then monkey-patch the existing API to provide the legacy functionality.
@@ -28,15 +31,14 @@
 ```
 
 ### Example
 
 Here is code that works on Spark JVM:
 
 ```python
-import congruity  # noqa: F401
 from pyspark.sql import SparkSession
 
 spark = SparkSession.builder.remote("sc://localhost").getOrCreate()
 data = [("Java", "20000"), ("Python", "100000"), ("Scala", "3000")]
 spark.sparkContext.parallelize(data).toDF()
 ```
 
@@ -48,119 +50,133 @@
 from pyspark.sql import SparkSession
 
 spark = SparkSession.builder.remote("sc://localhost").getOrCreate()
 data = [("Java", "20000"), ("Python", "100000"), ("Scala", "3000")]
 spark.sparkContext.parallelize(data).toDF()
 ```
 
-## Whats supported?
+## Contributing
+
+We very much welcome contributions to this project. The easiest way to start is to pick any of
+the below RDD or SparkContext methods and implement the compatibility layer. Once you have done
+that open a pull request and we will review it.
+
+## What's supported?
 
 ### RDD
 
 | RDD                               | API                | Comment                                                           |
 |-----------------------------------|--------------------|-------------------------------------------------------------------|
-| aggregate                         | :x:                |                                                                   |
+| aggregate                         | :white_check_mark: |                                                                   |
 | aggregateByKey                    | :x:                |                                                                   |
 | barrier                           | :x:                |                                                                   |
 | cache                             | :x:                |                                                                   |
 | cartesian                         | :x:                |                                                                   |
 | checkpoint                        | :x:                |                                                                   |
 | cleanShuffleDependencies          | :x:                |                                                                   |
 | coalesce                          | :x:                |                                                                   |
 | cogroup                           | :x:                |                                                                   |
 | collect                           | :white_check_mark: |                                                                   |
 | collectAsMap                      | :x:                |                                                                   |
 | collectWithJobGroup               | :x:                |                                                                   |
 | combineByKey                      | :x:                |                                                                   |
-| count                             | :x:                |                                                                   |
+| count                             | :white_check_mark: |                                                                   |
 | countApprox                       | :x:                |                                                                   |
 | countByKey                        | :x:                |                                                                   |
 | countByValue                      | :x:                |                                                                   |
 | distinct                          | :x:                |                                                                   |
-| filter                            | :x:                |                                                                   |
+| filter                            | :white_check_mark: |                                                                   |
 | first                             | :white_check_mark: |                                                                   |
 | flatMap                           | :x:                |                                                                   |
-| fold                              | :x:                |                                                                   |
+| fold                              | :white_check_mark: | First version                                                     |
 | foreach                           | :x:                |                                                                   |
 | foreachPartition                  | :x:                |                                                                   |
 | fullOuterJoin                     | :x:                |                                                                   |
 | getCheckpointFile                 | :x:                |                                                                   |
 | getNumPartitions                  | :x:                |                                                                   |
 | getResourceProfile                | :x:                |                                                                   |
 | getStorageLevel                   | :x:                |                                                                   |
-| glom                              | :x:                |                                                                   |
-| groupBy                           | :x:                |                                                                   |
-| groupByKey                        | :x:                |                                                                   |
+| glom                              | :white_check_mark: |                                                                   |
+| groupBy                           | :white_check_mark: |                                                                   |
+| groupByKey                        | :white_check_mark: |                                                                   |
 | groupWith                         | :x:                |                                                                   |
-| histogram                         | :x:                |                                                                   |
+| histogram                         | :white_check_mark: |                                                                   |
 | id                                | :x:                |                                                                   |
 | intersection                      | :x:                |                                                                   |
 | isCheckpointed                    | :x:                |                                                                   |
 | isEmpty                           | :x:                |                                                                   |
 | isLocallyCheckpointed             | :x:                |                                                                   |
 | join                              | :x:                |                                                                   |
-| keys                              | :x:                |                                                                   |
+| keyBy                             | :white_check_mark: |                                                                   |
+| keys                              | :white_check_mark: |                                                                   |
 | leftOuterJoin                     | :x:                |                                                                   |
 | localCheckpoint                   | :x:                |                                                                   |
 | lookup                            | :x:                |                                                                   |
 | map                               | :white_check_mark: |                                                                   |
-| mapPartitions                     | :x:                |                                                                   |
+| mapPartitions                     | :white_check_mark: | First version, based on mapInArrow.                               |
 | mapPartitionsWithIndex            | :x:                |                                                                   |
 | mapPartitionsWithSplit            | :x:                |                                                                   |
-| mapValues                         | :x:                |                                                                   |
-| max                               | :x:                |                                                                   |
-| mean                              | :x:                |                                                                   |
+| mapValues                         | :white_check_mark: |                                                                   |
+| max                               | :white_check_mark: |                                                                   |
+| mean                              | :white_check_mark: |                                                                   |
 | meanApprox                        | :x:                |                                                                   |
-| min                               | :x:                |                                                                   |
+| min                               | :white_check_mark: |                                                                   |
 | name                              | :x:                |                                                                   |
 | partitionBy                       | :x:                |                                                                   |
 | persist                           | :x:                |                                                                   |
 | pipe                              | :x:                |                                                                   |
 | randomSplit                       | :x:                |                                                                   |
-| reduce                            | :x:                |                                                                   |
+| reduce                            | :white_check_mark: |                                                                   |
 | reduceByKey                       | :x:                |                                                                   |
 | repartition                       | :x:                |                                                                   |
 | repartitionAndSortWithinPartition | :x:                |                                                                   |
 | rightOuterJoin                    | :x:                |                                                                   |
 | sample                            | :x:                |                                                                   |
 | sampleByKey                       | :x:                |                                                                   |
-| sampleStdev                       | :x:                |                                                                   |
-| sampleVariance                    | :x:                |                                                                   |
+| sampleStdev                       | :white_check_mark: |                                                                   |
+| sampleVariance                    | :white_check_mark: |                                                                   |
 | saveAsHadoopDataset               | :x:                |                                                                   |
 | saveAsHadoopFile                  | :x:                |                                                                   |
 | saveAsNewAPIHadoopDataset         | :x:                |                                                                   |
 | saveAsNewAPIHadoopFile            | :x:                |                                                                   |
 | saveAsPickleFile                  | :x:                |                                                                   |
 | saveAsTextFile                    | :x:                |                                                                   |
 | setName                           | :x:                |                                                                   |
 | sortBy                            | :x:                |                                                                   |
 | sortByKey                         | :x:                |                                                                   |
-| stats                             | :x:                |                                                                   |
-| stdev                             | :x:                |                                                                   |
+| stats                             | :white_check_mark: |                                                                   |
+| stdev                             | :white_check_mark: |                                                                   |
 | subtract                          | :x:                |                                                                   |
 | substractByKey                    | :x:                |                                                                   |
-| sum                               | :x:                |                                                                   |
+| sum                               | :white_check_mark: | First version.                                                    |
 | sumApprox                         | :x:                |                                                                   |
 | take                              | :white_check_mark: | Ordering might not be guaranteed in the same way as it is in RDD. |
 | takeOrdered                       | :x:                |                                                                   |
 | takeSample                        | :x:                |                                                                   |
-| toDF                              | :x:                |                                                                   |
+| toDF                              | :white_check_mark: |                                                                   |
 | toDebugString                     | :x:                |                                                                   |
 | toLocalIterator                   | :x:                |                                                                   |
 | top                               | :x:                |                                                                   |
 | treeAggregate                     | :x:                |                                                                   |
 | treeReduce                        | :x:                |                                                                   |
 | union                             | :x:                |                                                                   |
 | unpersist                         | :x:                |                                                                   |
-| values                            | :x:                |                                                                   |
-| variance                          | :x:                |                                                                   |
+| values                            | :white_check_mark: |                                                                   |
+| variance                          | :white_check_mark: |                                                                   |
 | withResources                     | :x:                |                                                                   |
 | zip                               | :x:                |                                                                   |
 | zipWithIndex                      | :x:                |                                                                   |
 | zipWithUniqueId                   | :x:                |                                                                   |
 
 ### SparkContext
 
 | RDD         | API                | Comment                         |
 |-------------|--------------------|---------------------------------|
 | parallelize | :white_check_mark: | Does not support numSlices yet. |
 
+## Limitations
+
+* Error handling and checking is kind of limited right now. We try
+  to emulate the existing behavior, but this is not always possible
+  because the invariants are not encode in Python but rather somewhere
+  in Scala.
+* `numSlices` - we don't emulate this behavior for now.
```

### Comparing `spark_congruity-0.0.1rc1/congruity/__init__.py` & `spark_congruity-0.0.1rc2/congruity/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc1/congruity/json_conversion.py` & `spark_congruity-0.0.1rc2/congruity/json_conversion.py`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc1/congruity/spark_context_adapter.py` & `spark_congruity-0.0.1rc2/congruity/spark_context_adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,16 +24,21 @@
 class SparkContextAdapter:
     _spark: SparkSession
 
     def __init__(self, spark: SparkSession):
         self._spark = spark
 
     def parallelize(self, data: Any, slices: Optional[int] = None) -> "RDDAdapter":
+        # TODO - the slices argument is not ideal here.
         # Create the binary DF from the data
         serialized = map(lambda x: dumps(x), data)
+        base_df = self._spark.createDataFrame(serialized, RDDAdapter.BIN_SCHEMA)
+        if slices is not None:
+            base_df = base_df.repartition(slices)
         return RDDAdapter(
-            self._spark.createDataFrame(serialized, RDDAdapter.BIN_SCHEMA), first_field=True
+            base_df,
+            first_field=True,
         )
 
 
 def adapt_to_spark_context(self: DataFrame) -> SparkContextAdapter:
     return SparkContextAdapter(self)
```

### Comparing `spark_congruity-0.0.1rc1/pyproject.toml` & `spark_congruity-0.0.1rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "spark-congruity"
-version = "0.0.1rc1"
+version = "0.0.1rc2"
 description = ""
 authors = ["Matthew Powers <matthewkevinpowers@gmail.com>", "Martin Grund <martin@databricks.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/databricks/congruity"
 repository = "https://github.com/databricks/congruity"
 classifiers = [
```

### Comparing `spark_congruity-0.0.1rc1/PKG-INFO` & `spark_congruity-0.0.1rc2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-congruity
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: 
 Home-page: https://github.com/databricks/congruity
 License: Apache-2.0
 Author: Matthew Powers
 Author-email: matthewkevinpowers@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/databricks/congruity
 Description-Content-Type: text/markdown
 
 # congruity
 
+[![GitHub Actions Build](https://github.com/databricks/congruity/actions/workflows/main.yml/badge.svg)](https://github.com/databricks/congruity/actions/workflows/main.yml)
+[![PyPI Downloads](https://static.pepy.tech/personalized-badge/spark-congruity?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads)](https://pypi.org/project/spark-congruity/)
+
 In many ways, the migration from using classic Spark applications using the full
 power and flexibility to be using only the Spark Connect compatible DataFrame API
 can be challenging.
 
 The goal of this library is to provide a compatibility layer that makes it easier to
 adopt Spark Connect. The library is designed to be simply imported in your application
 and will then monkey-patch the existing API to provide the legacy functionality.
@@ -52,15 +55,14 @@
 ```
 
 ### Example
 
 Here is code that works on Spark JVM:
 
 ```python
-import congruity  # noqa: F401
 from pyspark.sql import SparkSession
 
 spark = SparkSession.builder.remote("sc://localhost").getOrCreate()
 data = [("Java", "20000"), ("Python", "100000"), ("Scala", "3000")]
 spark.sparkContext.parallelize(data).toDF()
 ```
 
@@ -72,120 +74,133 @@
 from pyspark.sql import SparkSession
 
 spark = SparkSession.builder.remote("sc://localhost").getOrCreate()
 data = [("Java", "20000"), ("Python", "100000"), ("Scala", "3000")]
 spark.sparkContext.parallelize(data).toDF()
 ```
 
-## Whats supported?
+## Contributing
+
+We very much welcome contributions to this project. The easiest way to start is to pick any of
+the below RDD or SparkContext methods and implement the compatibility layer. Once you have done
+that open a pull request and we will review it.
+
+## What's supported?
 
 ### RDD
 
 | RDD                               | API                | Comment                                                           |
 |-----------------------------------|--------------------|-------------------------------------------------------------------|
-| aggregate                         | :x:                |                                                                   |
+| aggregate                         | :white_check_mark: |                                                                   |
 | aggregateByKey                    | :x:                |                                                                   |
 | barrier                           | :x:                |                                                                   |
 | cache                             | :x:                |                                                                   |
 | cartesian                         | :x:                |                                                                   |
 | checkpoint                        | :x:                |                                                                   |
 | cleanShuffleDependencies          | :x:                |                                                                   |
 | coalesce                          | :x:                |                                                                   |
 | cogroup                           | :x:                |                                                                   |
 | collect                           | :white_check_mark: |                                                                   |
 | collectAsMap                      | :x:                |                                                                   |
 | collectWithJobGroup               | :x:                |                                                                   |
 | combineByKey                      | :x:                |                                                                   |
-| count                             | :x:                |                                                                   |
+| count                             | :white_check_mark: |                                                                   |
 | countApprox                       | :x:                |                                                                   |
 | countByKey                        | :x:                |                                                                   |
 | countByValue                      | :x:                |                                                                   |
 | distinct                          | :x:                |                                                                   |
-| filter                            | :x:                |                                                                   |
+| filter                            | :white_check_mark: |                                                                   |
 | first                             | :white_check_mark: |                                                                   |
 | flatMap                           | :x:                |                                                                   |
-| fold                              | :x:                |                                                                   |
+| fold                              | :white_check_mark: | First version                                                     |
 | foreach                           | :x:                |                                                                   |
 | foreachPartition                  | :x:                |                                                                   |
 | fullOuterJoin                     | :x:                |                                                                   |
 | getCheckpointFile                 | :x:                |                                                                   |
 | getNumPartitions                  | :x:                |                                                                   |
 | getResourceProfile                | :x:                |                                                                   |
 | getStorageLevel                   | :x:                |                                                                   |
-| glom                              | :x:                |                                                                   |
-| groupBy                           | :x:                |                                                                   |
-| groupByKey                        | :x:                |                                                                   |
+| glom                              | :white_check_mark: |                                                                   |
+| groupBy                           | :white_check_mark: |                                                                   |
+| groupByKey                        | :white_check_mark: |                                                                   |
 | groupWith                         | :x:                |                                                                   |
-| histogram                         | :x:                |                                                                   |
+| histogram                         | :white_check_mark: |                                                                   |
 | id                                | :x:                |                                                                   |
 | intersection                      | :x:                |                                                                   |
 | isCheckpointed                    | :x:                |                                                                   |
 | isEmpty                           | :x:                |                                                                   |
 | isLocallyCheckpointed             | :x:                |                                                                   |
 | join                              | :x:                |                                                                   |
-| keys                              | :x:                |                                                                   |
+| keyBy                             | :white_check_mark: |                                                                   |
+| keys                              | :white_check_mark: |                                                                   |
 | leftOuterJoin                     | :x:                |                                                                   |
 | localCheckpoint                   | :x:                |                                                                   |
 | lookup                            | :x:                |                                                                   |
 | map                               | :white_check_mark: |                                                                   |
-| mapPartitions                     | :x:                |                                                                   |
+| mapPartitions                     | :white_check_mark: | First version, based on mapInArrow.                               |
 | mapPartitionsWithIndex            | :x:                |                                                                   |
 | mapPartitionsWithSplit            | :x:                |                                                                   |
-| mapValues                         | :x:                |                                                                   |
-| max                               | :x:                |                                                                   |
-| mean                              | :x:                |                                                                   |
+| mapValues                         | :white_check_mark: |                                                                   |
+| max                               | :white_check_mark: |                                                                   |
+| mean                              | :white_check_mark: |                                                                   |
 | meanApprox                        | :x:                |                                                                   |
-| min                               | :x:                |                                                                   |
+| min                               | :white_check_mark: |                                                                   |
 | name                              | :x:                |                                                                   |
 | partitionBy                       | :x:                |                                                                   |
 | persist                           | :x:                |                                                                   |
 | pipe                              | :x:                |                                                                   |
 | randomSplit                       | :x:                |                                                                   |
-| reduce                            | :x:                |                                                                   |
+| reduce                            | :white_check_mark: |                                                                   |
 | reduceByKey                       | :x:                |                                                                   |
 | repartition                       | :x:                |                                                                   |
 | repartitionAndSortWithinPartition | :x:                |                                                                   |
 | rightOuterJoin                    | :x:                |                                                                   |
 | sample                            | :x:                |                                                                   |
 | sampleByKey                       | :x:                |                                                                   |
-| sampleStdev                       | :x:                |                                                                   |
-| sampleVariance                    | :x:                |                                                                   |
+| sampleStdev                       | :white_check_mark: |                                                                   |
+| sampleVariance                    | :white_check_mark: |                                                                   |
 | saveAsHadoopDataset               | :x:                |                                                                   |
 | saveAsHadoopFile                  | :x:                |                                                                   |
 | saveAsNewAPIHadoopDataset         | :x:                |                                                                   |
 | saveAsNewAPIHadoopFile            | :x:                |                                                                   |
 | saveAsPickleFile                  | :x:                |                                                                   |
 | saveAsTextFile                    | :x:                |                                                                   |
 | setName                           | :x:                |                                                                   |
 | sortBy                            | :x:                |                                                                   |
 | sortByKey                         | :x:                |                                                                   |
-| stats                             | :x:                |                                                                   |
-| stdev                             | :x:                |                                                                   |
+| stats                             | :white_check_mark: |                                                                   |
+| stdev                             | :white_check_mark: |                                                                   |
 | subtract                          | :x:                |                                                                   |
 | substractByKey                    | :x:                |                                                                   |
-| sum                               | :x:                |                                                                   |
+| sum                               | :white_check_mark: | First version.                                                    |
 | sumApprox                         | :x:                |                                                                   |
 | take                              | :white_check_mark: | Ordering might not be guaranteed in the same way as it is in RDD. |
 | takeOrdered                       | :x:                |                                                                   |
 | takeSample                        | :x:                |                                                                   |
-| toDF                              | :x:                |                                                                   |
+| toDF                              | :white_check_mark: |                                                                   |
 | toDebugString                     | :x:                |                                                                   |
 | toLocalIterator                   | :x:                |                                                                   |
 | top                               | :x:                |                                                                   |
 | treeAggregate                     | :x:                |                                                                   |
 | treeReduce                        | :x:                |                                                                   |
 | union                             | :x:                |                                                                   |
 | unpersist                         | :x:                |                                                                   |
-| values                            | :x:                |                                                                   |
-| variance                          | :x:                |                                                                   |
+| values                            | :white_check_mark: |                                                                   |
+| variance                          | :white_check_mark: |                                                                   |
 | withResources                     | :x:                |                                                                   |
 | zip                               | :x:                |                                                                   |
 | zipWithIndex                      | :x:                |                                                                   |
 | zipWithUniqueId                   | :x:                |                                                                   |
 
 ### SparkContext
 
 | RDD         | API                | Comment                         |
 |-------------|--------------------|---------------------------------|
 | parallelize | :white_check_mark: | Does not support numSlices yet. |
 
+## Limitations
 
+* Error handling and checking is kind of limited right now. We try
+  to emulate the existing behavior, but this is not always possible
+  because the invariants are not encode in Python but rather somewhere
+  in Scala.
+* `numSlices` - we don't emulate this behavior for now.
```

