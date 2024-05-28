# Comparing `tmp/laktory-0.3.0.tar.gz` & `tmp/laktory-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laktory-0.3.0.tar", last modified: Tue May 28 04:50:35 2024, max compression
+gzip compressed data, was "laktory-0.3.1.tar", last modified: Tue May 28 05:24:43 2024, max compression
```

## Comparing `laktory-0.3.0.tar` & `laktory-0.3.1.tar`

### file list

```diff
@@ -1,511 +1,511 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.031995 laktory-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.939995 laktory-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/ISSUE_TEMPLATE/bug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/ISSUE_TEMPLATE/feature.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/scripts/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/scripts/update_quickstart_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/scripts/write_release_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/workflows/publish-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/workflows/run_quickstart.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-28 04:50:21.000000 laktory-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-05-28 04:50:21.000000 laktory-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 04:50:21.000000 laktory-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 04:50:21.000000 laktory-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-28 04:50:35.031995 laktory-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-28 04:50:21.000000 laktory-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/datetime.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/docs/api/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dispatcher/dispatcher.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dispatcher/dispatcherrunner.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dispatcher/jobrunner.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dispatcher/pipelinerunner.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/apply_changes.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/get_df.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/is_debug.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/is_mocked.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/read.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/read_stream.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/basemodel.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/dataproducer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/models/datasinks/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasinks/basedatasink.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasinks/filedatasink.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasinks/tabledatasink.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/basedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/filedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/memorydatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/pipelinenodedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/tabledatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/pipelinenode.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/pipelinenodeexpectation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/baseresource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/models/resources/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/accesscontrol.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/cluster.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/column.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/directory.md
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/dltpipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/externallocation.md
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/grants.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/group.md
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/job.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/metastore.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/metastoreassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/metastoredataaccess.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/mwspermissionassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/notebook.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/secret.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/secretacl.md
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/secretscope.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/serviceprincipal.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/serviceprincipalrole.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/sqlquery.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/user.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/userrole.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/volume.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/warehouse.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/workspacefile.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/models/resources/providers/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/providers/aws.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/providers/azure.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/providers/azurepulumi.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/providers/databricks.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/pulumiresource.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/terraformresource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/models/spark/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/spark/sparkchain.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/spark/sparkchainnode.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/spark/sparkfuncarg.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/stacks/pulumistack.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/stacks/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/stacks/terraformstack.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.943995 laktory-0.3.0/docs/api/spark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/groupby_and_agg.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/has_column.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/schema_flat.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/show_string.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/smart_join.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/window_filter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.967995 laktory-0.3.0/docs/api/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/_constants.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/add.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/convert_units.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/div.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/mul.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/poly1.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/poly2.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/roundp.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/scaled_power.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/string_split.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/sub.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/uuid.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.967995 laktory-0.3.0/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/governance.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.967995 laktory-0.3.0/docs/concepts/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/models.md
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/sourcessinks.md
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/sparkchain.md
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/spark.md
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/variables.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/demos.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.971995 laktory-0.3.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/compute.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/job.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/secrets.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/users.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.979995 laktory-0.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/databricks.png
--rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/delta_live_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)   240172 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/dlt_debug.png
--rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/kappa.png
--rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/lakehouse.png
--rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/logo_sg.png
--rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/logo_sg_ltb.png
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/logo_sw.png
--rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/logo_sw_ltw.png
--rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/medaillon_complex.png
--rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/medallion.png
--rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/okube.png
--rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/pl_quickstart.png
--rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/pl_stock_prices.png
--rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/pl_stock_prices_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/pulumi.png
--rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/stock_prices_lineage.png
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/terraform.png
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/what_is_laktory.png
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/lakehouseascode.md
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.979995 laktory-0.3.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/stylesheets/mkdocstrings.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.979995 laktory-0.3.0/laktory/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.983995 laktory-0.3.0/laktory/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_testing/stackvalidator.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_testing/stockprices.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.983995 laktory-0.3.0/laktory/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_quickstart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/quickstart_stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/dispatcherrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/dltpipelinerunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/jobrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dlt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/models/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/models/azurenative/
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/azurenative/storageblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16431 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/dataproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/models/datasinks/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasinks/basedatasink.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasinks/filedatasink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasinks/tabledatasink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.991995 laktory-0.3.0/laktory/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/basedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/filedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/memorydatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/pipelinenodedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/tabledatasource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.991995 laktory-0.3.0/laktory/models/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/cataloggrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/connectiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/externallocationgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/functiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/metastoregrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/registeredmodelgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/schemagrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/sharegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/storagecredentialgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/tablegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/viewgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/volumegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)    24209 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/pipelinenode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/pipelinenodeexpectation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.991995 laktory-0.3.0/laktory/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/baseresource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/models/resources/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/accesscontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/dltpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/externallocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/groupmember.py
--rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/metastoreassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/metastoredataaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/mwspermissionassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/secretacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/secretscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/serviceprincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/serviceprincipalrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/sqlquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/userrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/workspacefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/models/resources/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/awsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/azureprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/azurepulumiprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/baseprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/databricksprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/pulumiresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/terraformresource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/models/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/sparkchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/sparkchainnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/sparkfuncarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/stacks/pulumistack.py
--rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/stacks/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/stacks/terraformstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/polars/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/polars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.943995 laktory-0.3.0/laktory/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/resources/data/
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/resources/data/stock_prices.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/laktory/resources/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/resources/notebooks/dlt_laktory_pl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/resources/notebooks/job_laktory_pl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/laktory/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/laktory/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/groupby_and_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/has_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/schema_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/show_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/smart_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/watermark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/window_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/laktory/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.031995 laktory-0.3.0/laktory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-28 04:50:21.000000 laktory-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 04:50:21.000000 laktory-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-28 04:50:21.000000 laktory-0.3.0/scripts/databricks_api_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 04:50:21.000000 laktory-0.3.0/scripts/polars_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 04:50:21.000000 laktory-0.3.0/scripts/test_computed_filed.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 04:50:21.000000 laktory-0.3.0/scripts/test_db_connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 04:50:21.000000 laktory-0.3.0/settings/dev.env
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:50:35.031995 laktory-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.011995 laktory-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/build_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/brz_stock_prices/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/brz_stock_prices/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/brz_stock_prices/.part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/brz_stock_prices/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/yahoo-finance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/pl-spark-dlt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/pl-spark-job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/pl-spark-local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/pl-spark-streaming.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/slv_stock_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_meta/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_meta/.part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_meta/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.031995 laktory-0.3.0/tests/data/slv_stock_prices/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_prices/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_prices/.part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_prices/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stack_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stockprices0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stockprices1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stockprices2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_datasinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dlt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dltpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_pipeline_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_spark_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_spark_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_spark_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    27005 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.064216 laktory-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.968215 laktory-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.980215 laktory-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/ISSUE_TEMPLATE/feature.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.980215 laktory-0.3.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/scripts/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/scripts/update_quickstart_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/scripts/write_release_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.984215 laktory-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/workflows/publish-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/workflows/run_quickstart.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-28 05:24:32.000000 laktory-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-28 05:24:32.000000 laktory-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-05-28 05:24:32.000000 laktory-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 05:24:32.000000 laktory-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 05:24:32.000000 laktory-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-28 05:24:43.060216 laktory-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-28 05:24:32.000000 laktory-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.984215 laktory-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.984215 laktory-0.3.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/datetime.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.984215 laktory-0.3.1/docs/api/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dispatcher/dispatcher.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dispatcher/dispatcherrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dispatcher/jobrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dispatcher/pipelinerunner.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.988216 laktory-0.3.1/docs/api/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dlt/apply_changes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dlt/get_df.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dlt/is_debug.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dlt/is_mocked.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dlt/read.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/dlt/read_stream.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.988216 laktory-0.3.1/docs/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/basemodel.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/dataproducer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.988216 laktory-0.3.1/docs/api/models/datasinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/datasinks/basedatasink.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/datasinks/filedatasink.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/datasinks/tabledatasink.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.988216 laktory-0.3.1/docs/api/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/datasources/basedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/datasources/filedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/datasources/memorydatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/datasources/pipelinenodedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/datasources/tabledatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/pipelinenode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/pipelinenodeexpectation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.988216 laktory-0.3.1/docs/api/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/baseresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.996215 laktory-0.3.1/docs/api/models/resources/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/accesscontrol.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/cluster.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/directory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/dltpipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/externallocation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/grants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/group.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/metastore.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/metastoreassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/metastoredataaccess.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/mwspermissionassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/notebook.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/secretacl.md
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/secretscope.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/serviceprincipal.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/serviceprincipalrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/sqlquery.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/user.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/userrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/volume.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/warehouse.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/databricks/workspacefile.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.996215 laktory-0.3.1/docs/api/models/resources/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/providers/aws.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/providers/azure.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/providers/azurepulumi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/providers/databricks.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/pulumiresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/resources/terraformresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.996215 laktory-0.3.1/docs/api/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/spark/sparkchain.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/spark/sparkchainnode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/spark/sparkfuncarg.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.996215 laktory-0.3.1/docs/api/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/stacks/pulumistack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/stacks/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/models/stacks/terraformstack.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.972215 laktory-0.3.1/docs/api/spark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.996215 laktory-0.3.1/docs/api/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/dataframe/groupby_and_agg.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/dataframe/has_column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/dataframe/schema_flat.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/dataframe/show_string.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/dataframe/smart_join.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/dataframe/window_filter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.000216 laktory-0.3.1/docs/api/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/_constants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/add.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/convert_units.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/div.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/mul.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/poly1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/poly2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/roundp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/scaled_power.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/string_split.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/sub.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/api/spark/functions/uuid.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.000216 laktory-0.3.1/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/governance.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.000216 laktory-0.3.1/docs/concepts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/models/models.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/models/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/models/sourcessinks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/models/sparkchain.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/spark.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/concepts/variables.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/demos.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.004216 laktory-0.3.1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/guides/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/guides/compute.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/guides/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/guides/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/guides/secrets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/guides/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/guides/users.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.012216 laktory-0.3.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/databricks.png
+-rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/delta_live_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)   240172 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/dlt_debug.png
+-rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/kappa.png
+-rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/lakehouse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/logo_sg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/logo_sg_ltb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/logo_sw.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/logo_sw_ltw.png
+-rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/medaillon_complex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/medallion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/okube.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/pl_quickstart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/pl_stock_prices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/pl_stock_prices_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/pulumi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/stock_prices_lineage.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/terraform.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/images/what_is_laktory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/lakehouseascode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.012216 laktory-0.3.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-28 05:24:32.000000 laktory-0.3.1/docs/stylesheets/mkdocstrings.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.012216 laktory-0.3.1/laktory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.016216 laktory-0.3.1/laktory/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/_testing/stackvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/_testing/stockprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.016216 laktory-0.3.1/laktory/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/_quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/cli/quickstart_stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.020216 laktory-0.3.1/laktory/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/dispatcher/dispatcherrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/dispatcher/dltpipelinerunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/dispatcher/jobrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.020216 laktory-0.3.1/laktory/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/dlt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.020216 laktory-0.3.1/laktory/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.020216 laktory-0.3.1/laktory/models/azurenative/
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/azurenative/storageblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16431 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/dataproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.020216 laktory-0.3.1/laktory/models/datasinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasinks/basedatasink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasinks/filedatasink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasinks/tabledatasink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.020216 laktory-0.3.1/laktory/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasources/basedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasources/filedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasources/memorydatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasources/pipelinenodedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/datasources/tabledatasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.024216 laktory-0.3.1/laktory/models/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/cataloggrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/connectiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/externallocationgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/functiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/metastoregrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/registeredmodelgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/schemagrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/sharegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/storagecredentialgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/tablegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/viewgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/grants/volumegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24209 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/pipelinenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/pipelinenodeexpectation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.024216 laktory-0.3.1/laktory/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/baseresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.032216 laktory-0.3.1/laktory/models/resources/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/accesscontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/dltpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/externallocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/groupmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/metastoreassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/metastoredataaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/mwspermissionassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/secretacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/secretscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/serviceprincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/serviceprincipalrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/sqlquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/userrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/databricks/workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.032216 laktory-0.3.1/laktory/models/resources/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/providers/awsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/providers/azureprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/providers/azurepulumiprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/providers/baseprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/providers/databricksprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/pulumiresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/resources/terraformresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.032216 laktory-0.3.1/laktory/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/spark/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/spark/sparkchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/spark/sparkchainnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/spark/sparkfuncarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.032216 laktory-0.3.1/laktory/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/stacks/pulumistack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/stacks/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/models/stacks/terraformstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.032216 laktory-0.3.1/laktory/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/polars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.976215 laktory-0.3.1/laktory/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.032216 laktory-0.3.1/laktory/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/resources/data/stock_prices.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.032216 laktory-0.3.1/laktory/resources/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/resources/notebooks/dlt_laktory_pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/resources/notebooks/job_laktory_pl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.032216 laktory-0.3.1/laktory/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.036216 laktory-0.3.1/laktory/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/dataframe/groupby_and_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/dataframe/has_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/dataframe/schema_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/dataframe/show_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/dataframe/smart_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/dataframe/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/dataframe/window_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.036216 laktory-0.3.1/laktory/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/functions/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/functions/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/functions/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/spark/functions/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-28 05:24:32.000000 laktory-0.3.1/laktory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.060216 laktory-0.3.1/laktory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-28 05:24:42.000000 laktory-0.3.1/laktory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-28 05:24:42.000000 laktory-0.3.1/laktory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 05:24:42.000000 laktory-0.3.1/laktory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 05:24:42.000000 laktory-0.3.1/laktory.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 05:24:42.000000 laktory-0.3.1/laktory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 05:24:42.000000 laktory-0.3.1/laktory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-28 05:24:32.000000 laktory-0.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 05:24:32.000000 laktory-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.036216 laktory-0.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-28 05:24:32.000000 laktory-0.3.1/scripts/databricks_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 05:24:32.000000 laktory-0.3.1/scripts/polars_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 05:24:32.000000 laktory-0.3.1/scripts/test_computed_filed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 05:24:32.000000 laktory-0.3.1/scripts/test_db_connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.036216 laktory-0.3.1/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 05:24:32.000000 laktory-0.3.1/settings/dev.env
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 05:24:43.064216 laktory-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.044216 laktory-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/build_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.044216 laktory-0.3.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.044216 laktory-0.3.1/tests/data/brz_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/brz_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/brz_stock_prices/.part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/brz_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.976215 laktory-0.3.1/tests/data/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.976215 laktory-0.3.1/tests/data/events/yahoo-finance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.976215 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.976215 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:42.980215 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.044216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.044216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.048216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.048216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.048216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.048216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.048216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.048216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.052216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.052216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.052216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.052216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.052216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.052216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.056216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.056216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.056216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.056216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.056216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.056216 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/pl-spark-dlt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/pl-spark-job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/pl-spark-local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/pl-spark-streaming.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.060216 laktory-0.3.1/tests/data/slv_stock_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/slv_stock_meta/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/slv_stock_meta/.part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/slv_stock_meta/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:43.060216 laktory-0.3.1/tests/data/slv_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/slv_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/slv_stock_prices/.part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/slv_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/stack_empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/stockprices0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/stockprices1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/data/stockprices2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_datasinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_dlt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_dltpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_pipeline_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_spark_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_spark_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_spark_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27005 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-28 05:24:32.000000 laktory-0.3.1/tests/test_workspacefile.py
```

### Comparing `laktory-0.3.0/.github/ISSUE_TEMPLATE/bug.yaml` & `laktory-0.3.1/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/.github/ISSUE_TEMPLATE/feature.yaml` & `laktory-0.3.1/.github/ISSUE_TEMPLATE/feature.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/.github/scripts/bump_version.py` & `laktory-0.3.1/.github/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/.github/scripts/update_quickstart_stack.py` & `laktory-0.3.1/.github/scripts/update_quickstart_stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/.github/scripts/write_release_body.py` & `laktory-0.3.1/.github/scripts/write_release_body.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/.github/workflows/release.yml` & `laktory-0.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/.github/workflows/run_quickstart.yml` & `laktory-0.3.1/.github/workflows/run_quickstart.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/.github/workflows/test.yml` & `laktory-0.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/.gitignore` & `laktory-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/CHANGELOG.md` & `laktory-0.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Release History
 
-## [0.3.0] - Unreleased
+## [0.3.1] - Unreleased
+### Fixed
+* Updated ReadMe
+* Stack Validator unit test
+
+## [0.3.0] - 2024-05-28
 ### Added
 * `Pipeline` model, the new central component for building ETL pipelines
 * `PipelineNode` model, the `Pipeline` sub-component defining each dataframe in a pipeline
 * `FileDataSink` and `TableDataSink` sinks models
 * `PipelineNodeDataSource` and `MemoryDataSource` sources model
 * Future support for Polars and other types of dataframe
 ### Updated
```

### Comparing `laktory-0.3.0/LICENSE` & `laktory-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/api/models/resources/databricks/cluster.md` & `laktory-0.3.1/docs/api/models/resources/databricks/cluster.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/api/models/resources/databricks/grants.md` & `laktory-0.3.1/docs/api/models/resources/databricks/grants.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/api/models/resources/databricks/job.md` & `laktory-0.3.1/docs/api/models/resources/databricks/job.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/api/models/resources/databricks/metastoredataaccess.md` & `laktory-0.3.1/docs/api/models/resources/databricks/metastoredataaccess.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/cli.md` & `laktory-0.3.1/docs/concepts/cli.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/deployment.md` & `laktory-0.3.1/docs/concepts/deployment.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/design.md` & `laktory-0.3.1/docs/concepts/design.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/governance.md` & `laktory-0.3.1/docs/concepts/governance.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/models/dataevent.md` & `laktory-0.3.1/docs/concepts/models/dataevent.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/models/models.md` & `laktory-0.3.1/docs/concepts/models/models.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/models/pipeline.md` & `laktory-0.3.1/docs/concepts/models/pipeline.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/models/sourcessinks.md` & `laktory-0.3.1/docs/concepts/models/sourcessinks.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/models/sparkchain.md` & `laktory-0.3.1/docs/concepts/models/sparkchain.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/spark.md` & `laktory-0.3.1/docs/concepts/spark.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/stack.md` & `laktory-0.3.1/docs/concepts/stack.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/concepts/variables.md` & `laktory-0.3.1/docs/concepts/variables.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/databricks.png` & `laktory-0.3.1/docs/images/databricks.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/delta_live_tables.png` & `laktory-0.3.1/docs/images/delta_live_tables.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/dlt_debug.png` & `laktory-0.3.1/docs/images/dlt_debug.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/kappa.png` & `laktory-0.3.1/docs/images/kappa.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/lakehouse.png` & `laktory-0.3.1/docs/images/lakehouse.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/logo_sg.png` & `laktory-0.3.1/docs/images/logo_sg.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/logo_sg_ltb.png` & `laktory-0.3.1/docs/images/logo_sg_ltb.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/logo_sw.png` & `laktory-0.3.1/docs/images/logo_sw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/logo_sw_ltw.png` & `laktory-0.3.1/docs/images/logo_sw_ltw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/medaillon_complex.png` & `laktory-0.3.1/docs/images/medaillon_complex.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/medallion.png` & `laktory-0.3.1/docs/images/medallion.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/okube.png` & `laktory-0.3.1/docs/images/okube.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/pl_quickstart.png` & `laktory-0.3.1/docs/images/pl_quickstart.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/pl_stock_prices.png` & `laktory-0.3.1/docs/images/pl_stock_prices.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/pl_stock_prices_simple.png` & `laktory-0.3.1/docs/images/pl_stock_prices_simple.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/pulumi.png` & `laktory-0.3.1/docs/images/pulumi.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/stock_prices_lineage.png` & `laktory-0.3.1/docs/images/stock_prices_lineage.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/terraform.png` & `laktory-0.3.1/docs/images/terraform.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/images/what_is_laktory.png` & `laktory-0.3.1/docs/images/what_is_laktory.png`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/index.md` & `laktory-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/install.md` & `laktory-0.3.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/lakehouseascode.md` & `laktory-0.3.1/docs/lakehouseascode.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/quickstart.md` & `laktory-0.3.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/docs/stylesheets/mkdocstrings.css` & `laktory-0.3.1/docs/stylesheets/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/__init__.py` & `laktory-0.3.1/laktory/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/_logger.py` & `laktory-0.3.1/laktory/_logger.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/_parsers.py` & `laktory-0.3.1/laktory/_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/_settings.py` & `laktory-0.3.1/laktory/_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/_testing/stackvalidator.py` & `laktory-0.3.1/laktory/_testing/stackvalidator.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,14 +61,12 @@
         self.validate_pulumi()
         self.validate_terraform()
         os.chdir(cwd)
         shutil.rmtree(dirpath)
         settings.cli_raise_external_exceptions = c0
 
     def validate_pulumi(self):
-        pass
-        # self.pstack.preview(stack="okube/dev")
-        # TODO: Re-enable
+        self.pstack.preview(stack="okube/dev")
 
     def validate_terraform(self):
         self.tstack.init()
         self.tstack.plan()
```

### Comparing `laktory-0.3.0/laktory/_testing/stockprices.py` & `laktory-0.3.1/laktory/_testing/stockprices.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/cli/_common.py` & `laktory-0.3.1/laktory/cli/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/cli/_deploy.py` & `laktory-0.3.1/laktory/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/cli/_init.py` & `laktory-0.3.1/laktory/cli/_init.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/cli/_preview.py` & `laktory-0.3.1/laktory/cli/_preview.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/cli/_quickstart.py` & `laktory-0.3.1/laktory/cli/_quickstart.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/cli/_run.py` & `laktory-0.3.1/laktory/cli/_run.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/cli/_write.py` & `laktory-0.3.1/laktory/cli/_write.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/cli/quickstart_stack.yaml` & `laktory-0.3.1/laktory/cli/quickstart_stack.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/constants.py` & `laktory-0.3.1/laktory/constants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/datetime.py` & `laktory-0.3.1/laktory/datetime.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/dispatcher/dispatcher.py` & `laktory-0.3.1/laktory/dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/dispatcher/dispatcherrunner.py` & `laktory-0.3.1/laktory/dispatcher/dispatcherrunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/dispatcher/dltpipelinerunner.py` & `laktory-0.3.1/laktory/dispatcher/dltpipelinerunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/dispatcher/jobrunner.py` & `laktory-0.3.1/laktory/dispatcher/jobrunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/dlt/__init__.py` & `laktory-0.3.1/laktory/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/azurenative/storageblob.py` & `laktory-0.3.1/laktory/models/azurenative/storageblob.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/basemodel.py` & `laktory-0.3.1/laktory/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/dataevent.py` & `laktory-0.3.1/laktory/models/dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/dataproducer.py` & `laktory-0.3.1/laktory/models/dataproducer.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/datasinks/basedatasink.py` & `laktory-0.3.1/laktory/models/datasinks/basedatasink.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/datasinks/filedatasink.py` & `laktory-0.3.1/laktory/models/datasinks/filedatasink.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/datasinks/tabledatasink.py` & `laktory-0.3.1/laktory/models/datasinks/tabledatasink.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/datasources/basedatasource.py` & `laktory-0.3.1/laktory/models/datasources/basedatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/datasources/filedatasource.py` & `laktory-0.3.1/laktory/models/datasources/filedatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/datasources/memorydatasource.py` & `laktory-0.3.1/laktory/models/datasources/memorydatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/datasources/pipelinenodedatasource.py` & `laktory-0.3.1/laktory/models/datasources/pipelinenodedatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/datasources/tabledatasource.py` & `laktory-0.3.1/laktory/models/datasources/tabledatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/__init__.py` & `laktory-0.3.1/laktory/models/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/cataloggrant.py` & `laktory-0.3.1/laktory/models/grants/cataloggrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/connectiongrant.py` & `laktory-0.3.1/laktory/models/grants/connectiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/externallocationgrant.py` & `laktory-0.3.1/laktory/models/grants/externallocationgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/functiongrant.py` & `laktory-0.3.1/laktory/models/grants/functiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/metastoregrant.py` & `laktory-0.3.1/laktory/models/grants/metastoregrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/registeredmodelgrant.py` & `laktory-0.3.1/laktory/models/grants/registeredmodelgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/schemagrant.py` & `laktory-0.3.1/laktory/models/grants/schemagrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/sharegrant.py` & `laktory-0.3.1/laktory/models/grants/sharegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/storagecredentialgrant.py` & `laktory-0.3.1/laktory/models/grants/storagecredentialgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/tablegrant.py` & `laktory-0.3.1/laktory/models/grants/tablegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/viewgrant.py` & `laktory-0.3.1/laktory/models/grants/viewgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/grants/volumegrant.py` & `laktory-0.3.1/laktory/models/grants/volumegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/pipeline.py` & `laktory-0.3.1/laktory/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/pipelinenode.py` & `laktory-0.3.1/laktory/models/pipelinenode.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/pipelinenodeexpectation.py` & `laktory-0.3.1/laktory/models/pipelinenodeexpectation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/baseresource.py` & `laktory-0.3.1/laktory/models/resources/baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/__init__.py` & `laktory-0.3.1/laktory/models/resources/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/accesscontrol.py` & `laktory-0.3.1/laktory/models/resources/databricks/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/catalog.py` & `laktory-0.3.1/laktory/models/resources/databricks/catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/cluster.py` & `laktory-0.3.1/laktory/models/resources/databricks/cluster.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/column.py` & `laktory-0.3.1/laktory/models/resources/databricks/column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/dbfsfile.py` & `laktory-0.3.1/laktory/models/resources/databricks/dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/directory.py` & `laktory-0.3.1/laktory/models/resources/databricks/directory.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/dltpipeline.py` & `laktory-0.3.1/laktory/models/resources/databricks/dltpipeline.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/externallocation.py` & `laktory-0.3.1/laktory/models/resources/databricks/externallocation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/grants.py` & `laktory-0.3.1/laktory/models/resources/databricks/grants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/group.py` & `laktory-0.3.1/laktory/models/resources/databricks/group.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/groupmember.py` & `laktory-0.3.1/laktory/models/resources/databricks/groupmember.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/job.py` & `laktory-0.3.1/laktory/models/resources/databricks/job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/metastore.py` & `laktory-0.3.1/laktory/models/resources/databricks/metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/metastoreassignment.py` & `laktory-0.3.1/laktory/models/resources/databricks/metastoreassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/metastoredataaccess.py` & `laktory-0.3.1/laktory/models/resources/databricks/metastoredataaccess.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/mwspermissionassignment.py` & `laktory-0.3.1/laktory/models/resources/databricks/mwspermissionassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/notebook.py` & `laktory-0.3.1/laktory/models/resources/databricks/notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/permissions.py` & `laktory-0.3.1/laktory/models/resources/databricks/permissions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/schema.py` & `laktory-0.3.1/laktory/models/resources/databricks/schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/secret.py` & `laktory-0.3.1/laktory/models/resources/databricks/secret.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/secretacl.py` & `laktory-0.3.1/laktory/models/resources/databricks/secretacl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/secretscope.py` & `laktory-0.3.1/laktory/models/resources/databricks/secretscope.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/serviceprincipal.py` & `laktory-0.3.1/laktory/models/resources/databricks/serviceprincipal.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/serviceprincipalrole.py` & `laktory-0.3.1/laktory/models/resources/databricks/serviceprincipalrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/sqlquery.py` & `laktory-0.3.1/laktory/models/resources/databricks/sqlquery.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/table.py` & `laktory-0.3.1/laktory/models/resources/databricks/table.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/user.py` & `laktory-0.3.1/laktory/models/resources/databricks/user.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/userrole.py` & `laktory-0.3.1/laktory/models/resources/databricks/userrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/volume.py` & `laktory-0.3.1/laktory/models/resources/databricks/volume.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/warehouse.py` & `laktory-0.3.1/laktory/models/resources/databricks/warehouse.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/databricks/workspacefile.py` & `laktory-0.3.1/laktory/models/resources/databricks/workspacefile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/providers/awsprovider.py` & `laktory-0.3.1/laktory/models/resources/providers/awsprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/providers/azureprovider.py` & `laktory-0.3.1/laktory/models/resources/providers/azureprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/providers/azurepulumiprovider.py` & `laktory-0.3.1/laktory/models/resources/providers/azurepulumiprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/providers/baseprovider.py` & `laktory-0.3.1/laktory/models/resources/providers/baseprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/providers/databricksprovider.py` & `laktory-0.3.1/laktory/models/resources/providers/databricksprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/pulumiresource.py` & `laktory-0.3.1/laktory/models/resources/pulumiresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/resources/terraformresource.py` & `laktory-0.3.1/laktory/models/resources/terraformresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/spark/_common.py` & `laktory-0.3.1/laktory/models/spark/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/spark/sparkchain.py` & `laktory-0.3.1/laktory/models/spark/sparkchain.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/spark/sparkchainnode.py` & `laktory-0.3.1/laktory/models/spark/sparkchainnode.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/spark/sparkfuncarg.py` & `laktory-0.3.1/laktory/models/spark/sparkfuncarg.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/stacks/pulumistack.py` & `laktory-0.3.1/laktory/models/stacks/pulumistack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/stacks/stack.py` & `laktory-0.3.1/laktory/models/stacks/stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/models/stacks/terraformstack.py` & `laktory-0.3.1/laktory/models/stacks/terraformstack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/resources/data/stock_prices.json` & `laktory-0.3.1/laktory/resources/data/stock_prices.json`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/resources/notebooks/dlt_laktory_pl.py` & `laktory-0.3.1/laktory/resources/notebooks/dlt_laktory_pl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/resources/notebooks/job_laktory_pl.py` & `laktory-0.3.1/laktory/resources/notebooks/job_laktory_pl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/__init__.py` & `laktory-0.3.1/laktory/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/dataframe/__init__.py` & `laktory-0.3.1/laktory/spark/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/dataframe/groupby_and_agg.py` & `laktory-0.3.1/laktory/spark/dataframe/groupby_and_agg.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/dataframe/has_column.py` & `laktory-0.3.1/laktory/spark/dataframe/has_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/dataframe/schema_flat.py` & `laktory-0.3.1/laktory/spark/dataframe/schema_flat.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/dataframe/show_string.py` & `laktory-0.3.1/laktory/spark/dataframe/show_string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/dataframe/smart_join.py` & `laktory-0.3.1/laktory/spark/dataframe/smart_join.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/dataframe/watermark.py` & `laktory-0.3.1/laktory/spark/dataframe/watermark.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/dataframe/window_filter.py` & `laktory-0.3.1/laktory/spark/dataframe/window_filter.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/functions/_common.py` & `laktory-0.3.1/laktory/spark/functions/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/functions/logical.py` & `laktory-0.3.1/laktory/spark/functions/logical.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/functions/math.py` & `laktory-0.3.1/laktory/spark/functions/math.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/functions/string.py` & `laktory-0.3.1/laktory/spark/functions/string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/spark/functions/units.py` & `laktory-0.3.1/laktory/spark/functions/units.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory/version.py` & `laktory-0.3.1/laktory/version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/laktory.egg-info/SOURCES.txt` & `laktory-0.3.1/laktory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/mkdocs.yml` & `laktory-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/pyproject.toml` & `laktory-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/scripts/databricks_api_call.py` & `laktory-0.3.1/scripts/databricks_api_call.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/build_test_data.py` & `laktory-0.3.1/tests/build_test_data.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet` & `laktory-0.3.1/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/data/pl-spark-dlt.yaml` & `laktory-0.3.1/tests/data/pl-spark-dlt.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/data/pl-spark-job.yaml` & `laktory-0.3.1/tests/data/pl-spark-job.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/data/pl-spark-local.yaml` & `laktory-0.3.1/tests/data/pl-spark-local.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/data/pl-spark-streaming.yaml` & `laktory-0.3.1/tests/data/pl-spark-streaming.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet` & `laktory-0.3.1/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet` & `laktory-0.3.1/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/data/stack.yaml` & `laktory-0.3.1/tests/data/stack.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_basemodel.py` & `laktory-0.3.1/tests/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_baseresource.py` & `laktory-0.3.1/tests/test_baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_catalog.py` & `laktory-0.3.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_cli.py` & `laktory-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_column.py` & `laktory-0.3.1/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_dataevent.py` & `laktory-0.3.1/tests/test_dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_datasinks.py` & `laktory-0.3.1/tests/test_datasinks.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_datasources.py` & `laktory-0.3.1/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_datetime.py` & `laktory-0.3.1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_dbfsfile.py` & `laktory-0.3.1/tests/test_dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_dispatcher.py` & `laktory-0.3.1/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_dltpipeline.py` & `laktory-0.3.1/tests/test_dltpipeline.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_docstrings.py` & `laktory-0.3.1/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_job.py` & `laktory-0.3.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_metastore.py` & `laktory-0.3.1/tests/test_metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_notebook.py` & `laktory-0.3.1/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_parsers.py` & `laktory-0.3.1/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_pipeline.py` & `laktory-0.3.1/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_pipeline_node.py` & `laktory-0.3.1/tests/test_pipeline_node.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_schema.py` & `laktory-0.3.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_settings.py` & `laktory-0.3.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_spark_chain.py` & `laktory-0.3.1/tests/test_spark_chain.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_spark_dataframe.py` & `laktory-0.3.1/tests/test_spark_dataframe.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_spark_functions.py` & `laktory-0.3.1/tests/test_spark_functions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_sql_query.py` & `laktory-0.3.1/tests/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_stack.py` & `laktory-0.3.1/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_table.py` & `laktory-0.3.1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `laktory-0.3.0/tests/test_workspacefile.py` & `laktory-0.3.1/tests/test_workspacefile.py`

 * *Files identical despite different names*

