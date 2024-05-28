# Comparing `tmp/buildgrid-0.0.95.tar.gz` & `tmp/buildgrid-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildgrid-0.0.95.tar", last modified: Thu May 16 13:10:20 2024, max compression
+gzip compressed data, was "buildgrid-0.0.96.tar", last modified: Tue May 28 15:29:20 2024, max compression
```

## Comparing `buildgrid-0.0.95.tar` & `buildgrid-0.0.96.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.624997 buildgrid-0.0.95/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-16 13:09:51.000000 buildgrid-0.0.95/BuildGrid.doap
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-05-16 13:09:51.000000 buildgrid-0.0.95/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    11338 2024-05-16 13:09:51.000000 buildgrid-0.0.95/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-16 13:09:51.000000 buildgrid-0.0.95/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7030 2024-05-16 13:10:20.624997 buildgrid-0.0.95/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2932 2024-05-16 13:09:51.000000 buildgrid-0.0.95/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.521998 buildgrid-0.0.95/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.523998 buildgrid-0.0.95/buildgrid/_app/
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5675 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.525998 buildgrid-0.0.95/buildgrid/_app/commands/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_browser_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10608 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_cas.py
--rw-rw-rw-   0 root         (0) root         (0)     8817 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)    12570 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_janitor.py
--rw-rw-rw-   0 root         (0) root         (0)     4842 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_logstream.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_operation.py
--rw-rw-rw-   0 root         (0) root         (0)     8166 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_server.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/rpc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.526998 buildgrid-0.0.95/buildgrid/_app/settings/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   110867 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     8691 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/reference.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.527998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.528998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/with-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.528998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/clients/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/clients/asset-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.528998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/connections/
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/connections/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/connections/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.529998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/misc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/misc/channel.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.529998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/scheduler/memory.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3907 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/scheduler/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.531998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      971 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/bots.yaml
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/bytestream.yaml
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/cas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/execution.yaml
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/platform-queues.yml
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.534998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/disk.yaml
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/lru.yaml
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/redis-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/remote.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/replicated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      592 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/s3.yaml
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/sharded.yaml
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/sql-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/sql.yaml
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/with-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4776 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.534998 buildgrid-0.0.95/buildgrid/_protos/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.535998 buildgrid-0.0.95/buildgrid/_protos/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.535998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.535998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.535998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.537998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7795 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    27103 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    15404 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.537998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.539998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30140 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   136470 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    47588 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    47884 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.540998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.541998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7844 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.543998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.545998 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4156 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.545998 buildgrid-0.0.95/buildgrid/_protos/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.549998 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3824 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9955 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2881 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.549998 buildgrid-0.0.95/buildgrid/_protos/google/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.555998 buildgrid-0.0.95/buildgrid/_protos/google/api/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2291 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18246 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.556998 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7478 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     8880 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     8996 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.557998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.557998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.561998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5933 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18014 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2545 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5408 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6758 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.562998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.568998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    23457 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7140 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7256 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6133 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    21890 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5337 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9321 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4498 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2751 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.569998 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5084 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7984 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7133 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.574998 buildgrid-0.0.95/buildgrid/_protos/google/rpc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    13407 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4774 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1573 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_types.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.575998 buildgrid-0.0.95/buildgrid/browser/
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/browser/app.py
--rw-rw-rw-   0 root         (0) root         (0)    34436 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/browser/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/browser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.575998 buildgrid-0.0.95/buildgrid/cleanup/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.576998 buildgrid-0.0.95/buildgrid/cleanup/janitor/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3318 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/index.py
--rw-rw-rw-   0 root         (0) root         (0)     5829 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1403 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.579998 buildgrid-0.0.95/buildgrid/client/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5099 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/auth_token_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/authentication.py
--rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    41408 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/cas.py
--rw-rw-rw-   0 root         (0) root         (0)    13926 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/interceptors.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/logstream.py
--rw-rw-rw-   0 root         (0) root         (0)     3410 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/retrier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.582998 buildgrid-0.0.95/buildgrid/server/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.582998 buildgrid-0.0.95/buildgrid/server/actioncache/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.584998 buildgrid-0.0.95/buildgrid/server/actioncache/caches/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5564 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/action_cache_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     5593 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4197 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6534 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/redis_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6573 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/remote_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    11662 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/s3_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/write_once_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.585998 buildgrid-0.0.95/buildgrid/server/auth/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.586998 buildgrid-0.0.95/buildgrid/server/bots/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/bots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11156 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/bots/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7343 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/bots/job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)     5647 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/bots/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.587998 buildgrid-0.0.95/buildgrid/server/build_events/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/build_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/build_events/service.py
--rw-rw-rw-   0 root         (0) root         (0)     7213 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/build_events/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.588997 buildgrid-0.0.95/buildgrid/server/capabilities/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/capabilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7113 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/capabilities/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     3342 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/capabilities/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.588997 buildgrid-0.0.95/buildgrid/server/cas/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21766 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/instance.py
--rw-rw-rw-   0 root         (0) root         (0)    12330 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.591997 buildgrid-0.0.95/buildgrid/server/cas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.592998 buildgrid-0.0.95/buildgrid/server/cas/storage/index/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/index_abc.py
--rw-rw-rw-   0 root         (0) root         (0)    13464 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/redis.py
--rw-rw-rw-   0 root         (0) root         (0)    38579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.593998 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/lru_memory_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/remote.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/replicated.py
--rw-rw-rw-   0 root         (0) root         (0)    14426 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     6002 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/sharded.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/size_differentiated.py
--rw-rw-rw-   0 root         (0) root         (0)     9519 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     8154 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/storage_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     7796 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/context.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.594998 buildgrid-0.0.95/buildgrid/server/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9599 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/execution/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7517 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/execution/service.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/job_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    18608 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/metrics_names.py
--rw-rw-rw-   0 root         (0) root         (0)    14482 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19548 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.594998 buildgrid-0.0.95/buildgrid/server/operations/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.596998 buildgrid-0.0.95/buildgrid/server/operations/filtering/
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/filter_grammar.lark
--rw-rw-rw-   0 root         (0) root         (0)     5769 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/interpreter.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/sanitizer.py
--rw-rw-rw-   0 root         (0) root         (0)     4802 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.596998 buildgrid-0.0.95/buildgrid/server/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.597998 buildgrid-0.0.95/buildgrid/server/persistence/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.598997 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/README
--rw-rw-rw-   0 root         (0) root         (0)     2919 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/env.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.602998 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
--rw-rw-rw-   0 root         (0) root         (0)     4625 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
--rw-rw-rw-   0 root         (0) root         (0)    79716 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/impl.py
--rw-rw-rw-   0 root         (0) root         (0)     8915 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/notifier.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.603998 buildgrid-0.0.95/buildgrid/server/redis/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/redis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6197 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/redis/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/request_metadata_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.603998 buildgrid-0.0.95/buildgrid/server/s3/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/s3/s3utils.py
--rw-rw-rw-   0 root         (0) root         (0)    30687 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/server.py
--rw-rw-rw-   0 root         (0) root         (0)     6126 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/servicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.604997 buildgrid-0.0.95/buildgrid/server/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/sql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22200 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/sql/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/sql/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.605998 buildgrid-0.0.95/buildgrid/server/utils/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/utils/async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/utils/context.py
--rw-rw-rw-   0 root         (0) root         (0)    10885 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/utils/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5450 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    12244 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.617998 buildgrid-0.0.95/buildgrid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7030 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21169 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1233 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.516998 buildgrid-0.0.95/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.609998 buildgrid-0.0.95/data/config/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/all-in-one.yml
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/artifacts.yml
--rwxrwxrwx   0 root         (0) root         (0)     1351 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/basic-with-disk.yml
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/bots-interface.yml
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/default.yml
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/index-sqlite-no-execution.yml
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/index-sqlite.yml
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/logstream.yml
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/monitoring-controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/multi-layer-storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/redis-cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/s3-indexed-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/storage-redis.yml
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/storage-s3.yml
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/with-metering.yml
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/with-pgbouncer.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.609998 buildgrid-0.0.95/docs/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.609998 buildgrid-0.0.95/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.611997 buildgrid-0.0.95/docs/source/data/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/basic-disk-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/bazel-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/buildstream-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/cas-and-ac.yml
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/cas-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/execution-and-bots.yml
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/sqlite-index-cas-only.yml
--rw-rw-rw-   0 root         (0) root         (0)     1425 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5463 2024-05-16 13:09:52.000000 buildgrid-0.0.95/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-16 13:10:20.625998 buildgrid-0.0.95/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      643 2024-05-16 13:09:52.000000 buildgrid-0.0.95/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.613998 buildgrid-0.0.95/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.517998 buildgrid-0.0.95/tests/auth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.616998 buildgrid-0.0.95/tests/auth/data/
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/auth.yaml
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwks-valid.json
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-conflicting.secret
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-matching.secret
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-conflicting.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-jwk-encrypted.token
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-matching.priv.key
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-matching.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)     3829 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15407 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_execution_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     2199 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)    12358 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_multithreaded_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_request_metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32384 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    10567 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.743185 buildgrid-0.0.96/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-28 15:28:48.000000 buildgrid-0.0.96/BuildGrid.doap
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-05-28 15:28:48.000000 buildgrid-0.0.96/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11338 2024-05-28 15:28:48.000000 buildgrid-0.0.96/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-28 15:28:48.000000 buildgrid-0.0.96/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7030 2024-05-28 15:29:20.743185 buildgrid-0.0.96/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2024-05-28 15:28:48.000000 buildgrid-0.0.96/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.632186 buildgrid-0.0.96/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.634186 buildgrid-0.0.96/buildgrid/_app/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5675 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.637186 buildgrid-0.0.96/buildgrid/_app/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_browser_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10608 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_cas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8817 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)    12570 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_janitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_operation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8166 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/rpc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.638186 buildgrid-0.0.96/buildgrid/_app/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   110867 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     8691 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/reference.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.638186 buildgrid-0.0.96/buildgrid/_app/settings/schemas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.639186 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/with-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.640185 buildgrid-0.0.96/buildgrid/_app/settings/schemas/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/clients/asset-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.640185 buildgrid-0.0.96/buildgrid/_app/settings/schemas/connections/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/connections/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/connections/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.641186 buildgrid-0.0.96/buildgrid/_app/settings/schemas/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/misc/channel.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.641186 buildgrid-0.0.96/buildgrid/_app/settings/schemas/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/scheduler/memory.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/scheduler/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.643185 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      971 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/bots.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/bytestream.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/cas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/execution.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/platform-queues.yml
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.646185 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/disk.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/lru.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/redis-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/remote.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/replicated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/s3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/sharded.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/sql-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/sql.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/with-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.646185 buildgrid-0.0.96/buildgrid/_protos/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.647186 buildgrid-0.0.96/buildgrid/_protos/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.647186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.647186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.647186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.649186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7795 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    27103 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15404 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.650185 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.652186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30140 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   136470 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    47588 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    47884 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.652186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.654186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7844 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.656185 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.657186 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.658186 buildgrid-0.0.96/buildgrid/_protos/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.662186 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9955 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.662186 buildgrid-0.0.96/buildgrid/_protos/google/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.668186 buildgrid-0.0.96/buildgrid/_protos/google/api/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18246 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.670185 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7478 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     8880 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     8996 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.670185 buildgrid-0.0.96/buildgrid/_protos/google/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.671186 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.675186 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18014 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6758 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.675186 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.681186 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    23457 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7140 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7256 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21890 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9321 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.683185 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7133 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.688186 buildgrid-0.0.96/buildgrid/_protos/google/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    13407 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.689185 buildgrid-0.0.96/buildgrid/browser/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/browser/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    34436 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/browser/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/browser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.690185 buildgrid-0.0.96/buildgrid/cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.691186 buildgrid-0.0.96/buildgrid/cleanup/janitor/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3318 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     5829 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.694186 buildgrid-0.0.96/buildgrid/client/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5099 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4457 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/auth_token_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/authentication.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    41408 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/cas.py
+-rw-rw-rw-   0 root         (0) root         (0)    13926 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/interceptors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3410 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/retrier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.697185 buildgrid-0.0.96/buildgrid/server/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.697185 buildgrid-0.0.96/buildgrid/server/actioncache/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.700185 buildgrid-0.0.96/buildgrid/server/actioncache/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8125 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/action_cache_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5605 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6546 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/redis_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6573 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/remote_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    11674 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/s3_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/write_once_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3703 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.701186 buildgrid-0.0.96/buildgrid/server/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.702185 buildgrid-0.0.96/buildgrid/server/bots/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/bots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11230 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/bots/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7343 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/bots/job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)     5647 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/bots/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.702185 buildgrid-0.0.96/buildgrid/server/build_events/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/build_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/build_events/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7213 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/build_events/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.703185 buildgrid-0.0.96/buildgrid/server/capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/capabilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7113 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/capabilities/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     3342 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/capabilities/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.704186 buildgrid-0.0.96/buildgrid/server/cas/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21156 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)    12330 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.707185 buildgrid-0.0.96/buildgrid/server/cas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.708186 buildgrid-0.0.96/buildgrid/server/cas/storage/index/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/index_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13464 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)    38579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.709185 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/lru_memory_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/remote.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/replicated.py
+-rw-rw-rw-   0 root         (0) root         (0)    14426 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6056 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/sharded.py
+-rw-rw-rw-   0 root         (0) root         (0)     7039 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/size_differentiated.py
+-rw-rw-rw-   0 root         (0) root         (0)     9519 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     9510 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/storage_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7850 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.709185 buildgrid-0.0.96/buildgrid/server/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9678 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/execution/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7517 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/execution/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/job_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    18608 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/metrics_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    14482 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19548 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.710185 buildgrid-0.0.96/buildgrid/server/operations/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.712185 buildgrid-0.0.96/buildgrid/server/operations/filtering/
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/filter_grammar.lark
+-rw-rw-rw-   0 root         (0) root         (0)     5769 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/interpreter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/sanitizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.712185 buildgrid-0.0.96/buildgrid/server/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.713185 buildgrid-0.0.96/buildgrid/server/persistence/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.714186 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/README
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.719185 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
+-rw-rw-rw-   0 root         (0) root         (0)     4625 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    79760 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     8915 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.719185 buildgrid-0.0.96/buildgrid/server/redis/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/redis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/redis/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/request_metadata_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.720185 buildgrid-0.0.96/buildgrid/server/s3/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/s3/s3utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31657 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     6126 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/servicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.720185 buildgrid-0.0.96/buildgrid/server/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/sql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22200 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/sql/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/sql/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4806 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.721186 buildgrid-0.0.96/buildgrid/server/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/utils/async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/utils/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    10885 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/utils/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12244 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.735185 buildgrid-0.0.96/buildgrid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7030 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21169 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.627186 buildgrid-0.0.96/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.726185 buildgrid-0.0.96/data/config/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/all-in-one.yml
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/artifacts.yml
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/basic-with-disk.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/bots-interface.yml
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/default.yml
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/index-sqlite-no-execution.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/index-sqlite.yml
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/logstream.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/monitoring-controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/multi-layer-storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/redis-cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/s3-indexed-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/storage-redis.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/storage-s3.yml
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/with-metering.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/with-pgbouncer.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.727185 buildgrid-0.0.96/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.727185 buildgrid-0.0.96/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.729185 buildgrid-0.0.96/docs/source/data/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/basic-disk-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/bazel-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/buildstream-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/cas-and-ac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/cas-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/execution-and-bots.yml
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/sqlite-index-cas-only.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5463 2024-05-28 15:28:48.000000 buildgrid-0.0.96/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-28 15:29:20.744186 buildgrid-0.0.96/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      643 2024-05-28 15:28:48.000000 buildgrid-0.0.96/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.731186 buildgrid-0.0.96/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.628186 buildgrid-0.0.96/tests/auth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.735185 buildgrid-0.0.96/tests/auth/data/
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/auth.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwks-valid.json
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-conflicting.secret
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-matching.secret
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-conflicting.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-jwk-encrypted.token
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-matching.priv.key
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-matching.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)     3829 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15407 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_execution_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_multithreaded_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_request_metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32384 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    10567 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_utils.py
```

### Comparing `buildgrid-0.0.95/BuildGrid.doap` & `buildgrid-0.0.96/BuildGrid.doap`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/CONTRIBUTING.rst` & `buildgrid-0.0.96/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/LICENSE` & `buildgrid-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/PKG-INFO` & `buildgrid-0.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.95
+Version: 0.0.96
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `buildgrid-0.0.95/README.rst` & `buildgrid-0.0.96/README.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/__init__.py` & `buildgrid-0.0.96/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/__init__.py` & `buildgrid-0.0.96/buildgrid/_app/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/cli.py` & `buildgrid-0.0.96/buildgrid/_app/cli.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/__init__.py` & `buildgrid-0.0.96/buildgrid/_app/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_actioncache.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_browser_backend.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_browser_backend.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_capabilities.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_cas.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_cleanup.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_execute.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_execute.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_janitor.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_janitor.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_logstream.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_operation.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_operation.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/cmd_server.py` & `buildgrid-0.0.96/buildgrid/_app/commands/cmd_server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/commands/rpc_utils.py` & `buildgrid-0.0.96/buildgrid/_app/commands/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/__init__.py` & `buildgrid-0.0.96/buildgrid/_app/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/parser.py` & `buildgrid-0.0.96/buildgrid/_app/settings/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/reference.yml` & `buildgrid-0.0.96/buildgrid/_app/settings/reference.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/config.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/config.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/connections/sql.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/connections/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/misc/channel.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/misc/channel.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/scheduler/sql.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/scheduler/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/action-cache.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/bots.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/bots.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/execution.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/execution.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/remote.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/remote.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/s3.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/s3.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/sql-index.yaml` & `buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/sql-index.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_enums.py` & `buildgrid-0.0.96/buildgrid/_enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_exceptions.py` & `buildgrid-0.0.96/buildgrid/_exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py` & `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py` & `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/__init__.py` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2.py` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi` & `buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_types.py` & `buildgrid-0.0.96/buildgrid/_types.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/_version.py` & `buildgrid-0.0.96/buildgrid/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.0.95"
+__version__ = "0.0.96"
```

### Comparing `buildgrid-0.0.95/buildgrid/browser/__init__.py` & `buildgrid-0.0.96/buildgrid/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/browser/app.py` & `buildgrid-0.0.96/buildgrid/browser/app.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/browser/rest_api.py` & `buildgrid-0.0.96/buildgrid/browser/rest_api.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/browser/utils.py` & `buildgrid-0.0.96/buildgrid/browser/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/cleanup/__init__.py` & `buildgrid-0.0.96/buildgrid/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/cleanup/cleanup.py` & `buildgrid-0.0.96/buildgrid/cleanup/cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/cleanup/janitor/__init__.py` & `buildgrid-0.0.96/buildgrid/cleanup/janitor/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/cleanup/janitor/config.py` & `buildgrid-0.0.96/buildgrid/cleanup/janitor/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/cleanup/janitor/index.py` & `buildgrid-0.0.96/buildgrid/cleanup/janitor/index.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/cleanup/janitor/s3.py` & `buildgrid-0.0.96/buildgrid/cleanup/janitor/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/cleanup/janitor/utils.py` & `buildgrid-0.0.96/buildgrid/cleanup/janitor/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/__init__.py` & `buildgrid-0.0.96/buildgrid/client/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/actioncache.py` & `buildgrid-0.0.96/buildgrid/client/actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/asset.py` & `buildgrid-0.0.96/buildgrid/client/asset.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import logging
 from datetime import datetime
 from typing import Any, Iterable, Mapping, Optional
 
 import grpc
 from google.protobuf.timestamp_pb2 import Timestamp
 
 import buildgrid.server.context as context_module
@@ -26,14 +27,16 @@
     PushDirectoryResponse,
     Qualifier,
 )
 from buildgrid._protos.build.bazel.remote.asset.v1.remote_asset_pb2_grpc import FetchStub, PushStub
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import Digest
 from buildgrid.client.retrier import GrpcRetrier
 
+LOGGER = logging.getLogger(__name__)
+
 
 class AssetClient:
     """Client for Fetch and Push services defined in remote_asset protocol"""
 
     def __init__(
         self,
         channel: grpc.Channel,
@@ -49,14 +52,15 @@
         self._retrier = GrpcRetrier(retries=retries, max_backoff=max_backoff, should_backoff=should_backoff)
 
     def __enter__(self) -> "AssetClient":
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self._channel.close()
+        LOGGER.info("Stopped AssetClient")
 
     def push_blob(
         self,
         *,
         uris: Iterable[str],
         qualifiers: Mapping[str, str],
         blob_digest: Digest,
```

### Comparing `buildgrid-0.0.95/buildgrid/client/auth_token_loader.py` & `buildgrid-0.0.96/buildgrid/client/auth_token_loader.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/authentication.py` & `buildgrid-0.0.96/buildgrid/client/authentication.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/capabilities.py` & `buildgrid-0.0.96/buildgrid/client/capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/cas.py` & `buildgrid-0.0.96/buildgrid/client/cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/channel.py` & `buildgrid-0.0.96/buildgrid/client/channel.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/interceptors.py` & `buildgrid-0.0.96/buildgrid/client/interceptors.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/logstream.py` & `buildgrid-0.0.96/buildgrid/client/logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/client/retrier.py` & `buildgrid-0.0.96/buildgrid/client/retrier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/__init__.py` & `buildgrid-0.0.96/buildgrid/server/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/__init__.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/caches/__init__.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/caches/action_cache_abc.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/caches/lru_cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,135 +9,128 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import collections
 import logging
-from abc import ABC, abstractmethod
-from typing import Any, Optional, TypeVar
+from typing import Tuple
 
-from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import DESCRIPTOR as RE_DESCRIPTOR
-from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import (
-    ActionResult,
-    Digest,
-    DigestFunction,
-    Directory,
-    Tree,
-)
-from buildgrid.server.cas.instance import EMPTY_BLOB_DIGEST
+from buildgrid._exceptions import NotFoundError
+from buildgrid._protos.build.bazel.remote.execution.v2 import remote_execution_pb2
+from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import ActionResult, Digest
+from buildgrid.server.actioncache.caches.action_cache_abc import ActionCacheABC
 from buildgrid.server.cas.storage.storage_abc import StorageABC
-from buildgrid.server.servicer import Instance
-from buildgrid.utils import get_hash_type
+from buildgrid.server.metrics_names import AC_UNUSABLE_CACHE_HITS_METRIC_NAME
+from buildgrid.server.metrics_utils import publish_counter_metric
 
 LOGGER = logging.getLogger(__name__)
 
 
-T = TypeVar("T", bound="ActionCacheABC")
+class LruActionCache(ActionCacheABC):
+    """In-memory Action Cache implementation with LRU eviction.
 
+    This cache has a configurable fixed size, evicting the least recently
+    accessed entry when adding a new entry would exceed the fixed size. The
+    cache is entirely stored in memory so its contents are lost on restart.
+
+    This type of cache is ideal for use cases that need a simple and fast
+    cache, with no requirements for longevity of the cache content. It is not
+    recommended to use this type of cache in situations where you may wish to
+    obtain cached results a reasonable time in the future, due to its fixed
+    size.
+
+    """
+
+    def __init__(
+        self, storage: StorageABC, max_cached_refs: int, allow_updates: bool = True, cache_failed_actions: bool = True
+    ):
+        """Initialise a new in-memory LRU Action Cache.
 
-class ActionCacheABC(Instance, ABC):
-    SERVICE_NAME = RE_DESCRIPTOR.services_by_name["ActionCache"].full_name
+        Args:
+            storage (StorageABC): Storage backend instance to be used.
+            max_cached_refs (int): Maximum number of entries to store in the cache.
+            allow_updates (bool): Whether to allow writing to the cache. If false,
+                this is a read-only cache for all clients.
+            cache_failed_actions (bool): Whether or not to cache Actions with
+                non-zero exit codes.
 
-    def __init__(self, allow_updates: bool = False, storage: Optional[StorageABC] = None):
-        self._allow_updates = allow_updates
-        self._storage = storage
+        """
+        super().__init__(storage=storage)
 
-    @property
-    def allow_updates(self) -> bool:
-        return self._allow_updates
-
-    def hash_type(self) -> "DigestFunction.Value.ValueType":
-        return get_hash_type()
-
-    def __enter__(self: T) -> T:
-        self.start()
-        return self
-
-    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
-        self.stop()
-
-    def start(self) -> None:
-        if self._storage is not None:
-            self._storage.start()
-
-    def stop(self) -> None:
-        if self._storage is not None:
-            self._storage.stop()
-
-    # NOTE: This method exists for compatibility reasons. Ideally it should never
-    # be used with an up-to-date configuration.
-    def set_instance_name(self, instance_name: str) -> None:
-        LOGGER.warning(
-            "Cache instances should be defined in a 'caches' list and passed "
-            "to an ActionCache service, rather than defined in the 'services' "
-            "list themselves."
-        )
-        super().set_instance_name(instance_name)
+        self._cache_failed_actions = cache_failed_actions
+        self._storage = storage
+        self._allow_updates = allow_updates
+        self._max_cached_refs = max_cached_refs
+        self._digest_map = collections.OrderedDict()  # type: ignore
 
-    @abstractmethod
     def get_action_result(self, action_digest: Digest) -> ActionResult:
-        raise NotImplementedError()
+        """Retrieves the cached result for an Action.
+
+        If there is no cached result found, returns None.
+
+        Args:
+            action_digest (Digest): The digest of the Action to retrieve the
+                cached result of.
+
+        """
+        key = self._get_key(action_digest)
+        if key in self._digest_map:
+            assert self._storage, "Storage used before initialization"
+            action_result = self._storage.get_message(self._digest_map[key], remote_execution_pb2.ActionResult)
+
+            if action_result is not None:
+                if self._referenced_blobs_still_exist(action_digest, action_result):
+                    self._digest_map.move_to_end(key)
+                    return action_result
+
+                publish_counter_metric(AC_UNUSABLE_CACHE_HITS_METRIC_NAME, 1, {"instance-name": self._instance_name})
+
+                if self._allow_updates:
+                    LOGGER.debug(
+                        f"Removing {action_digest.hash}/{action_digest.size_bytes}"
+                        "from cache due to missing blobs in CAS"
+                    )
+                    del self._digest_map[key]
+
+        raise NotFoundError(f"Key not found: {key}")
 
-    @abstractmethod
     def update_action_result(self, action_digest: Digest, action_result: ActionResult) -> None:
-        raise NotImplementedError()
+        """Stores a result for an Action in the cache.
+
+        If the result has a non-zero exit code and `cache_failed_actions` is False
+        for this cache, the result is not cached.
+
+        Args:
+            action_digest (Digest): The digest of the Action whose result is
+                being cached.
+            action_result (ActionResult): The result to cache for the given
+                Action digest.
+
+        """
+        if self._cache_failed_actions or action_result.exit_code == 0:
+            key = self._get_key(action_digest)
+            if not self._allow_updates:
+                raise NotImplementedError("Updating cache not allowed")
+
+            if self._max_cached_refs == 0:
+                return
+
+            while len(self._digest_map) >= self._max_cached_refs:
+                self._digest_map.popitem(last=False)
+
+            assert self._storage, "Storage used before initialization"
+            result_digest = self._storage.put_message(action_result)
+            self._digest_map[key] = result_digest
+
+            LOGGER.info(f"Result cached for action [{action_digest.hash}/{action_digest.size_bytes}]")
 
-    def _action_result_blobs_still_exist(self, action_result: ActionResult) -> bool:
-        """Checks CAS for ActionResult output blobs existence.
+    def _get_key(self, action_digest: Digest) -> Tuple[str, int]:
+        """Get a hashable cache key from a given Action digest.
 
         Args:
-            action_result (ActionResult): ActionResult to search referenced
-            output blobs for.
+            action_digest (Digest): The digest to produce a cache key for.
 
-        Returns:
-            True if all referenced blobs are present in CAS, False otherwise.
         """
-        if not self._storage:
-            return True
-        blobs_needed = []
-
-        for output_file in action_result.output_files:
-            blobs_needed.append(output_file.digest)
-
-        for output_directory in action_result.output_directories:
-            if output_directory.HasField("tree_digest"):
-                blobs_needed.append(output_directory.tree_digest)
-                tree = self._storage.get_message(output_directory.tree_digest, Tree)
-                if tree is None:
-                    return False
-
-                for file_node in tree.root.files:
-                    blobs_needed.append(file_node.digest)
-
-                for child in tree.children:
-                    for file_node in child.files:
-                        blobs_needed.append(file_node.digest)
-            elif output_directory.HasField("root_directory_digest"):
-                # GetTree would be more efficient but that is not part of StorageABC
-                queue = [output_directory.root_directory_digest]
-                while queue:
-                    directory_blobs = self._storage.bulk_read_blobs(queue)
-                    if len(directory_blobs) < len(queue):
-                        # At least one directory is missing
-                        return False
-
-                    directories = [Directory.FromString(b) for b in directory_blobs.values()]
-                    blobs_needed.extend([file_node.digest for d in directories for file_node in d.files])
-                    queue = [subdir.digest for d in directories for subdir in d.directories]
-
-        if action_result.stdout_digest.hash and not action_result.stdout_raw:
-            blobs_needed.append(action_result.stdout_digest)
-
-        if action_result.stderr_digest.hash and not action_result.stderr_raw:
-            blobs_needed.append(action_result.stderr_digest)
-
-        # No need to check the underlying storage for the empty blob as it is a special case blob which always exists
-        # It is possible that the empty blob is not actually present in the underlying storage
-        blobs_to_check = [blob for blob in blobs_needed if blob != EMPTY_BLOB_DIGEST]
-
-        missing = self._storage.missing_blobs(blobs_to_check)
-        if len(missing) != 0:
-            LOGGER.debug(f"Missing {len(missing)}/{len(blobs_needed)} blobs")
-            return False
-        return True
+        return (action_digest.hash, action_digest.size_bytes)
```

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/caches/mirrored_cache.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/caches/mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/caches/redis_cache.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/caches/redis_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self._migrate_entries = migrate_entries
 
     @redis_client_exception_wrapper
     def get_action_result(self, action_digest: Digest) -> ActionResult:
         key = self._get_key(action_digest)
         action_result = self._get_action_result(key, action_digest)
         if action_result is not None:
-            if self._action_result_blobs_still_exist(action_result):
+            if self._referenced_blobs_still_exist(action_digest, action_result):
                 return action_result
 
             publish_counter_metric(AC_UNUSABLE_CACHE_HITS_METRIC_NAME, 1, {"instance_name": self._instance_name})
 
             if self._allow_updates:
                 LOGGER.debug(
                     f"Removing {action_digest.hash}/{action_digest.size_bytes}"
```

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/caches/remote_cache.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/caches/remote_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/caches/s3_cache.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/caches/s3_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
         Returns:
             The cached ActionResult matching the given key or raises
             NotFoundError.
         """
         action_result = self._get_action_result(action_digest)
         if action_result is not None:
-            if self._action_result_blobs_still_exist(action_result):
+            if self._referenced_blobs_still_exist(action_digest, action_result):
                 return action_result
 
             publish_counter_metric(AC_UNUSABLE_CACHE_HITS_METRIC_NAME, 1, {"instance_name": self._instance_name})
 
             if self._allow_updates:
                 LOGGER.debug(
                     f"Removing {action_digest.hash}/{action_digest.size_bytes} "
```

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/caches/with_cache.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/caches/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/caches/write_once_cache.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/caches/write_once_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/instance.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     # --- Public API ---
 
     def start(self) -> None:
         self._cache.start()
 
     def stop(self) -> None:
         self._cache.stop()
+        LOGGER.info(f"Stopped ActionCache instance for '{self._instance_name}")
 
     @property
     def allow_updates(self) -> bool:
         return self._cache.allow_updates
 
     def hash_type(self) -> "DigestFunction.Value.ValueType":
         return get_hash_type()
```

### Comparing `buildgrid-0.0.95/buildgrid/server/actioncache/service.py` & `buildgrid-0.0.96/buildgrid/server/actioncache/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/auth/__init__.py` & `buildgrid-0.0.96/buildgrid/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/auth/config.py` & `buildgrid-0.0.96/buildgrid/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/auth/enums.py` & `buildgrid-0.0.96/buildgrid/server/auth/enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/auth/exceptions.py` & `buildgrid-0.0.96/buildgrid/server/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/auth/manager.py` & `buildgrid-0.0.96/buildgrid/server/auth/manager.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/bots/__init__.py` & `buildgrid-0.0.96/buildgrid/server/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/bots/instance.py` & `buildgrid-0.0.96/buildgrid/server/bots/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     def start(self) -> None:
         self._stack.enter_context(self.scheduler)
         self._stack.enter_context(self._job_assigner)
         self._stack.enter_context(self.reaper)
 
     def stop(self) -> None:
         self._stack.close()
+        LOGGER.info(f"Stopped Bots instance for '{self._instance_name}'")
 
     def set_instance_name(self, instance_name: str) -> None:
         super().set_instance_name(instance_name)
         self.scheduler.set_instance_name(instance_name)
 
     create_bot_session_ignored_exceptions = (RetriableError,)
```

### Comparing `buildgrid-0.0.95/buildgrid/server/bots/job_assigner.py` & `buildgrid-0.0.96/buildgrid/server/bots/job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/bots/service.py` & `buildgrid-0.0.96/buildgrid/server/bots/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/build_events/__init__.py` & `buildgrid-0.0.96/buildgrid/server/build_events/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/build_events/service.py` & `buildgrid-0.0.96/buildgrid/server/build_events/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/build_events/storage.py` & `buildgrid-0.0.96/buildgrid/server/build_events/storage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/capabilities/__init__.py` & `buildgrid-0.0.96/buildgrid/server/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/capabilities/instance.py` & `buildgrid-0.0.96/buildgrid/server/capabilities/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/capabilities/service.py` & `buildgrid-0.0.96/buildgrid/server/capabilities/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/__init__.py` & `buildgrid-0.0.96/buildgrid/server/cas/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/instance.py` & `buildgrid-0.0.96/buildgrid/server/cas/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
         self._storage.set_instance_name(instance_name)
 
     def start(self) -> None:
         self._storage.start()
 
     def stop(self) -> None:
         self._storage.stop()
+        LOGGER.info(f"Stopped CAS instance for '{self._instance_name}'")
 
     def hash_type(self) -> "DigestFunction.Value.ValueType":
         return self._storage.hash_type()
 
     def max_batch_total_size_bytes(self) -> int:
         return self._storage.max_batch_total_size_bytes()
 
@@ -322,41 +323,28 @@
             directories.extend(tree.children)
             yield from (
                 GetTreeResponse(directories=directories[start : start + request.page_size])
                 for start in range(0, len(directories), request.page_size)
             )
             return
 
+        results = []
         with Counter(metric_name=CAS_DOWNLOADED_BYTES_METRIC_NAME, instance_name=self._instance_name) as bytes_counter:
-            # From the spec, a NotFound response only occurs if the root directory is missing.
-            root_directory = storage.get_message(request.root_digest, Directory)
-            if not root_directory:
-                raise NotFoundError(
-                    f"Root digest not found: {request.root_digest.hash}/{request.root_digest.size_bytes}"
-                )
+            response = GetTreeResponse()
+            for dir in storage.get_tree(request.root_digest):
+                bytes_counter.increment(sum(directory.digest.size_bytes for directory in dir.directories))
+                response.directories.append(dir)
+                results.append(dir)
+                if len(response.directories) >= request.page_size:
+                    yield response
+                    response.Clear()
 
             bytes_counter.increment(request.root_digest.size_bytes)
-
-            results = [root_directory]
-            offset = 0
-            queue = [subdir.digest for subdir in root_directory.directories]
-            while queue:
-                bytes_counter.increment(sum(d.size_bytes for d in queue))
-                blobs = storage.bulk_read_blobs(queue)
-
-                directories = [Directory.FromString(b) for b in blobs.values()]
-                queue = [subdir.digest for d in directories for subdir in d.directories]
-
-                results.extend(directories)
-                while len(results) - offset >= request.page_size:
-                    yield GetTreeResponse(directories=results[offset : offset + request.page_size])
-                    offset += request.page_size
-
-            if len(results) - offset > 0:
-                yield GetTreeResponse(directories=results[offset:])
+            if response.directories:
+                yield response
             if results:
                 self.put_tree_cache(request.root_digest, results[0], results[1:])
 
 
 class ByteStreamInstance(Instance):
     SERVICE_NAME = bs_pb2.DESCRIPTOR.services_by_name["ByteStream"].full_name
```

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/service.py` & `buildgrid-0.0.96/buildgrid/server/cas/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/__init__.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/disk.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/disk.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/index/__init__.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/index/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/index/index_abc.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/index/index_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/index/redis.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/index/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/lru_memory_cache.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/lru_memory_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/redis.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/remote.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/remote.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/replicated.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/replicated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/s3.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/sharded.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/sharded.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         if self._threadpool:
             self._stack.enter_context(self._threadpool)
         for storage in self._storages.values():
             self._stack.enter_context(storage)
 
     def stop(self) -> None:
         self._stack.close()
+        LOGGER.info(f"Stopped {type(self).__name__}")
 
     def _storage_from_digest(self, digest: Digest) -> StorageABC:
         def _score(shard_name: str, digest: Digest) -> int:
             hash = mmh3.hash(f"{shard_name}\t{digest.hash}", signed=False)
             return hash
 
         shard_name = min(self._storages.keys(), key=lambda name: _score(name, digest))
```

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/size_differentiated.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/size_differentiated.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
         if self._threadpool:
             self._stack.enter_context(self._threadpool)
         for storage_tuple in self._storages:
             self._stack.enter_context(storage_tuple.storage)
 
     def stop(self) -> None:
         self._stack.close()
+        LOGGER.info(f"Stopped {type(self).__name__}")
 
     def has_blob(self, digest: Digest) -> bool:
         LOGGER.debug(f"Checking for blob: [{digest}]")
         storage = self._storage_from_digest(digest)
         return storage.has_blob(digest)
 
     def get_blob(self, digest: Digest) -> Optional[IO[bytes]]:
```

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/sql.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/storage_abc.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/storage_abc.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 The abstract base class for storage providers.
 """
 
 import abc
 import io
 import logging
 from tempfile import TemporaryFile
-from typing import IO, Any, Dict, List, Optional, Tuple, Type, TypeVar
+from typing import IO, Any, Dict, Iterator, List, Optional, Tuple, Type, TypeVar
 
+from buildgrid._exceptions import NotFoundError
 from buildgrid._protos.build.bazel.remote.execution.v2 import remote_execution_pb2
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import (
     CacheCapabilities,
     Digest,
+    Directory,
     SymlinkAbsolutePathStrategy,
 )
 from buildgrid._protos.google.rpc import code_pb2
 from buildgrid._protos.google.rpc.status_pb2 import Status
 from buildgrid._types import MessageType
 from buildgrid.settings import HASH, MAX_IN_MEMORY_BLOB_SIZE_BYTES, MAX_REQUEST_SIZE
 from buildgrid.utils import get_hash_type
@@ -67,15 +69,15 @@
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.stop()
 
     def start(self) -> None:
         pass
 
     def stop(self) -> None:
-        pass
+        LOGGER.info(f"Stopped {type(self).__name__}")
 
     @abc.abstractmethod
     def has_blob(self, digest: Digest) -> bool:
         """Return True if the blob with the given instance/digest exists."""
         raise NotImplementedError()
 
     @abc.abstractmethod
@@ -181,14 +183,39 @@
         if message_blob is None:
             return None
         try:
             return message_type.FromString(message_blob.read())
         finally:
             message_blob.close()
 
+    def get_tree(self, root_digest: Digest, raise_on_missing_subdir: bool = False) -> Iterator[Directory]:
+        # From the spec, a NotFound response only occurs if the root directory is missing.
+        root_directory = self.get_message(root_digest, Directory)
+        if root_directory is None:
+            raise NotFoundError(f"Root digest not found: {root_digest.hash}/{root_digest.size_bytes}")
+        yield root_directory
+
+        queue = [subdir.digest for subdir in root_directory.directories]
+        while queue:
+            blobs = self.bulk_read_blobs(queue)
+
+            # GetTree allows for missing subtrees, but knowing some digests
+            # are missing without scanning the result on the caller side
+            # makes certain usages more efficient
+            if raise_on_missing_subdir and len(blobs) < len(queue):
+                raise NotFoundError(
+                    f"Missing entries under root directory: {root_digest.hash}/{root_digest.size_bytes}"
+                )
+
+            directories = [Directory.FromString(b) for b in blobs.values()]
+            queue = [subdir.digest for d in directories for subdir in d.directories]
+
+            if len(directories) > 0:
+                yield from directories
+
     @property
     def instance_name(self) -> Optional[str]:
         if hasattr(self, "_instance_name"):
             return self._instance_name
         return None
 
     def set_instance_name(self, instance_name: str) -> None:
```

### Comparing `buildgrid-0.0.95/buildgrid/server/cas/storage/with_cache.py` & `buildgrid-0.0.96/buildgrid/server/cas/storage/with_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         if self._defer_fallback_writes:
             self._stack.enter_context(self._executor)
         self._stack.enter_context(self._cache)
         self._stack.enter_context(self._fallback)
 
     def stop(self) -> None:
         self._stack.close()
+        LOGGER.info(f"Stopped {type(self).__name__}")
 
     def has_blob(self, digest: Digest) -> bool:
         try:
             if self._defer_fallback_writes and self._cache.has_blob(digest):
                 return True
         except Exception:
             LOGGER.warning(f"Failed to check existence of [{digest}] in cache storage", exc_info=True)
```

### Comparing `buildgrid-0.0.95/buildgrid/server/context.py` & `buildgrid-0.0.96/buildgrid/server/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/controller.py` & `buildgrid-0.0.96/buildgrid/server/controller.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/execution/__init__.py` & `buildgrid-0.0.96/buildgrid/server/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/execution/instance.py` & `buildgrid-0.0.96/buildgrid/server/execution/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
     def start(self) -> None:
         self.scheduler.start(start_job_watcher=True)
         self._stack.callback(self.scheduler.stop)
 
     def stop(self) -> None:
         self._stack.close()
+        LOGGER.info(f"Stopped Execution instance for '{self._instance_name}'")
 
     def set_instance_name(self, instance_name: str) -> None:
         super().set_instance_name(instance_name)
         self.scheduler.set_instance_name(instance_name)
 
     def hash_type(self) -> "DigestFunction.Value.ValueType":
         return get_hash_type()
```

### Comparing `buildgrid-0.0.95/buildgrid/server/execution/service.py` & `buildgrid-0.0.96/buildgrid/server/execution/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/job_metrics.py` & `buildgrid-0.0.96/buildgrid/server/job_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/metrics_names.py` & `buildgrid-0.0.96/buildgrid/server/metrics_names.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/metrics_utils.py` & `buildgrid-0.0.96/buildgrid/server/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/monitoring.py` & `buildgrid-0.0.96/buildgrid/server/monitoring.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/__init__.py` & `buildgrid-0.0.96/buildgrid/server/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/filtering/__init__.py` & `buildgrid-0.0.96/buildgrid/server/operations/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/filtering/filter.py` & `buildgrid-0.0.96/buildgrid/server/operations/filtering/filter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/filtering/filter_grammar.lark` & `buildgrid-0.0.96/buildgrid/server/operations/filtering/filter_grammar.lark`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/filtering/interpreter.py` & `buildgrid-0.0.96/buildgrid/server/operations/filtering/interpreter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/filtering/parser.py` & `buildgrid-0.0.96/buildgrid/server/operations/filtering/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/filtering/sanitizer.py` & `buildgrid-0.0.96/buildgrid/server/operations/filtering/sanitizer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/instance.py` & `buildgrid-0.0.96/buildgrid/server/operations/instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 """
 OperationsInstance
 ==================
 An instance of the LongRunningOperations Service.
 """
+import logging
 from typing import Dict, Optional, Tuple
 
 from buildgrid._exceptions import InvalidArgumentError, NotFoundError, RetriableError
 from buildgrid._protos.google.longrunning.operations_pb2 import DESCRIPTOR as OPS_DESCRIPTOR
 from buildgrid._protos.google.longrunning.operations_pb2 import ListOperationsResponse, Operation
 from buildgrid.server.metrics_names import (
     OPERATIONS_CANCEL_OPERATION_EXCEPTION_COUNT_METRIC_NAME,
@@ -33,14 +34,16 @@
 )
 from buildgrid.server.metrics_utils import DurationMetric, ExceptionCounter
 from buildgrid.server.operations.filtering import DEFAULT_OPERATION_FILTERS, FilterParser
 from buildgrid.server.persistence.sql.impl import SQLDataStore
 from buildgrid.server.servicer import Instance
 from buildgrid.settings import DEFAULT_MAX_LIST_OPERATION_PAGE_SIZE
 
+LOGGER = logging.getLogger(__name__)
+
 
 class OperationsInstance(Instance):
     SERVICE_NAME = OPS_DESCRIPTOR.services_by_name["Operations"].full_name
 
     def __init__(
         self, scheduler: SQLDataStore, max_list_operations_page_size: int = DEFAULT_MAX_LIST_OPERATION_PAGE_SIZE
     ) -> None:
@@ -50,14 +53,15 @@
     # --- Public API ---
 
     def start(self) -> None:
         self.scheduler.start()
 
     def stop(self) -> None:
         self.scheduler.stop()
+        LOGGER.info(f"Stopped Operations instance for '{self._instance_name}'")
 
     get_operation_ignored_exceptions = (RetriableError,)
 
     @DurationMetric(OPERATIONS_GET_OPERATION_TIME_METRIC_NAME, instanced=True)
     @ExceptionCounter(
         OPERATIONS_GET_OPERATION_EXCEPTION_COUNT_METRIC_NAME,
         ignored_exceptions=get_operation_ignored_exceptions,
```

### Comparing `buildgrid-0.0.95/buildgrid/server/operations/service.py` & `buildgrid-0.0.96/buildgrid/server/operations/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/__init__.py` & `buildgrid-0.0.96/buildgrid/server/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/__init__.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/env.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/env.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/script.py.mako` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/impl.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
 
         if start_job_watcher:
             self._stack.enter_context(self.execution_timer)
             self._stack.enter_context(self.ops_notifier)
 
     def stop(self) -> None:
         self._stack.close()
+        LOGGER.info("Stopped SQLDataStore")
 
     def set_instance_name(self, instance_name: str) -> None:
         self._instance_name = instance_name
 
     def _job_in_instance(self) -> ClauseElement:
         return or_(JobEntry.instance_name == self._instance_name, JobEntry.instance_name.is_(None))
```

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/models.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/models.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/notifier.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/notifier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/persistence/sql/utils.py` & `buildgrid-0.0.96/buildgrid/server/persistence/sql/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/redis/__init__.py` & `buildgrid-0.0.96/buildgrid/server/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/redis/provider.py` & `buildgrid-0.0.96/buildgrid/server/redis/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/request_metadata_utils.py` & `buildgrid-0.0.96/buildgrid/server/request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/s3/__init__.py` & `buildgrid-0.0.96/buildgrid/server/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/s3/s3utils.py` & `buildgrid-0.0.96/buildgrid/server/s3/s3utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/server.py` & `buildgrid-0.0.96/buildgrid/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 import sys
 import threading
 import time
 import traceback
 from collections import defaultdict
 from contextlib import ExitStack
 from datetime import datetime
-from multiprocessing import Queue
-from queue import Empty
+from queue import Empty, Queue
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
 import grpc
 from grpc_reflection.v1alpha import reflection
 
 from buildgrid._enums import BotStatus, LeaseState, LogRecordLevel, MetricCategories, OperationStage
 from buildgrid._exceptions import PermissionDeniedError
@@ -481,14 +480,15 @@
             reflection.enable_server_reflection([reflection.SERVICE_NAME] + reflection_services, grpc_server)
         else:
             LOGGER.info("Server reflection is not enabled.")
 
         return grpc_server
 
     def stop(self, *args: Any, **kwargs: Any) -> None:
+        LOGGER.info("Stopping BuildGrid server")
         self._stack.close()
 
     def _logging_worker(self, shutdown_requested: threading.Event) -> None:
         """Publishes log records to the monitoring bus."""
 
         logging_formatter = logging.Formatter(fmt=LOG_RECORD_FORMAT)
         logging_handler = logging.handlers.QueueHandler(self._logging_queue)
@@ -555,14 +555,35 @@
                     sys.stdout.write("Exception in logging worker\n")
                     sys.stdout.flush()
                     traceback.print_exc()
                 except Exception:
                     # There's not a lot we can do at this point really.
                     pass
 
+        if shutdown_requested.is_set():
+            # Reset logging, so any logging after shutting down the logging worker
+            # still gets written to stdout and the queue doesn't get any more logs
+            stream_handler = logging.StreamHandler(stream=sys.stdout)
+            stream_handler.setFormatter(logging_formatter)
+            root_logger = logging.getLogger()
+
+            for log_filter in root_logger.filters[:]:
+                stream_handler.addFilter(log_filter)
+                root_logger.removeFilter(log_filter)
+
+            for log_handler in root_logger.handlers[:]:
+                for log_filter in log_handler.filters[:]:
+                    stream_handler.addFilter(log_filter)
+                root_logger.removeHandler(log_handler)
+            root_logger.addHandler(stream_handler)
+
+            # Drain the log message queue
+            while self._logging_queue.qsize() > 0:
+                logging_worker()
+
     def _forge_log_record(
         self,
         *,
         domain: str,
         level: LogRecordLevel,
         message: str,
         creation_time: datetime,
```

### Comparing `buildgrid-0.0.95/buildgrid/server/servicer.py` & `buildgrid-0.0.96/buildgrid/server/servicer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/sql/__init__.py` & `buildgrid-0.0.96/buildgrid/server/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/sql/provider.py` & `buildgrid-0.0.96/buildgrid/server/sql/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/sql/sqlutils.py` & `buildgrid-0.0.96/buildgrid/server/sql/sqlutils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/threading.py` & `buildgrid-0.0.96/buildgrid/server/threading.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import contextvars
+import logging
 import threading
 from concurrent import futures
 from concurrent.futures import Future
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional, Tuple, TypeVar
 
 _T = TypeVar("_T")
 
 if TYPE_CHECKING:
     from typing_extensions import ParamSpec
 
     _P = ParamSpec("_P")
 
 
+LOGGER = logging.getLogger(__name__)
+
+
 class ContextThreadPoolExecutor(futures.ThreadPoolExecutor):
     def __init__(
         self,
         max_workers: Optional[int] = None,
         thread_name_prefix: str = "",
         initializer: Optional[Callable[[], Any]] = None,
         initargs: "Tuple[Any, ...]" = (),
@@ -121,16 +125,19 @@
         if not self._thread:
             self._thread = ContextThread(
                 target=lambda: self._target(self._shutdown_requested), name=self._name, daemon=True
             )
             self._thread.start()
 
     def stop(self) -> None:
-        self._shutdown_requested.set()
-        if self._on_shutdown_requested:
-            self._on_shutdown_requested()
-        if self._thread:
-            self._thread.join()
+        if not self._shutdown_requested.is_set():
+            LOGGER.info(f"Stopping {self._name} worker")
+            self._shutdown_requested.set()
+            if self._on_shutdown_requested:
+                self._on_shutdown_requested()
+            if self._thread:
+                self._thread.join()
+            LOGGER.info(f"Stopped {self._name} worker")
 
     def wait(self, timeout: Optional[float] = None) -> None:
         if self._thread:
             self._thread.join(timeout=timeout)
```

### Comparing `buildgrid-0.0.95/buildgrid/server/utils/__init__.py` & `buildgrid-0.0.96/buildgrid/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/utils/async_lru_cache.py` & `buildgrid-0.0.96/buildgrid/server/utils/async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/utils/context.py` & `buildgrid-0.0.96/buildgrid/server/utils/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/server/utils/decorators.py` & `buildgrid-0.0.96/buildgrid/server/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/settings.py` & `buildgrid-0.0.96/buildgrid/settings.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid/utils.py` & `buildgrid-0.0.96/buildgrid/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid.egg-info/PKG-INFO` & `buildgrid-0.0.96/buildgrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.95
+Version: 0.0.96
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `buildgrid-0.0.95/buildgrid.egg-info/SOURCES.txt` & `buildgrid-0.0.96/buildgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/buildgrid.egg-info/requires.txt` & `buildgrid-0.0.96/buildgrid.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/all-in-one.yml` & `buildgrid-0.0.96/data/config/all-in-one.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/artifacts.yml` & `buildgrid-0.0.96/data/config/artifacts.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/basic-with-disk.yml` & `buildgrid-0.0.96/data/config/basic-with-disk.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/bots-interface.yml` & `buildgrid-0.0.96/data/config/bots-interface.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/cache.yml` & `buildgrid-0.0.96/data/config/cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/controller.yml` & `buildgrid-0.0.96/data/config/controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/default.yml` & `buildgrid-0.0.96/data/config/default.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/index-sqlite-no-execution.yml` & `buildgrid-0.0.96/data/config/index-sqlite-no-execution.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/index-sqlite.yml` & `buildgrid-0.0.96/data/config/index-sqlite.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/monitoring-controller.yml` & `buildgrid-0.0.96/data/config/monitoring-controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/multi-layer-storage.yml` & `buildgrid-0.0.96/data/config/multi-layer-storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/redis-cache.yml` & `buildgrid-0.0.96/data/config/redis-cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/s3-indexed-cas.yml` & `buildgrid-0.0.96/data/config/s3-indexed-cas.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/storage-redis.yml` & `buildgrid-0.0.96/data/config/storage-redis.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/storage-s3.yml` & `buildgrid-0.0.96/data/config/storage-s3.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/storage.yml` & `buildgrid-0.0.96/data/config/storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/with-metering.yml` & `buildgrid-0.0.96/data/config/with-metering.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/data/config/with-pgbouncer.yml` & `buildgrid-0.0.96/data/config/with-pgbouncer.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/docs/Makefile` & `buildgrid-0.0.96/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/docs/source/data/execution-and-bots.yml` & `buildgrid-0.0.96/docs/source/data/execution-and-bots.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/docs/source/data/sqlite-index-cas-only.yml` & `buildgrid-0.0.96/docs/source/data/sqlite-index-cas-only.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/docs/source/index.rst` & `buildgrid-0.0.96/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/pyproject.toml` & `buildgrid-0.0.96/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "setuptools >= 44",
     "wheel >= 0.35",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "buildgrid"
-version = "0.0.95"
+version = "0.0.96"
 requires-python = ">=3.8"
 description = "A remote execution service"
 readme = "README.rst"
 license = {text = "Apache License, Version 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `buildgrid-0.0.95/setup.cfg` & `buildgrid-0.0.96/setup.cfg`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/setup.py` & `buildgrid-0.0.96/setup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/auth/data/auth.yaml` & `buildgrid-0.0.96/tests/auth/data/auth.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/auth/data/jwt-rs256-jwk-encrypted.token` & `buildgrid-0.0.96/tests/auth/data/jwt-rs256-jwk-encrypted.token`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/auth/data/jwt-rs256-matching.priv.key` & `buildgrid-0.0.96/tests/auth/data/jwt-rs256-matching.priv.key`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_async_lru_cache.py` & `buildgrid-0.0.96/tests/test_async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_execution_instance.py` & `buildgrid-0.0.96/tests/test_execution_instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_job_assigner.py` & `buildgrid-0.0.96/tests/test_job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_metrics_utils.py` & `buildgrid-0.0.96/tests/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_mirrored_cache.py` & `buildgrid-0.0.96/tests/test_mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_multithreaded_metrics.py` & `buildgrid-0.0.96/tests/test_multithreaded_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_parser.py` & `buildgrid-0.0.96/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_request_metadata_utils.py` & `buildgrid-0.0.96/tests/test_request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_scheduler.py` & `buildgrid-0.0.96/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.95/tests/test_utils.py` & `buildgrid-0.0.96/tests/test_utils.py`

 * *Files identical despite different names*

