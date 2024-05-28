# Comparing `tmp/laktory-0.2.1.tar.gz` & `tmp/laktory-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laktory-0.2.1.tar", last modified: Tue May  7 03:26:49 2024, max compression
+gzip compressed data, was "laktory-0.3.0.tar", last modified: Tue May 28 04:50:35 2024, max compression
```

## Comparing `laktory-0.2.1.tar` & `laktory-0.3.0.tar`

### file list

```diff
@@ -1,493 +1,511 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.487642 laktory-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.395642 laktory-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.403642 laktory-0.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/ISSUE_TEMPLATE/bug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/ISSUE_TEMPLATE/feature.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/scripts/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/scripts/update_quickstart_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/scripts/write_release_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/workflows/publish-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/workflows/run_quickstart.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-07 03:26:40.000000 laktory-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-07 03:26:40.000000 laktory-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 03:26:40.000000 laktory-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 03:26:40.000000 laktory-0.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-07 03:26:49.487642 laktory-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-07 03:26:40.000000 laktory-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/datetime.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/docs/api/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dispatcher/dispatcher.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dispatcher/dispatcherrunner.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dispatcher/jobrunner.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dispatcher/pipelinerunner.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.411642 laktory-0.2.1/docs/api/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/apply_changes.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/get_df.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/is_debug.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/is_mocked.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/read.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/read_stream.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.411642 laktory-0.2.1/docs/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/basemodel.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/accesscontrol.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/cluster.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/directory.md
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/externallocation.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/grants.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/group.md
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/job.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/metastore.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/metastoreassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/metastoredataaccess.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/mwspermissionassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/notebook.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/secret.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/secretacl.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/secretscope.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/serviceprincipal.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/serviceprincipalrole.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/sqlquery.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/user.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/userrole.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/warehouse.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/workspacefile.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/dataeventheader.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/dataproducer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/datasources/basedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/datasources/eventdatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/datasources/tabledatasource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/providers/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/providers/aws.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/providers/azure.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/providers/azurepulumi.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/providers/databricks.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/resources/baseresource.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/resources/pulumiresource.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/resources/terraformresource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/spark/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/spark/sparkchain.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/spark/sparkchainnode.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/spark/sparkfuncarg.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.419642 laktory-0.2.1/docs/api/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/column.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/tablebuilder.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/tableexpectation.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/volume.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.419642 laktory-0.2.1/docs/api/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/stacks/pulumistack.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/stacks/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/stacks/terraformstack.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.395642 laktory-0.2.1/docs/api/spark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.419642 laktory-0.2.1/docs/api/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/groupby_and_agg.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/has_column.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/schema_flat.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/show_string.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/smart_join.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/window_filter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.423642 laktory-0.2.1/docs/api/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/_constants.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/add.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/convert_units.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/div.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/mul.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/poly1.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/poly2.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/roundp.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/scaled_power.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/string_split.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/sub.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/uuid.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.423642 laktory-0.2.1/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/governance.md
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/models.md
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/spark.md
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/table.md
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/tablebuilder.md
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/variables.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/demos.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.427642 laktory-0.2.1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/compute.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/job.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/secrets.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/users.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.431642 laktory-0.2.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/databricks.png
--rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/delta_live_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/dlt_debug.png
--rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/kappa.png
--rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/lakehouse.png
--rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/logo_sg.png
--rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/logo_sg_ltb.png
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/logo_sw.png
--rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/logo_sw_ltw.png
--rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/medaillon_complex.png
--rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/medallion.png
--rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/okube.png
--rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/pl_quickstart.png
--rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/pl_stock_prices.png
--rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/pl_stock_prices_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/pulumi.png
--rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/stock_prices_lineage.png
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/terraform.png
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/what_is_laktory.png
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/lakehouseascode.md
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.431642 laktory-0.2.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/stylesheets/mkdocstrings.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.435642 laktory-0.2.1/laktory/
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.435642 laktory-0.2.1/laktory/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_testing/stackvalidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_testing/stockprices.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_quickstart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/quickstart_stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/dispatcherrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/jobrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/pipelinerunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dlt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/models/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/models/azurenative/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/azurenative/storageblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/basemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.443642 laktory-0.2.1/laktory/models/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/accesscontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/externallocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/groupmember.py
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/metastoreassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/metastoredataaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/mwspermissionassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/secretacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/secretscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/serviceprincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/serviceprincipalrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/sqlquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/userrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/workspacefile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/dataeventheader.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/dataproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.447642 laktory-0.2.1/laktory/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/datasources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/datasources/basedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/datasources/eventdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/datasources/tabledatasource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.447642 laktory-0.2.1/laktory/models/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/cataloggrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/connectiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/externallocationgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/functiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/metastoregrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/registeredmodelgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/schemagrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/sharegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/storagecredentialgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/tablegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/viewgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/volumegrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.451642 laktory-0.2.1/laktory/models/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/awsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/azureprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/azurepulumiprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/baseprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/databricksprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.451642 laktory-0.2.1/laktory/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/resources/baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/resources/pulumiresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/resources/terraformresource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.451642 laktory-0.2.1/laktory/models/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/sparkchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/sparkchainnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/sparkfuncarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.451642 laktory-0.2.1/laktory/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12014 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/tablebuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/tableexpectation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/stacks/pulumistack.py
--rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/stacks/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/stacks/terraformstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/laktory/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/resources/data/
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/data/stock_prices.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/resources/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/notebooks/dlt_brz_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/notebooks/dlt_gld_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/notebooks/dlt_slv_star_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/notebooks/dlt_slv_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/groupby_and_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/has_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/schema_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/show_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/smart_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/watermark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/window_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.483642 laktory-0.2.1/laktory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-07 03:26:40.000000 laktory-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-07 03:26:40.000000 laktory-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.459642 laktory-0.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 03:26:40.000000 laktory-0.2.1/scripts/databricks_api_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 03:26:40.000000 laktory-0.2.1/scripts/test_computed_filed.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 03:26:40.000000 laktory-0.2.1/scripts/test_db_connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.459642 laktory-0.2.1/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 03:26:40.000000 laktory-0.2.1/settings/dev.env
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:49.487642 laktory-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.463642 laktory-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/build_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/brz_stock_prices/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/brz_stock_prices/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/brz_stock_prices/.part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/brz_stock_prices/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/brz_stock_prices/part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/tests/data/events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/tests/data/events/yahoo-finance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.403642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.483642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.483642 laktory-0.2.1/tests/data/slv_stock_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_meta/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_meta/.part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_meta/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_meta/part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.483642 laktory-0.2.1/tests/data/slv_stock_prices/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_prices/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_prices/.part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_prices/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_prices/part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stack_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stockprices0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stockprices1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stockprices2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_dlt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_spark_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_spark_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_spark_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26494 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_table_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.031995 laktory-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.939995 laktory-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/ISSUE_TEMPLATE/feature.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/scripts/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/scripts/update_quickstart_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/scripts/write_release_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/workflows/publish-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/workflows/run_quickstart.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-28 04:50:21.000000 laktory-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-28 04:50:21.000000 laktory-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-05-28 04:50:21.000000 laktory-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 04:50:21.000000 laktory-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 04:50:21.000000 laktory-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-28 04:50:35.031995 laktory-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-28 04:50:21.000000 laktory-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/datetime.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.951995 laktory-0.3.0/docs/api/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dispatcher/dispatcher.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dispatcher/dispatcherrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dispatcher/jobrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dispatcher/pipelinerunner.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/apply_changes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/get_df.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/is_debug.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/is_mocked.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/read.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/dlt/read_stream.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/basemodel.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/dataproducer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/models/datasinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasinks/basedatasink.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasinks/filedatasink.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasinks/tabledatasink.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/basedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/filedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/memorydatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/pipelinenodedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/datasources/tabledatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/pipelinenode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/pipelinenodeexpectation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.955995 laktory-0.3.0/docs/api/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/baseresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/models/resources/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/accesscontrol.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/cluster.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/directory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/dltpipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/externallocation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/grants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/group.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/metastore.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/metastoreassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/metastoredataaccess.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/mwspermissionassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/notebook.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/secretacl.md
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/secretscope.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/serviceprincipal.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/serviceprincipalrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/sqlquery.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/user.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/userrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/volume.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/warehouse.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/databricks/workspacefile.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/models/resources/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/providers/aws.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/providers/azure.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/providers/azurepulumi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/providers/databricks.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/pulumiresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/resources/terraformresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/spark/sparkchain.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/spark/sparkchainnode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/spark/sparkfuncarg.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/stacks/pulumistack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/stacks/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/models/stacks/terraformstack.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.943995 laktory-0.3.0/docs/api/spark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.963995 laktory-0.3.0/docs/api/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/groupby_and_agg.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/has_column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/schema_flat.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/show_string.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/smart_join.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/dataframe/window_filter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.967995 laktory-0.3.0/docs/api/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/_constants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/add.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/convert_units.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/div.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/mul.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/poly1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/poly2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/roundp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/scaled_power.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/string_split.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/sub.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/api/spark/functions/uuid.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.967995 laktory-0.3.0/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/governance.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.967995 laktory-0.3.0/docs/concepts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/models.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/sourcessinks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/models/sparkchain.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/spark.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/concepts/variables.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/demos.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.971995 laktory-0.3.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/compute.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/secrets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/guides/users.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.979995 laktory-0.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/databricks.png
+-rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/delta_live_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)   240172 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/dlt_debug.png
+-rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/kappa.png
+-rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/lakehouse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/logo_sg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/logo_sg_ltb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/logo_sw.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/logo_sw_ltw.png
+-rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/medaillon_complex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/medallion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/okube.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/pl_quickstart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/pl_stock_prices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/pl_stock_prices_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/pulumi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/stock_prices_lineage.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/terraform.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/images/what_is_laktory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/lakehouseascode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.979995 laktory-0.3.0/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-28 04:50:21.000000 laktory-0.3.0/docs/stylesheets/mkdocstrings.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.979995 laktory-0.3.0/laktory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.983995 laktory-0.3.0/laktory/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_testing/stackvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_testing/stockprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.983995 laktory-0.3.0/laktory/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/cli/quickstart_stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/dispatcherrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/dltpipelinerunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dispatcher/jobrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/dlt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/models/azurenative/
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/azurenative/storageblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16431 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/dataproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.987995 laktory-0.3.0/laktory/models/datasinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasinks/basedatasink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasinks/filedatasink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasinks/tabledatasink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.991995 laktory-0.3.0/laktory/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/basedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/filedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/memorydatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/pipelinenodedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/datasources/tabledatasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.991995 laktory-0.3.0/laktory/models/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/cataloggrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/connectiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/externallocationgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/functiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/metastoregrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/registeredmodelgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/schemagrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/sharegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/storagecredentialgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/tablegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/viewgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/grants/volumegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24209 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/pipelinenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/pipelinenodeexpectation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.991995 laktory-0.3.0/laktory/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/baseresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/models/resources/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/accesscontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/dltpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/externallocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/groupmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/metastoreassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/metastoredataaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/mwspermissionassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/secretacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/secretscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/serviceprincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/serviceprincipalrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/sqlquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/userrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/databricks/workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/models/resources/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/awsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/azureprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/azurepulumiprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/baseprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/providers/databricksprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/pulumiresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/resources/terraformresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/sparkchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/sparkchainnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/spark/sparkfuncarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/stacks/pulumistack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/stacks/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/models/stacks/terraformstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/polars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.943995 laktory-0.3.0/laktory/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.999995 laktory-0.3.0/laktory/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/resources/data/stock_prices.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/laktory/resources/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/resources/notebooks/dlt_laktory_pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/resources/notebooks/job_laktory_pl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/laktory/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/laktory/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/groupby_and_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/has_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/schema_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/show_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/smart_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/dataframe/window_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/laktory/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/spark/functions/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-28 04:50:21.000000 laktory-0.3.0/laktory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.031995 laktory-0.3.0/laktory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 04:50:34.000000 laktory-0.3.0/laktory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-28 04:50:21.000000 laktory-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 04:50:21.000000 laktory-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-28 04:50:21.000000 laktory-0.3.0/scripts/databricks_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 04:50:21.000000 laktory-0.3.0/scripts/polars_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 04:50:21.000000 laktory-0.3.0/scripts/test_computed_filed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 04:50:21.000000 laktory-0.3.0/scripts/test_db_connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.003995 laktory-0.3.0/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 04:50:21.000000 laktory-0.3.0/settings/dev.env
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:50:35.031995 laktory-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.011995 laktory-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/build_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/brz_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/brz_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/brz_stock_prices/.part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/brz_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/yahoo-finance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:34.947995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.015995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.019995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.023995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/pl-spark-dlt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/pl-spark-job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/pl-spark-local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/pl-spark-streaming.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.027995 laktory-0.3.0/tests/data/slv_stock_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_meta/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_meta/.part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_meta/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:35.031995 laktory-0.3.0/tests/data/slv_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_prices/.part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stack_empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stockprices0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stockprices1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/data/stockprices2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_datasinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dlt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_dltpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_pipeline_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_spark_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_spark_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_spark_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27005 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-28 04:50:21.000000 laktory-0.3.0/tests/test_workspacefile.py
```

### Comparing `laktory-0.2.1/.github/ISSUE_TEMPLATE/bug.yaml` & `laktory-0.3.0/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/.github/ISSUE_TEMPLATE/feature.yaml` & `laktory-0.3.0/.github/ISSUE_TEMPLATE/feature.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/.github/scripts/bump_version.py` & `laktory-0.3.0/.github/scripts/bump_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         v0 = version.parse(v0)
         v1 = version.Version(f"{v0.major}.{v0.minor}.{v0.micro + 1}")
     print(f"Bumping laktory to {v1}")
 
     # Update version file
     print(f"Updating _version.py")
     with open(version_filepath, "w") as fp:
-        fp.write(f'VERSION = "{v1}"')
+        fp.write(f'VERSION = "{v1}"\n')
 
     # Set version as git action variable
     print(f"Setting git env var version {git_env_filepath}")
     with open(git_env_filepath, "a") as fp:
         fp.write(f"version={v1}")
 
     # Update CHANGELOG
```

### Comparing `laktory-0.2.1/.github/scripts/update_quickstart_stack.py` & `laktory-0.3.0/.github/scripts/update_quickstart_stack.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,13 +30,13 @@
         description="Update notebooks to install specific version of laktory"
     )
     parser.add_argument("branch_name", type=str, help="Laktory branch name")
     parser.add_argument(
         "--notebooks_path",
         type=str,
         help="Path of the notebooks directory",
-        default="./notebooks/pipelines",
+        default="./notebooks/dlt",
     )
     args = parser.parse_args()
 
     # Execute
     main(args.branch_name, args.notebooks_path)
```

### Comparing `laktory-0.2.1/.github/scripts/write_release_body.py` & `laktory-0.3.0/.github/scripts/write_release_body.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/.github/workflows/release.yml` & `laktory-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/.github/workflows/run_quickstart.yml` & `laktory-0.3.0/.github/workflows/run_quickstart.yml`

 * *Files 0% similar despite different names*

```diff
@@ -68,12 +68,12 @@
         run: laktory deploy -e dev -y
         working-directory: ${{ env.CWD }}
         env:
           DATABRICKS_HOST: ${{ vars.DATABRICKS_HOST }}
           DATABRICKS_TOKEN: ${{ secrets.DATABRICKS_TOKEN }}
 
       - name: laktory run
-        run: laktory run -e dev -p pl-quickstart
+        run: laktory run -e dev -dlt pl-quickstart
         working-directory: ${{ env.CWD }}
         env:
           DATABRICKS_HOST: ${{ vars.DATABRICKS_HOST }}
           DATABRICKS_TOKEN: ${{ secrets.DATABRICKS_TOKEN }}
```

### Comparing `laktory-0.2.1/.github/workflows/test.yml` & `laktory-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/.gitignore` & `laktory-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/CHANGELOG.md` & `laktory-0.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 # Release History
 
-## [0.2.1] - Unreleased
+## [0.3.0] - Unreleased
+### Added
+* `Pipeline` model, the new central component for building ETL pipelines
+* `PipelineNode` model, the `Pipeline` sub-component defining each dataframe in a pipeline
+* `FileDataSink` and `TableDataSink` sinks models
+* `PipelineNodeDataSource` and `MemoryDataSource` sources model
+* Future support for Polars and other types of dataframe
+### Updated
+* Enabled CDC support for both `FileDataSource` and `TableDataSource`
+### Breaking changes
+* Merged `DataEventHeader` into `DataEvent` model
+* Renamed `EventDataSource` model to `FileDataSource`
+* Renamed `name` attribute to `table_name` in `TableDataSource` model
+* Removed `SparkChain` support in DataSources
+* Renamed `Pipeline` model to `DLTPipeline` model
+* Cloud resources moved under models.resources.{provider}.{resource_class} to avoid collisions with future classes.
+* Removed `TableBuilder`. `PipelineNode` should be used instead
+
+## [0.2.1] - 2024-05-07
 ### Added
 * Support for spark chain for a data source
 * Support for broadcasting in a data source
 * YAML model dump for all base models
 ### Fixed
-* Function selection for pyspark connect DataFrames
+* Function selection for pyspark connect dataframes
 
 ## [0.2.0] - 2024-05-02
 ### Added
 * `SparkChain` a high level class allowing to declare and execute spark operations on a dataframe 
 * `SparkColumnNode` the node of a `SparkChain` that builds a new column
-* `SparkTableNode` the node of a `SparkChain` that returns a new DataFrame
+* `SparkTableNode` the node of a `SparkChain` that returns a new dataframe
 * Moved `filter`, `selects` and `watermarks` properties to `models.BaseDataSource` so that it can be used for all source types
 * `models.BaseDataSource` `renames` attribute for renaming columns of the source table
 * `models.BaseDataSource` `drops` attribute for dropping columns of the source table
 * spark DataFrame `watermark` returns the watermark column and threshold if any 
 * spark DataFrame `smart_join` joins, cleans duplicated columns and supports watermarking 
 * spark DataFrame `groupby_and_agg` groupby and aggregates in a single function 
 * spark DataFrame `window_filter` takes the first n rows over a window
```

### Comparing `laktory-0.2.1/LICENSE` & `laktory-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/PKG-INFO` & `laktory-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.2.1
+Version: 0.3.0
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: databricks-sdk
 Requires-Dist: inflect
+Requires-Dist: networkx
 Requires-Dist: planck
 Requires-Dist: prompt_toolkit
 Requires-Dist: pulumi
 Requires-Dist: pulumi_databricks>=1.36
 Requires-Dist: pulumi_random
 Requires-Dist: pyyaml
 Requires-Dist: pydantic>=2
@@ -33,18 +34,21 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flit; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-video; extra == "dev"
+Requires-Dist: plotly; extra == "dev"
 Provides-Extra: spark
 Requires-Dist: pandas; extra == "spark"
 Requires-Dist: pyarrow; extra == "spark"
 Requires-Dist: pyspark; extra == "spark"
+Provides-Extra: polars
+Requires-Dist: polars; extra == "polars"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-examples; extra == "test"
 Requires-Dist: yfinance; extra == "test"
 Provides-Extra: azure
 Requires-Dist: azure-identity; extra == "azure"
```

### Comparing `laktory-0.2.1/README.md` & `laktory-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/api/models/databricks/cluster.md` & `laktory-0.3.0/docs/api/models/resources/databricks/cluster.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-::: laktory.models.Cluster
+::: laktory.models.resources.databricks.Cluster
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterAutoScale
+::: laktory.models.resources.databricks.cluster.ClusterAutoScale
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterInitScriptVolumes
+::: laktory.models.resources.databricks.cluster.ClusterInitScriptVolumes
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterInitScriptWorkspace
+::: laktory.models.resources.databricks.cluster.ClusterInitScriptWorkspace
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterInitScript
+::: laktory.models.resources.databricks.cluster.ClusterInitScript
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterLibraryCran
+::: laktory.models.resources.databricks.cluster.ClusterLibraryCran
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterLibraryMaven
+::: laktory.models.resources.databricks.cluster.ClusterLibraryMaven
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterInitScript
+::: laktory.models.resources.databricks.cluster.ClusterInitScript
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterLibraryPypi
+::: laktory.models.resources.databricks.cluster.ClusterLibraryPypi
 
 ---
 
-::: laktory.models.databricks.cluster.ClusterLibrary
+::: laktory.models.resources.databricks.cluster.ClusterLibrary
```

### Comparing `laktory-0.2.1/docs/api/models/databricks/grants.md` & `laktory-0.3.0/docs/api/models/resources/databricks/grants.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-::: laktory.models.Grants
+::: laktory.models.resources.databricks.Grants
 
 ---
 
-::: laktory.models.databricks.grants.Grant
+::: laktory.models.resources.databricks.grants.Grant
 
 --- 
 Each grant model allows a set of privileges to a principal and operate on a securable object.
 More details on privileges available [here](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types).
 
 
 ::: laktory.models.CatalogGrant
```

### Comparing `laktory-0.2.1/docs/api/models/databricks/metastoredataaccess.md` & `laktory-0.3.0/docs/api/models/resources/databricks/metastoredataaccess.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-::: laktory.models.MetastoreDataAccess
+::: laktory.models.resources.databricks.MetastoreDataAccess
 
 ---
 
-::: laktory.models.databricks.metastoredataaccess.MetastoreDataAccessAwsIamRole
+::: laktory.models.resources.databricks.metastoredataaccess.MetastoreDataAccessAwsIamRole
 
 ---
 
-::: laktory.models.databricks.metastoredataaccess.MetastoreDataAccessAzureManagedIdentity
+::: laktory.models.resources.databricks.metastoredataaccess.MetastoreDataAccessAzureManagedIdentity
 
 ---
 
-::: laktory.models.databricks.metastoredataaccess.MetastoreDataAccessAzureServicePrincipal
+::: laktory.models.resources.databricks.metastoredataaccess.MetastoreDataAccessAzureServicePrincipal
 
 ---
 
-::: laktory.models.databricks.metastoredataaccess.MetastoreDataAccessDatabricksGcpServiceAccount
+::: laktory.models.resources.databricks.metastoredataaccess.MetastoreDataAccessDatabricksGcpServiceAccount
 
 ---
 
-::: laktory.models.databricks.metastoredataaccess.MetastoreDataAccessGcpServiceAccountKey
+::: laktory.models.resources.databricks.metastoredataaccess.MetastoreDataAccessGcpServiceAccountKey
```

### Comparing `laktory-0.2.1/docs/concepts/cli.md` & `laktory-0.3.0/docs/concepts/cli.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #### preview
 `laktory preview` validates your yaml stack and describe new resources to be deployed or changes to existing ones.  Similar to `pulumi preview` or `terraform validate/plan`.
 
 #### deploy
 `laktory deploy` executes the deployment by creating or updating resources.  Similar to `pulumi up` or `terraform apply`.
 
 #### run
-`laktory run` execute remote job or pipeline and monitor failures until completion.
+`laktory run` execute remote job or DLT pipeline and monitor failures until completion. Local execution (without an orchestrator) of a pipeline is not yet supported.
 
 ### CI/CD
 These commands can be run locally, but really start to provide value in the context of a CI/CD pipeline in which 
 complex testing, validation and deployment flows can be built. An example of such workflows is provided in the 
 [lakehouse-as-code](https://github.com/okube-ai/lakehouse-as-code/tree/cli_run/.github/workflows) repository.
 
 In this case, we have 2 workflows:
```

### Comparing `laktory-0.2.1/docs/concepts/dataevent.md` & `laktory-0.3.0/docs/concepts/models/dataevent.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ??? "API Documentation"
-    [`laktory.models.DataEventHeader`][laktory.models.DataEventHeader]<br>
     [`laktory.models.DataEvent`][laktory.models.DataEvent]<br>
 
-The `DataEvent` (and `DataEventHeader`) models are supporting the event-based architecture described in [Design Principles](design.md).
+The `DataEvent` model is supporting the event-based architecture described in [Design Principles](design.md).
 They define the metadata (name, producer, timestamp, etc.) as well as the data (payload) of an event.
 They can be used both in the context of generating and consuming data.
 
 ### Generation
 Suppose you have a scheduled- or trigger-based service that fetch stock prices and want to publish them to a storage account, the landing of your lakehouse.
 
 First declare the event and assign it some data
@@ -34,25 +33,9 @@
 In this case, a Databricks Volume is used, but other methods like `event.to_path()` or `to_azure_storage_container()` are also available.
 
 The default path for the event follows the standard convention
 > {events_root}/{producer_name}/{event_name}/{year}/{month}/{day}/{event_name}_{year}{month}{day}T{timestamp}.{format}
 
 But you may customize it using environment variable `WORKSPACE_LANDING_ROOT` or `events_root`, `tstamp_in_path` and `suffix` arguments.
 
-### Consumption
-Similarly one can leverage the `DataEventHeader` model to simplify reading events from the landing storage. 
-It is essentially a strip down version of the `DataEvent` model in which the `data` does not need to be provided.
-
-```py
-from laktory import models
-
-event = models.DataEventHeader(
-    name="stock_price",
-    producer={"name": "yahoo-finance"},
-)
-
-df = spark.read.load(event.event_root)
-```
-Again, the default path is assumed, but it could be customized.
-
 ### Format
 Currently, data events can be stored and read from `JSON`, `CSV` and `PARQUET` formats. More may be added in the future.
```

### Comparing `laktory-0.2.1/docs/concepts/deployment.md` & `laktory-0.3.0/docs/concepts/deployment.md`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 ## Pulumi - Python
 If you prefer writing infrastructure as code with python, Laktory integrates nicely with Pulumi python.
 
 ```py title="__main__.py"
 from laktory import models
 
 # Declare pipeline
-pipeline = models.Pipeline(
+pipeline = models.DLTPipeline(
     name="pl-stock-prices",
     libraries=[{"notebooks": {"path": "/pipelines/dlt_brz_template.py"}}],
 )
 
 # Deploy
 pipeline.to_pulumi()
 ```
```

### Comparing `laktory-0.2.1/docs/concepts/design.md` & `laktory-0.3.0/docs/concepts/design.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,17 +62,14 @@
 
 ### Silver
 In the Silver layer of the lakehouse, data undergoes "just-enough" matching, merging, conformation, and cleansing from the Bronze layer, creating an "Enterprise view" of key business entities. 
 This layer facilitates self-service analytics, ad-hoc reporting, and advanced analytics by bringing diverse data sources into a unified view. 
 Following an ELT methodology prioritizing speed, agility, and minimal transformations, the Silver layer serves as a source for Departmental Analysts, Data Engineers, and Data Scientists. 
 The Silver Layer employs 3rd-Normal Form-like data models, supporting efficient data modeling and acting as an intermediate step before more complex transformations in the Gold layer.
 
-### Silver Star
-The Silver Star layer is Laktory-specific and represents a subset of the silver layer in which data has been de-normalized. It often involves joining multiples tables, while preserving the number of rows found in the left silver table. 
-
 ### Gold
 The Gold layer in a lakehouse holds highly refined and aggregated data, powering analytics, machine learning, and production applications. 
 These tables represent transformed knowledge, not just information, and are crucial for analysts.
 Data shared with customers is typically stored exclusively in the Gold layer.
 Regularly scheduled updates control costs and establish SLAs for data freshness. 
 Although a lakehouse minimizes deadlock issues, Gold tables are often stored separately to avoid cloud data request limits.
 Pre-handling aggregations, joins, and filtering before writing to the Gold layer ensures users experience low-latency query performance.
```

### Comparing `laktory-0.2.1/docs/concepts/governance.md` & `laktory-0.3.0/docs/concepts/governance.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/concepts/models.md` & `laktory-0.3.0/docs/concepts/models/models.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Laktory is built on top of a collection of nested [pydantic](https://docs.pydantic.dev/latest/concepts/models/) models. 
 Each model is a subclass of `pydantic.BaseModel` and offer a few additional methods and properties. 
 The serializable nature of these models makes it possible to define a lakehouse using a declarative approach.
 
 ## Declaration
-Let's explore the declaration of `Column`, `Table` and `Pipeline` models as an example. 
+Let's explore the declaration of `Column`, `Table` and `Schema` models as an example. 
 
 ### Python Sequential
+
 ```py
 from laktory import models
 
-x = models.Column(name="x", type="double")
-y = models.Column(name="y", type="double")
-z = models.Column(name="z", type="double")
-
-table_xy = models.Table(name="table_xy", columns=[x, y])
-table_xyz = models.Table(name="table_xyz", columns=[x, y, z])
-
-pipeline = models.Pipeline(
-    name="my-pipeline",
-    catalog="dev",
-    target="finance",
+x = models.resources.databricks.Column(name="x", type="double")
+y = models.resources.databricks.Column(name="y", type="double")
+z = models.resources.databricks.Column(name="z", type="double")
+
+table_xy = models.resources.databricks.Table(name="table_xy", columns=[x, y])
+table_xyz = models.resources.databricks.Table(name="table_xyz", columns=[x, y, z])
+
+pipeline = models.resources.databricks.Schema(
+    catalog_name="dev",
+    name="finance",
     tables=[table_xy, table_xyz],
 )
 ```
 
 ### Python Nested
+
 ```py
 from laktory import models
 
-pipeline = models.Pipeline(
-    name="my-pipeline",
-    catalog="dev",
-    target="finance",
+pipeline = models.resources.databricks.Schema(
+    catalog_name="dev",
+    name="finance",
     tables=[
         {
             "name": "table_xy",
             "columns": [
                 {"name": "x", "type": "double"},
                 {"name": "y", "type": "double"},
             ],
@@ -52,18 +52,17 @@
 )
 ```
 
 ### YAML configuration
 In most cases however, it is best practice to declare these models as `yaml` configuration files to decouple modeling and implementation.
 Here is the same example using a configuration file.
 
-```yaml title="my-pipeline.yaml"
-name: my-pipeline
-catalog: dev
-target: finance
+```yaml title="my-schema.yaml"
+catalog_name: dev
+name: finance
 tables: 
   - name: "table_xy"
     columns:
       - name: x
         type: double
       - name: y
         type: double
@@ -77,26 +76,25 @@
         type: double    
 ```
 
 ```py title="main.py"
 from laktory import models
 
 with open("my-pipeline.yaml", "r") as fp:
-    pipeline = models.Pipeline.model_validate_yaml(fp)
+    schema = models.resources.databricks.Schema.model_validate_yaml(fp)
 ```
-Using any of the above approaches will result in the exact same `pipeline` python object.
+Using any of the above approaches will result in the exact same `schema` python object.
 
 #### YAML nesting
 Laktory supports nested yaml files, meaning that you can include or inject another yaml file from the base
 one. Using this approach, the example above could be re-written as
 
-```yaml title="my-pipeline.yaml"
-name: my-pipeline
-catalog: dev
-target: finance
+```yaml title="my-schema.yaml"
+catalog_name: dev
+name: finance
 tables: 
   - ${include.table1.yaml}
   - ${include.table2.yaml}
 ```
 
 ```yaml title="table1.yaml"
 name: "table_xy"
```

### Comparing `laktory-0.2.1/docs/concepts/spark.md` & `laktory-0.3.0/docs/concepts/spark.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import laktory.spark.functions as LF
 
 df = spark.createDataFrame(pd.DataFrame({"x": [1, 2, 3]}))
 df = df.withColumn("y", LF.poly1("x", -1, 1.0))
 ```
 These functions are by default available when declaring a column in a pipeline `Table` model.
 
-## DataFrame methods
+## Dataframe methods
 In this case the methods are designed to be applied directly on a spark dataframe.
 ```py
 import pandas as pd
 from laktory.spark.dataframe import has_column
 
 df = spark.createDataFrame(pd.DataFrame({"x": [1, 2, 3]}))
 has_column(df, "x")
```

### Comparing `laktory-0.2.1/docs/concepts/stack.md` & `laktory-0.3.0/docs/concepts/stack.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/concepts/variables.md` & `laktory-0.3.0/docs/concepts/variables.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/databricks.png` & `laktory-0.3.0/docs/images/databricks.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/delta_live_tables.png` & `laktory-0.3.0/docs/images/delta_live_tables.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/kappa.png` & `laktory-0.3.0/docs/images/kappa.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/lakehouse.png` & `laktory-0.3.0/docs/images/lakehouse.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/logo_sg.png` & `laktory-0.3.0/docs/images/logo_sg.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/logo_sg_ltb.png` & `laktory-0.3.0/docs/images/logo_sg_ltb.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/logo_sw.png` & `laktory-0.3.0/docs/images/logo_sw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/logo_sw_ltw.png` & `laktory-0.3.0/docs/images/logo_sw_ltw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/medaillon_complex.png` & `laktory-0.3.0/docs/images/medaillon_complex.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/medallion.png` & `laktory-0.3.0/docs/images/medallion.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/okube.png` & `laktory-0.3.0/docs/images/okube.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/pl_quickstart.png` & `laktory-0.3.0/docs/images/pl_quickstart.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/pl_stock_prices.png` & `laktory-0.3.0/docs/images/pl_stock_prices.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/pl_stock_prices_simple.png` & `laktory-0.3.0/docs/images/pl_stock_prices_simple.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/pulumi.png` & `laktory-0.3.0/docs/images/pulumi.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/stock_prices_lineage.png` & `laktory-0.3.0/docs/images/stock_prices_lineage.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/terraform.png` & `laktory-0.3.0/docs/images/terraform.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/images/what_is_laktory.png` & `laktory-0.3.0/docs/images/what_is_laktory.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/install.md` & `laktory-0.3.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/lakehouseascode.md` & `laktory-0.3.0/docs/lakehouseascode.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/docs/quickstart.md` & `laktory-0.3.0/docs/quickstart.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,25 +16,22 @@
 #### Stack File
 ??? "API Documentation"
     [`laktory.models.Stack`][laktory.models.Stack]<br>
 
 The `stack.yaml` file is the main entry point defining the `name` of the stack, the selected `backend` and the list
 of `resources` to be deployed. 
 
-In this example, we define 4 resources:
+In this example, we define 3 resources:
 
 - 1 data file (DBFSFile)
-- 2 notebooks
-- 1 pipeline 
-
-The pipeline also defines the data transformation for the bronze and silver tables.
+- 1 notebooks
+- 1 pipeline
 
 #### Notebook Files
-The `notebooks/pipelines/dlt_brz_template.py` and `notebooks/pipelines/dlt_slv_template.py` files are the notebooks
-used by the pipeline.
+The `notebooks/dlt/dlt_laktory_pl.py` file is the standard notebook used by Laktory pipelines using DLT orchestrator.
 
 #### Data File
 The `data/stock_prices.json` file is a data file storing stock prices. 
 Normally, data would be mounted in Volumes from cloud storage, but for the simplicity a small data file is deployed as a
 DBFS file. 
 
 ### Set Environment Variables
@@ -55,62 +52,80 @@
 
 Then, simply deploy using
 ```cmd
 laktory deploy --env dev
 ```
 
 ### Run your pipeline
-Once deployed, you pipeline is ready to be run.
+Once deployed, you pipeline is ready to be run through Databricks UI
 ![pl-stock-prices](images/pl_quickstart.png)
 
+or using laktory CLI
+```cmd
+laktory run --dlt pl-quickstart
+```
+
 ### Debug your pipeline
 If you need to debug or modify one of your pipeline's notebook, Laktory makes it very easy by allowing you to run and inspect (with some limitations) the output data outside of the DLT pipeline.
 
-```py title="dlt_slv_template.py"
+```py title="dlt_laktory_pl.py"
 from laktory import dlt
-from laktory import read_metadata
+from laktory import models
 from laktory import get_logger
+from laktory import settings
 
 dlt.spark = spark
 logger = get_logger(__name__)
 
 # Read pipeline definition
 pl_name = spark.conf.get("pipeline_name", "pl-quickstart")
-pl = read_metadata(pipeline=pl_name)
+filepath = f"/Workspace{settings.workspace_laktory_root}pipelines/{pl_name}.json"
+with open(filepath, "r") as fp:
+    pl = models.Pipeline.model_validate_json(fp.read())
+
+# --------------------------------------------------------------------------- #
+# Tables and Views Definition                                                 #
+# --------------------------------------------------------------------------- #
 
 
-# Define table
-def define_table(table):
-    @dlt.table(name=table.name, comment=table.comment)
+def define_table(node):
+    @dlt.table_or_view(
+        name=node.name,
+        comment=node.description,
+        as_view=node.sink is None,
+    )
+    @dlt.expect_all(node.warning_expectations)
+    @dlt.expect_all_or_drop(node.drop_expectations)
+    @dlt.expect_all_or_fail(node.fail_expectations)
     def get_df():
-        logger.info(f"Building {table.name} table")
+        logger.info(f"Building {node.name} node")
 
-        # Read Source
-        df = table.builder.read_source(spark)
+        # Execute node
+        df = node.execute(spark=spark, udfs=udfs)
         df.printSchema()
 
-        # Process
-        df = table.builder.process(df, spark=spark)
-
         # Return
         return df
 
     return get_df
 
 
 # --------------------------------------------------------------------------- #
 # Execution                                                                   #
 # --------------------------------------------------------------------------- #
 
-# Build tables
-for table in pl.tables:
-    if table.layer == "SILVER":
-        wrapper = define_table(table)
-        df = dlt.get_df(wrapper)
-        display(df)
+# Build nodes
+for node in pl.nodes:
+
+    if node.dlt_template != "DEFAULT":
+        continue
+
+    wrapper = define_table(node)
+    df = dlt.get_df(wrapper)
+    display(df)
 ```
 
 Output:
 
 ![pl-stock-prices](images/dlt_debug.png)
```

### Comparing `laktory-0.2.1/docs/stylesheets/mkdocstrings.css` & `laktory-0.3.0/docs/stylesheets/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/__init__.py` & `laktory-0.3.0/laktory/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,13 @@
 from .dispatcher.dispatcher import Dispatcher
 
 # --------------------------------------------------------------------------- #
 # Objects                                                                     #
 # --------------------------------------------------------------------------- #
 
 from ._logger import get_logger
-from .metadata import read_metadata
 from .models.resources.pulumiresource import pulumi_outputs
 from .models.resources.pulumiresource import pulumi_resources
 from .cli.app import app
 from .version import show_version_info
 from .datetime import unix_timestamp
 from .datetime import utc_datetime
```

### Comparing `laktory-0.2.1/laktory/_logger.py` & `laktory-0.3.0/laktory/_logger.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/_parsers.py` & `laktory-0.3.0/laktory/_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/_settings.py` & `laktory-0.3.0/laktory/_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     # databricks_warehouse_id: Union[str, None] = Field(None, alias="databricks_warehouse_id")
     databricks_host: Union[str, None] = Field(None)
     databricks_token: Union[str, None] = Field(None)
     databricks_account_id: Union[str, None] = Field(None)
     databricks_warehouse_id: Union[str, None] = Field(None)
 
     @model_validator(mode="after")
-    def excluded_fields(self) -> Any:
+    def update_landing_root(self) -> Any:
         if self.workspace_landing_root == "":
             self.workspace_landing_root = (
                 f"/Volumes/{self.workspace_env}/sources/landing/"
             )
 
         return self
```

### Comparing `laktory-0.2.1/laktory/_testing/stackvalidator.py` & `laktory-0.3.0/laktory/_testing/stackvalidator.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/cli/_common.py` & `laktory-0.3.0/laktory/cli/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/cli/_deploy.py` & `laktory-0.3.0/laktory/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/cli/_init.py` & `laktory-0.3.0/laktory/cli/_init.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/cli/_preview.py` & `laktory-0.3.0/laktory/cli/_preview.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/cli/_quickstart.py` & `laktory-0.3.0/laktory/cli/_quickstart.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,29 +95,28 @@
 
     # Node type id
     if node_type is None:
         node_type = prompt(
             f"Node type for pipeline (e.g.: Standard_DS3_v2, c5.2xlarge, etc.): "
         )
 
-    if not os.path.exists("./notebooks/pipelines"):
-        os.makedirs("./notebooks/pipelines")
+    if not os.path.exists("./notebooks/dlt"):
+        os.makedirs("./notebooks/dlt")
     if not os.path.exists("./data"):
         os.makedirs("./data")
 
     # Copy notebooks
     for filename in [
-        "dlt_brz_template.py",
-        "dlt_slv_template.py",
+        "dlt_laktory_pl.py",
     ]:
         with open(os.path.join(DIRPATH, f"../resources/notebooks/{filename}")) as fp:
             data = fp.read()
             data = data.replace("pl-stock-prices", "pl-quickstart")
 
-        with open(f"./notebooks/pipelines/{filename}", "w") as fp:
+        with open(f"./notebooks/dlt/{filename}", "w") as fp:
             fp.write(data)
 
     # Copy data
     for filename in [
         "stock_prices.json",
     ]:
         with open(os.path.join(DIRPATH, f"../resources/data/{filename}")) as fp:
@@ -125,15 +124,15 @@
 
         with open(f"./data/{filename}", "w") as fp:
             fp.write(data)
 
     # Read template stack
     template_stack = read_template()
     template_stack.backend = backend
-    template_stack.resources.pipelines["pl-quickstart"].clusters[
+    template_stack.resources.pipelines["pl-quickstart"].dlt.clusters[
         0
     ].node_type_id = node_type
 
     # Build stack
     if backend == "pulumi":
 
         template_stack.resources.providers = {}
@@ -164,16 +163,16 @@
     # Dump data
     data = stack.model_dump(exclude_none=True)
     data = remove_empty(data)
 
     # Clean up resources
     if backend != "pulumi" and "pulumi" in data.keys():
         del data["pulumi"]
-    for k, n in data["resources"]["notebooks"].items():
-        del data["resources"]["notebooks"][k]["path"]
+    for k, n in data["resources"]["databricks_notebooks"].items():
+        del data["resources"]["databricks_notebooks"][k]["path"]
 
     # Sort data
     d = {}
     for k in [
         "name",
         "organization",
         "backend",
```

### Comparing `laktory-0.2.1/laktory/cli/_run.py` & `laktory-0.3.0/laktory/cli/_run.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from laktory.cli.app import app
 from laktory.dispatcher.dispatcher import Dispatcher
 
 
 @app.command()
 def run(
     job: Annotated[str, typer.Option("--job", "-j", help="Job name")] = None,
-    pipeline: Annotated[str, typer.Option("--pipeline", "-p", help="Job name")] = None,
+    dlt: Annotated[str, typer.Option("--dlt", "-dlt", help="Job name")] = None,
     timeout: Annotated[
         float,
         typer.Option(
             "--timeout", "-t", help="Maximum allowed time (in seconds) for run"
         ),
     ] = 1200,
     raise_exception: Annotated[
@@ -37,22 +37,22 @@
         str, typer.Option("--env", "-e", help="Name of the environment")
     ] = None,
     filepath: Annotated[
         str, typer.Option(help="Stack (yaml) filepath.")
     ] = "./stack.yaml",
 ):
     """
-    Execute remote job or pipeline and monitor failures until completion.
+    Execute remote job or DLT pipeline and monitor failures until completion.
 
     Parameters
     ----------
     job:
-        Name of the job to run (mutually exclusive with pipeline)
-    pipeline:
-        Name of the pipeline to run (mutually exclusive with pipeline)
+        Name of the job to run (mutually exclusive with dlt)
+    dlt:
+        Name of the DLT pipeline to run (mutually exclusive with job)
     timeout:
         Maximum allowed time (in seconds) for run.
     raise_exception:
         Raise exception on failure
     current_run_action:
         Action to take for currently running job or pipline.
     full_refresh:
@@ -61,24 +61,24 @@
         Name of the environment.
     filepath:
         Stack (yaml) filepath.
 
     Examples
     --------
     ```cmd
-    laktory run --env dev -p pl-stock-prices --full_refresh --action CANCEL
+    laktory run --env dev --dlt pl-stock-prices --full_refresh --action CANCEL
     ```
 
     """
 
     # Set Resource Name
-    if job and pipeline:
-        raise ValueError("Only one of `job` or `pipeline` should be set.")
-    if not (job or pipeline):
-        raise ValueError("One of `job` or `pipeline` should be set.")
+    if job and dlt:
+        raise ValueError("Only one of `job` or `dlt` should be set.")
+    if not (job or dlt):
+        raise ValueError("One of `job` or `dlt` should be set.")
 
     # Set Dispatcher
     controller = CLIController(
         env=environment,
         stack_filepath=filepath,
     )
     dispatcher = Dispatcher(stack=controller.stack)
@@ -88,15 +88,15 @@
         dispatcher.run_job(
             job_name=job,
             timeout=timeout,
             raise_exception=raise_exception,
             current_run_action=current_run_action,
         )
 
-    if pipeline:
-        dispatcher.run_pipeline(
-            pipeline_name=pipeline,
+    if dlt:
+        dispatcher.run_dlt(
+            dlt_name=dlt,
             timeout=timeout,
             raise_exception=raise_exception,
             current_run_action=current_run_action,
             full_refresh=full_refresh,
         )
```

### Comparing `laktory-0.2.1/laktory/cli/_write.py` & `laktory-0.3.0/laktory/cli/_write.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/constants.py` & `laktory-0.3.0/laktory/constants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/datetime.py` & `laktory-0.3.0/laktory/datetime.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/dispatcher/dispatcher.py` & `laktory-0.3.0/laktory/dispatcher/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from databricks.sdk import WorkspaceClient
 
 from laktory._useragent import DATABRICKS_USER_AGENT
 from laktory._useragent import VERSION
 from laktory.models.stacks.stack import Stack
-from laktory.dispatcher.pipelinerunner import PipelineRunner
+from laktory.dispatcher.dltpipelinerunner import DLTPipelineRunner
 from laktory.dispatcher.jobrunner import JobRunner
 
 
 class Dispatcher:
     """
     The dispatcher is a manager that can be used to run and monitor remote jobs
-    and pipelines defined in a stack. It is generally used through Laktory CLI
-    `run` command, but may be used directly in scripts and python programs.
+    and DLT pipelines defined in a stack. It is generally used through Laktory
+    CLI `run` command, but may be used directly in scripts and python
+    programs.
 
     Parameters
     ----------
     stack
         Stack object
     env
         Selected environment
@@ -48,19 +49,31 @@
         self._wc = None
         self.resources = {}
 
         self.init_resources()
 
     def init_resources(self):
         """Set resource for each of the resources defined in the stack"""
+
         for k, pl in self.stack.resources.pipelines.items():
-            self.resources[k] = PipelineRunner(dispatcher=self, name=pl.name)
+            if pl.dlt is not None:
+                self.resources[pl.dlt.name] = DLTPipelineRunner(
+                    dispatcher=self, name=pl.dlt.name
+                )
+
+            if pl.databricks_job is not None:
+                self.resources[pl.databricks_job.name] = JobRunner(
+                    dispatcher=self, name=pl.databricks_job.name
+                )
+
+        for k, pl in self.stack.resources.databricks_dltpipelines.items():
+            self.resources[pl.name] = DLTPipelineRunner(dispatcher=self, name=pl.name)
 
-        for k, job in self.stack.resources.jobs.items():
-            self.resources[k] = JobRunner(dispatcher=self, name=job.name)
+        for k, job in self.stack.resources.databricks_jobs.items():
+            self.resources[job.name] = JobRunner(dispatcher=self, name=job.name)
 
     # ----------------------------------------------------------------------- #
     # Environment                                                             #
     # ----------------------------------------------------------------------- #
 
     @property
     def env(self) -> str:
@@ -165,22 +178,22 @@
             Arguments passed to `JobRunner.run()`
         **kwargs:
             Keyword arguments passed to `JobRunner.run()`
         """
         job = self.resources[job_name]
         job.run(*args, **kwargs)
 
-    def run_pipeline(self, pipeline_name: str, *args, **kwargs):
+    def run_dlt(self, dlt_name: str, *args, **kwargs):
         """
-        Run pipeline with name `pipeline_name`
+        Run DLT pipeline with name `dlt_name`
 
         Parameters
         ----------
-        pipeline_name:
-            Name of the pipeline
+        dlt_name:
+            Name of the DLT pipeline
         *args:
             Arguments passed to `JobRunner.run()`
         **kwargs:
             Keyword arguments passed to `JobRunner.run()`
         """
-        pl = self.resources[pipeline_name]
+        pl = self.resources[dlt_name]
         pl.run(*args, **kwargs)
```

### Comparing `laktory-0.2.1/laktory/dispatcher/dispatcherrunner.py` & `laktory-0.3.0/laktory/dispatcher/dispatcherrunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/dispatcher/jobrunner.py` & `laktory-0.3.0/laktory/dispatcher/jobrunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/dispatcher/pipelinerunner.py` & `laktory-0.3.0/laktory/dispatcher/dltpipelinerunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from laktory.dispatcher.dispatcherrunner import DispatcherRunner
 from laktory.datetime import unix_timestamp
 from laktory._logger import get_logger
 
 logger = get_logger(__name__)
 
 
-class PipelineRunner(DispatcherRunner):
+class DLTPipelineRunner(DispatcherRunner):
     """
-    Pipeline runner.
+    DLT Pipeline runner.
     """
 
     _update_start: StartUpdateResponse = None
     _update: GetUpdateResponse = None
 
     def get_id(self) -> str:
         """Get deployed pipeline id"""
```

### Comparing `laktory-0.2.1/laktory/dlt/__init__.py` & `laktory-0.3.0/laktory/dlt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from laktory._logger import get_logger
-from laktory.spark import DataFrame
+from laktory.spark import SparkDataFrame
 
 try:
     from dlt import *
     from dlt import read as _read
     from dlt import read_stream as _read_stream
     from dlt import apply_changes as _apply_changes
 except Exception:
@@ -43,15 +43,15 @@
         return True
 
 
 def is_debug() -> bool:
     """
     Debug flag. If `True`, DLT readers are replaced with laktory functions
     allowing to run a notebook outside of a pipeline and preview the content
-    of the output DataFrame.
+    of the output dataframe.
 
     Returns
     -------
     :
         Debug flag
     """
     try:
@@ -59,26 +59,26 @@
     except Exception:
         return True
     if spark.conf.get("pipelines.dbrVersion", None) is None:
         return True
     return False
 
 
-def get_df(df_wrapper) -> DataFrame:
+def get_df(df_wrapper) -> SparkDataFrame:
     """
     When executed in debug mode (ref `dlt.is_debug`), executes and returns
-    the output DataFrame of a function decorated with `@dlt.table` or
+    the output dataframe of a function decorated with `@dlt.table` or
     `@dlt.view`. Returns None when `is_debug()` is `False`.
 
     This method is not supported when a table using DLT views as input.
 
     Returns
     -------
     :
-        Output DataFrame
+        Output dataframe
 
     Examples
     --------
     ```py
     from laktory import dlt
 
     dlt.spark = spark
@@ -106,23 +106,23 @@
 
 
 # --------------------------------------------------------------------------- #
 # Overwrite                                                                   #
 # --------------------------------------------------------------------------- #
 
 
-def read(*args, **kwargs) -> DataFrame:
+def read(*args, **kwargs) -> SparkDataFrame:
     """
     When `is_debug()` is `True` read table from storage, else read table from
     pipeline with native Databricks `dlt.read`
 
     Returns
     -------
     :
-        Ouput DataFrame
+        Ouput dataframe
 
     Examples
     --------
     ```py
     from laktory import dlt
 
     dlt.spark = spark
@@ -151,15 +151,15 @@
     """
     When `is_debug()` is `True` read table from storage as stream, else read
     table from pipeline with native Databricks `dlt.read_stream`
 
     Returns
     -------
     :
-        Ouput DataFrame
+        Ouput dataframe
 
     Examples
     --------
     ```py
     from laktory import dlt
 
     dlt.spark = spark
@@ -181,61 +181,62 @@
     else:
         # Remove catalog and schema from naming space
         args = list(args)
         args[0] = args[0].split(".")[-1]
         return _read_stream(*args, **kwargs)
 
 
-def apply_changes(*args, table=None, **kwargs):
+def apply_changes(*args, node=None, **kwargs):
     """
     When `is_debug()` is `True` read source CDC table from storage, else run
     native Databricks `dlt.apply_changes`
 
     Returns
     -------
     :
-        Ouput DataFrame
+        Output dataframe
 
     Examples
     --------
     ```py
     from laktory import dlt
     from laktory import models
 
     dlt.spark = spark
 
-    def define_table(table):
-        dlt.create_streaming_table(name=table.name)
-        df = dlt.apply_changes(**table.builder.apply_changes_kwargs)
+    def define_table(node):
+        dlt.create_streaming_table(name=node.name)
+        df = dlt.apply_changes(**node.apply_changes_kwargs)
         return df
 
     define_table(
-        models.Table(
+        models.PipelineNode(
             name="slv_stock_prices",
-            builder={
-                "table_source": {
-                    "name": "brz_stock_prices",
-                    "cdc": {
-                        "primary_keys": ["asset_symbol"],
-                        "sequence_by": "change_id",
-                        "scd_type": 2,
-                    },
+            source={
+                "table_name": "brz_stock_prices",
+                "cdc": {
+                    "primary_keys": ["asset_symbol"],
+                    "sequence_by": "change_id",
+                    "scd_type": 2,
                 },
             },
+            sink={
+                "table_name": "brz_stock_prices",
+            },
         )
     )
     ```
     """
     if is_debug():
-        if table is None:
+        if node is None:
             return
-        df = table.read_source(spark=spark)
+        df = node.source.read(spark=spark)
         # TODO: Apply changes
         logger.warning(
-            "Laktory does not currently support applying CDC changes. Returned DataFrame is CDC source."
+            "Laktory does not currently support applying CDC changes. Returned dataframe is CDC source."
         )
         return df
     else:
         return _apply_changes(*args, **kwargs)
 
 
 # --------------------------------------------------------------------------- #
```

### Comparing `laktory-0.2.1/laktory/models/azurenative/storageblob.py` & `laktory-0.3.0/laktory/models/azurenative/storageblob.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pulumi
 from typing import Union
 from typing import Literal
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.mwspermissionassignment import MwsPermissionAssignment
+from laktory.models.resources.databricks.mwspermissionassignment import (
+    MwsPermissionAssignment,
+)
 
 
 class StorageBlob(BaseModel, PulumiResource):
     """
     Databricks group
 
     Attributes
```

### Comparing `laktory-0.2.1/laktory/models/basemodel.py` & `laktory-0.3.0/laktory/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/accesscontrol.py` & `laktory-0.3.0/laktory/models/resources/databricks/accesscontrol.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
         Name of the user to assign the permission to.
 
     Examples
     --------
     ```py
     from laktory import models
 
-    p = models.AccessControl(group_name="role-engineers", permission_level="READ")
+    p = models.resources.databricks.AccessControl(
+        group_name="role-engineers", permission_level="READ"
+    )
     ```
     """
 
     group_name: str = None
     permission_level: str
     service_principal_name: str = None
     user_name: str = None
```

### Comparing `laktory-0.2.1/laktory/models/databricks/cluster.py` & `laktory-0.3.0/laktory/models/resources/databricks/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Literal
 from typing import Union
 from pydantic import Field
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.accesscontrol import AccessControl
-from laktory.models.databricks.permissions import Permissions
+from laktory.models.resources.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.permissions import Permissions
 
 
 class ClusterAutoScale(BaseModel):
     """
     Cluster Autoscale
 
     Attributes
@@ -242,15 +242,15 @@
 
 
     Examples
     --------
     ```py
     from laktory import models
 
-    cluster = models.Cluster(
+    cluster = models.resources.databricks.Cluster(
         name="default",
         spark_version="14.0.x-scala2.12",
         data_security_mode="USER_ISOLATION",
         node_type_id="Standard_DS3_v2",
         autoscale={
             "min_workers": 1,
             "max_workers": 4,
```

### Comparing `laktory-0.2.1/laktory/models/databricks/dbfsfile.py` & `laktory-0.3.0/laktory/models/resources/databricks/dbfsfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import Any
 from typing import Union
 from pydantic import model_validator
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.accesscontrol import AccessControl
-from laktory.models.databricks.permissions import Permissions
+from laktory.models.resources.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.permissions import Permissions
 
 
 class DbfsFile(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks DBFS File
 
     Attributes
```

### Comparing `laktory-0.2.1/laktory/models/databricks/directory.py` & `laktory-0.3.0/laktory/models/resources/databricks/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         When `True`, subdirectories are also deleted when the directory is deleted
 
     Examples
     --------
     ```py
     from laktory import models
 
-    d = models.Directory(path="/queries/views")
+    d = models.resources.databricks.Directory(path="/queries/views")
     print(d)
     '''
     resource_name_=None options=ResourceOptions(variables={}, depends_on=[], provider=None, aliases=None, delete_before_replace=True, ignore_changes=None, import_=None, parent=None, replace_on_changes=None) variables={} path='/queries/views' delete_recursive=None
     '''
     print(d.resource_key)
     #> queries-views
     print(d.resource_name)
```

### Comparing `laktory-0.2.1/laktory/models/databricks/externallocation.py` & `laktory-0.3.0/laktory/models/resources/databricks/externallocation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/grants.py` & `laktory-0.3.0/laktory/models/resources/databricks/grants.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Name of the volume to assign the permission to.
 
     Examples
     --------
     ```py
     from laktory import models
 
-    grants = models.Grants(
+    grants = models.resources.databricks.Grants(
         catalog="dev",
         grants=[{"principal": "metastore-admins", "privileges": ["CREATE_SCHEMA"]}],
     )
     ```
     """
 
     grants: list[Grant]
```

### Comparing `laktory-0.2.1/laktory/models/databricks/group.py` & `laktory-0.3.0/laktory/models/resources/databricks/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Union
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.mwspermissionassignment import MwsPermissionAssignment
+from laktory.models.resources.databricks.mwspermissionassignment import (
+    MwsPermissionAssignment,
+)
 
 
 class Group(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks group
 
     Attributes
@@ -22,15 +24,15 @@
         When `True`, the group is allowed to have workspace access
 
     Examples
     --------
     ```py
     from laktory import models
 
-    d = models.Group(display_name="role-engineers")
+    d = models.resources.databricks.Group(display_name="role-engineers")
     ```
     """
 
     allow_cluster_create: bool = False
     display_name: str
     id: Union[str, None] = None
     workspace_access: bool = None
```

### Comparing `laktory-0.2.1/laktory/models/databricks/groupmember.py` & `laktory-0.3.0/laktory/models/resources/databricks/groupmember.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/job.py` & `laktory-0.3.0/laktory/models/resources/databricks/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any
 from typing import Literal
 from typing import Union
 from pydantic import model_validator
 from pydantic import Field
 from laktory._settings import settings
 from laktory.models.basemodel import BaseModel
-from laktory.models.databricks.cluster import Cluster
-from laktory.models.databricks.cluster import ClusterLibrary
-from laktory.models.databricks.accesscontrol import AccessControl
-from laktory.models.databricks.permissions import Permissions
+from laktory.models.resources.databricks.cluster import Cluster
+from laktory.models.resources.databricks.cluster import ClusterLibrary
+from laktory.models.resources.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.permissions import Permissions
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
 
 
 class JobCluster(Cluster):
     """
     Job Cluster. Same attributes as `laktory.models.Cluster`, except for
@@ -677,15 +677,15 @@
 
     access_controls:
       - group_name: account users
         permission_level: CAN_VIEW
       - group_name: role-engineers
         permission_level: CAN_MANAGE_RUN
     '''
-    job = models.Job.model_validate_yaml(io.StringIO(job_yaml))
+    job = models.resources.databricks.Job.model_validate_yaml(io.StringIO(job_yaml))
     ```
 
     References
     ----------
 
     * [Databricks Job](https://docs.databricks.com/en/workflows/jobs/create-run-jobs.html)
     * [Pulumi Databricks Job](https://www.pulumi.com/registry/packages/databricks/api-docs/job/#databricks-job)
```

### Comparing `laktory-0.2.1/laktory/models/databricks/metastore.py` & `laktory-0.3.0/laktory/models/resources/databricks/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.metastoreassignment import MetastoreAssignment
-from laktory.models.databricks.metastoredataaccess import MetastoreDataAccess
+from laktory.models.resources.databricks.metastoreassignment import MetastoreAssignment
+from laktory.models.resources.databricks.metastoredataaccess import MetastoreDataAccess
 from laktory.models.grants.metastoregrant import MetastoreGrant
-from laktory.models.databricks.grants import Grants
+from laktory.models.resources.databricks.grants import Grants
 
 
 class Metastore(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks Metastore
 
     Attributes
```

### Comparing `laktory-0.2.1/laktory/models/databricks/metastoreassignment.py` & `laktory-0.3.0/laktory/models/resources/databricks/metastoreassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/metastoredataaccess.py` & `laktory-0.3.0/laktory/models/resources/databricks/metastoredataaccess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union
 from laktory.models.basemodel import BaseModel
-from laktory.models.databricks.grants import Grants
+from laktory.models.resources.databricks.grants import Grants
 from laktory.models.grants.storagecredentialgrant import StorageCredentialGrant
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
 
 
 class MetastoreDataAccessAwsIamRole(BaseModel):
     """
```

### Comparing `laktory-0.2.1/laktory/models/databricks/mwspermissionassignment.py` & `laktory-0.3.0/laktory/models/resources/databricks/mwspermissionassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/notebook.py` & `laktory-0.3.0/laktory/models/resources/databricks/notebook.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Literal
 from typing import Union
 from pydantic import model_validator
 from laktory import constants
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.accesscontrol import AccessControl
-from laktory.models.databricks.permissions import Permissions
+from laktory.models.resources.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.permissions import Permissions
 
 
 class Notebook(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks Notebook
 
     Attributes
@@ -30,21 +30,23 @@
         Path to notebook in source code format on local filesystem.
 
     Examples
     --------
     ```py
     from laktory import models
 
-    notebook = models.Notebook(
-        source="./notebooks/pipelines/dlt_brz_template.py",
+    notebook = models.resources.databricks.Notebook(
+        source="./notebooks/dlt/dlt_laktory_pl.py",
     )
     print(notebook.path)
-    #> /.laktory/pipelines/dlt_brz_template.py
+    #> /.laktory/dlt/dlt_laktory_pl.py
 
-    notebook = models.Notebook(source="./notebooks/create_view.py", dirpath="/views/")
+    notebook = models.resources.databricks.Notebook(
+        source="./notebooks/create_view.py", dirpath="/views/"
+    )
     print(notebook.path)
     #> /views/create_view.py
     ```
     """
 
     access_controls: list[AccessControl] = []
     dirpath: str = None
```

### Comparing `laktory-0.2.1/laktory/models/databricks/permissions.py` & `laktory-0.3.0/laktory/models/resources/databricks/permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from laktory.models.basemodel import BaseModel
-from laktory.models.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.accesscontrol import AccessControl
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
 
 
 class Permissions(BaseModel, PulumiResource, TerraformResource):
     access_controls: list[AccessControl]
     pipeline_id: str = None
```

### Comparing `laktory-0.2.1/laktory/models/databricks/pipeline.py` & `laktory-0.3.0/laktory/models/resources/databricks/dltpipeline.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-import json
-import os
 from typing import Any
 from typing import Literal
 from typing import Union
 from pydantic import model_validator
 from pydantic import Field
 
-from laktory._settings import settings
-from laktory.constants import CACHE_ROOT
 from laktory.models.basemodel import BaseModel
-from laktory.models.databricks.cluster import Cluster
-from laktory.models.databricks.accesscontrol import AccessControl
-from laktory.models.databricks.permissions import Permissions
+from laktory.models.resources.databricks.cluster import Cluster
+from laktory.models.resources.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.permissions import Permissions
+from laktory.models.datasources.tabledatasource import TableDataSource
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.workspacefile import WorkspaceFile
-from laktory.models.sql.table import Table
 
 
 class PipelineLibraryFile(BaseModel):
     """
     Pipeline Library File specifications
 
     Attributes
@@ -130,34 +125,15 @@
         ]:
             if getattr(self, f, None) not in [None, [], {}]:
                 raise ValueError(f"Field {f} should be null")
 
         return self
 
 
-class PipelineUDF(BaseModel):
-    """
-    Pipeline User Define Function
-
-    Attributes
-    ----------
-    module_name:
-        Name of the module from which the function needs to be imported.
-    function_name:
-        Name of the function.
-    module_path:
-        Workspace filepath of the module, if not in the same directory as the pipeline notebook
-    """
-
-    module_name: str
-    function_name: str
-    module_path: str = None
-
-
-class Pipeline(BaseModel, PulumiResource, TerraformResource):
+class DLTPipeline(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks Delta Live Tables (DLT) Pipeline
 
     Attributes
     ----------
     access_controls:
         Pipeline access controls
@@ -188,21 +164,17 @@
         If `True`, Photon engine enabled.
     serverless:
         If `True`, serverless is enabled
     storage:
         A location on DBFS or cloud storage where output data and metadata required for pipeline execution are stored.
         By default, tables are stored in a subdirectory of this location. Change of this parameter forces recreation
         of the pipeline. (Conflicts with `catalog`).
-    tables:
-        List of tables to build
     target:
         The name of a database (in either the Hive metastore or in a UC catalog) for persisting pipeline output data.
         Configuring the target setting allows you to view and query the pipeline output data from the Databricks UI.
-    udfs:
-        List of user defined functions provided to the table builders.
 
     Examples
     --------
     Assuming the configuration yaml file
     ```py
     import io
     from laktory import models
@@ -231,67 +203,18 @@
 
     access_controls:
       - group_name: account users
         permission_level: CAN_VIEW
       - group_name: role-engineers
         permission_level: CAN_RUN
 
-    # --------------------------------------------------------------------------- #
-    # Tables                                                                      #
-    # --------------------------------------------------------------------------- #
-
-    tables:
-      - name: brz_stock_prices
-        timestamp_key: data.created_at
-        builder:
-          layer: BRONZE
-          event_source:
-            name: stock_price
-            producer:
-              name: yahoo-finance
-            read_as_stream: True
-
-      - name: slv_stock_prices
-        timestamp_key: created_at
-        builder:
-          layer: SILVER
-          table_source:
-            name: brz_stock_prices
-            read_as_stream: True
-          spark_chain:
-            nodes:
-              - column:
-                    name: created_at
-                    type: timestamp
-                spark_func_name: coalesce
-                spark_func_args:
-                  - data._created_at
-
-              - column:
-                    name: symbol
-                    type: string
-                spark_func_name: coalesce
-                spark_func_args:
-                  - data.symbol
-
-              - column:
-                    name: open
-                    type: double
-                spark_func_name: coalesce
-                spark_func_args:
-                  - data.open
-
-              - column:
-                    name: close
-                    type: double
-                spark_func_name: coalesce
-                spark_func_args:
-                  - data.close
     '''
-    pipeline = models.Pipeline.model_validate_yaml(io.StringIO(pipeline_yaml))
+    pipeline = models.resources.databricks.DLTPipeline.model_validate_yaml(
+        io.StringIO(pipeline_yaml)
+    )
     ```
 
     References
     ----------
 
     * [Databricks Pipeline](https://docs.databricks.com/api/workspace/pipelines/create)
     * [Pulumi Databricks Pipeline](https://www.pulumi.com/registry/packages/databricks/api-docs/pipeline/)
@@ -309,95 +232,43 @@
     # filters
     libraries: list[PipelineLibrary] = None
     name: str
     notifications: list[PipelineNotifications] = []
     photon: bool = None
     serverless: bool = None
     storage: str = None
-    tables: list[Table] = []
     target: str = None
-    udfs: list[PipelineUDF] = []
-
-    @model_validator(mode="after")
-    def assign_pipeline_to_tables(self) -> Any:
-        for t in self.tables:
-            t.builder.pipeline_name = self.name
-            t.catalog_name = self.catalog
-            t.schema_name = self.target
-            for c in t.columns:
-                c.table_name = t.name
-                c.catalog_name = t.catalog_name
-                c.schema_name = t.schema_name
-
-            # Assign to sources
-            if t.builder.table_source is not None:
-                if t.builder.table_source.catalog_name is None:
-                    t.builder.table_source.catalog_name = self.catalog
-                if t.builder.table_source.schema_name is None:
-                    t.builder.table_source.schema_name = self.target
-
-        return self
 
     # ----------------------------------------------------------------------- #
     # Resource Properties                                                     #
     # ----------------------------------------------------------------------- #
 
     @property
     def resource_type_id(self) -> str:
         """
-        pl
+        dlt
         """
-        return "pl"
+        return "dlt"
 
     @property
     def additional_core_resources(self) -> list[PulumiResource]:
         """
         - permissions
-        - configuration workspace file
-        - configuration workspace file permissions
         """
         resources = []
 
         if self.access_controls:
             resources += [
                 Permissions(
                     resource_name=f"permissions-{self.resource_name}",
                     access_controls=self.access_controls,
                     pipeline_id=f"${{resources.{self.resource_name}.id}}",
                 )
             ]
 
-        # Configuration file
-        source = os.path.join(CACHE_ROOT, f"tmp-{self.name}.json")
-        d = self.model_dump(exclude_none=True)
-        d = self.inject_vars(d)
-        s = json.dumps(d, indent=4)
-        with open(source, "w", newline="\n") as fp:
-            fp.write(s)
-        filepath = f"{settings.workspace_laktory_root}pipelines/{self.name}.json"
-        file = WorkspaceFile(
-            path=filepath,
-            source=source,
-        )
-        resources += [file]
-
-        resources += [
-            Permissions(
-                resource_name=f"permissions-{file.resource_name}",
-                access_controls=[
-                    AccessControl(
-                        permission_level="CAN_READ",
-                        group_name="account users",
-                    )
-                ],
-                workspace_file_path=filepath,
-                options={"depends_on": [f"${{resources.{file.resource_name}}}"]},
-            )
-        ]
-
         return resources
 
     # ----------------------------------------------------------------------- #
     # Pulumi Properties                                                       #
     # ----------------------------------------------------------------------- #
 
     @property
@@ -410,17 +281,15 @@
 
         return databricks.Pipeline
 
     @property
     def pulumi_excludes(self) -> Union[list[str], dict[str, bool]]:
         return {
             "access_controls": True,
-            "tables": True,
             "clusters": {"__all__": {"access_controls"}},
-            "udfs": True,
         }
 
     @property
     def pulumi_properties(self):
         d = super().pulumi_properties
         k = "clusters"
         if k in d:
```

### Comparing `laktory-0.2.1/laktory/models/databricks/secret.py` & `laktory-0.3.0/laktory/models/resources/databricks/secret.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/secretacl.py` & `laktory-0.3.0/laktory/models/resources/databricks/secretacl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/secretscope.py` & `laktory-0.3.0/laktory/models/resources/databricks/secretscope.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Any
 from typing import Union
 from pydantic import Field
 from pydantic import model_validator
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.secret import Secret
-from laktory.models.databricks.secretacl import SecretAcl
+from laktory.models.resources.databricks.secret import Secret
+from laktory.models.resources.databricks.secretacl import SecretAcl
 
 
 class SecretScopePermission(BaseModel):
     """
     Secret scope permission
 
     Attributes
@@ -60,15 +60,15 @@
         List of secret to add to the scope
 
     Examples
     --------
     ```py
     from laktory import models
 
-    ss = models.SecretScope(
+    ss = models.resources.databricks.SecretScope(
         name="azure",
         secrets=[
             {"key": "keyvault-url", "value": "https://my-secrets.vault.azure.net/"},
             {"key": "client-id", "value": "f461daa2-c281-4166-bc3e-538b90223184"},
         ],
         permissions=[
             {"permission": "READ", "principal": "role-metastore-admins"},
```

### Comparing `laktory-0.2.1/laktory/models/databricks/serviceprincipal.py` & `laktory-0.3.0/laktory/models/resources/databricks/serviceprincipal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Union
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.serviceprincipalrole import ServicePrincipalRole
-from laktory.models.databricks.groupmember import GroupMember
+from laktory.models.resources.databricks.serviceprincipalrole import (
+    ServicePrincipalRole,
+)
+from laktory.models.resources.databricks.groupmember import GroupMember
 
 
 class ServicePrincipal(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks account service principal
 
     Attributes
@@ -28,15 +30,15 @@
         List of roles assigned to the user e.g. ("account_admin")
 
     Examples
     --------
     ```py
     from laktory import models
 
-    sp = models.ServicePrincipal(
+    sp = models.resources.databricks.ServicePrincipal(
         display_name="neptune",
         application_id="baf147d1-a856-4de0-a570-8a56dbd7e234",
         group_ids=[
             "${resources.group-role-engineer.id}",
             "${resources.group-role-analyst.id}",
             "${resources.group-domain-finance.id}",
             "${resources.group-domain-engineering.id}",
```

### Comparing `laktory-0.2.1/laktory/models/databricks/serviceprincipalrole.py` & `laktory-0.3.0/laktory/models/resources/databricks/serviceprincipalrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/sqlquery.py` & `laktory-0.3.0/laktory/models/resources/databricks/sqlquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Any
 from typing import Literal
 from typing import Union
 from pydantic import model_validator
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.accesscontrol import AccessControl
-from laktory.models.databricks.permissions import Permissions
+from laktory.models.resources.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.permissions import Permissions
 
 
 class SqlQuery(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks SQL Query
 
     Attributes
@@ -34,15 +34,15 @@
         List of tags
 
     Examples
     --------
     ```py
     from laktory import models
 
-    q = models.SqlQuery(
+    q = models.resources.databricks.SqlQuery(
         name="create-view",
         query="CREATE VIEW google_stock_prices AS SELECT * FROM stock_prices WHERE symbol = 'GOOGL'",
         data_source_id="09z739ce103q9374",
         parent="folders/2479128258235163",
         access_controls=[
             {
                 "group_name": "role-engineers",
```

### Comparing `laktory-0.2.1/laktory/models/databricks/user.py` & `laktory-0.3.0/laktory/models/resources/databricks/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.userrole import UserRole
-from laktory.models.databricks.groupmember import GroupMember
+from laktory.models.resources.databricks.userrole import UserRole
+from laktory.models.resources.databricks.groupmember import GroupMember
 
 
 class User(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks user
 
     Attributes
@@ -27,15 +27,15 @@
         When `True`, the user is allowed to have workspace access
 
     Examples
     --------
     ```py
     from laktory import models
 
-    u = models.User(
+    u = models.resources.databricks.User(
         user_name="john.doe@okube.ai",
         display_name="John Doe",
         group_ids=[
             "${resources.group-role-engineer.id}",
             "${resources.group-domain-finance.id}",
         ],
         roles=["account_admin"],
```

### Comparing `laktory-0.2.1/laktory/models/databricks/userrole.py` & `laktory-0.3.0/laktory/models/resources/databricks/userrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/databricks/warehouse.py` & `laktory-0.3.0/laktory/models/resources/databricks/warehouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Literal
 from typing import Union
 from laktory._settings import settings
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.accesscontrol import AccessControl
-from laktory.models.databricks.permissions import Permissions
+from laktory.models.resources.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.permissions import Permissions
 
 
 class WarehouseCustomTag(BaseModel):
     """
     Warehouse Custom Tag specifications
 
     Attributes
@@ -76,15 +76,15 @@
         SQL warehouse type.
 
     Examples
     --------
     ```py
     from laktory import models
 
-    warehouse = models.Warehouse(
+    warehouse = models.resources.databricks.Warehouse(
         name="default",
         cluster_size="2X-Small",
         auto_stop_mins=30,
         channel_name="CHANNEL_NAME_PREVIEW",
         enable_photon=True,
         enable_serverless_compute=True,
         access_controls=[{"group_name": "account users", "permission_level": "CAN_USE"}],
```

### Comparing `laktory-0.2.1/laktory/models/databricks/workspacefile.py` & `laktory-0.3.0/laktory/models/resources/databricks/workspacefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Any
 from typing import Union
 from pydantic import model_validator
 from laktory import constants
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.databricks.accesscontrol import AccessControl
-from laktory.models.databricks.permissions import Permissions
+from laktory.models.resources.databricks.accesscontrol import AccessControl
+from laktory.models.resources.databricks.permissions import Permissions
 
 
 class WorkspaceFile(BaseModel, PulumiResource, TerraformResource):
     """
     Databricks Workspace File
 
     Attributes
```

### Comparing `laktory-0.2.1/laktory/models/dataevent.py` & `laktory-0.3.0/laktory/models/dataevent.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,64 +4,87 @@
 from typing import Any
 from typing import Literal
 from typing import Union
 
 from pydantic import Field
 from pydantic import ConfigDict
 
-from laktory.models.dataeventheader import DataEventHeader
+from laktory.models.basemodel import BaseModel
 from laktory.models.dataproducer import DataProducer
 from laktory._settings import settings
 from laktory._logger import get_logger
 
 logger = get_logger(__name__)
 
+# Metadata to exclude
 EXCLUDES = [
     "events_root_",
-    "event_path",
+    "event_root_",
     "tstamp_col",
     "tstamp_in_path",
 ]
 
 
-class DataEvent(DataEventHeader):
+class DataEvent(BaseModel):
     """
     Data Event class defines both the context (metadata) describing a data
     event and its content. It is generally used to write data to a storage
     location.
 
     Attributes
     ----------
-    data
+    data:
         Event data stored as a (key, value) object
-    tstamp_col
+    description:
+        Data event description
+    event_root:
+        Root path for specific event. Default value: `{settings.workspace_landing_root}/events/my-event`
+    events_root:
+        Root path for all events. Default value: `{settings.workspace_landing_root}/events/`
+    name:
+        Data event name
+    producer:
+        Data event producer
+    tstamp_col:
         Column storing event UTC timestamp
-    tstamp_in_path
+    tstamp_in_path:
         If `True`, includes timestamp if data event filepath
 
     Examples
     --------
     This is example one
     ```py
     from laktory import models
     from datetime import datetime
 
     event = models.DataEvent(
         name="stock_price",
         producer={"name": "yahoo-finance"},
+    )
+    print(event)
+    '''
+    variables={} data=None description=None events_root_=None event_root_=None name='stock_price' producer=DataProducer(variables={}, name='yahoo-finance', description=None, party=1) tstamp_col='created_at' tstamp_in_path=True
+    '''
+
+    print(event.event_root)
+    #> /Volumes/dev/sources/landing/events/yahoo-finance/stock_price/
+
+    event = models.DataEvent(
+        name="stock_price",
+        producer={"name": "yahoo-finance"},
         data={
             "created_at": datetime(2023, 8, 23),
             "symbol": "GOOGL",
             "open": 130.25,
             "close": 132.33,
         },
     )
     print(event)
     '''
-    variables={} name='stock_price' description=None producer=DataProducer(variables={}, name='yahoo-finance', description=None, party=1) events_root_=None event_root_=None data={'created_at': datetime.datetime(2023, 8, 23, 0, 0), 'symbol': 'GOOGL', 'open': 130.25, 'close': 132.33, '_name': 'stock_price', '_producer_name': 'yahoo-finance', '_created_at': datetime.datetime(2023, 8, 23, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='UTC'))} tstamp_col='created_at' tstamp_in_path=True
+    variables={} data={'created_at': datetime.datetime(2023, 8, 23, 0, 0), 'symbol': 'GOOGL', 'open': 130.25, 'close': 132.33, '_name': 'stock_price', '_producer_name': 'yahoo-finance', '_created_at': datetime.datetime(2023, 8, 23, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='UTC'))} description=None events_root_=None event_root_=None name='stock_price' producer=DataProducer(variables={}, name='yahoo-finance', description=None, party=1) tstamp_col='created_at' tstamp_in_path=True
     '''
 
     print(event.dirpath)
     #> /Volumes/dev/sources/landing/events/yahoo-finance/stock_price/2023/08/23/
 
     print(event.get_landing_filepath())
     '''
@@ -69,34 +92,39 @@
     '''
 
     print(event.get_storage_filepath())
     #> /events/yahoo-finance/stock_price/2023/08/23/stock_price_20230823T000000000Z.json
     ```
     """
 
-    name: str = Field(..., alias="event_name")
-    description: Union[str, None] = Field(None, alias="event_description")
-    producer: DataProducer = Field(None, alias="event_producer", description="producer")
-    data: dict
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    data: Union[dict, None] = None
+    description: Union[str, None] = None
+    events_root_: Union[str, None] = Field(None, alias="events_root")
+    event_root_: Union[str, None] = Field(None, alias="event_root")
+    name: str
+    producer: DataProducer = None
     tstamp_col: str = "created_at"
     tstamp_in_path: bool = True
 
     def model_post_init(self, __context):
         super().model_post_init(__context)
+
         # Add metadata
-        self.data["_name"] = self.name
-        self.data["_producer_name"] = self.producer.name
-        tstamp = self.data.get(self.tstamp_col)
-        if isinstance(tstamp, str):
-            tstamp = datetime.fromisoformat(tstamp)
-        elif tstamp is None:
-            tstamp = datetime.utcnow()
-        if not tstamp.tzinfo:
-            tstamp = tstamp.replace(tzinfo=ZoneInfo("UTC"))
-        self.data["_created_at"] = tstamp
+        if self.data is not None:
+            self.data["_name"] = self.name
+            self.data["_producer_name"] = self.producer.name
+            tstamp = self.data.get(self.tstamp_col)
+            if isinstance(tstamp, str):
+                tstamp = datetime.fromisoformat(tstamp)
+            elif tstamp is None:
+                tstamp = datetime.utcnow()
+            if not tstamp.tzinfo:
+                tstamp = tstamp.replace(tzinfo=ZoneInfo("UTC"))
+            self.data["_created_at"] = tstamp
 
     # ----------------------------------------------------------------------- #
     # Properties                                                              #
     # ----------------------------------------------------------------------- #
 
     @property
     def created_at(self) -> datetime:
@@ -104,14 +132,41 @@
         return self.data["_created_at"]
 
     # ----------------------------------------------------------------------- #
     # Paths                                                                   #
     # ----------------------------------------------------------------------- #
 
     @property
+    def events_root(self) -> str:
+        """Must be computed to dynamically account for settings (env variable at run time)"""
+        if self.events_root_:
+            return self.events_root_
+        return settings.workspace_landing_root + "events/"
+
+    @property
+    def event_root(self) -> str:
+        """
+        Root path for the event. Default path is `{self.events_roots}/{producer_name}/{event_name}/`, but it may
+        be overwritten by self.event_root_.
+
+        Returns
+        -------
+        str
+            Event path
+        """
+        if self.event_root_:
+            return self.event_root_
+
+        producer = ""
+        if self.producer is not None:
+            producer = self.producer.name + "/"
+        v = f"{self.events_root}{producer}{self.name}/"
+        return v
+
+    @property
     def dirpath(self) -> str:
         """Path of the directory storing the event data."""
         dirpath = self.event_root
         if self.tstamp_in_path:
             t = self.created_at
             dirpath += f"{t.year:04d}/{t.month:02d}/{t.day:02d}/"
         return dirpath
@@ -233,21 +288,21 @@
     ) -> None:
         """
         Write data event to local file path, given a format `fmt` and a
         `suffix`.
 
         Parameters
         ----------
-        suffix
+        suffix:
             File path suffix
-        fmt
+        fmt:
             File format
-        overwrite
+        overwrite:
             Overwrite file if already exists
-        skip_if_exists
+        skip_if_exists:
             If `True` and file already exists, writing is skipped.
         """
         path = self.get_landing_filepath(suffix=suffix, fmt=fmt)
         dirpath = os.path.dirname(path)
 
         if not os.path.exists(dirpath):
             os.makedirs(dirpath)
@@ -279,27 +334,27 @@
     ) -> None:
         """
         Write data event to azure storage container, given a format `fmt` and a
         `suffix`.
 
         Parameters
         ----------
-        suffix
+        suffix:
             File path suffix
-        fmt
+        fmt:
             File format
-        container_client
+        container_client:
             Authorized Azure container client
-        account_url
+        account_url:
             URL of storage account
-        container_name
+        container_name:
             Name of the storage container
-        overwrite
+        overwrite:
             Overwrite file if already exists
-        skip_if_exists
+        skip_if_exists:
             If `True` and file already exists, writing is skipped.
         """
         # Set container client
         if container_client is None:
             from azure.storage.blob import ContainerClient
             from azure.identity import DefaultAzureCredential
 
@@ -355,23 +410,23 @@
     ) -> None:
         """
         Write data event to azure storage container, given a format `fmt` and a
         `suffix`.
 
         Parameters
         ----------
-        suffix
+        suffix:
             File path suffix
-        fmt
+        fmt:
             File format
-        s3_resource
+        s3_resource:
             Authorized S3 bucket resource
-        overwrite
+        overwrite:
             Overwrite file if already exists
-        skip_if_exists
+        skip_if_exists:
             If `True` and file already exists, writing is skipped.
         """
         import boto3
 
         if s3_resource is None:
             s3_resource = boto3.resource(
                 service_name="s3",
```

### Comparing `laktory-0.2.1/laktory/models/dataproducer.py` & `laktory-0.3.0/laktory/models/dataproducer.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/datasources/eventdatasource.py` & `laktory-0.3.0/laktory/models/datasources/filedatasource.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,105 @@
-from pydantic import model_validator
-from laktory.spark import DataFrame
+import os.path
+
 from typing import Literal
 
-from laktory.models.dataeventheader import DataEventHeader
 from laktory.models.datasources.basedatasource import BaseDataSource
+from laktory.spark import SparkDataFrame
+from laktory.polars import PolarsDataFrame
 from laktory._logger import get_logger
 
 logger = get_logger(__name__)
 
 
-class EventDataSource(BaseDataSource, DataEventHeader):
+class FileDataSource(BaseDataSource):
     """
-    Data source using events data (files), generally used in the context of a
-    data pipeline.
+    Data source using disk files, such as data events (json/csv) and
+    dataframe parquets. It is generally used in the context of a data pipeline.
 
     Attributes
     ----------
-    fmt
-        Format of the stored data
+    format:
+        Format of the data files
     header
         If `True`, first line of CSV files is assumed to be the column names.
     multiline
         If `True`, JSON files are parsed assuming that an object maybe be
         defined on multiple lines (as opposed to having a single object
         per line)
     read_options:
         Other options passed to `spark.read.options`
     schema_location:
-        Path for events schema. If `None`, `event_root` is used.
-    type
-        Type of infrastructure storing the data
+        Path for files schema. If `None`, parent directory of `path` is used
 
     Examples
     ---------
     ```python
     from laktory import models
 
-    source = models.EventDataSource(
-        name="stock_price",
-        producer={"name": "yahoo-finance"},
-        fmt="JSON",
-        read_as_stream=False,
+    source = models.FileDataSource(
+        path="/Volumes/sources/landing/events/yahoo-finance/stock_price",
+        format="JSON",
+        as_stream=False,
     )
     # df = source.read(spark)
     ```
     """
 
-    fmt: Literal["JSON", "CSV", "PARQUET", "DELTA"] = "JSON"
+    format: Literal["CSV", "PARQUET", "DELTA", "JSON"] = "JSON"
     header: bool = True
     multiline: bool = False
+    path: str
     read_options: dict[str, str] = {}
     schema_location: str = None
-    type: Literal["STORAGE_EVENTS", "STREAM_KINESIS", "STREAM_KAFKA"] = "STORAGE_EVENTS"
 
     # ----------------------------------------------------------------------- #
-    # Readers                                                                 #
+    # Properties                                                              #
     # ----------------------------------------------------------------------- #
 
-    def _read(self, spark) -> DataFrame:
-        if self.mock_df is not None:
-            logger.info(f"Reading event data source ({self.name}) from memory")
-            return self.mock_df
-        if self.type == "STORAGE_EVENTS":
-            return self._read_storage(spark)
-        else:
-            raise NotImplementedError()
+    @property
+    def _id(self):
+        return str(self.path)
+
+    # ----------------------------------------------------------------------- #
+    # Readers                                                                 #
+    # ----------------------------------------------------------------------- #
 
-    def _read_storage(self, spark) -> DataFrame:
-        if self.read_as_stream:
-            logger.info(f"Reading {self.event_root} as stream")
+    def _read_spark(self, spark) -> SparkDataFrame:
+        if self.as_stream:
+            logger.info(f"Reading {self._id} as stream")
 
             schema_location = self.schema_location
             if schema_location is None:
-                schema_location = self.event_root
+                schema_location = os.path.dirname(self.path)
 
             # Set reader
             reader = (
                 spark.readStream.format("cloudFiles")
-                .option("cloudFiles.format", self.fmt)
+                .option("cloudFiles.format", self.format)
                 .option("cloudFiles.schemaLocation", schema_location)
                 .option("cloudFiles.inferColumnTypes", True)
                 .option("cloudFiles.schemaEvolutionMode", "addNewColumns")
                 .option("cloudFiles.allowOverwrites", True)
             )
 
         else:
-            logger.info(f"Reading {self.event_root} as static")
+            logger.info(f"Reading {self._id} as static")
 
             # Set reader
-            reader = spark.read.format(self.fmt)
+            reader = spark.read.format(self.format)
 
         reader = (
             reader.option("multiLine", self.multiline)  # only apply to JSON format
             .option("mergeSchema", True)
             .option("recursiveFileLookup", True)
             .option("header", self.header)  # only apply to CSV format
         )
         if self.read_options:
             reader = reader.options(**self.read_options)
 
         # Load
-        df = reader.load(self.event_root)
+        df = reader.load(self.path)
 
         # Not supported by UC
         # .withColumn("file", F.input_file_name())
 
         return df
```

### Comparing `laktory-0.2.1/laktory/models/grants/__init__.py` & `laktory-0.3.0/laktory/models/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/grants/cataloggrant.py` & `laktory-0.3.0/laktory/models/grants/cataloggrant.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
     privileges: list[
         Literal[
             "ALL_PRIVILEGES",
```

### Comparing `laktory-0.2.1/laktory/models/grants/connectiongrant.py` & `laktory-0.3.0/laktory/models/grants/viewgrant.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from typing import Literal
 from laktory.models.basemodel import BaseModel
 
+PRIVILEGES = [
+    "ALL_PRIVILEGES",
+    "SELECT",
+]
 
-class ConnectionGrant(BaseModel):
+
+class ViewGrant(BaseModel):
     """
-    Privileges granted to a principal and operating on a connection
+    Privileges granted to a principal and operating on a view
 
     Attributes
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
     privileges: list[
         Literal[
             "ALL_PRIVILEGES",
-            "CREATE_FOREIGN_CATALOG",
-            "USE_CONNECTION",
+            "SELECT",
         ]
     ]
```

### Comparing `laktory-0.2.1/laktory/models/grants/externallocationgrant.py` & `laktory-0.3.0/laktory/models/grants/externallocationgrant.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
     privileges: list[
         Literal[
             "ALL_PRIVILEGES",
```

### Comparing `laktory-0.2.1/laktory/models/grants/functiongrant.py` & `laktory-0.3.0/laktory/models/grants/functiongrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
     privileges: list[Literal["ALL_PRIVILEGES", "EXECUTE"]]
```

### Comparing `laktory-0.2.1/laktory/models/grants/metastoregrant.py` & `laktory-0.3.0/laktory/models/grants/metastoregrant.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
     privileges: list[
         Literal[
             "CREATE_CATALOG",
```

### Comparing `laktory-0.2.1/laktory/models/grants/registeredmodelgrant.py` & `laktory-0.3.0/laktory/models/grants/volumegrant.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from typing import Literal
 from laktory.models.basemodel import BaseModel
 
 
-class RegisteredModelGrant(BaseModel):
+class VolumeGrant(BaseModel):
     """
-    Privileges granted to a principal and operating on a registered model
+    Privileges granted to a principal and operating on a volume
 
     Attributes
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
-    privileges: list[Literal["ALL_PRIVILEGES", "EXECUTE"]]
+    privileges: list[
+        Literal[
+            "ALL_PRIVILEGES",
+            "READ_VOLUME",
+            "WRITE_VOLUME",
+        ]
+    ]
```

### Comparing `laktory-0.2.1/laktory/models/grants/schemagrant.py` & `laktory-0.3.0/laktory/models/grants/schemagrant.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
     privileges: list[
         Literal[
             "ALL_PRIVILEGES",
```

### Comparing `laktory-0.2.1/laktory/models/grants/sharegrant.py` & `laktory-0.3.0/laktory/models/grants/connectiongrant.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from typing import Literal
 from laktory.models.basemodel import BaseModel
 
 
-class ShareGrant(BaseModel):
+class ConnectionGrant(BaseModel):
     """
-    Privileges granted to a principal and operating on a share
+    Privileges granted to a principal and operating on a connection
 
     Attributes
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
-    privileges: list[Literal["SELECT"]]
+    privileges: list[
+        Literal[
+            "ALL_PRIVILEGES",
+            "CREATE_FOREIGN_CATALOG",
+            "USE_CONNECTION",
+        ]
+    ]
```

### Comparing `laktory-0.2.1/laktory/models/grants/storagecredentialgrant.py` & `laktory-0.3.0/laktory/models/grants/storagecredentialgrant.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
     privileges: list[
         Literal[
             "ALL PRIVILEGES",
```

### Comparing `laktory-0.2.1/laktory/models/grants/tablegrant.py` & `laktory-0.3.0/laktory/models/grants/sharegrant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from typing import Literal
 from laktory.models.basemodel import BaseModel
 
 
-class TableGrant(BaseModel):
+class ShareGrant(BaseModel):
     """
-    Privileges granted to a principal and operating on a table
+    Privileges granted to a principal and operating on a share
 
     Attributes
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
     ----------
-
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
-    privileges: list[Literal["ALL_PRIVILEGES", "SELECT", "MODIFY"]]
-
-
-t = TableGrant(principal="a", privileges=["SELECT"])
+    privileges: list[Literal["SELECT"]]
```

### Comparing `laktory-0.2.1/laktory/models/grants/viewgrant.py` & `laktory-0.3.0/laktory/models/grants/registeredmodelgrant.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 from typing import Literal
 from laktory.models.basemodel import BaseModel
 
-PRIVILEGES = [
-    "ALL_PRIVILEGES",
-    "SELECT",
-]
 
-
-class ViewGrant(BaseModel):
+class RegisteredModelGrant(BaseModel):
     """
-    Privileges granted to a principal and operating on a view
+    Privileges granted to a principal and operating on a registered model
 
     Attributes
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
-    privileges: list[
-        Literal[
-            "ALL_PRIVILEGES",
-            "SELECT",
-        ]
-    ]
+    privileges: list[Literal["ALL_PRIVILEGES", "EXECUTE"]]
```

### Comparing `laktory-0.2.1/laktory/models/grants/volumegrant.py` & `laktory-0.3.0/laktory/models/grants/tablegrant.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from typing import Literal
 from laktory.models.basemodel import BaseModel
 
 
-class VolumeGrant(BaseModel):
+class TableGrant(BaseModel):
     """
-    Privileges granted to a principal and operating on a volume
+    Privileges granted to a principal and operating on a table
 
     Attributes
     ----------
     principal
         User, group or service principal name
     privileges
         List of allowed privileges
 
     References
-
+    ----------
     * [privilege types](https://docs.databricks.com/en/sql/language-manual/sql-ref-privileges.html#privilege-types)
     """
 
     principal: str
-    privileges: list[
-        Literal[
-            "ALL_PRIVILEGES",
-            "READ_VOLUME",
-            "WRITE_VOLUME",
-        ]
-    ]
+    privileges: list[Literal["ALL_PRIVILEGES", "SELECT", "MODIFY"]]
+
+
+t = TableGrant(principal="a", privileges=["SELECT"])
```

### Comparing `laktory-0.2.1/laktory/models/providers/awsprovider.py` & `laktory-0.3.0/laktory/models/resources/providers/awsprovider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from laktory.models.basemodel import BaseModel
-from laktory.models.providers.baseprovider import BaseProvider
+from laktory.models.resources.providers.baseprovider import BaseProvider
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
 
 
 class ProviderDefaultTags(BaseModel):
     tags: dict[str, str] = None
```

### Comparing `laktory-0.2.1/laktory/models/providers/azureprovider.py` & `laktory-0.3.0/laktory/models/resources/providers/azureprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from laktory.models.providers.baseprovider import BaseProvider
+from laktory.models.resources.providers.baseprovider import BaseProvider
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
 
 
 class AzureProvider(BaseProvider, PulumiResource, TerraformResource):
     """
     Azure Provider
```

### Comparing `laktory-0.2.1/laktory/models/providers/azurepulumiprovider.py` & `laktory-0.3.0/laktory/models/resources/providers/azurepulumiprovider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from laktory.models.providers.baseprovider import BaseProvider
+from laktory.models.resources.providers.baseprovider import BaseProvider
 from laktory.models.resources.pulumiresource import PulumiResource
 
 
 class AzurePulumiProvider(BaseProvider, PulumiResource):
     """
     Azure Pulumi (Native) Provider
```

### Comparing `laktory-0.2.1/laktory/models/providers/baseprovider.py` & `laktory-0.3.0/laktory/models/resources/providers/baseprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/providers/databricksprovider.py` & `laktory-0.3.0/laktory/models/resources/providers/databricksprovider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import Field
-from laktory.models.providers.baseprovider import BaseProvider
+from laktory.models.resources.providers.baseprovider import BaseProvider
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
 
 
 class DatabricksProvider(BaseProvider, PulumiResource, TerraformResource):
     """
     Databricks Provider
```

### Comparing `laktory-0.2.1/laktory/models/resources/baseresource.py` & `laktory-0.3.0/laktory/models/resources/baseresource.py`

 * *Files 8% similar despite different names*

```diff
@@ -162,28 +162,39 @@
     @property
     def core_resources(self):
         """
         List of core resources to be deployed with this laktory model:
         - class instance (self)
         """
         if self._core_resources is None:
-            # Get all resources
+            # Add self
             self._core_resources = []
             if self.self_as_core_resources:
                 self._core_resources += [self]
-            self._core_resources += self.additional_core_resources
 
-            # Propagate options
-            r0 = self._core_resources[0]
-            provider = r0.options.provider
-            k0 = f"${{resources.{r0.resource_name}}}"
-            for r in self._core_resources[1:]:
-                if provider:
-                    if r.options.provider is None:
-                        r.options.provider = provider
-
-                do = r.options.depends_on
-                if k0 not in do:
-                    do += [k0]
-                r.options.depends_on = do
+            # Add additional
+            def get_additional_resources(r):
+                resources = []
+
+                provider = r.options.provider
+                k0 = f"${{resources.{r.resource_name}}}"
+                for _r in r.additional_core_resources:
+                    if provider:
+                        if _r.options.provider is None:
+                            _r.options.provider = provider
+
+                    do = _r.options.depends_on
+                    if r.self_as_core_resources and k0 not in do:
+                        do += [k0]
+                    _r.options.depends_on = do
+
+                    if _r.self_as_core_resources:
+                        resources += [_r]
+
+                    for __r in get_additional_resources(_r):
+                        resources += [__r]
+
+                return resources
+
+            self._core_resources += get_additional_resources(self)
 
         return self._core_resources
```

### Comparing `laktory-0.2.1/laktory/models/resources/pulumiresource.py` & `laktory-0.3.0/laktory/models/resources/pulumiresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/resources/terraformresource.py` & `laktory-0.3.0/laktory/models/resources/terraformresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/spark/_common.py` & `laktory-0.3.0/laktory/models/spark/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/spark/sparkchain.py` & `laktory-0.3.0/laktory/models/spark/sparkchain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Union
 
 from laktory._logger import get_logger
 from laktory.models.basemodel import BaseModel
 from laktory.models.spark.sparkchainnode import SparkChainNode
-from laktory.spark import DataFrame
+from laktory.spark import SparkDataFrame
 
 logger = get_logger(__name__)
 
 
 # --------------------------------------------------------------------------- #
 # Main Class                                                                  #
 # --------------------------------------------------------------------------- #
 
 
 class SparkChain(BaseModel):
     """
     The Spark Chain class defines a series of transformation to be applied to
-    a DataFrame. Each transformation is expressed as a node (SparkChainNode
+    a dataframe. Each transformation is expressed as a node (SparkChainNode
     object) that, upon execution, returns a new dataframe. As a convenience,
     `column` can be specified to create a new column. In this case, the spark
     function or sql expression is expected to return a column instead of a
-    DataFrame. Each node is executed sequentially in the provided order. A node
+    dataframe. Each node is executed sequentially in the provided order. A node
     may also be another Spark Chain.
 
     Attributes
     ----------
     nodes:
         The list of transformations to be executed.
 
@@ -72,15 +72,15 @@
                     "x_tmp",
                 ],
             },
         ]
     )
 
     # Execute Chain
-    df = sc.execute(df0, spark=spark)
+    df = sc.execute(df0)
 
     # Print result
     print(df.toPandas().to_string())
     '''
           cos_x        x2
     0  0.540302  1.000000
     1 -0.416147  1.414214
@@ -92,23 +92,23 @@
     nodes: list[Union[SparkChainNode, "SparkChain"]]
     _columns: list[list[str]] = []
 
     @property
     def columns(self):
         return self._columns
 
-    def execute(self, df, udfs=None, spark=None) -> DataFrame:
+    def execute(self, df, udfs=None) -> SparkDataFrame:
         logger.info("Executing Spark chain")
 
         for inode, node in enumerate(self.nodes):
             self._columns += [df.columns]
 
             tnode = type(node)
-            logger.info(f"Executing node {inode} ({tnode.__name__}).")
-            df = node.execute(df, udfs=udfs, spark=spark)
+            logger.info(f"Executing spark chain node {inode} ({tnode.__name__}).")
+            df = node.execute(df, udfs=udfs)
 
         return df
 
 
 SparkChain.model_rebuild()
```

### Comparing `laktory-0.2.1/laktory/models/spark/sparkchainnode.py` & `laktory-0.3.0/laktory/models/spark/sparkchainnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Union
 from typing import Callable
 
 from laktory._logger import get_logger
 from laktory.constants import SUPPORTED_TYPES
 from laktory.models.basemodel import BaseModel
 from laktory.models.spark.sparkfuncarg import SparkFuncArg
-from laktory.spark import DataFrame
-from laktory.spark import Column
+from laktory.spark import SparkDataFrame
+from laktory.spark import SparkColumn
 from laktory.models.spark._common import parse_args
 from laktory.models.spark._common import parse_kwargs
 from laktory.exceptions import MissingColumnError
 from laktory.exceptions import MissingColumnsError
 
 logger = get_logger(__name__)
 
@@ -50,18 +50,18 @@
                     f"Type {v} is not supported. Select one of {SUPPORTED_TYPES}"
                 )
         return v
 
 
 class SparkChainNode(BaseModel):
     """
-    SparkChain node that output a DataFrame upon execution. As a convenience,
+    SparkChain node that output a dataframe upon execution. As a convenience,
     `column` can be specified to create a new column. In this case, the spark
     function or sql expression is expected to return a column instead of a
-    DataFrame. Each node is executed sequentially in the provided order. A node
+    dataframe. Each node is executed sequentially in the provided order. A node
     may also be another Spark Chain.
 
     Attributes
     ----------
     allow_missing_column_args:
         If `True`, spark func column arguments are allowed to be missing
         without raising an exception.
@@ -123,15 +123,15 @@
     3  3 -0.989992  3.0
     '''
 
     node = models.SparkChainNode(
         spark_func_name="drop_duplicates",
         spark_func_args=[["x"]],
     )
-    df = node.execute(df0, spark=spark)
+    df = node.execute(df0)
 
     print(df.toPandas().to_string())
     '''
        x
     0  1
     1  2
     2  3
@@ -164,45 +164,42 @@
 
     # ----------------------------------------------------------------------- #
     # Class Methods                                                           #
     # ----------------------------------------------------------------------- #
 
     def execute(
         self,
-        df: DataFrame,
-        udfs: list[Callable[[...], Union[Column, DataFrame]]] = None,
+        df: SparkDataFrame,
+        udfs: list[Callable[[...], Union[SparkColumn, SparkDataFrame]]] = None,
         return_col: bool = False,
-        spark=None,
-    ) -> Union[DataFrame, Column]:
+    ) -> Union[SparkDataFrame, SparkColumn]:
         """
         Build Spark Column
 
         Parameters
         ----------
         df:
-            Input DataFrame
+            Input dataframe
         udfs:
             User-defined functions
         return_col
             If `True` and column specified, function returns `Column` object
-            instead of DataFrame.
-        spark:
-            Spark Session
+            instead of dataframe.
 
         Returns
         -------
-            Output DataFrame
+            Output dataframe
         """
         import pyspark.sql.functions as F
         from pyspark.sql.dataframe import DataFrame
         from pyspark.sql.connect.dataframe import DataFrame as DataFrameConnect
         from pyspark.sql import Column
         from laktory.spark.dataframe import has_column
         from laktory.spark import functions as LF
-        from laktory.spark import DataFrame as LDF
+        from laktory.spark import SparkDataFrame as LDF
 
         if udfs is None:
             udfs = []
         udfs = {f.__name__: f for f in udfs}
 
         # From SQL expression
         if self.sql_expression:
@@ -214,17 +211,17 @@
                 if self.column.type not in ["_any"]:
                     col = col.cast(self.column.type)
                 if return_col:
                     return col
                 return self.add_column(df, col)
             else:
                 raise NotImplementedError("sql_expression not supported yet")
-                #     df.createOrReplaceTempView("_df")
-                #     df = spark.sql(self.sql_expression)
-                #     return df
+                # TODO: This implementation should workd, but it should be tested and documented
+                df = df.sparkSession.sql(self.sql_expression, df=df)
+                return df
 
         # From Spark Function
         func_name = self.spark_func_name
         if self.spark_func_name is None:
             if self.is_column:
                 func_name = "coalesce"
             else:
@@ -306,15 +303,15 @@
 
         if len(_args) > 0 and len(args) < 1:
             raise MissingColumnsError(missing_column_names)
 
         # Build kwargs
         kwargs = {}
         for k, _arg in _kwargs.items():
-            kwargs[k] = _arg.eval(spark)
+            kwargs[k] = _arg.eval(df.sparkSession)
 
         # Function call
         logger.info(f"{self.id} as {func_name}({args}, {kwargs})")
 
         if self.is_column:
             col = f(*args, **kwargs)
             if self.column.type not in ["_any"]:
```

### Comparing `laktory-0.2.1/laktory/models/spark/sparkfuncarg.py` & `laktory-0.3.0/laktory/models/spark/sparkfuncarg.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,22 +25,20 @@
     @field_validator("value")
     def value_to_data_source(cls, v: Any) -> Any:
         """
         Data source can't be set as an expected value type as it would create
         a circular dependency. Instead, we check at validation if the value
         could be instantiated as a DataSource object.
         """
-        from laktory.models.datasources.eventdatasource import EventDataSource
-        from laktory.models.datasources.tabledatasource import TableDataSource
+        from laktory.models.datasources import classes
 
-        try:
-            v = TableDataSource(**v)
-        except:
+        for c in classes:
             try:
-                v = EventDataSource(**v)
+                v = c(**v)
+                break
             except:
                 pass
 
         return v
 
     def eval(self, spark=None):
         from laktory.models.datasources.basedatasource import BaseDataSource
```

### Comparing `laktory-0.2.1/laktory/models/sql/catalog.py` & `laktory-0.3.0/laktory/models/resources/databricks/catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 from typing import Literal
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.sql.schema import Schema
+from laktory.models.resources.databricks.schema import Schema
 from laktory.models.grants.cataloggrant import CatalogGrant
-from laktory.models.databricks.grants import Grants
+from laktory.models.resources.databricks.grants import Grants
 
 
 class Catalog(BaseModel, PulumiResource, TerraformResource):
     """
     A catalog is the first layer of Unity Catalog’s three-level namespace. It’s
     used to organize your data assets.
 
@@ -37,15 +37,15 @@
         default to the metastore root location.
 
     Examples
     --------
     ```py
     from laktory import models
 
-    catalog = models.Catalog(
+    catalog = models.resources.databricks.Catalog(
         name="dev",
         grants=[
             {"principal": "account users", "privileges": ["USE_CATALOG", "USE_SCHEMA"]}
         ],
         schemas=[
             {
                 "name": "engineering",
```

### Comparing `laktory-0.2.1/laktory/models/sql/column.py` & `laktory-0.3.0/laktory/models/resources/databricks/column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/sql/schema.py` & `laktory-0.3.0/laktory/models/resources/databricks/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Union
 
 from laktory.models.basemodel import BaseModel
-from laktory.models.databricks.grants import Grants
+from laktory.models.resources.databricks.grants import Grants
 from laktory.models.grants.schemagrant import SchemaGrant
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
-from laktory.models.sql.table import Table
-from laktory.models.sql.volume import Volume
+from laktory.models.resources.databricks.table import Table
+from laktory.models.resources.databricks.volume import Volume
 
 
 class Schema(BaseModel, PulumiResource, TerraformResource):
     """
     A schema (also called a database) is the second layer of Unity Catalog’s
     three-level namespace. A schema organizes tables and views.
 
@@ -36,15 +36,15 @@
         List of volumes stored in the schema
 
     Examples
     --------
     ```py
     from laktory import models
 
-    schema = models.Schema(
+    schema = models.resources.databricks.Schema(
         catalog_name="dev",
         name="engineering",
         grants=[{"principal": "domain-engineering", "privileges": ["SELECT"]}],
     )
     ```
 
     References
```

### Comparing `laktory-0.2.1/laktory/models/sql/tableexpectation.py` & `laktory-0.3.0/laktory/models/pipelinenodeexpectation.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,39 +2,40 @@
 
 from laktory._logger import get_logger
 from laktory.models.basemodel import BaseModel
 
 logger = get_logger(__name__)
 
 
-class TableExpectation(BaseModel):
+class PipelineNodeExpectation(BaseModel):
     """
-    Specifications for aggregation by group or time window.
+    Definition of an expectation for a given node output DataFrame. It consists
+    of an SQL expression of the expectation and of an action to be taken if the
+    expectation is not met. Similar to DLT Table Expectation. Currently only
+    supported with DLT pipeline orchestrator.
 
     Attributes
     ----------
     name:
         Name of the expectation
     expression:
         SQL expression definition the constraint
     action:
         Action to take when expectation is not met.
-        `ALLOW`: Invalid records are written to the target; failure is reported
-                 as a metric for the dataset.
-        `DROP`: Invalid records are dropped before data is written to the
-                target; failure is reported as a metrics for the dataset.
-        `FAIL`: Invalid records prevent the update from succeeding. Manual
-                intervention is required before re-processing.
+        `ALLOW`: Write invalid records to the output DataFrame, but log
+        exception.
+        `DROP`: Drop Invalid records to the output DataFrame and log exception.
+        `FAIL`: Raise exception when invalid records are found.
 
     Examples
     --------
     ```py
     from laktory import models
 
-    e = models.TableExpectation(
+    e = models.PipelineNodeExpectation(
         name="valid timestamp",
         expression="col(“timestamp”) > '2012-01-01'",
         action="DROP",
     )
     print(e)
     '''
     variables={} name='valid timestamp' expression="col(“timestamp”) > '2012-01-01'" action='DROP'
```

### Comparing `laktory-0.2.1/laktory/models/sql/volume.py` & `laktory-0.3.0/laktory/models/resources/databricks/volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal
 from typing import Union
 from laktory.models.basemodel import BaseModel
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
 from laktory.models.grants.volumegrant import VolumeGrant
-from laktory.models.databricks.grants import Grants
+from laktory.models.resources.databricks.grants import Grants
 
 
 class Volume(BaseModel, PulumiResource, TerraformResource):
     """
     Volumes are Unity Catalog objects representing a logical volume of storage
     in a cloud object storage location. Volumes provide capabilities for
     accessing, storing, governing, and organizing files. While tables provide
@@ -34,15 +34,15 @@
         List of grants operating on the volume
 
     Examples
     --------
     ```py
     from laktory import models
 
-    volume = models.Volume(
+    volume = models.resources.databricks.Volume(
         name="landing",
         catalog_name="dev",
         schema_name="sources",
         volume_type="EXTERNAL",
         storage_location="abfss://landing@lakehouse-storage.dfs.core.windows.net/",
         grants=[
             {"principal": "account users", "privileges": ["READ_VOLUME"]},
```

### Comparing `laktory-0.2.1/laktory/models/stacks/pulumistack.py` & `laktory-0.3.0/laktory/models/stacks/pulumistack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/models/stacks/stack.py` & `laktory-0.3.0/laktory/models/stacks/stack.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 from typing import Any
 from typing import Literal
 from pydantic import model_validator
 
 from laktory._logger import get_logger
 from laktory._parsers import merge_dicts
 from laktory.models.basemodel import BaseModel
-from laktory.models.databricks.dbfsfile import DbfsFile
-from laktory.models.databricks.cluster import Cluster
-from laktory.models.databricks.directory import Directory
-from laktory.models.databricks.group import Group
-from laktory.models.databricks.job import Job
-from laktory.models.databricks.externallocation import ExternalLocation
-from laktory.models.databricks.metastore import Metastore
-from laktory.models.databricks.metastoredataaccess import MetastoreDataAccess
-from laktory.models.databricks.notebook import Notebook
-from laktory.models.databricks.pipeline import Pipeline
-from laktory.models.databricks.secret import Secret
-from laktory.models.databricks.secretscope import SecretScope
-from laktory.models.databricks.serviceprincipal import ServicePrincipal
-from laktory.models.databricks.sqlquery import SqlQuery
-from laktory.models.databricks.user import User
-from laktory.models.databricks.warehouse import Warehouse
-from laktory.models.databricks.workspacefile import WorkspaceFile
-from laktory.models.providers.baseprovider import BaseProvider
-from laktory.models.providers.awsprovider import AWSProvider
-from laktory.models.providers.azureprovider import AzureProvider
-from laktory.models.providers.azurepulumiprovider import AzurePulumiProvider
-from laktory.models.providers.databricksprovider import DatabricksProvider
-from laktory.models.sql.catalog import Catalog
-from laktory.models.sql.schema import Schema
-from laktory.models.sql.table import Table
-from laktory.models.sql.volume import Volume
+from laktory.models.pipeline import Pipeline
+from laktory.models.resources.baseresource import ResourceOptions
+from laktory.models.resources.databricks.catalog import Catalog
+from laktory.models.resources.databricks.cluster import Cluster
+from laktory.models.resources.databricks.dbfsfile import DbfsFile
+from laktory.models.resources.databricks.directory import Directory
+from laktory.models.resources.databricks.dltpipeline import DLTPipeline
+from laktory.models.resources.databricks.externallocation import ExternalLocation
+from laktory.models.resources.databricks.group import Group
+from laktory.models.resources.databricks.job import Job
+from laktory.models.resources.databricks.metastore import Metastore
+from laktory.models.resources.databricks.metastoredataaccess import MetastoreDataAccess
+from laktory.models.resources.databricks.notebook import Notebook
+from laktory.models.resources.databricks.schema import Schema
+from laktory.models.resources.databricks.secret import Secret
+from laktory.models.resources.databricks.secretscope import SecretScope
+from laktory.models.resources.databricks.serviceprincipal import ServicePrincipal
+from laktory.models.resources.databricks.sqlquery import SqlQuery
+from laktory.models.resources.databricks.table import Table
+from laktory.models.resources.databricks.user import User
+from laktory.models.resources.databricks.volume import Volume
+from laktory.models.resources.databricks.warehouse import Warehouse
+from laktory.models.resources.databricks.workspacefile import WorkspaceFile
+from laktory.models.resources.providers.awsprovider import AWSProvider
+from laktory.models.resources.providers.azureprovider import AzureProvider
+from laktory.models.resources.providers.azurepulumiprovider import AzurePulumiProvider
+from laktory.models.resources.providers.baseprovider import BaseProvider
+from laktory.models.resources.providers.databricksprovider import DatabricksProvider
 
 logger = get_logger(__name__)
 
 DIRPATH = "./"
 
 
 class Terraform(BaseModel):
@@ -62,80 +64,83 @@
 
 class StackResources(BaseModel):
     """
     Resources definition for a given stack or stack environment.
 
     Attributes
     ----------
-    dbfsfiles:
-        DbfsFiles
-    catalogs:
-        Catalogs
-    clusters:
-        Clusters
-    directories:
-        Directories
-    externallocations:
-        External Locations
-    groups:
-        Groups
-    jobs:
-        Jobs
-    metastores:
-        Metastores
-    notebooks:
-        Notebooks
-    pipelines:
-        Pipelines
-    schemas:
-        Schemas
-    secretscopes:
-        SecretScopes
-    serviceprincipals:
-        ServicePrincipals
-    sqlqueries:
-        SQLQueries
-    tables:
-        Tables
+    databricks_dbfsfiles:
+        Databricks DbfsFiles
+    databricks_catalogs:
+        Databricks Catalogs
+    databricks_clusters:
+        Databricks Clusters
+    databricks_directories:
+        Databricks Directories
+    databricks_externallocations:
+        Databricks External Locations
+    databricks_groups:
+        Databricks Groups
+    databricks_jobs:
+        Databricks Jobs
+    databricks_metastores:
+        Databricks Metastores
+    databricks_notebooks:
+        Databricks Notebooks
+    databricks_dltpipelines:
+        Databricks DLT Pipelines
+    databricks_schemas:
+        Databricks Schemas
+    databricks_secretscopes:
+        Databricks SecretScopes
+    databricks_serviceprincipals:
+        Databricks ServicePrincipals
+    databricks_sqlqueries:
+        Databricks SQLQueries
+    databricks_tables:
+        Databricks Tables
     providers:
         Providers
-    users:
-        Users
-    volumes:
-        Volumes
-    warehouses:
-        Warehouses
-    workspacefiles:
-        WorkspacFiles
+    databricks_users:
+        Databricks Users
+    databricks_volumes:
+        Databricks Volumes
+    databricks_warehouses:
+        Databricks Warehouses
+    databricks_workspacefiles:
+        Databricks WorkspacFiles
+    pipelines:
+        Laktory Pipelines
     """
 
-    dbfsfiles: dict[str, DbfsFile] = {}
-    catalogs: dict[str, Catalog] = {}
-    clusters: dict[str, Cluster] = {}
-    directories: dict[str, Directory] = {}
-    externallocations: dict[str, ExternalLocation] = {}
-    groups: dict[str, Group] = {}
-    jobs: dict[str, Job] = {}
-    metastoredataaccesses: dict[str, MetastoreDataAccess] = {}
-    metastores: dict[str, Metastore] = {}
-    notebooks: dict[str, Notebook] = {}
+    databricks_dbfsfiles: dict[str, DbfsFile] = {}
+    databricks_catalogs: dict[str, Catalog] = {}
+    databricks_clusters: dict[str, Cluster] = {}
+    databricks_directories: dict[str, Directory] = {}
+    databricks_externallocations: dict[str, ExternalLocation] = {}
+    databricks_groups: dict[str, Group] = {}
+    databricks_jobs: dict[str, Job] = {}
+    databricks_metastoredataaccesses: dict[str, MetastoreDataAccess] = {}
+    databricks_metastores: dict[str, Metastore] = {}
+    databricks_notebooks: dict[str, Notebook] = {}
+    databricks_dltpipelines: dict[str, DLTPipeline] = {}
+    databricks_schemas: dict[str, Schema] = {}
+    databricks_secrets: dict[str, Secret] = {}
+    databricks_secretscopes: dict[str, SecretScope] = {}
+    databricks_serviceprincipals: dict[str, ServicePrincipal] = {}
+    databricks_sqlqueries: dict[str, SqlQuery] = {}
+    databricks_tables: dict[str, Table] = {}
+    databricks_users: dict[str, User] = {}
+    databricks_volumes: dict[str, Volume] = {}
+    databricks_warehouses: dict[str, Warehouse] = {}
+    databricks_workspacefiles: dict[str, WorkspaceFile] = {}
     pipelines: dict[str, Pipeline] = {}
-    schemas: dict[str, Schema] = {}
-    secrets: dict[str, Secret] = {}
-    secretscopes: dict[str, SecretScope] = {}
-    serviceprincipals: dict[str, ServicePrincipal] = {}
-    sqlqueries: dict[str, SqlQuery] = {}
-    tables: dict[str, Table] = {}
     providers: dict[
         str, Union[AWSProvider, AzureProvider, AzurePulumiProvider, DatabricksProvider]
     ] = {}
-    users: dict[str, User] = {}
-    volumes: dict[str, Volume] = {}
-    warehouses: dict[str, Warehouse] = {}
-    workspacefiles: dict[str, WorkspaceFile] = {}
 
     @model_validator(mode="after")
     def update_resource_names(self) -> Any:
         for k, r in self._get_all().items():
             if r.resource_name_ and k != r.resource_name_:
                 raise ValueError(
                     f"Provided resource name {r.resource_name_} does not match provided key {k}"
@@ -257,24 +262,24 @@
         pulumi={
             "config": {
                 "databricks:host": "${vars.DATABRICKS_HOST}",
                 "databricks:token": "${vars.DATABRICKS_TOKEN}",
             },
         },
         resources={
-            "pipelines": {
+            "databricks_dltpipelines": {
                 "pl-stock-prices": {
                     "name": "pl-stock-prices",
                     "development": "${vars.is_dev}",
                     "libraries": [
                         {"notebook": {"path": "/pipelines/dlt_brz_template.py"}},
                     ],
                 }
             },
-            "jobs": {
+            "databricks_jobs": {
                 "job-stock-prices": {
                     "name": "job-stock-prices",
                     "clusters": [
                         {
                             "name": "main",
                             "spark_version": "14.0.x-scala2.12",
                             "node_type_id": "Standard_DS3_v2",
@@ -288,15 +293,15 @@
                                 "notebook_path": "/.laktory/jobs/ingest_stock_prices.py",
                             },
                         },
                         {
                             "task_key": "pipeline",
                             "depends_ons": [{"task_key": "ingest"}],
                             "pipeline_task": {
-                                "pipeline_id": "${resources.pl-stock-prices.id}",
+                                "pipeline_id": "${resources.dlt-pl-stock-prices.id}",
                             },
                         },
                     ],
                 }
             },
         },
         variables={
@@ -314,29 +319,30 @@
                 }
             },
         },
     )
 
     print(stack)
     '''
-    variables={'org': 'okube'} backend='pulumi' description=None environments={'dev': EnvironmentSettings(variables={'is_dev': True}, resources=None), 'prod': EnvironmentSettings(variables={'is_dev': False}, resources=None)} name='workspace' organization=None pulumi=Pulumi(variables={}, config={'databricks:host': '${vars.DATABRICKS_HOST}', 'databricks:token': '${vars.DATABRICKS_TOKEN}'}, outputs={}) resources=StackResources(variables={}, dbfsfiles={}, catalogs={}, clusters={}, directories={}, externallocations={}, groups={}, jobs={'job-stock-prices': Job(resource_name_='job-stock-prices', options=ResourceOptions(variables={}, depends_on=[], provider=None, aliases=None, delete_before_replace=True, ignore_changes=None, import_=None, parent=None, replace_on_changes=None), variables={}, access_controls=[], clusters=[JobCluster(resource_name_=None, options=ResourceOptions(variables={}, depends_on=[], provider=None, aliases=None, delete_before_replace=True, ignore_changes=None, import_=None, parent=None, replace_on_changes=None), variables={}, access_controls=None, apply_policy_default_values=None, autoscale=None, autotermination_minutes=None, cluster_id=None, custom_tags=None, data_security_mode='USER_ISOLATION', driver_instance_pool_id=None, driver_node_type_id=None, enable_elastic_disk=None, enable_local_disk_encryption=None, idempotency_token=None, init_scripts=[], instance_pool_id=None, is_pinned=None, libraries=None, name='main', node_type_id='Standard_DS3_v2', num_workers=None, policy_id=None, runtime_engine=None, single_user_name=None, spark_conf={}, spark_env_vars={}, spark_version='14.0.x-scala2.12', ssh_public_keys=[])], continuous=None, control_run_state=None, email_notifications=None, format=None, health=None, max_concurrent_runs=None, max_retries=None, min_retry_interval_millis=None, name='job-stock-prices', notification_settings=None, parameters=[], retry_on_timeout=None, run_as=None, schedule=None, tags={}, tasks=[JobTask(variables={}, condition_task=None, depends_ons=None, description=None, email_notifications=None, existing_cluster_id=None, health=None, job_cluster_key='main', libraries=None, max_retries=None, min_retry_interval_millis=None, notebook_task=JobTaskNotebookTask(variables={}, notebook_path='/.laktory/jobs/ingest_stock_prices.py', base_parameters=None, source=None), notification_settings=None, pipeline_task=None, retry_on_timeout=None, run_if=None, run_job_task=None, sql_task=None, task_key='ingest', timeout_seconds=None), JobTask(variables={}, condition_task=None, depends_ons=[JobTaskDependsOn(variables={}, task_key='ingest', outcome=None)], description=None, email_notifications=None, existing_cluster_id=None, health=None, job_cluster_key=None, libraries=None, max_retries=None, min_retry_interval_millis=None, notebook_task=None, notification_settings=None, pipeline_task=JobTaskPipelineTask(variables={}, pipeline_id='${resources.pl-stock-prices.id}', full_refresh=None), retry_on_timeout=None, run_if=None, run_job_task=None, sql_task=None, task_key='pipeline', timeout_seconds=None)], timeout_seconds=None, trigger=None, webhook_notifications=None)}, metastoredataaccesses={}, metastores={}, notebooks={}, pipelines={'pl-stock-prices': Pipeline(resource_name_='pl-stock-prices', options=ResourceOptions(variables={}, depends_on=[], provider=None, aliases=None, delete_before_replace=True, ignore_changes=None, import_=None, parent=None, replace_on_changes=None), variables={}, access_controls=[], allow_duplicate_names=None, catalog=None, channel='PREVIEW', clusters=[], configuration={}, continuous=None, development='${vars.is_dev}', edition=None, libraries=[PipelineLibrary(variables={}, file=None, notebook=PipelineLibraryNotebook(variables={}, path='/pipelines/dlt_brz_template.py'))], name='pl-stock-prices', notifications=[], photon=None, serverless=None, storage=None, tables=[], target=None, udfs=[])}, schemas={}, secrets={}, secretscopes={}, serviceprincipals={}, sqlqueries={}, tables={}, providers={}, users={}, volumes={}, warehouses={}, workspacefiles={}) terraform=Terraform(variables={}, backend=None)
+    variables={'org': 'okube'} backend='pulumi' description=None environments={'dev': EnvironmentSettings(variables={'is_dev': True}, resources=None), 'prod': EnvironmentSettings(variables={'is_dev': False}, resources=None)} name='workspace' organization=None pulumi=Pulumi(variables={}, config={'databricks:host': '${vars.DATABRICKS_HOST}', 'databricks:token': '${vars.DATABRICKS_TOKEN}'}, outputs={}) resources=StackResources(variables={}, databricks_dbfsfiles={}, databricks_catalogs={}, databricks_clusters={}, databricks_directories={}, databricks_externallocations={}, databricks_groups={}, databricks_jobs={'job-stock-prices': Job(resource_name_='job-stock-prices', options=ResourceOptions(variables={}, depends_on=[], provider=None, aliases=None, delete_before_replace=True, ignore_changes=None, import_=None, parent=None, replace_on_changes=None), variables={}, access_controls=[], clusters=[JobCluster(resource_name_=None, options=ResourceOptions(variables={}, depends_on=[], provider=None, aliases=None, delete_before_replace=True, ignore_changes=None, import_=None, parent=None, replace_on_changes=None), variables={}, access_controls=None, apply_policy_default_values=None, autoscale=None, autotermination_minutes=None, cluster_id=None, custom_tags=None, data_security_mode='USER_ISOLATION', driver_instance_pool_id=None, driver_node_type_id=None, enable_elastic_disk=None, enable_local_disk_encryption=None, idempotency_token=None, init_scripts=[], instance_pool_id=None, is_pinned=None, libraries=None, name='main', node_type_id='Standard_DS3_v2', num_workers=None, policy_id=None, runtime_engine=None, single_user_name=None, spark_conf={}, spark_env_vars={}, spark_version='14.0.x-scala2.12', ssh_public_keys=[])], continuous=None, control_run_state=None, email_notifications=None, format=None, health=None, max_concurrent_runs=None, max_retries=None, min_retry_interval_millis=None, name='job-stock-prices', notification_settings=None, parameters=[], retry_on_timeout=None, run_as=None, schedule=None, tags={}, tasks=[JobTask(variables={}, condition_task=None, depends_ons=None, description=None, email_notifications=None, existing_cluster_id=None, health=None, job_cluster_key='main', libraries=None, max_retries=None, min_retry_interval_millis=None, notebook_task=JobTaskNotebookTask(variables={}, notebook_path='/.laktory/jobs/ingest_stock_prices.py', base_parameters=None, source=None), notification_settings=None, pipeline_task=None, retry_on_timeout=None, run_if=None, run_job_task=None, sql_task=None, task_key='ingest', timeout_seconds=None), JobTask(variables={}, condition_task=None, depends_ons=[JobTaskDependsOn(variables={}, task_key='ingest', outcome=None)], description=None, email_notifications=None, existing_cluster_id=None, health=None, job_cluster_key=None, libraries=None, max_retries=None, min_retry_interval_millis=None, notebook_task=None, notification_settings=None, pipeline_task=JobTaskPipelineTask(variables={}, pipeline_id='${resources.dlt-pl-stock-prices.id}', full_refresh=None), retry_on_timeout=None, run_if=None, run_job_task=None, sql_task=None, task_key='pipeline', timeout_seconds=None)], timeout_seconds=None, trigger=None, webhook_notifications=None)}, databricks_metastoredataaccesses={}, databricks_metastores={}, databricks_notebooks={}, databricks_dltpipelines={'pl-stock-prices': DLTPipeline(resource_name_='pl-stock-prices', options=ResourceOptions(variables={}, depends_on=[], provider=None, aliases=None, delete_before_replace=True, ignore_changes=None, import_=None, parent=None, replace_on_changes=None), variables={}, access_controls=[], allow_duplicate_names=None, catalog=None, channel='PREVIEW', clusters=[], configuration={}, continuous=None, development='${vars.is_dev}', edition=None, libraries=[PipelineLibrary(variables={}, file=None, notebook=PipelineLibraryNotebook(variables={}, path='/pipelines/dlt_brz_template.py'))], name='pl-stock-prices', notifications=[], photon=None, serverless=None, storage=None, target=None)}, databricks_schemas={}, databricks_secrets={}, databricks_secretscopes={}, databricks_serviceprincipals={}, databricks_sqlqueries={}, databricks_tables={}, databricks_users={}, databricks_volumes={}, databricks_warehouses={}, databricks_workspacefiles={}, pipelines={}, providers={}) terraform=Terraform(variables={}, backend=None)
     '''
     ```
 
     """
 
     backend: Literal["pulumi", "terraform"] = None
     description: str = None
     environments: dict[str, EnvironmentSettings] = {}
     name: str
     organization: Union[str, None] = None
     pulumi: Pulumi = Pulumi()
     resources: Union[StackResources, None] = StackResources()
     terraform: Terraform = Terraform()
     variables: dict[str, Any] = {}
+    _envs: dict[str, EnvironmentStack] = None
 
     # ----------------------------------------------------------------------- #
     # Properties                                                              #
     # ----------------------------------------------------------------------- #
 
     @property
     def envs(self) -> dict[str, EnvironmentStack]:
@@ -346,35 +352,77 @@
         overwrites.
 
         Returns
         -------
         :
             Environment definitions.
         """
-        ENV_FIELDS = ["pulumi", "resources", "terraform", "variables"]
 
-        d = self.model_dump(exclude_none=True)
-        _envs = d.pop("environments")
+        if self._envs is None:
 
-        # Restore fields excluded from dump
-        for rtype in d.get("resources", {}):
-            for k, r in d["resources"][rtype].items():
-                r["options"] = getattr(self.resources, rtype)[k].options.model_dump(
-                    exclude_none=True
-                )
+            ENV_FIELDS = ["pulumi", "resources", "terraform", "variables"]
 
-        envs = {}
-        for env_name, env in self.environments.items():
-            for k in ENV_FIELDS:
-                if k in d:
-                    d[k] = merge_dicts(d[k], _envs[env_name].get(k, {}))
+            # Because options is an excluded field for all resources and
+            # sub-resources, we need to manually dump it and add it to
+            # the base dump
+            def dump_with_options(obj: Any) -> Any:
+
+                # Check data type, call recursively if not a BaseModel
+                if isinstance(obj, list):
+                    return [dump_with_options(v) for v in obj]
+                elif isinstance(obj, dict):
+                    return {k: dump_with_options(v) for k, v in obj.items()}
+                elif not isinstance(obj, BaseModel):
+                    return obj
+
+                # Get model dump
+                model = obj
+                data = model.model_dump(exclude_none=True)
+
+                # Loop through all model fields
+                for field_name, field in model.model_fields.items():
+
+                    # Explicitly dump options if found in the model
+                    if field_name == "options" and field.annotation == ResourceOptions:
+                        data["options"] = model.options.model_dump(exclude_none=True)
+
+                    if field_name == "resource_name_" and model.resource_name_:
+                        data["resource_name_"] = model.resource_name_
+
+                    # Parse list
+                    if isinstance(data.get(field_name, None), list):
+                        data[field_name] = [
+                            dump_with_options(v) for v in getattr(model, field_name)
+                        ]
+
+                    # Parse dict (might result from a dict or a BaseModel)
+                    elif isinstance(data.get(field_name, None), dict):
+                        a = getattr(model, field_name)
+
+                        if isinstance(a, dict):
+                            for k in a.keys():
+                                data[field_name][k] = dump_with_options(a[k])
+                        else:
+                            data[field_name] = dump_with_options(a)
+
+                return data
+
+            d = dump_with_options(self)
+            _envs = d.pop("environments")
+
+            envs = {}
+            for env_name, env in self.environments.items():
+                for k in ENV_FIELDS:
+                    if k in d:
+                        d[k] = merge_dicts(d[k], _envs[env_name].get(k, {}))
+                envs[env_name] = EnvironmentStack(**d)
 
-            envs[env_name] = EnvironmentStack(**d)
+            self._envs = envs
 
-        return envs
+        return self._envs
 
     # ----------------------------------------------------------------------- #
     # Pulumi Methods                                                          #
     # ----------------------------------------------------------------------- #
 
     def to_pulumi(self, env: Union[str, None] = None):
         """
```

### Comparing `laktory-0.2.1/laktory/models/stacks/terraformstack.py` & `laktory-0.3.0/laktory/models/stacks/terraformstack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/resources/data/stock_prices.json` & `laktory-0.3.0/laktory/resources/data/stock_prices.json`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/resources/notebooks/dlt_brz_template.py` & `laktory-0.3.0/laktory/resources/notebooks/dlt_laktory_pl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,93 @@
 # MAGIC %pip install laktory
 
 # COMMAND ----------
+import importlib
+import sys
+import os
 import pyspark.sql.functions as F
 
 from laktory import dlt
-from laktory import read_metadata
+from laktory import models
 from laktory import get_logger
+from laktory import settings
 
 dlt.spark = spark
 logger = get_logger(__name__)
 
-
 # Read pipeline definition
 pl_name = spark.conf.get("pipeline_name", "pl-stock-prices")
-pl = read_metadata(pipeline=pl_name)
+filepath = f"/Workspace{settings.workspace_laktory_root}pipelines/{pl_name}.json"
+with open(filepath, "r") as fp:
+    pl = models.Pipeline.model_validate_json(fp.read())
+
 
+# Import User Defined Functions
+sys.path.append(f"/Workspace{settings.workspace_laktory_root}pipelines/")
+udfs = []
+for udf in pl.udfs:
+    if udf.module_path:
+        sys.path.append(os.path.abspath(udf.module_path))
+    module = importlib.import_module(udf.module_name)
+    udfs += [getattr(module, udf.function_name)]
 
 # --------------------------------------------------------------------------- #
-# Non-CDC Tables                                                              #
+# Tables and Views Definition                                                 #
 # --------------------------------------------------------------------------- #
 
 
-def define_table(table):
+def define_table(node):
     @dlt.table_or_view(
-        name=table.name,
-        comment=table.comment,
-        as_view=table.builder.as_dlt_view,
+        name=node.name,
+        comment=node.description,
+        as_view=node.sink is None,
     )
-    @dlt.expect_all(table.warning_expectations)
-    @dlt.expect_all_or_drop(table.drop_expectations)
-    @dlt.expect_all_or_fail(table.fail_expectations)
+    @dlt.expect_all(node.warning_expectations)
+    @dlt.expect_all_or_drop(node.drop_expectations)
+    @dlt.expect_all_or_fail(node.fail_expectations)
     def get_df():
-        logger.info(f"Building {table.name} table")
+        logger.info(f"Building {node.name} node")
 
-        # Read Source
-        df = table.builder.read_source(spark)
+        # Execute node
+        df = node.execute(spark=spark, udfs=udfs)
         df.printSchema()
 
-        # Process
-        df = table.builder.process(df, udfs=None, spark=spark)
-
         # Return
         return df
 
     return get_df
 
 
 # --------------------------------------------------------------------------- #
 # CDC tables                                                                  #
 # --------------------------------------------------------------------------- #
 
 
-def define_cdc_table(table):
+def define_cdc_table(node):
     dlt.create_streaming_table(
-        name=table.name,
-        comment=table.comment,
+        name=node.name,
+        comment=node.comment,
     )
 
-    df = dlt.apply_changes(**table.builder.apply_changes_kwargs)
+    df = dlt.apply_changes(**node.apply_changes_kwargs)
 
     return df
 
 
 # --------------------------------------------------------------------------- #
 # Execution                                                                   #
 # --------------------------------------------------------------------------- #
 
-# Build tables
-for table in pl.tables:
-    if table.builder.template == "BRONZE":
-        if table.is_from_cdc:
-            df = define_cdc_table(table)
-            display(df)
-
-        else:
-            wrapper = define_table(table)
-            df = dlt.get_df(wrapper)
-            display(df)
+# Build nodes
+for node in pl.nodes:
+
+    if node.dlt_template != "DEFAULT":
+        continue
+
+    if node.is_from_cdc:
+        df = define_cdc_table(node)
+        display(df)
+
+    else:
+        wrapper = define_table(node)
+        df = dlt.get_df(wrapper)
+        display(df)
```

### Comparing `laktory-0.2.1/laktory/spark/dataframe/__init__.py` & `laktory-0.3.0/laktory/spark/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/dataframe/groupby_and_agg.py` & `laktory-0.3.0/laktory/spark/dataframe/groupby_and_agg.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/dataframe/has_column.py` & `laktory-0.3.0/laktory/spark/dataframe/has_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/dataframe/schema_flat.py` & `laktory-0.3.0/laktory/spark/dataframe/schema_flat.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/dataframe/show_string.py` & `laktory-0.3.0/laktory/spark/dataframe/show_string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/dataframe/smart_join.py` & `laktory-0.3.0/laktory/spark/dataframe/smart_join.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/dataframe/watermark.py` & `laktory-0.3.0/laktory/spark/dataframe/watermark.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/dataframe/window_filter.py` & `laktory-0.3.0/laktory/spark/dataframe/window_filter.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/functions/_common.py` & `laktory-0.3.0/laktory/spark/functions/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/functions/logical.py` & `laktory-0.3.0/laktory/spark/functions/logical.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/functions/math.py` & `laktory-0.3.0/laktory/spark/functions/math.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/functions/string.py` & `laktory-0.3.0/laktory/spark/functions/string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/spark/functions/units.py` & `laktory-0.3.0/laktory/spark/functions/units.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory/version.py` & `laktory-0.3.0/laktory/version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/laktory.egg-info/PKG-INFO` & `laktory-0.3.0/laktory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.2.1
+Version: 0.3.0
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: databricks-sdk
 Requires-Dist: inflect
+Requires-Dist: networkx
 Requires-Dist: planck
 Requires-Dist: prompt_toolkit
 Requires-Dist: pulumi
 Requires-Dist: pulumi_databricks>=1.36
 Requires-Dist: pulumi_random
 Requires-Dist: pyyaml
 Requires-Dist: pydantic>=2
@@ -33,18 +34,21 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flit; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-video; extra == "dev"
+Requires-Dist: plotly; extra == "dev"
 Provides-Extra: spark
 Requires-Dist: pandas; extra == "spark"
 Requires-Dist: pyarrow; extra == "spark"
 Requires-Dist: pyspark; extra == "spark"
+Provides-Extra: polars
+Requires-Dist: polars; extra == "polars"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-examples; extra == "test"
 Requires-Dist: yfinance; extra == "test"
 Provides-Extra: azure
 Requires-Dist: azure-identity; extra == "azure"
```

### Comparing `laktory-0.2.1/laktory.egg-info/SOURCES.txt` & `laktory-0.3.0/laktory.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -31,59 +31,64 @@
 docs/api/dlt/get_df.md
 docs/api/dlt/is_debug.md
 docs/api/dlt/is_mocked.md
 docs/api/dlt/read.md
 docs/api/dlt/read_stream.md
 docs/api/models/basemodel.md
 docs/api/models/dataevent.md
-docs/api/models/dataeventheader.md
 docs/api/models/dataproducer.md
-docs/api/models/databricks/accesscontrol.md
-docs/api/models/databricks/cluster.md
-docs/api/models/databricks/directory.md
-docs/api/models/databricks/externallocation.md
-docs/api/models/databricks/grants.md
-docs/api/models/databricks/group.md
-docs/api/models/databricks/job.md
-docs/api/models/databricks/metastore.md
-docs/api/models/databricks/metastoreassignment.md
-docs/api/models/databricks/metastoredataaccess.md
-docs/api/models/databricks/mwspermissionassignment.md
-docs/api/models/databricks/notebook.md
-docs/api/models/databricks/pipeline.md
-docs/api/models/databricks/secret.md
-docs/api/models/databricks/secretacl.md
-docs/api/models/databricks/secretscope.md
-docs/api/models/databricks/serviceprincipal.md
-docs/api/models/databricks/serviceprincipalrole.md
-docs/api/models/databricks/sqlquery.md
-docs/api/models/databricks/user.md
-docs/api/models/databricks/userrole.md
-docs/api/models/databricks/warehouse.md
-docs/api/models/databricks/workspacefile.md
+docs/api/models/pipeline.md
+docs/api/models/pipelinenode.md
+docs/api/models/pipelinenodeexpectation.md
+docs/api/models/datasinks/basedatasink.md
+docs/api/models/datasinks/filedatasink.md
+docs/api/models/datasinks/tabledatasink.md
 docs/api/models/datasources/basedatasource.md
-docs/api/models/datasources/eventdatasource.md
+docs/api/models/datasources/filedatasource.md
+docs/api/models/datasources/memorydatasource.md
+docs/api/models/datasources/pipelinenodedatasource.md
 docs/api/models/datasources/tabledatasource.md
-docs/api/models/providers/aws.md
-docs/api/models/providers/azure.md
-docs/api/models/providers/azurepulumi.md
-docs/api/models/providers/databricks.md
 docs/api/models/resources/baseresource.md
 docs/api/models/resources/pulumiresource.md
 docs/api/models/resources/terraformresource.md
+docs/api/models/resources/databricks/accesscontrol.md
+docs/api/models/resources/databricks/catalog.md
+docs/api/models/resources/databricks/cluster.md
+docs/api/models/resources/databricks/column.md
+docs/api/models/resources/databricks/directory.md
+docs/api/models/resources/databricks/dltpipeline.md
+docs/api/models/resources/databricks/externallocation.md
+docs/api/models/resources/databricks/grants.md
+docs/api/models/resources/databricks/group.md
+docs/api/models/resources/databricks/job.md
+docs/api/models/resources/databricks/metastore.md
+docs/api/models/resources/databricks/metastoreassignment.md
+docs/api/models/resources/databricks/metastoredataaccess.md
+docs/api/models/resources/databricks/mwspermissionassignment.md
+docs/api/models/resources/databricks/notebook.md
+docs/api/models/resources/databricks/schema.md
+docs/api/models/resources/databricks/secret.md
+docs/api/models/resources/databricks/secretacl.md
+docs/api/models/resources/databricks/secretscope.md
+docs/api/models/resources/databricks/serviceprincipal.md
+docs/api/models/resources/databricks/serviceprincipalrole.md
+docs/api/models/resources/databricks/sqlquery.md
+docs/api/models/resources/databricks/table.md
+docs/api/models/resources/databricks/user.md
+docs/api/models/resources/databricks/userrole.md
+docs/api/models/resources/databricks/volume.md
+docs/api/models/resources/databricks/warehouse.md
+docs/api/models/resources/databricks/workspacefile.md
+docs/api/models/resources/providers/aws.md
+docs/api/models/resources/providers/azure.md
+docs/api/models/resources/providers/azurepulumi.md
+docs/api/models/resources/providers/databricks.md
 docs/api/models/spark/sparkchain.md
 docs/api/models/spark/sparkchainnode.md
 docs/api/models/spark/sparkfuncarg.md
-docs/api/models/sql/catalog.md
-docs/api/models/sql/column.md
-docs/api/models/sql/schema.md
-docs/api/models/sql/table.md
-docs/api/models/sql/tablebuilder.md
-docs/api/models/sql/tableexpectation.md
-docs/api/models/sql/volume.md
 docs/api/models/stacks/pulumistack.md
 docs/api/models/stacks/stack.md
 docs/api/models/stacks/terraformstack.md
 docs/api/spark/dataframe/groupby_and_agg.md
 docs/api/spark/dataframe/has_column.md
 docs/api/spark/dataframe/schema_flat.md
 docs/api/spark/dataframe/show_string.md
@@ -98,25 +103,25 @@
 docs/api/spark/functions/poly2.md
 docs/api/spark/functions/roundp.md
 docs/api/spark/functions/scaled_power.md
 docs/api/spark/functions/string_split.md
 docs/api/spark/functions/sub.md
 docs/api/spark/functions/uuid.md
 docs/concepts/cli.md
-docs/concepts/dataevent.md
 docs/concepts/deployment.md
 docs/concepts/design.md
 docs/concepts/governance.md
-docs/concepts/models.md
-docs/concepts/pipeline.md
 docs/concepts/spark.md
 docs/concepts/stack.md
-docs/concepts/table.md
-docs/concepts/tablebuilder.md
 docs/concepts/variables.md
+docs/concepts/models/dataevent.md
+docs/concepts/models/models.md
+docs/concepts/models/pipeline.md
+docs/concepts/models/sourcessinks.md
+docs/concepts/models/sparkchain.md
 docs/guides/catalog.md
 docs/guides/compute.md
 docs/guides/job.md
 docs/guides/pipeline.md
 docs/guides/secrets.md
 docs/guides/table.md
 docs/guides/users.md
@@ -146,15 +151,15 @@
 laktory/_parsers.py
 laktory/_settings.py
 laktory/_useragent.py
 laktory/_version.py
 laktory/constants.py
 laktory/datetime.py
 laktory/exceptions.py
-laktory/metadata.py
+laktory/types.py
 laktory/version.py
 laktory.egg-info/PKG-INFO
 laktory.egg-info/SOURCES.txt
 laktory.egg-info/dependency_links.txt
 laktory.egg-info/entry_points.txt
 laktory.egg-info/requires.txt
 laktory.egg-info/top_level.txt
@@ -170,99 +175,103 @@
 laktory/cli/_run.py
 laktory/cli/_write.py
 laktory/cli/app.py
 laktory/cli/quickstart_stack.yaml
 laktory/dispatcher/__init__.py
 laktory/dispatcher/dispatcher.py
 laktory/dispatcher/dispatcherrunner.py
+laktory/dispatcher/dltpipelinerunner.py
 laktory/dispatcher/jobrunner.py
-laktory/dispatcher/pipelinerunner.py
 laktory/dlt/__init__.py
 laktory/models/__init__.py
 laktory/models/basemodel.py
 laktory/models/dataevent.py
-laktory/models/dataeventheader.py
 laktory/models/dataproducer.py
+laktory/models/pipeline.py
+laktory/models/pipelinenode.py
+laktory/models/pipelinenodeexpectation.py
 laktory/models/azurenative/storageblob.py
-laktory/models/databricks/__init__.py
-laktory/models/databricks/accesscontrol.py
-laktory/models/databricks/cluster.py
-laktory/models/databricks/dbfsfile.py
-laktory/models/databricks/directory.py
-laktory/models/databricks/externallocation.py
-laktory/models/databricks/grants.py
-laktory/models/databricks/group.py
-laktory/models/databricks/groupmember.py
-laktory/models/databricks/job.py
-laktory/models/databricks/metastore.py
-laktory/models/databricks/metastoreassignment.py
-laktory/models/databricks/metastoredataaccess.py
-laktory/models/databricks/mwspermissionassignment.py
-laktory/models/databricks/notebook.py
-laktory/models/databricks/permissions.py
-laktory/models/databricks/pipeline.py
-laktory/models/databricks/secret.py
-laktory/models/databricks/secretacl.py
-laktory/models/databricks/secretscope.py
-laktory/models/databricks/serviceprincipal.py
-laktory/models/databricks/serviceprincipalrole.py
-laktory/models/databricks/sqlquery.py
-laktory/models/databricks/user.py
-laktory/models/databricks/userrole.py
-laktory/models/databricks/warehouse.py
-laktory/models/databricks/workspacefile.py
+laktory/models/datasinks/__init__.py
+laktory/models/datasinks/basedatasink.py
+laktory/models/datasinks/filedatasink.py
+laktory/models/datasinks/tabledatasink.py
 laktory/models/datasources/__init__.py
 laktory/models/datasources/basedatasource.py
-laktory/models/datasources/eventdatasource.py
+laktory/models/datasources/filedatasource.py
+laktory/models/datasources/memorydatasource.py
+laktory/models/datasources/pipelinenodedatasource.py
 laktory/models/datasources/tabledatasource.py
 laktory/models/grants/__init__.py
 laktory/models/grants/cataloggrant.py
 laktory/models/grants/connectiongrant.py
 laktory/models/grants/externallocationgrant.py
 laktory/models/grants/functiongrant.py
 laktory/models/grants/metastoregrant.py
 laktory/models/grants/registeredmodelgrant.py
 laktory/models/grants/schemagrant.py
 laktory/models/grants/sharegrant.py
 laktory/models/grants/storagecredentialgrant.py
 laktory/models/grants/tablegrant.py
 laktory/models/grants/viewgrant.py
 laktory/models/grants/volumegrant.py
-laktory/models/providers/__init__.py
-laktory/models/providers/awsprovider.py
-laktory/models/providers/azureprovider.py
-laktory/models/providers/azurepulumiprovider.py
-laktory/models/providers/baseprovider.py
-laktory/models/providers/databricksprovider.py
 laktory/models/resources/__init__.py
 laktory/models/resources/baseresource.py
 laktory/models/resources/pulumiresource.py
 laktory/models/resources/terraformresource.py
+laktory/models/resources/databricks/__init__.py
+laktory/models/resources/databricks/accesscontrol.py
+laktory/models/resources/databricks/catalog.py
+laktory/models/resources/databricks/cluster.py
+laktory/models/resources/databricks/column.py
+laktory/models/resources/databricks/dbfsfile.py
+laktory/models/resources/databricks/directory.py
+laktory/models/resources/databricks/dltpipeline.py
+laktory/models/resources/databricks/externallocation.py
+laktory/models/resources/databricks/grants.py
+laktory/models/resources/databricks/group.py
+laktory/models/resources/databricks/groupmember.py
+laktory/models/resources/databricks/job.py
+laktory/models/resources/databricks/metastore.py
+laktory/models/resources/databricks/metastoreassignment.py
+laktory/models/resources/databricks/metastoredataaccess.py
+laktory/models/resources/databricks/mwspermissionassignment.py
+laktory/models/resources/databricks/notebook.py
+laktory/models/resources/databricks/permissions.py
+laktory/models/resources/databricks/schema.py
+laktory/models/resources/databricks/secret.py
+laktory/models/resources/databricks/secretacl.py
+laktory/models/resources/databricks/secretscope.py
+laktory/models/resources/databricks/serviceprincipal.py
+laktory/models/resources/databricks/serviceprincipalrole.py
+laktory/models/resources/databricks/sqlquery.py
+laktory/models/resources/databricks/table.py
+laktory/models/resources/databricks/user.py
+laktory/models/resources/databricks/userrole.py
+laktory/models/resources/databricks/volume.py
+laktory/models/resources/databricks/warehouse.py
+laktory/models/resources/databricks/workspacefile.py
+laktory/models/resources/providers/__init__.py
+laktory/models/resources/providers/awsprovider.py
+laktory/models/resources/providers/azureprovider.py
+laktory/models/resources/providers/azurepulumiprovider.py
+laktory/models/resources/providers/baseprovider.py
+laktory/models/resources/providers/databricksprovider.py
 laktory/models/spark/__init__.py
 laktory/models/spark/_common.py
 laktory/models/spark/sparkchain.py
 laktory/models/spark/sparkchainnode.py
 laktory/models/spark/sparkfuncarg.py
-laktory/models/sql/__init__.py
-laktory/models/sql/catalog.py
-laktory/models/sql/column.py
-laktory/models/sql/schema.py
-laktory/models/sql/table.py
-laktory/models/sql/tablebuilder.py
-laktory/models/sql/tableexpectation.py
-laktory/models/sql/volume.py
 laktory/models/stacks/__init__.py
 laktory/models/stacks/pulumistack.py
 laktory/models/stacks/stack.py
 laktory/models/stacks/terraformstack.py
+laktory/polars/__init__.py
 laktory/resources/data/stock_prices.json
-laktory/resources/notebooks/dlt_brz_template.py
-laktory/resources/notebooks/dlt_gld_template.py
-laktory/resources/notebooks/dlt_slv_star_template.py
-laktory/resources/notebooks/dlt_slv_template.py
+laktory/resources/notebooks/dlt_laktory_pl.py
+laktory/resources/notebooks/job_laktory_pl.py
 laktory/spark/__init__.py
 laktory/spark/dataframe/__init__.py
 laktory/spark/dataframe/groupby_and_agg.py
 laktory/spark/dataframe/has_column.py
 laktory/spark/dataframe/schema_flat.py
 laktory/spark/dataframe/show_string.py
 laktory/spark/dataframe/smart_join.py
@@ -271,62 +280,69 @@
 laktory/spark/functions/__init__.py
 laktory/spark/functions/_common.py
 laktory/spark/functions/logical.py
 laktory/spark/functions/math.py
 laktory/spark/functions/string.py
 laktory/spark/functions/units.py
 scripts/databricks_api_call.py
+scripts/polars_etl.py
 scripts/test_computed_filed.py
 scripts/test_db_connect.py
 settings/dev.env
 tests/__init__.py
 tests/build_test_data.py
 tests/test_basemodel.py
 tests/test_baseresource.py
 tests/test_catalog.py
 tests/test_cli.py
 tests/test_column.py
 tests/test_constants.py
 tests/test_dataevent.py
+tests/test_datasinks.py
 tests/test_datasources.py
 tests/test_datetime.py
 tests/test_dbfsfile.py
 tests/test_directory.py
 tests/test_dispatcher.py
 tests/test_dlt.py
+tests/test_dltpipeline.py
 tests/test_docstrings.py
 tests/test_job.py
 tests/test_logger.py
 tests/test_metastore.py
 tests/test_notebook.py
 tests/test_parsers.py
 tests/test_pipeline.py
+tests/test_pipeline_node.py
 tests/test_providers.py
 tests/test_schema.py
 tests/test_settings.py
 tests/test_spark_chain.py
 tests/test_spark_dataframe.py
 tests/test_spark_functions.py
 tests/test_sql_query.py
 tests/test_stack.py
 tests/test_table.py
-tests/test_table_builder.py
 tests/test_user.py
 tests/test_useragent.py
 tests/test_version_info.py
 tests/test_workspacefile.py
+tests/data/pl-spark-dlt.yaml
+tests/data/pl-spark-job.yaml
+tests/data/pl-spark-local.yaml
+tests/data/pl-spark-streaming.yaml
 tests/data/stack.yaml
 tests/data/stack_empty.yaml
 tests/data/stockprices0.yaml
 tests/data/stockprices1.yaml
 tests/data/stockprices2.yaml
 tests/data/brz_stock_prices/._SUCCESS.crc
-tests/data/brz_stock_prices/.part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet.crc
+tests/data/brz_stock_prices/.part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet.crc
 tests/data/brz_stock_prices/_SUCCESS
-tests/data/brz_stock_prices/part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet
+tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet
 tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
@@ -400,14 +416,14 @@
 tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
 tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
 tests/data/slv_stock_meta/._SUCCESS.crc
-tests/data/slv_stock_meta/.part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet.crc
+tests/data/slv_stock_meta/.part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet.crc
 tests/data/slv_stock_meta/_SUCCESS
-tests/data/slv_stock_meta/part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet
+tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet
 tests/data/slv_stock_prices/._SUCCESS.crc
-tests/data/slv_stock_prices/.part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet.crc
+tests/data/slv_stock_prices/.part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet.crc
 tests/data/slv_stock_prices/_SUCCESS
-tests/data/slv_stock_prices/part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet
+tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet
```

### Comparing `laktory-0.2.1/mkdocs.yml` & `laktory-0.3.0/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -119,19 +119,19 @@
     - Demos: demos.md
     - Installation: install.md
     - Quickstart: quickstart.md
 
   - Concepts:
     - Design Principles: concepts/design.md
     - Models:
-      - Intro: concepts/models.md
-      - Data Event: concepts/dataevent.md
-      - Table: concepts/table.md
-      - Table Builder: concepts/tablebuilder.md
-      - Pipeline: concepts/pipeline.md
+      - Intro: concepts/models/models.md
+      - Pipeline: concepts/models/pipeline.md
+      - Data Sources and Sinks: concepts/models/sourcessinks.md
+      - Spark Chain: concepts/models/sparkchain.md
+      - Data Event: conceptsmodels/dataevent.md
     - Stack: concepts/stack.md
     - Variables: concepts/variables.md
     - Deployment (IaC): concepts/deployment.md
     - CLI: concepts/cli.md
     - Spark Extension: concepts/spark.md
     - Data Governance: concepts/governance.md
 
@@ -144,66 +144,74 @@
     - Job: guides/job.md
     - Secrets: guides/secrets.md
 
   - Lakehouse As Code: lakehouseascode.md
   - API Reference:
     - Models:
       - BaseModel: api/models/basemodel.md
-      - DataEventHeader: api/models/dataeventheader.md
+#      - DataEventHeader: api/models/dataeventheader.md
       - DataEvent: api/models/dataevent.md
       - DataProducer: api/models/dataproducer.md
+      - DataSinks:
+        - BaseDataSink: api/models/datasinks/basedatasink.md
+        - FileDataSink: api/models/datasinks/filedatasink.md
+        - TableDataSink: api/models/datasinks/tabledatasink.md
       - DataSources:
         - BaseDataSource: api/models/datasources/basedatasource.md
-        - EventDataSource: api/models/datasources/eventdatasource.md
+        - FileDataSource: api/models/datasources/filedatasource.md
+        - MemoryDataSource: api/models/datasources/memorydatasource.md
+        - PipelineNodeDataSource: api/models/datasources/pipelinenodedatasource.md
         - TableDataSource: api/models/datasources/tabledatasource.md
-      - Databricks:
-        - AccessControl: api/models/databricks/accesscontrol.md
-        - api/models/databricks/cluster.md
-        - api/models/databricks/directory.md
-        - ExternalLocation: api/models/databricks/externallocation.md
-        - api/models/databricks/grants.md
-        - api/models/databricks/group.md
-        - api/models/databricks/job.md
-        - api/models/databricks/metastore.md
-        - MetastoreAssignment: api/models/databricks/metastoreassignment.md
-        - MetastoreDataAccess: api/models/databricks/metastoredataaccess.md
-        - MwsPermissionAssignment: api/models/databricks/mwspermissionassignment.md
-        - api/models/databricks/mws.md
-        - api/models/databricks/notebook.md
-        - Pipeline: api/models/databricks/pipeline.md
-        - api/models/databricks/secret.md
-        - SecretAcl: api/models/databricks/secretacl.md
-        - SecretScope: api/models/databricks/secretscope.md
-        - ServicePrincipal: api/models/databricks/serviceprincipal.md
-        - ServicePrincipalRole: api/models/databricks/serviceprincipalrole.md
-        - SqlQuery: api/models/databricks/sqlquery.md
-        - api/models/databricks/user.md
-        - UserRole: api/models/databricks/userrole.md
-        - api/models/databricks/warehouse.md
-        - WorkspaceFile: api/models/databricks/workspacefile.md
-      - Providers:
-        - AzureProvider: api/models/providers/azure.md
-        - AzurePulumiProvider: api/models/providers/azurepulumi.md
-        - AWSProvider: api/models/providers/aws.md
-        - DatabricksProvider: api/models/providers/databricks.md
+      - Pipelines:
+        - Pipeline: api/models/pipeline.md
+        - PipelineNode: api/models/pipelinenode.md
+        - PipelineNodeExpectation: api/models/pipelinenodeexpectation.md
       - Resources:
         - BaseResource: api/models/resources/baseresource.md
         - PulumiResource: api/models/resources/pulumiresource.md
+        - TerraformResource: api/models/resources/terraformresource.md
+        - Databricks:
+          - AccessControl: api/models/resources/databricks/accesscontrol.md
+          - api/models/resources/databricks/cluster.md
+          - api/models/resources/databricks/directory.md
+          - DLT Pipeline: api/models/resources/databricks/dltpipeline.md
+          - ExternalLocation: api/models/resources/databricks/externallocation.md
+          - api/models/resources/databricks/grants.md
+          - api/models/resources/databricks/group.md
+          - api/models/resources/databricks/job.md
+          - api/models/resources/databricks/metastore.md
+          - MetastoreAssignment: api/models/resources/databricks/metastoreassignment.md
+          - MetastoreDataAccess: api/models/resources/databricks/metastoredataaccess.md
+          - MwsPermissionAssignment: api/models/resources/databricks/mwspermissionassignment.md
+          - api/models/resources/databricks/mws.md
+          - api/models/resources/databricks/notebook.md
+          - api/models/resources/databricks/secret.md
+          - SecretAcl: api/models/resources/databricks/secretacl.md
+          - SecretScope: api/models/resources/databricks/secretscope.md
+          - ServicePrincipal: api/models/resources/databricks/serviceprincipal.md
+          - ServicePrincipalRole: api/models/resources/databricks/serviceprincipalrole.md
+          - SqlQuery: api/models/resources/databricks/sqlquery.md
+          - api/models/resources/databricks/user.md
+          - UserRole: api/models/resources/databricks/userrole.md
+          - api/models/resources/databricks/warehouse.md
+          - WorkspaceFile: api/models/resources/databricks/workspacefile.md
+          - api/models/resources/databricks/catalog.md
+          - api/models/resources/databricks/column.md
+          - api/models/resources/databricks/schema.md
+          - api/models/resources/databricks/table.md
+          - api/models/resources/databricks/volume.md
+        - Providers:
+          - AzureProvider: api/models/resources/providers/azure.md
+          - AzurePulumiProvider: api/resources/models/providers/azurepulumi.md
+          - AWSProvider: api/models/resources/providers/aws.md
+          - DatabricksProvider: api/resources/models/providers/databricks.md
       - Spark:
         - SparkChain: api/models/spark/sparkchain.md
         - SparkChainNode: api/models/spark/sparkchainnode.md
         - SparkFuncArg: api/models/spark/sparkfuncarg.md
-      - SQL:
-          - api/models/sql/catalog.md
-          - api/models/sql/column.md
-          - api/models/sql/schema.md
-          - api/models/sql/table.md
-          - TableExpectations: api/models/sql/tableexpectation.md
-          - TableBuilder: api/models/sql/tablebuilder.md
-          - api/models/sql/volume.md
       - Stacks:
           - Stack: api/models/stacks/stack.md
           - PulumiStack: api/models/stacks/pulumistack.md
           - TerraformStack: api/models/stacks/terraformstack.md
     - CLI: api/cli.md
     - Spark:
       - DataFrame:
```

### Comparing `laktory-0.2.1/pyproject.toml` & `laktory-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = [
     "databricks-sdk",
     "inflect",
+    "networkx",
     "planck",
     "prompt_toolkit",
     "pulumi",
     "pulumi_databricks>=1.36",  # required to monitor laktory usage
     "pulumi_random",
     "pyyaml",
     "pydantic>=2",
@@ -54,20 +55,24 @@
     "black",
     "flit",
     "mkdocs",
     "mkdocstrings[python]",
     "mkdocs-material",
     "mkdocs-video",
 #    "mkdocs-snippets",
+    "plotly",
 ]
 spark = [
     "pandas",
     "pyarrow",
     "pyspark",
 ]
+polars = [
+    "polars"
+]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-examples",
 #    "tox"
     "yfinance",
 ]
```

### Comparing `laktory-0.2.1/scripts/databricks_api_call.py` & `laktory-0.3.0/scripts/databricks_api_call.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/build_test_data.py` & `laktory-0.3.0/tests/build_test_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,24 +68,24 @@
 
 
 # --------------------------------------------------------------------------- #
 # Build Pandas DataFrame                                                      #
 # --------------------------------------------------------------------------- #
 
 pdf = pd.DataFrame([e.model_dump() for e in events])
-del pdf["event_root"]
+# del pdf["event_root"]
 # pdf.to_json(os.path.join(rootpath, "brz_stock_prices.json"))
 
 
 # --------------------------------------------------------------------------- #
 # Write Bronze DataFrame                                                      #
 # --------------------------------------------------------------------------- #
 
 df = spark.createDataFrame(
-    pdf,
+    pdf[["name", "description", "producer", "data"]],
     schema=T.StructType(
         [
             T.StructField("name", T.StringType()),
             T.StructField("description", T.StringType()),
             T.StructField(
                 "producer",
                 T.StructType(
@@ -113,30 +113,30 @@
                     ]
                 ),
             ),
         ]
     ),
 )
 df = df.repartition(1)
-df.write.parquet(os.path.join(rootpath, "brz_stock_prices"), mode="overwrite")
+df.write.parquet(os.path.join(rootpath, "brz_stock_prices"), mode="OVERWRITE")
 
 
 # --------------------------------------------------------------------------- #
 # Build Silver DataFrame                                                      #
 # --------------------------------------------------------------------------- #
 
 # Stock prices
 cols0 = df.columns
 df = df.withColumn("created_at", F.col("data._created_at").cast(T.TimestampType()))
 df = df.withColumn("symbol", F.col("data.symbol").cast(T.StringType()))
 df = df.withColumn("open", F.col("data.open").cast(T.DoubleType()))
 df = df.withColumn("close", F.col("data.close").cast(T.DoubleType()))
 df = df.drop(*cols0)
 df = df.repartition(1)
-df.write.parquet(os.path.join(rootpath, "slv_stock_prices"), mode="overwrite")
+df.write.parquet(os.path.join(rootpath, "slv_stock_prices"), mode="OVERWRITE")
 
 # Metadata
 df_meta = spark.createDataFrame(
     pd.DataFrame(
         {
             "symbol2": ["AAPL", "GOOGL", "AMZN"],
             "currency": ["USD"] * 3,
@@ -146,9 +146,9 @@
                 "1997-05-15T13:30:00.000Z",
             ],
         }
     )
 )
 df_meta = df_meta.repartition(1)
 df_meta.write.format("parquet").save(
-    os.path.join(rootpath, "slv_stock_meta"), mode="overwrite"
+    os.path.join(rootpath, "slv_stock_meta"), mode="OVERWRITE"
 )
```

### Comparing `laktory-0.2.1/tests/data/brz_stock_prices/part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet` & `laktory-0.3.0/tests/data/brz_stock_prices/part-00000-877096dd-1964-482e-9873-76361150a331-c000.snappy.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -245,108 +245,108 @@
 00000f40: 6800 150a 2502 1803 6c6f 7700 150c 2502  h...%...low...%.
 00000f50: 1805 5f6e 616d 6525 004c 1c00 0000 150c  .._name%.L......
 00000f60: 2502 180e 5f70 726f 6475 6365 725f 6e61  %..._producer_na
 00000f70: 6d65 2500 4c1c 0000 0015 0c25 0218 0b5f  me%.L......%..._
 00000f80: 6372 6561 7465 645f 6174 2500 4c1c 0000  created_at%.L...
 00000f90: 0015 0c25 0218 0340 6964 2500 4c1c 0000  ...%...@id%.L...
 00000fa0: 0016 a001 191c 19fc 0f26 501c 150c 1935  .........&P....5
-00000fb0: 0408 0619 1804 6e61 6d65 1502 16a0 0116  ......name......
+00000fb0: 0804 0619 1804 6e61 6d65 1502 16a0 0116  ......name......
 00000fc0: 8801 1690 0126 5026 081c 180b 7374 6f63  .....&P&....stoc
 00000fd0: 6b5f 7072 6963 6518 0b73 746f 636b 5f70  k_price..stock_p
 00000fe0: 7269 6365 1600 280b 7374 6f63 6b5f 7072  rice..(.stock_pr
 00000ff0: 6963 6518 0b73 746f 636b 5f70 7269 6365  ice..stock_price
 00001000: 0019 2c15 0415 0415 0200 1500 1504 1502  ..,.............
 00001010: 0000 16fc 3615 1416 ae2f 154a 0026 9801  ....6..../.J.&..
-00001020: 1c15 0c19 3508 0006 1918 0b64 6573 6372  ....5......descr
+00001020: 1c15 0c19 3500 0806 1918 0b64 6573 6372  ....5......descr
 00001030: 6970 7469 6f6e 1502 16a0 0116 3e16 4226  iption......>.B&
 00001040: 9801 3c36 a001 0019 1c15 0015 0015 0200  ..<6............
 00001050: 0016 9037 1516 16f8 2f15 2000 26a6 021c  ...7..../. .&...
-00001060: 150c 1935 0408 0619 2808 7072 6f64 7563  ...5....(.produc
+00001060: 150c 1935 0804 0619 2808 7072 6f64 7563  ...5....(.produc
 00001070: 6572 046e 616d 6515 0216 a001 168c 0116  er.name.........
 00001080: 9401 26a6 0226 da01 1c18 0d79 6168 6f6f  ..&..&.....yahoo
 00001090: 2d66 696e 616e 6365 180d 7961 686f 6f2d  -finance..yahoo-
 000010a0: 6669 6e61 6e63 6516 0028 0d79 6168 6f6f  finance..(.yahoo
 000010b0: 2d66 696e 616e 6365 180d 7961 686f 6f2d  -finance..yahoo-
 000010c0: 6669 6e61 6e63 6500 192c 1504 1504 1502  finance..,......
 000010d0: 0015 0015 0415 0200 0016 a637 1516 1698  ...........7....
-000010e0: 3015 5200 26ee 021c 150c 1935 0800 0619  0.R.&......5....
+000010e0: 3015 5200 26ee 021c 150c 1935 0008 0619  0.R.&......5....
 000010f0: 2808 7072 6f64 7563 6572 0b64 6573 6372  (.producer.descr
 00001100: 6970 7469 6f6e 1502 16a0 0116 3e16 4226  iption......>.B&
 00001110: ee02 3c36 a001 0019 1c15 0015 0015 0200  ..<6............
 00001120: 0016 bc37 1516 16ea 3015 2000 26e2 031c  ...7....0. .&...
-00001130: 1502 1935 0408 0619 2808 7072 6f64 7563  ...5....(.produc
+00001130: 1502 1935 0804 0619 2808 7072 6f64 7563  ...5....(.produc
 00001140: 6572 0570 6172 7479 1502 16a0 0116 7216  er.party......r.
 00001150: 7a26 e203 26b0 031c 1804 0100 0000 1804  z&..&...........
 00001160: 0100 0000 1600 2804 0100 0000 1804 0100  ......(.........
 00001170: 0000 0019 2c15 0415 0415 0200 1500 1504  ....,...........
 00001180: 1502 0000 16d2 3715 1616 8a31 152e 0026  ......7....1...&
-00001190: d006 1c15 0c19 3504 0806 1928 0464 6174  ......5....(.dat
+00001190: d006 1c15 0c19 3508 0406 1928 0464 6174  ......5....(.dat
 000011a0: 610a 6372 6561 7465 645f 6174 1502 16a0  a.created_at....
 000011b0: 0116 e808 16a6 0326 d006 26aa 041c 3600  .......&..&...6.
 000011c0: 2813 3230 3233 2d30 392d 3239 5430 303a  (.2023-09-29T00:
 000011d0: 3030 3a30 3018 1332 3032 332d 3039 2d30  00:00..2023-09-0
 000011e0: 3154 3030 3a30 303a 3030 0019 2c15 0415  1T00:00:00..,...
 000011f0: 0415 0200 1500 1504 1502 0000 16e8 3715  ..............7.
-00001200: 1816 b831 156a 0026 b808 1c15 0c19 3504  ...1.j.&......5.
-00001210: 0806 1928 0464 6174 6106 7379 6d62 6f6c  ...(.data.symbol
+00001200: 1816 b831 156a 0026 b808 1c15 0c19 3508  ...1.j.&......5.
+00001210: 0406 1928 0464 6174 6106 7379 6d62 6f6c  ...(.data.symbol
 00001220: 1502 16a0 0116 b601 16ba 0126 b808 26d0  ...........&..&.
 00001230: 071c 3600 2804 4d53 4654 1804 4141 504c  ..6.(.MSFT..AAPL
 00001240: 0019 2c15 0415 0415 0200 1500 1504 1502  ..,.............
 00001250: 0000 1680 3815 1616 a232 152e 0026 8a09  ....8....2...&..
-00001260: 1c15 0a19 3508 0006 1928 0464 6174 6104  ....5....(.data.
+00001260: 1c15 0a19 3500 0806 1928 0464 6174 6104  ....5....(.data.
 00001270: 6f70 656e 1502 16a0 0116 c20a 16f4 0726  open...........&
 00001280: 8a09 3c18 0800 0000 6066 3275 4018 0800  ..<.....`f2u@...
 00001290: 0000 608f 025f 4016 0028 0800 0000 6066  ..`.._@..(....`f
 000012a0: 3275 4018 0800 0000 608f 025f 4000 191c  2u@.....`.._@...
 000012b0: 1500 1500 1502 0000 1696 3815 1816 d032  ..........8....2
-000012c0: 153e 0026 fe10 1c15 0a19 3508 0006 1928  .>.&......5....(
+000012c0: 153e 0026 fe10 1c15 0a19 3500 0806 1928  .>.&......5....(
 000012d0: 0464 6174 6105 636c 6f73 6515 0216 a001  .data.close.....
 000012e0: 16c0 0a16 8008 26fe 103c 1808 0000 0040  ......&..<.....@
 000012f0: 332b 7540 1808 0000 0060 b87e 5f40 1600  3+u@.....`.~_@..
 00001300: 2808 0000 0040 332b 7540 1808 0000 0060  (....@3+u@.....`
 00001310: b87e 5f40 0019 1c15 0015 0015 0200 0016  .~_@............
 00001320: ae38 1518 168e 3315 3e00 26fe 181c 150a  .8....3.>.&.....
-00001330: 1935 0800 0619 2804 6461 7461 0468 6967  .5....(.data.hig
+00001330: 1935 0008 0619 2804 6461 7461 0468 6967  .5....(.data.hig
 00001340: 6815 0216 a001 16c2 0a16 f007 26fe 183c  h...........&..<
 00001350: 1808 0000 0080 c24d 7540 1808 0000 00c0  .......Mu@......
 00001360: 1ea5 5f40 1600 2808 0000 0080 c24d 7540  .._@..(......Mu@
 00001370: 1808 0000 00c0 1ea5 5f40 0019 1c15 0015  ........_@......
 00001380: 0015 0200 0016 c638 1518 16cc 3315 3e00  .......8....3.>.
-00001390: 26ee 201c 150a 1935 0800 0619 2804 6461  &. ....5....(.da
+00001390: 26ee 201c 150a 1935 0008 0619 2804 6461  &. ....5....(.da
 000013a0: 7461 036c 6f77 1502 16a0 0116 c20a 16f0  ta.low..........
 000013b0: 0726 ee20 3c18 0800 0000 c01e 0975 4018  .&. <........u@.
 000013c0: 0800 0000 608f c25e 4016 0028 0800 0000  ....`..^@..(....
 000013d0: c01e 0975 4018 0800 0000 608f c25e 4000  ...u@.....`..^@.
 000013e0: 191c 1500 1500 1502 0000 16de 3815 1816  ............8...
-000013f0: 8a34 153e 0026 a629 1c15 0c19 3504 0806  .4.>.&.)....5...
+000013f0: 8a34 153e 0026 a629 1c15 0c19 3508 0406  .4.>.&.)....5...
 00001400: 1928 0464 6174 6105 5f6e 616d 6515 0216  .(.data._name...
 00001410: a001 1688 0116 9001 26a6 2926 de28 1c18  ........&.)&.(..
 00001420: 0b73 746f 636b 5f70 7269 6365 180b 7374  .stock_price..st
 00001430: 6f63 6b5f 7072 6963 6516 0028 0b73 746f  ock_price..(.sto
 00001440: 636b 5f70 7269 6365 180b 7374 6f63 6b5f  ck_price..stock_
 00001450: 7072 6963 6500 192c 1504 1504 1502 0015  price..,........
 00001460: 0015 0415 0200 0016 f638 1516 16c8 3415  .........8....4.
-00001470: 4a00 26ba 2a1c 150c 1935 0408 0619 2804  J.&.*....5....(.
+00001470: 4a00 26ba 2a1c 150c 1935 0804 0619 2804  J.&.*....5....(.
 00001480: 6461 7461 0e5f 7072 6f64 7563 6572 5f6e  data._producer_n
 00001490: 616d 6515 0216 a001 168c 0116 9401 26ba  ame...........&.
 000014a0: 2a26 ee29 1c18 0d79 6168 6f6f 2d66 696e  *&.)...yahoo-fin
 000014b0: 616e 6365 180d 7961 686f 6f2d 6669 6e61  ance..yahoo-fina
 000014c0: 6e63 6516 0028 0d79 6168 6f6f 2d66 696e  nce..(.yahoo-fin
 000014d0: 616e 6365 180d 7961 686f 6f2d 6669 6e61  ance..yahoo-fina
 000014e0: 6e63 6500 192c 1504 1504 1502 0015 0015  nce..,..........
 000014f0: 0415 0200 0016 8c39 1516 1692 3515 5200  .......9....5.R.
-00001500: 26ae 2d1c 150c 1935 0408 0619 2804 6461  &.-....5....(.da
+00001500: 26ae 2d1c 150c 1935 0804 0619 2804 6461  &.-....5....(.da
 00001510: 7461 0b5f 6372 6561 7465 645f 6174 1502  ta._created_at..
 00001520: 16a0 0116 9009 16ac 0326 ae2d 2682 2b1c  .........&.-&.+.
 00001530: 3600 2814 3230 3233 2d30 392d 3239 5430  6.(.2023-09-29T0
 00001540: 303a 3030 3a30 305a 1814 3230 3233 2d30  0:00:00Z..2023-0
 00001550: 392d 3031 5430 303a 3030 3a30 305a 0019  9-01T00:00:00Z..
 00001560: 2c15 0415 0415 0200 1500 1504 1502 0000  ,...............
 00001570: 16a2 3915 1816 e435 156e 0026 e62e 1c15  ..9....5.n.&....
-00001580: 0c19 3504 0806 1928 0464 6174 6103 4069  ..5....(.data.@i
+00001580: 0c19 3508 0406 1928 0464 6174 6103 4069  ..5....(.data.@i
 00001590: 6415 0216 a001 1678 1680 0126 e62e 26ae  d......x...&..&.
 000015a0: 2e1c 1803 5f69 6418 035f 6964 1600 2803  ...._id.._id..(.
 000015b0: 5f69 6418 035f 6964 0019 2c15 0415 0415  _id.._id..,.....
 000015c0: 0200 1500 1504 1502 0000 16ba 3915 1616  ............9...
 000015d0: d236 152a 0016 c244 16a0 0126 0816 a62f  .6.*...D...&.../
 000015e0: 1400 0019 2c18 186f 7267 2e61 7061 6368  ....,..org.apach
 000015f0: 652e 7370 6172 6b2e 7665 7273 696f 6e18  e.spark.version.
```

### Comparing `laktory-0.2.1/tests/data/slv_stock_meta/part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet` & `laktory-0.3.0/tests/data/slv_stock_meta/part-00000-7aba5fec-c547-47b9-9053-b535a9cbd961-c000.snappy.parquet`

 * *Files 10% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 00000160: 1600 0000 191c 16f2 0115 d601 1600 0000  ................
 00000170: 1502 194c 480c 7370 6172 6b5f 7363 6865  ...LH.spark_sche
 00000180: 6d61 1506 0015 0c25 0218 0773 796d 626f  ma.....%...symbo
 00000190: 6c32 2500 4c1c 0000 0015 0c25 0218 0863  l2%.L......%...c
 000001a0: 7572 7265 6e63 7925 004c 1c00 0000 150c  urrency%.L......
 000001b0: 2502 180c 6669 7273 745f 7472 6164 6564  %...first_traded
 000001c0: 2500 4c1c 0000 0016 0619 1c19 3c26 081c  %.L.........<&..
-000001d0: 150c 1935 0800 0619 1807 7379 6d62 6f6c  ...5......symbol
+000001d0: 150c 1935 0008 0619 1807 7379 6d62 6f6c  ...5......symbol
 000001e0: 3215 0216 0616 6c16 7026 083c 3600 2805  2.....l.p&.<6.(.
 000001f0: 474f 4f47 4c18 0441 4150 4c00 191c 1500  GOOGL..AAPL.....
 00000200: 1500 1502 0000 169e 0515 1416 c803 1530  ...............0
-00000210: 0026 b001 1c15 0c19 3504 0806 1918 0863  .&......5......c
+00000210: 0026 b001 1c15 0c19 3508 0406 1918 0863  .&......5......c
 00000220: 7572 7265 6e63 7915 0216 0616 7216 7a26  urrency.....r.z&
 00000230: b001 2678 1c18 0355 5344 1803 5553 4416  ..&x...USD..USD.
 00000240: 0028 0355 5344 1803 5553 4400 192c 1504  .(.USD..USD..,..
 00000250: 1504 1502 0015 0015 0415 0200 0016 b205  ................
 00000260: 1516 16f8 0315 2a00 26f2 011c 150c 1935  ......*.&......5
-00000270: 0800 0619 180c 6669 7273 745f 7472 6164  ......first_trad
+00000270: 0008 0619 180c 6669 7273 745f 7472 6164  ......first_trad
 00000280: 6564 1502 1606 16e4 0116 d601 26f2 013c  ed..........&..<
 00000290: 3600 2817 3230 3034 2d30 382d 3139 5431  6.(.2004-08-19T1
 000002a0: 333a 3330 3a30 302e 3030 5a18 1831 3938  3:30:00.00Z..198
 000002b0: 302d 3132 2d31 3254 3134 3a33 303a 3030  0-12-12T14:30:00
 000002c0: 2e30 3030 5a00 191c 1500 1500 1502 0000  .000Z...........
 000002d0: 16c8 0515 1816 a204 157c 0016 c203 1606  .........|......
 000002e0: 2608 16c0 0314 0000 192c 1818 6f72 672e  &........,..org.
```

### Comparing `laktory-0.2.1/tests/data/slv_stock_prices/part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet` & `laktory-0.3.0/tests/data/slv_stock_prices/part-00000-f272d903-4f35-4abd-a905-1ea1a1e38110-c000.snappy.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -89,30 +89,30 @@
 00000580: 191c 16b4 0415 f407 1600 0000 191c 16a8  ................
 00000590: 0c15 8008 1600 0000 1502 195c 480c 7370  ...........\H.sp
 000005a0: 6172 6b5f 7363 6865 6d61 1508 0015 0625  ark_schema.....%
 000005b0: 0218 0a63 7265 6174 6564 5f61 7400 150c  ...created_at...
 000005c0: 2502 1806 7379 6d62 6f6c 2500 4c1c 0000  %...symbol%.L...
 000005d0: 0015 0a25 0218 046f 7065 6e00 150a 2502  ...%...open...%.
 000005e0: 1805 636c 6f73 6500 16a0 0119 1c19 4c26  ..close.......L&
-000005f0: f801 1c15 0619 3504 0806 1918 0a63 7265  ......5......cre
+000005f0: f801 1c15 0619 3508 0406 1918 0a63 7265  ......5......cre
 00000600: 6174 6564 5f61 7415 0216 a001 16b0 0516  ated_at.........
 00000610: f002 26f8 0126 081c 3600 0019 2c15 0415  ..&..&..6...,...
 00000620: 0415 0200 1500 1504 1502 0000 16d2 1515  ................
-00000630: 1800 26e0 031c 150c 1935 0408 0619 1806  ..&......5......
+00000630: 1800 26e0 031c 150c 1935 0804 0619 1806  ..&......5......
 00000640: 7379 6d62 6f6c 1502 16a0 0116 b801 16bc  symbol..........
 00000650: 0126 e003 26f8 021c 3600 2804 4d53 4654  .&..&...6.(.MSFT
 00000660: 1804 4141 504c 0019 2c15 0415 0415 0200  ..AAPL..,.......
 00000670: 1500 1504 1502 0000 16ea 1515 1616 a814  ................
-00000680: 152e 0026 b404 1c15 0a19 3508 0006 1918  ...&......5.....
+00000680: 152e 0026 b404 1c15 0a19 3500 0806 1918  ...&......5.....
 00000690: 046f 7065 6e15 0216 a001 16c2 0a16 f407  .open...........
 000006a0: 26b4 043c 1808 0000 0060 6632 7540 1808  &..<.....`f2u@..
 000006b0: 0000 0060 8f02 5f40 1600 2808 0000 0060  ...`.._@..(....`
 000006c0: 6632 7540 1808 0000 0060 8f02 5f40 0019  f2u@.....`.._@..
 000006d0: 1c15 0015 0015 0200 0016 8016 1518 16d6  ................
-000006e0: 1415 3e00 26a8 0c1c 150a 1935 0800 0619  ..>.&......5....
+000006e0: 1415 3e00 26a8 0c1c 150a 1935 0008 0619  ..>.&......5....
 000006f0: 1805 636c 6f73 6515 0216 a001 16c0 0a16  ..close.........
 00000700: 8008 26a8 0c3c 1808 0000 0040 332b 7540  ..&..<.....@3+u@
 00000710: 1808 0000 0060 b87e 5f40 1600 2808 0000  .....`.~_@..(...
 00000720: 0040 332b 7540 1808 0000 0060 b87e 5f40  .@3+u@.....`.~_@
 00000730: 0019 1c15 0015 0015 0200 0016 9816 1518  ................
 00000740: 1694 1515 3e00 16ea 1b16 a001 2608 16a0  ....>.......&...
 00000750: 1414 0000 192c 1818 6f72 672e 6170 6163  .....,..org.apac
```

### Comparing `laktory-0.2.1/tests/data/stack.yaml` & `laktory-0.3.0/tests/data/stack.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,29 @@
   providers:
     databricks:  # for terraform, provider name must match resource type prefix
       host: ${vars.DATABRICKS_HOST}
       token: ${vars.DATABRICKS_TOKEN}
   pipelines:
     pl-custom-name:
       name: pl-stock-prices-ut-stack
-      libraries:
-        - notebook:
-            path: /pipelines/dlt_brz_template.py
-      access_controls:
-        - group_name: account users
-          permission_level: CAN_VIEW
-        - group_name: role-engineers
-          permission_level: CAN_RUN
-      options:
-        provider: ${resources.databricks}
-  jobs:
+      orchestrator: DLT
+      nodes: []
+      dlt:
+        resource_name: dlt-custom-name
+        libraries:
+          - notebook:
+              path: /pipelines/dlt_brz_template.py
+        access_controls:
+          - group_name: account users
+            permission_level: CAN_VIEW
+          - group_name: role-engineers
+            permission_level: CAN_RUN
+        options:
+          provider: ${resources.databricks}
+  databricks_jobs:
     job-stock-prices-ut-stack:
       name: job-stock-prices-ut-stack
       clusters:
         - name: main
           spark_version: 14.0.x-scala2.12
           node_type_id: ${vars.node_type_id}
           spark_env_vars:
@@ -41,28 +45,29 @@
           libraries:
             - pypi:
                 package: laktory==0.0.27
             - pypi:
                 package: yfinance
         - task_key: run-pipeline
           pipeline_task:
-            pipeline_id: ${resources.pl-custom-name.id}  # LAKTORY STYLE
-#            pipeline_id: ${resources.pipelines.pl-custom-name.id}  # BUNDLES STYLE
+            pipeline_id: ${resources.dlt-custom-name.id}  # LAKTORY STYLE
+#            pipeline_id: ${resources.dltpipelines.pl-custom-name.id}  # BUNDLES STYLE
 #            pipeline_id: ${databricks_pipeline.pl-custom-name.id}  # TERRAFORM STYLE
 #            pipeline_id: ${pl-custom-name.id}  # PULUMI STYLE
 
 environments:
   dev:
     variables:
       env: dev
       is_dev: true
       node_type_id: Standard_DS3_v2
   prod:
     resources:
       pipelines:
         pl-custom-name:
-          development: False
+          dlt:
+            development: False
     variables:
       env: prod
       is_dev: false
       node_type_id: Standard_DS4_v2
```

### Comparing `laktory-0.2.1/tests/test_basemodel.py` & `laktory-0.3.0/tests/test_basemodel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pulumi
 import os
 
 from laktory.models import BaseModel
-from laktory.models import Table
-from laktory.models import Schema
-from laktory.models import Job
+from laktory.models.resources.databricks import Table
+from laktory.models.resources.databricks import Schema
+from laktory.models.resources.databricks import Job
 from laktory import settings
 from laktory._testing import Paths
 from pulumi_random import RandomString
 
 paths = Paths(__file__)
 
 env = RandomString("env", length=3, upper=False, numeric=False, special=False)
@@ -110,26 +110,14 @@
     print(dump)
     assert dump == {
         "comment": None,
         "grants": None,
         "name": "${vars.env}.${vars.schema_name}",
         "tables": [
             {
-                "builder": {
-                    "layer": None,
-                    "template": None,
-                    "addLaktoryColumns": True,
-                    "asDltView": False,
-                    "dropDuplicates": None,
-                    "dropSourceColumns": None,
-                    "eventSource": None,
-                    "pipelineName": None,
-                    "tableSource": None,
-                    "sparkChain": None,
-                },
                 "columns": [
                     {
                         "comment": None,
                         "name": "open",
                         "pii": None,
                         "type": "double",
                         "unit": None,
@@ -147,40 +135,25 @@
                         "catalogName": None,
                         "raiseMissingArgException": True,
                         "schemaName": None,
                         "tableName": "AAPL",
                     },
                 ],
                 "comment": None,
-                "data": None,
-                "expectations": [],
                 "grants": None,
                 "name": "AAPL",
                 "catalogName": "${vars.env}",
                 "dataSourceFormat": "DELTA",
                 "primaryKey": None,
                 "schemaName": "${vars.env}.${vars.schema_name}",
                 "tableType": "MANAGED",
-                "timestampKey": None,
                 "viewDefinition": None,
                 "warehouseId": "08b717ce051a0261",
             },
             {
-                "builder": {
-                    "layer": None,
-                    "template": None,
-                    "addLaktoryColumns": True,
-                    "asDltView": False,
-                    "dropDuplicates": None,
-                    "dropSourceColumns": None,
-                    "eventSource": None,
-                    "pipelineName": None,
-                    "tableSource": None,
-                    "sparkChain": None,
-                },
                 "columns": [
                     {
                         "comment": None,
                         "name": "${vars.dynamic_column}",
                         "pii": None,
                         "type": "double",
                         "unit": None,
@@ -198,24 +171,21 @@
                         "catalogName": None,
                         "raiseMissingArgException": True,
                         "schemaName": None,
                         "tableName": "GOOGL",
                     },
                 ],
                 "comment": None,
-                "data": None,
-                "expectations": [],
                 "grants": None,
                 "name": "GOOGL",
                 "catalogName": "${vars.env}",
                 "dataSourceFormat": "DELTA",
                 "primaryKey": None,
                 "schemaName": "${vars.env}.${vars.schema_name}",
                 "tableType": "MANAGED",
-                "timestampKey": None,
                 "viewDefinition": None,
                 "warehouseId": "08b717ce051a0261",
             },
         ],
         "volumes": [],
         "catalogName": "${vars.env}",
         "forceDestroy": True,
```

### Comparing `laktory-0.2.1/tests/test_baseresource.py` & `laktory-0.3.0/tests/test_baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/test_catalog.py` & `laktory-0.3.0/tests/test_catalog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from laktory.models import Catalog
+from laktory.models.resources.databricks import Catalog
 
 
 catalog = Catalog(
     name="dev",
     grants=[
         {"principal": "account users", "privileges": ["USE_CATALOG", "USE_SCHEMA"]}
     ],
```

### Comparing `laktory-0.2.1/tests/test_cli.py` & `laktory-0.3.0/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
     data = stack.model_dump(exclude_none=True)
 
     assert stack.backend == "pulumi"
     assert stack.name == "quickstart"
     assert stack.pulumi.config["databricks:host"] == "${vars.DATABRICKS_HOST}"
     assert stack.pulumi.config["databricks:token"] == "${vars.DATABRICKS_TOKEN}"
-    assert len(stack.resources.dbfsfiles) == 1
-    assert len(stack.resources.notebooks) == 2
+    assert len(stack.resources.databricks_dbfsfiles) == 1
+    assert len(stack.resources.databricks_notebooks) == 1
     assert len(stack.resources.pipelines) == 1
 
 
 def test_quickstart_terraform():
     filepath = os.path.join(paths.tmp, "stack_quickstart_terraform.yaml")
     result = runner.invoke(
         app,
@@ -86,16 +86,16 @@
 
     data = stack.model_dump(exclude_none=True)
 
     assert stack.backend == "terraform"
     assert stack.name == "quickstart"
     assert stack.resources.providers["databricks"].host == "${vars.DATABRICKS_HOST}"
     assert stack.resources.providers["databricks"].token == "${vars.DATABRICKS_TOKEN}"
-    assert len(stack.resources.dbfsfiles) == 1
-    assert len(stack.resources.notebooks) == 2
+    assert len(stack.resources.databricks_dbfsfiles) == 1
+    assert len(stack.resources.databricks_notebooks) == 1
     assert len(stack.resources.pipelines) == 1
 
 
 def atest_deploy_pulumi():
     # TODO: Figure out how to run in isolation. Currently, pulumi up commands
     # are run concurrently because of the multiple python testing environment
     # which result in:  Conflict: Another update is currently in progress
```

### Comparing `laktory-0.2.1/tests/test_column.py` & `laktory-0.3.0/tests/test_column.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import json
 import yaml
 
-from laktory.models import Column
+from laktory.models.resources.databricks import Column
 from laktory._testing import Paths
 from laktory._testing.stockprices import df_brz as df
 
 paths = Paths(__file__)
 GOOGL = {
     "name": "close",
     "type": "double",
```

### Comparing `laktory-0.2.1/tests/test_dataevent.py` & `laktory-0.3.0/tests/test_dataevent.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,76 +7,68 @@
 from laktory import models
 from laktory import settings
 from laktory._testing import Paths
 
 paths = Paths(__file__)
 
 
-# Header
-class StockPriceDataEventHeader(models.DataEventHeader):
-    name: str = "stock_price"
-    producer: models.DataProducer = models.DataProducer(name="yahoo-finance")
-
-
-header = StockPriceDataEventHeader()
-
-
 # Event
 with open(
     os.path.join(
         paths.data,
         "./events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json",
     )
 ) as fp:
     event = json.load(fp)
 event = models.DataEvent(**event)
+header = event.model_copy(deep=True)
+header.data = None
+
 
+def test_dataevent_header():
 
-def test_dataeventheader():
     print(header.model_dump())
     assert header.model_dump() == {
-        "name": "stock_price",
+        "data": None,
         "description": None,
+        # "event_root": None,
+        "name": "stock_price",
         "producer": {"name": "yahoo-finance", "description": None, "party": 1},
-        "events_root_": None,
-        "event_root_": None,
     }
     assert header.events_root == "/Volumes/dev/sources/landing/events/"
     assert (
         header.event_root
         == "/Volumes/dev/sources/landing/events/yahoo-finance/stock_price/"
     )
 
 
-def test_dataeventheader_root():
+def test_dataevent_root():
     # Custom value for events root
-    header = models.DataEventHeader(name="my-event", events_root="test")
-    header2 = models.DataEventHeader(
-        **header.model_dump(by_alias=True, exclude_none=True)
-    )
+    header = models.DataEvent(name="my-event", events_root="test")
+    # header2 = models.DataEvent(
+    #     **header.model_dump(by_alias=True, exclude_none=True)
+    # )
     assert header.events_root == "test"
-    assert header2.events_root == "test"
+    # assert header2.events_root == "test"
 
     # Default value
-    header = models.DataEventHeader(name="my-event")
+    header = models.DataEvent(name="my-event")
     assert header.events_root == "/Volumes/dev/sources/landing/events/"
     root0 = settings.workspace_landing_root
-    header2 = models.DataEventHeader(
-        **header.model_dump(by_alias=True, exclude_none=True)
-    )
+    header2 = models.DataEvent(**header.model_dump(by_alias=True, exclude_none=True))
     settings.workspace_landing_root = "custom_root/"
     assert header.events_root == "custom_root/events/"
     assert header2.events_root == "custom_root/events/"
     settings.workspace_landing_root = root0
 
     # Custom value for event root
-    header = models.DataEventHeader(name="my-event", event_root="/Landing/my_event")
+    header = models.DataEvent(name="my-event", event_root="/Landing/my_event")
     print(header)
     assert header.event_root == "/Landing/my_event"
-    header = models.DataEventHeader(**header.model_dump(exclude_none=True))
+    header = models.DataEvent(**header.model_dump(exclude_none=True))
 
 
 def test_dataevent():
     assert event.producer.name == "yahoo-finance"
     assert event.data["symbol"] == "AAPL"
     assert event.data["open"] == pytest.approx(189.49, abs=0.01)
     assert event.data["_producer_name"] == "yahoo-finance"
@@ -89,17 +81,17 @@
 
 
 def test_model_dump():
     # Without exclusions
     d = event.model_dump(exclude=[])
     print(d)
     assert d == {
-        "event_name": "stock_price",
-        "event_description": None,
-        "event_producer": {"name": "yahoo-finance", "description": None, "party": 1},
+        "name": "stock_price",
+        "description": None,
+        "producer": {"name": "yahoo-finance", "description": None, "party": 1},
         "events_root": None,
         "event_root": None,
         "data": {
             "created_at": "2023-09-01T00:00:00",
             "symbol": "AAPL",
             "open": 189.49000549316406,
             "close": 189.4600067138672,
@@ -116,18 +108,18 @@
 
     assert event.events_root == "/Volumes/dev/sources/landing/events/"
 
     # With exclusions
     d = event.model_dump()
     print(d)
     assert d == {
-        "event_name": "stock_price",
-        "event_description": None,
-        "event_producer": {"name": "yahoo-finance", "description": None, "party": 1},
-        "event_root": None,
+        "name": "stock_price",
+        "description": None,
+        "producer": {"name": "yahoo-finance", "description": None, "party": 1},
+        # "event_root": None,
         "data": {
             "created_at": "2023-09-01T00:00:00",
             "symbol": "AAPL",
             "open": 189.49000549316406,
             "close": 189.4600067138672,
             "high": 189.9199981689453,
             "low": 188.27999877929688,
@@ -169,22 +161,15 @@
 
     event.to_aws_s3_bucket(bucket_name="okube-unit-testing", overwrite=True)
     with pytest.raises(FileExistsError):
         event.to_aws_s3_bucket(bucket_name="okube-unit-testing")
     event.to_aws_s3_bucket(bucket_name="okube-unit-testing", skip_if_exists=True)
 
 
-def test_to_databricks_mount():
-    # TODO: add tests
-    pass
-    # event.to_databricks_mount()
-
-
 if __name__ == "__main__":
-    test_dataeventheader()
-    test_dataeventheader_root()
+    test_dataevent_header()
+    test_dataevent_root()
     test_dataevent()
     test_model_dump()
     test_event_without_tstamp()
     test_to_azure_storage_container()
     test_to_aws_s3_bucket()
-    test_to_databricks_mount()
```

### Comparing `laktory-0.2.1/tests/test_datasources.py` & `laktory-0.3.0/tests/test_datasources.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from pyspark.sql import SparkSession
 import os
 import pandas as pd
 
-from laktory.models.datasources import EventDataSource
+from laktory.models.datasources import FileDataSource
+from laktory.models.datasources import MemoryDataSource
 from laktory.models.datasources import TableDataSource
 from laktory._testing import Paths
 from laktory._testing import spark
 
 paths = Paths(__file__)
 
 # DataFrame
@@ -18,92 +18,85 @@
         "c": [3, 0, 3],
         "n": [4, 0, 4],
     },
 )
 df0 = spark.createDataFrame(pdf)
 
 
-def test_event_data_source():
-    source = EventDataSource(
-        name="stock_price",
-        producer={"name": "yahoo_finance"},
-    )
-    assert (
-        source.event_root
-        == "/Volumes/dev/sources/landing/events/yahoo_finance/stock_price/"
+def test_file_data_source():
+    source = FileDataSource(
+        path="Volumes/sources/landing/events/yahoo_finance/stock_price"
     )
+
+    assert source.path == "Volumes/sources/landing/events/yahoo_finance/stock_price"
+    assert source.dataframe_type == "SPARK"
+    assert not source.as_stream
     assert not source.is_cdc
 
 
-def test_event_data_source_read():
-    source = EventDataSource(
-        name="stock_price",
-        producer={"name": "yahoo-finance"},
-        events_root=os.path.join(paths.data, "./events/"),
-        read_as_stream=False,
+def test_file_data_source_read():
+    source = FileDataSource(
+        path=os.path.join(paths.data, "./events/yahoo-finance/stock_price"),
+        as_stream=False,
     )
     df = source.read(spark)
     assert df.count() == 80
     assert df.columns == [
         "data",
         "description",
-        "event_root_",
         "name",
         "producer",
     ]
 
 
-def test_table_data_source(df0=df0):
-    source = TableDataSource(
-        mock_df=df0,
-        path="/Volumes/tables/stock_prices/",
+def test_memory_data_source(df0=df0):
+    source = MemoryDataSource(
+        df=df0,
         filter="b != 0",
         selects=["a", "b", "c"],
         renames={"a": "aa", "b": "bb", "c": "cc"},
         broadcast=True,
-        spark_chain={
-            "nodes": [
-                {
-                    "column": {"name": "chain"},
-                    "spark_func_name": "lit",
-                    "spark_func_args": ["chain"],
-                }
-            ]
-        },
     )
 
-    # Test paths
-    assert source.path == "/Volumes/tables/stock_prices/"
-    assert source.from_path
-    assert source.path_or_full_name == "/Volumes/tables/stock_prices/"
-
     # Test reader
     df = source.read(spark)
-    assert df.columns == ["aa", "bb", "cc", "chain"]
+    assert df.columns == ["aa", "bb", "cc"]
     assert df.count() == 2
-    assert df.toPandas()["chain"].tolist() == ["chain", "chain"]
+    # assert df.toPandas()["chain"].tolist() == ["chain", "chain"]
 
     # Select with rename
-    source = TableDataSource(
-        mock_df=df0,
-        path="/Volumes/tables/stock_prices/",
+    source = MemoryDataSource(
+        df=df0,
         selects={"x": "x1", "n": "n1"},
     )
     df = source.read(spark)
     assert df.columns == ["x1", "n1"]
     assert df.count() == 3
 
     # Drop
-    source = TableDataSource(
-        mock_df=df0,
-        path="/Volumes/tables/stock_prices/",
+    source = MemoryDataSource(
+        df=df0,
         drops=["b", "c", "n"],
     )
     df = source.read(spark)
+    df.show()
     assert df.columns == ["x", "a"]
     assert df.count() == 3
 
 
+def test_table_data_source():
+    source = TableDataSource(
+        catalog_name="dev",
+        schema_name="finance",
+        table_name="slv_stock_prices",
+    )
+
+    # Test meta
+    assert source.full_name == "dev.finance.slv_stock_prices"
+    assert source._id == "dev.finance.slv_stock_prices"
+
+
 if __name__ == "__main__":
-    test_event_data_source()
-    test_event_data_source_read()
+    test_file_data_source()
+    test_file_data_source_read()
+    test_memory_data_source()
     test_table_data_source()
```

### Comparing `laktory-0.2.1/tests/test_datetime.py` & `laktory-0.3.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/test_dbfsfile.py` & `laktory-0.3.0/tests/test_dbfsfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from laktory.models import DbfsFile
+from laktory.models.resources.databricks import DbfsFile
 
 dbfs_file = DbfsFile(
     source="./test_workspacefile.py",
     dirpath="/tmp/",
     access_controls=[{"permission_level": "CAN_READ", "group_name": "account users"}],
 )
```

### Comparing `laktory-0.2.1/tests/test_docstrings.py` & `laktory-0.3.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/test_job.py` & `laktory-0.3.0/tests/test_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from laktory.models import Job
+from laktory.models.resources.databricks import Job
 from laktory import pulumi_outputs
 
 job = Job(
     name="job-stock-prices",
     clusters=[
         {
             "name": "main",
@@ -18,15 +18,15 @@
             "notebook_task": {
                 "notebook_path": "job/ingest_stock_prices",
             },
             "task_key": "ingestion",
         },
         {
             "depends_ons": [{"task_key": "ingestion"}],
-            "pipeline_task": {"pipeline_id": "${resources.pl-stock-prices.id}"},
+            "pipeline_task": {"pipeline_id": "${resources.dlt-pl-stock-prices.id}"},
             "task_key": "pipeline",
         },
         {
             "task_key": "view",
             "sql_task": {
                 "query": {"query_id": "456"},
                 "warehouse_id": "123",
@@ -119,15 +119,15 @@
                 "job_cluster_key": None,
                 "libraries": None,
                 "max_retries": None,
                 "min_retry_interval_millis": None,
                 "notebook_task": None,
                 "notification_settings": None,
                 "pipeline_task": {
-                    "pipeline_id": "${resources.pl-stock-prices.id}",
+                    "pipeline_id": "${resources.dlt-pl-stock-prices.id}",
                     "full_refresh": None,
                 },
                 "retry_on_timeout": None,
                 "run_if": None,
                 "run_job_task": None,
                 "sql_task": None,
                 "task_key": "pipeline",
@@ -165,15 +165,15 @@
         "timeout_seconds": None,
         "trigger": None,
         "webhook_notifications": None,
     }
 
 
 def test_job_pulumi():
-    pulumi_outputs["pl-stock-prices.id"] = "12345"
+    pulumi_outputs["dlt-pl-stock-prices.id"] = "12345"
     assert job.resource_name == "job-stock-prices"
     assert job.options.model_dump(exclude_none=True) == {
         "depends_on": [],
         "delete_before_replace": True,
     }
     data = job.pulumi_properties
     print(data)
```

### Comparing `laktory-0.2.1/tests/test_metastore.py` & `laktory-0.3.0/tests/test_metastore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from laktory.models import Metastore
+from laktory.models.resources.databricks import Metastore
 
 
 metastore = Metastore(
     name="metastore-lakehouse",
     cloud="azure",
     storage_root="abfss://metastore@o3stglakehousedev.dfs.core.windows.net/",
     region="eastus",
```

### Comparing `laktory-0.2.1/tests/test_notebook.py` & `laktory-0.3.0/tests/test_notebook.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from laktory.models import Notebook
+from laktory.models.resources.databricks import Notebook
 
 nb = Notebook(
     source="./test_notebook.py",
     path="/laktory/hello",
 )
```

### Comparing `laktory-0.2.1/tests/test_parsers.py` & `laktory-0.3.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/test_schema.py` & `laktory-0.3.0/tests/test_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from laktory.models import Table
-from laktory.models import Schema
-from laktory.models import Column
+from laktory.models.resources.databricks import Table
+from laktory.models.resources.databricks import Schema
+from laktory.models.resources.databricks import Column
 
 schema = Schema(
     name="flights",
     catalog_name="laktory_testing",
     tables=[
         Table(
             name="f1549",
```

### Comparing `laktory-0.2.1/tests/test_settings.py` & `laktory-0.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/test_spark_chain.py` & `laktory-0.3.0/tests/test_spark_chain.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/test_spark_dataframe.py` & `laktory-0.3.0/tests/test_spark_dataframe.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/test_spark_functions.py` & `laktory-0.3.0/tests/test_spark_functions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.1/tests/test_sql_query.py` & `laktory-0.3.0/tests/test_sql_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from laktory.models import SqlQuery
+from laktory.models.resources.databricks import SqlQuery
 
 query = SqlQuery(
     name="google-prices",
     parent="/queries",
     query="SELECT * FROM dev.finance.slv_stock_prices",
     data_source_id="12345",
 )
```

### Comparing `laktory-0.2.1/tests/test_stack.py` & `laktory-0.3.0/tests/test_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,34 +38,36 @@
             },
             "prod": {
                 "variables": {
                     "env": "prod",
                     "is_dev": False,
                     "node_type_id": "Standard_DS4_v2",
                 },
-                "resources": {"pipelines": {"pl-custom-name": {"development": False}}},
+                "resources": {
+                    "pipelines": {"pl-custom-name": {"dlt": {"development": False}}}
+                },
             },
         },
         "name": "unit-testing",
         "organization": "okube",
         "pulumi": {
             "config": {
                 "databricks:host": "${vars.DATABRICKS_HOST}",
                 "databricks:token": "${vars.DATABRICKS_TOKEN}",
             },
             "outputs": {},
         },
         "resources": {
-            "dbfsfiles": {},
-            "catalogs": {},
-            "clusters": {},
-            "directories": {},
-            "externallocations": {},
-            "groups": {},
-            "jobs": {
+            "databricks_dbfsfiles": {},
+            "databricks_catalogs": {},
+            "databricks_clusters": {},
+            "databricks_directories": {},
+            "databricks_externallocations": {},
+            "databricks_groups": {},
+            "databricks_jobs": {
                 "job-stock-prices-ut-stack": {
                     "access_controls": [],
                     "clusters": [
                         {
                             "apply_policy_default_values": None,
                             "autoscale": None,
                             "autotermination_minutes": None,
@@ -165,15 +167,15 @@
                             "job_cluster_key": None,
                             "libraries": None,
                             "max_retries": None,
                             "min_retry_interval_millis": None,
                             "notebook_task": None,
                             "notification_settings": None,
                             "pipeline_task": {
-                                "pipeline_id": "${resources.pl-custom-name.id}",
+                                "pipeline_id": "${resources.dlt-custom-name.id}",
                                 "full_refresh": None,
                             },
                             "retry_on_timeout": None,
                             "run_if": None,
                             "run_job_task": None,
                             "sql_task": None,
                             "task_key": "run-pipeline",
@@ -181,63 +183,73 @@
                         },
                     ],
                     "timeout_seconds": None,
                     "trigger": None,
                     "webhook_notifications": None,
                 }
             },
-            "metastoredataaccesses": {},
-            "metastores": {},
-            "notebooks": {},
+            "databricks_metastoredataaccesses": {},
+            "databricks_metastores": {},
+            "databricks_notebooks": {},
+            "databricks_dltpipelines": {},
+            "databricks_schemas": {},
+            "databricks_secrets": {},
+            "databricks_secretscopes": {},
+            "databricks_serviceprincipals": {},
+            "databricks_sqlqueries": {},
+            "databricks_tables": {},
+            "databricks_users": {},
+            "databricks_volumes": {},
+            "databricks_warehouses": {},
+            "databricks_workspacefiles": {},
             "pipelines": {
                 "pl-custom-name": {
-                    "access_controls": [
-                        {
-                            "group_name": "account users",
-                            "permission_level": "CAN_VIEW",
-                            "service_principal_name": None,
-                            "user_name": None,
-                        },
-                        {
-                            "group_name": "role-engineers",
-                            "permission_level": "CAN_RUN",
-                            "service_principal_name": None,
-                            "user_name": None,
-                        },
-                    ],
-                    "allow_duplicate_names": None,
-                    "catalog": None,
-                    "channel": "PREVIEW",
-                    "clusters": [],
-                    "configuration": {},
-                    "continuous": None,
-                    "development": None,
-                    "edition": None,
-                    "libraries": [
-                        {
-                            "file": None,
-                            "notebook": {"path": "/pipelines/dlt_brz_template.py"},
-                        }
-                    ],
+                    "databricks_job": None,
+                    "dlt": {
+                        "access_controls": [
+                            {
+                                "group_name": "account users",
+                                "permission_level": "CAN_VIEW",
+                                "service_principal_name": None,
+                                "user_name": None,
+                            },
+                            {
+                                "group_name": "role-engineers",
+                                "permission_level": "CAN_RUN",
+                                "service_principal_name": None,
+                                "user_name": None,
+                            },
+                        ],
+                        "allow_duplicate_names": None,
+                        "catalog": None,
+                        "channel": "PREVIEW",
+                        "clusters": [],
+                        "configuration": {},
+                        "continuous": None,
+                        "development": None,
+                        "edition": None,
+                        "libraries": [
+                            {
+                                "file": None,
+                                "notebook": {"path": "/pipelines/dlt_brz_template.py"},
+                            }
+                        ],
+                        "name": "pl-stock-prices-ut-stack",
+                        "notifications": [],
+                        "photon": None,
+                        "serverless": None,
+                        "storage": None,
+                        "target": None,
+                    },
                     "name": "pl-stock-prices-ut-stack",
-                    "notifications": [],
-                    "photon": None,
-                    "serverless": None,
-                    "storage": None,
-                    "tables": [],
-                    "target": None,
+                    "nodes": [],
+                    "orchestrator": "DLT",
                     "udfs": [],
                 }
             },
-            "schemas": {},
-            "secrets": {},
-            "secretscopes": {},
-            "serviceprincipals": {},
-            "sqlqueries": {},
-            "tables": {},
             "providers": {
                 "databricks": {
                     "account_id": None,
                     "auth_type": None,
                     "azure_client_id": None,
                     "azure_client_secret": None,
                     "azure_environment": None,
@@ -263,18 +275,14 @@
                     "retry_timeout_seconds": None,
                     "skip_verify": None,
                     "token": "${vars.DATABRICKS_TOKEN}",
                     "username": None,
                     "warehouse_id": None,
                 }
             },
-            "users": {},
-            "volumes": {},
-            "warehouses": {},
-            "workspacefiles": {},
         },
         "terraform": {
             "backend": {
                 "azurerm": {
                     "resource_group_name": "o3-rg-laktory-dev",
                     "storage_account_name": "o3stglaktorydev",
                     "container_name": "unit-testing",
@@ -318,15 +326,15 @@
                             "jobClusterKey": "main",
                             "notebookTask": {
                                 "notebookPath": "/jobs/ingest_stock_metadata.py"
                             },
                             "taskKey": "ingest-metadata",
                         },
                         {
-                            "pipelineTask": {"pipelineId": "${pl-custom-name.id}"},
+                            "pipelineTask": {"pipelineId": "${dlt-custom-name.id}"},
                             "taskKey": "run-pipeline",
                         },
                     ],
                     "jobClusters": [
                         {
                             "jobClusterKey": "main",
                             "newCluster": {
@@ -342,15 +350,15 @@
                                 "sshPublicKeys": [],
                             },
                         }
                     ],
                 },
                 "options": {"dependsOn": [], "deleteBeforeReplace": True},
             },
-            "pl-custom-name": {
+            "dlt-custom-name": {
                 "type": "databricks:Pipeline",
                 "properties": {
                     "channel": "PREVIEW",
                     "clusters": [],
                     "configuration": {},
                     "libraries": [
                         {"notebook": {"path": "/pipelines/dlt_brz_template.py"}}
@@ -360,54 +368,48 @@
                 },
                 "options": {
                     "provider": "${databricks}",
                     "dependsOn": [],
                     "deleteBeforeReplace": True,
                 },
             },
-            "permissions-pl-custom-name": {
+            "permissions-dlt-custom-name": {
                 "type": "databricks:Permissions",
                 "properties": {
                     "accessControls": [
                         {"groupName": "account users", "permissionLevel": "CAN_VIEW"},
                         {"groupName": "role-engineers", "permissionLevel": "CAN_RUN"},
                     ],
-                    "pipelineId": "${pl-custom-name.id}",
+                    "pipelineId": "${dlt-custom-name.id}",
                 },
                 "options": {
                     "provider": "${databricks}",
-                    "dependsOn": ["${pl-custom-name}"],
+                    "dependsOn": ["${dlt-custom-name}"],
                     "deleteBeforeReplace": True,
                 },
             },
             "workspace-file-laktory-pipelines-pl-stock-prices-ut-stack-json": {
                 "type": "databricks:WorkspaceFile",
                 "properties": {
                     "path": "/.laktory/pipelines/pl-stock-prices-ut-stack.json",
                     "source": "./tmp-pl-stock-prices-ut-stack.json",
                 },
-                "options": {
-                    "provider": "${databricks}",
-                    "dependsOn": ["${pl-custom-name}"],
-                    "deleteBeforeReplace": True,
-                },
+                "options": {"dependsOn": [], "deleteBeforeReplace": True},
             },
             "permissions-workspace-file-laktory-pipelines-pl-stock-prices-ut-stack-json": {
                 "type": "databricks:Permissions",
                 "properties": {
                     "accessControls": [
                         {"groupName": "account users", "permissionLevel": "CAN_READ"}
                     ],
                     "workspaceFilePath": "/.laktory/pipelines/pl-stock-prices-ut-stack.json",
                 },
                 "options": {
-                    "provider": "${databricks}",
                     "dependsOn": [
-                        "${workspace-file-laktory-pipelines-pl-stock-prices-ut-stack-json}",
-                        "${pl-custom-name}",
+                        "${workspace-file-laktory-pipelines-pl-stock-prices-ut-stack-json}"
                     ],
                     "deleteBeforeReplace": True,
                 },
             },
             "databricks": {
                 "type": "pulumi:providers:databricks",
                 "properties": {
@@ -444,15 +446,15 @@
     data0["variables"]["is_dev"] = False
     data0["variables"]["node_type_id"] = "Standard_DS4_v2"
     cluster = data0["resources"]["job-stock-prices-ut-stack"]["properties"][
         "jobClusters"
     ][0]["newCluster"]
     cluster["nodeTypeId"] = "Standard_DS4_v2"
     cluster["sparkEnvVars"]["LAKTORY_WORKSPACE_ENV"] = "prod"
-    data0["resources"]["pl-custom-name"]["properties"]["development"] = False
+    data0["resources"]["dlt-custom-name"]["properties"]["development"] = False
     assert data == data0
 
 
 def test_pulumi_preview():
     pstack = stack.to_pulumi(env="dev")
     pstack.preview(stack="okube/dev")
 
@@ -497,15 +499,15 @@
                             "library": [
                                 {"pypi": {"package": "laktory==0.0.27"}},
                                 {"pypi": {"package": "yfinance"}},
                             ],
                         },
                         {
                             "pipeline_task": {
-                                "pipeline_id": "${databricks_pipeline.pl-custom-name.id}"
+                                "pipeline_id": "${databricks_pipeline.dlt-custom-name.id}"
                             },
                             "task_key": "run-pipeline",
                         },
                     ],
                     "job_cluster": [
                         {
                             "job_cluster_key": "main",
@@ -522,54 +524,50 @@
                                 "ssh_public_keys": [],
                             },
                         }
                     ],
                 }
             },
             "databricks_pipeline": {
-                "pl-custom-name": {
+                "dlt-custom-name": {
                     "channel": "PREVIEW",
                     "configuration": {},
                     "name": "pl-stock-prices-ut-stack",
                     "cluster": [],
                     "library": [
                         {"notebook": {"path": "/pipelines/dlt_brz_template.py"}}
                     ],
                     "notification": [],
                     "provider": "databricks",
                 }
             },
             "databricks_permissions": {
-                "permissions-pl-custom-name": {
-                    "pipeline_id": "${databricks_pipeline.pl-custom-name.id}",
+                "permissions-dlt-custom-name": {
+                    "pipeline_id": "${databricks_pipeline.dlt-custom-name.id}",
                     "access_control": [
                         {"group_name": "account users", "permission_level": "CAN_VIEW"},
                         {"group_name": "role-engineers", "permission_level": "CAN_RUN"},
                     ],
-                    "depends_on": ["databricks_pipeline.pl-custom-name"],
+                    "depends_on": ["databricks_pipeline.dlt-custom-name"],
                     "provider": "databricks",
                 },
                 "permissions-workspace-file-laktory-pipelines-pl-stock-prices-ut-stack-json": {
                     "workspace_file_path": "/.laktory/pipelines/pl-stock-prices-ut-stack.json",
                     "access_control": [
                         {"group_name": "account users", "permission_level": "CAN_READ"}
                     ],
                     "depends_on": [
-                        "databricks_workspace_file.workspace-file-laktory-pipelines-pl-stock-prices-ut-stack-json",
-                        "databricks_pipeline.pl-custom-name",
+                        "databricks_workspace_file.workspace-file-laktory-pipelines-pl-stock-prices-ut-stack-json"
                     ],
-                    "provider": "databricks",
                 },
             },
             "databricks_workspace_file": {
                 "workspace-file-laktory-pipelines-pl-stock-prices-ut-stack-json": {
                     "path": "/.laktory/pipelines/pl-stock-prices-ut-stack.json",
                     "source": "./tmp-pl-stock-prices-ut-stack.json",
-                    "depends_on": ["databricks_pipeline.pl-custom-name"],
-                    "provider": "databricks",
                 }
             },
         },
     }
 
     # Dev
     data = stack.to_terraform(env="dev").model_dump()
@@ -588,15 +586,15 @@
     data["provider"]["databricks"]["token"] = "***"
     data0 = copy.deepcopy(data_default)
     cluster = data0["resource"]["databricks_job"]["job-stock-prices-ut-stack"][
         "job_cluster"
     ][0]["new_cluster"]
     cluster["node_type_id"] = "Standard_DS4_v2"
     cluster["spark_env_vars"]["LAKTORY_WORKSPACE_ENV"] = "prod"
-    data0["resource"]["databricks_pipeline"]["pl-custom-name"]["development"] = False
+    data0["resource"]["databricks_pipeline"]["dlt-custom-name"]["development"] = False
     assert data == data0
 
 
 def test_terraform_plan():
     tstack = stack.to_terraform(env="dev")
     tstack.terraform.backend = (
         None  # TODO: Add credentials to git actions to use azure backend
@@ -605,15 +603,15 @@
     tstack.plan()
 
 
 def test_all_resources():
     from tests.test_catalog import catalog
     from tests.test_directory import directory
     from tests.test_job import job
-    from tests.test_pipeline import pl
+    from tests.test_pipeline import pl_dlt
     from tests.test_metastore import metastore
     from tests.test_notebook import nb
     from tests.test_schema import schema
     from tests.test_sql_query import query
     from tests.test_user import user
     from tests.test_user import group
     from tests.test_workspacefile import workspace_file
@@ -622,33 +620,39 @@
     paths = Paths(__file__)
 
     nb.source = os.path.join(paths.root, nb.source)
     workspace_file.source = os.path.join(paths.root, workspace_file.source)
 
     validator = StackValidator(
         resources={
-            "catalogs": [catalog],
-            "directories": [directory],
-            "jobs": [job],
-            "metastores": [metastore],
-            "pipelines": [pl],  # required by job
-            "notebooks": [nb],
-            "schemas": [schema],
-            "sqlqueries": [query],
-            "groups": [group],
-            "users": [user],
-            "workspacefiles": [workspace_file],
+            "databricks_catalogs": [catalog],
+            "databricks_directories": [directory],
+            "databricks_jobs": [job],
+            "databricks_metastores": [metastore],
+            "databricks_notebooks": [nb],
+            "databricks_schemas": [schema],
+            "databricks_sqlqueries": [query],
+            "databricks_groups": [group],
+            "databricks_users": [user],
+            "databricks_workspacefiles": [workspace_file],
+            "pipelines": [pl_dlt],  # required by job
         },
         providers={
             "provider-workspace-neptune": {
                 "host": "${vars.DATABRICKS_HOST}",
                 # "azure_client_id": "0",
                 # "azure_client_secret": "0",
                 # "azure_tenant_id": "0",
-            }
+            },
+            "databricks1": {
+                "host": "${vars.DATABRICKS_HOST}",
+            },
+            "databricks2": {
+                "host": "${vars.DATABRICKS_HOST}",
+            },
         },
     )
 
     validator.validate()
 
 
 if __name__ == "__main__":
```

### Comparing `laktory-0.2.1/tests/test_table_builder.py` & `laktory-0.3.0/tests/test_pipeline_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 import os
+import shutil
+
 from pyspark.sql import functions as F
 
 from laktory import models
 from laktory._testing import spark
 from laktory._testing import Paths
 
 paths = Paths(__file__)
 
 # Data
 df_brz = spark.read.parquet(os.path.join(paths.data, "./brz_stock_prices"))
 df_slv = spark.read.parquet(os.path.join(paths.data, "./slv_stock_prices"))
 
 
-def test_read_and_process():
-    builder = models.TableBuilder(
-        event_source={
-            "name": "brz_stock_prices",
+def test_execute():
+
+    sink_path = os.path.join(paths.tmp, "pl_node_sink")
+
+    node = models.PipelineNode(
+        name="slv_stock_prices",
+        source={
+            "table_name": "brz_stock_prices",
             "mock_df": df_brz,
         },
-        spark_chain={
+        transformer={
             "nodes": [
                 {
-                    "column": {
-                        "name": "created_at",
-                        "type": "timestamp",
-                    },
-                    "sql_expression": "data._created_at",
-                },
-                {
-                    "column": {"name": "symbol", "type": "string"},
-                    "sql_expression": "data.symbol",
+                    "column": {"name": "created_at", "type": "timestamp"},
+                    "sql_expression": "data.created_at",
                 },
                 {
-                    "column": {"name": "open", "type": "double"},
-                    "sql_expression": "data.open",
+                    "column": {"name": "symbol"},
+                    "spark_func_name": "coalesce",
+                    "spark_func_args": ["data.symbol"],
                 },
                 {
                     "column": {"name": "close", "type": "double"},
                     "sql_expression": "data.close",
                 },
                 {
                     "spark_func_name": "drop",
-                    "spark_func_args": [
-                        "description",
-                        "data",
-                        "producer",
-                    ],
+                    "spark_func_args": ["data", "producer", "name", "description"],
                 },
             ]
         },
+        sink={
+            "path": sink_path,
+            "format": "PARQUET",
+            "mode": "OVERWRITE",
+        },
     )
+    df0 = node.execute()
+    df1 = spark.read.format("PARQUET").load(sink_path)
 
-    # Read and process
-    df = builder.read_source(spark)
-    df = builder.process(df)
+    assert df1.columns == df0.columns
+    assert df1.columns == ["created_at", "symbol", "close"]
+    assert df1.count() == df_brz.count()
 
-    # Test
-    assert df.columns == ["name", "created_at", "symbol", "open", "close"]
-    assert df.count() == 80
+    # Cleanup
+    shutil.rmtree(sink_path)
 
 
 def test_bronze():
-    builder = models.TableBuilder(
+    node = models.PipelineNode(
         layer="BRONZE",
-        event_source={
-            "name": "brz_stock_prices",
+        name="slv_stock_prices",
+        source={
+            "table_name": "brz_stock_prices",
             "mock_df": df_brz,
         },
-        spark_chain={
+        transformer={
             "nodes": [
                 {
                     "column": {"name": "symbol", "type": "string"},
                     "sql_expression": "data.symbol",
                 },
             ]
         },
     )
 
     # Read and process
-    df = builder.read_source(spark)
-    df = builder.process(df)
+    df = node.execute(spark)
 
     # Test
-    assert not builder.drop_source_columns
-    assert not builder.drop_duplicates
-    assert builder.layer == "BRONZE"
-    assert builder.template == "BRONZE"
-    assert builder.add_laktory_columns
+    assert not node.drop_source_columns
+    assert not node.drop_duplicates
+    assert node.layer == "BRONZE"
+    assert node.add_layer_columns
     assert df.columns == [
         "name",
         "description",
         "producer",
         "data",
         "symbol",
         "_bronze_at",
@@ -99,91 +100,91 @@
 
 
 def test_silver():
     df = df_brz.select(df_brz.columns)
     df = df.withColumn("_bronze_at", F.current_timestamp())
     df = df.union(df)
 
-    builder = models.TableBuilder(
+    node = models.PipelineNode(
         layer="SILVER",
-        table_source={
-            "name": "slv_stock_prices",
+        source={
+            "table_name": "slv_stock_prices",
             "mock_df": df,
         },
-        spark_chain={
+        transformer={
             "nodes": [
                 {
                     "column": {"name": "symbol", "type": "string"},
                     "sql_expression": "data.symbol",
                 },
             ]
         },
         drop_duplicates=True,
     )
 
     # Read and process
-    df = builder.read_source(spark)
-    df = builder.process(df)
+    df = node.execute(spark)
 
     # Test
-    assert builder.drop_source_columns
-    assert builder.drop_duplicates
-    assert builder.layer == "SILVER"
-    assert builder.template == "SILVER"
-    assert builder.add_laktory_columns
+    assert node.drop_source_columns
+    assert node.drop_duplicates
+    assert node.layer == "SILVER"
+    assert node.add_layer_columns
     assert df.columns == ["_bronze_at", "symbol", "_silver_at"]
     assert df.count() == 80
 
 
 def test_cdc():
-    table = models.Table(
-        name="brz_users_type1",
-        builder={
-            "table_source": {
-                "name": "brz_users_cdc",
-                "cdc": {
-                    "primary_keys": ["userId"],
-                    "sequence_by": "sequenceNum",
-                    "apply_as_deletes": "operation = 'DELETE'",
-                    "scd_type": 1,
-                    "except_columns": ["operation", "sequenceNum"],
-                },
+    node = models.PipelineNode(
+        source={
+            "table_name": "brz_users_type1",
+            "cdc": {
+                "primary_keys": ["userId"],
+                "sequence_by": "sequenceNum",
+                "apply_as_deletes": "operation = 'DELETE'",
+                "scd_type": 1,
+                "except_columns": ["operation", "sequenceNum"],
             },
         },
     )
 
-    assert table.builder.apply_changes_kwargs == {
-        "apply_as_deletes": "operation = 'DELETE'",
-        "apply_as_truncates": None,
-        "column_list": [],
-        "except_column_list": ["operation", "sequenceNum"],
-        "ignore_null_updates": None,
-        "keys": ["userId"],
-        "sequence_by": "sequenceNum",
-        "source": "brz_users_cdc",
-        "stored_as_scd_type": 1,
-        "target": "brz_users_type1",
-        "track_history_column_list": None,
-        "track_history_except_column_list": None,
-    }
-    assert table.builder.is_from_cdc
-
-    # TODO: Run test with demo data
-    # from pyspark.sql import SparkSession
-
-    # spark = SparkSession.builder.appName("UnitTesting").getOrCreate()
-    #
-    # df_cdc = spark.createDataFrame(pd.DataFrame({
-    #     "userId": [124, 123, 125, 126, 123, 125, 125, 123],
-    #     "name": ["Raul", "Isabel", "Mercedes", "Lily", None, "Mercedes", "Mercedes", "Isabel"],
-    #     "city": ["Oaxaca", "Monterrey", "Tijuana", "Cancun", None, "Guadalajara", "Mexicali", "Chihuahua"],
-    #     "operation": ["INSERT", "INSERT", "INSERT", "INSERT", "DELETE", "UPDATE", "UPDATE", "UPDATE"],
-    #     "sequenceNum": [1, 1, 2, 2, 6, 6, 5, 5],
-    # }))
-    # df_cdc.show()
+    # TODO: Test CDC transformations when ready
+    print(node)
+
+
+#
+#     assert table.builder.apply_changes_kwargs == {
+#         "apply_as_deletes": "operation = 'DELETE'",
+#         "apply_as_truncates": None,
+#         "column_list": [],
+#         "except_column_list": ["operation", "sequenceNum"],
+#         "ignore_null_updates": None,
+#         "keys": ["userId"],
+#         "sequence_by": "sequenceNum",
+#         "source": "brz_users_cdc",
+#         "stored_as_scd_type": 1,
+#         "target": "brz_users_type1",
+#         "track_history_column_list": None,
+#         "track_history_except_column_list": None,
+#     }
+#     assert table.builder.is_from_cdc
+#
+#     # TODO: Run test with demo data
+#     # from pyspark.sql import SparkSession
+#
+#     # spark = SparkSession.builder.appName("UnitTesting").getOrCreate()
+#     #
+#     # df_cdc = spark.createDataFrame(pd.DataFrame({
+#     #     "userId": [124, 123, 125, 126, 123, 125, 125, 123],
+#     #     "name": ["Raul", "Isabel", "Mercedes", "Lily", None, "Mercedes", "Mercedes", "Isabel"],
+#     #     "city": ["Oaxaca", "Monterrey", "Tijuana", "Cancun", None, "Guadalajara", "Mexicali", "Chihuahua"],
+#     #     "operation": ["INSERT", "INSERT", "INSERT", "INSERT", "DELETE", "UPDATE", "UPDATE", "UPDATE"],
+#     #     "sequenceNum": [1, 1, 2, 2, 6, 6, 5, 5],
+#     # }))
+#     # df_cdc.show()
 
 
 if __name__ == "__main__":
-    test_read_and_process()
+    test_execute()
     test_bronze()
     test_silver()
     test_cdc()
```

### Comparing `laktory-0.2.1/tests/test_workspacefile.py` & `laktory-0.3.0/tests/test_workspacefile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from laktory.models import WorkspaceFile
+from laktory.models.resources.databricks import WorkspaceFile
 
 workspace_file = WorkspaceFile(
     source="./test_workspacefile.py",
     dirpath="/init_scripts/",
     access_controls=[{"permission_level": "CAN_READ", "group_name": "account users"}],
 )
```

