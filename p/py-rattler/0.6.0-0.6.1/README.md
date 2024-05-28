# Comparing `tmp/py_rattler-0.6.0.tar.gz` & `tmp/py_rattler-0.6.1.tar.gz`

## Comparing `py_rattler-0.6.0.tar` & `py_rattler-0.6.1.tar`

### file list

```diff
@@ -1,493 +1,493 @@
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/Cargo.toml
--rw-r--r--   0     1001      127     1011 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/CHANGELOG.md
--rw-r--r--   0     1001      127     1394 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/build.rs
--rw-r--r--   0     1001      127    77341 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/src/lib.rs
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/Cargo.toml
--rw-r--r--   0     1001      127     4106 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/CHANGELOG.md
--rw-r--r--   0     1001      127     2053 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/fs.rs
--rw-r--r--   0     1001      127     2392 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/lib.rs
--rw-r--r--   0     1001      127     3671 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/read.rs
--rw-r--r--   0     1001      127       98 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/reqwest/mod.rs
--rw-r--r--   0     1001      127     6148 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs
--rw-r--r--   0     1001      127     4387 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/seek.rs
--rw-r--r--   0     1001      127     1732 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs
--rw-r--r--   0     1001      127     3101 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/fs.rs
--rw-r--r--   0     1001      127      113 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/mod.rs
--rw-r--r--   0     1001      127    14225 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/write.rs
--rw-r--r--   0     1001      127     9266 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/tests/extract.rs
--rw-r--r--   0     1001      127     7864 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/tests/write.rs
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/Cargo.toml
--rw-r--r--   0     1001      127     3679 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/CHANGELOG.md
--rw-r--r--   0     1001      127     8878 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/builder.rs
--rw-r--r--   0     1001      127      871 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/channel.rs
--rw-r--r--   0     1001      127     5792 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/conda.rs
--rw-r--r--   0     1001      127     2006 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/file_format_version.rs
--rw-r--r--   0     1001      127     4879 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/hash.rs
--rw-r--r--   0     1001      127    24726 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/lib.rs
--rw-r--r--   0     1001      127     6083 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/deserialize.rs
--rw-r--r--   0     1001      127     2613 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/mod.rs
--rw-r--r--   0     1001      127     9114 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/serialize.rs
--rw-r--r--   0     1001      127     8630 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/v3.rs
--rw-r--r--   0     1001      127     5293 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/pypi.rs
--rw-r--r--   0     1001      127     1480 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/pypi_indexes.rs
--rw-r--r--   0     1001      127    15803 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap
--rw-r--r--   0     1001      127    22538 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap
--rw-r--r--   0     1001      127   487177 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap
--rw-r--r--   0     1001      127    40002 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap
--rw-r--r--   0     1001      127    52187 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap
--rw-r--r--   0     1001      127  1811359 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap
--rw-r--r--   0     1001      127   487177 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap
--rw-r--r--   0     1001      127    19608 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap
--rw-r--r--   0     1001      127    40002 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap
--rw-r--r--   0     1001      127    52187 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap
--rw-r--r--   0     1001      127  1811359 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap
--rw-r--r--   0     1001      127    10278 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap
--rw-r--r--   0     1001      127   242145 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap
--rw-r--r--   0     1001      127     6457 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/url_or_path.rs
--rw-r--r--   0     1001      127       22 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/mod.rs
--rw-r--r--   0     1001      127     1693 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs
--rw-r--r--   0     1001      127      372 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/mod.rs
--rw-r--r--   0     1001      127     2012 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/ordered.rs
--rw-r--r--   0     1001      127     1571 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs
--rw-r--r--   0     1001      127     7945 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs
--rw-r--r--   0     1001      127     1441 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs
--rw-r--r--   0     1001      127     1407 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs
--rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/simple_spawn_blocking/Cargo.toml
--rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/simple_spawn_blocking/src/lib.rs
--rw-r--r--   0     1001      127      692 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/simple_spawn_blocking/src/tokio.rs
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/Cargo.toml
--rw-r--r--   0     1001      127     4303 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/CHANGELOG.md
--rw-r--r--   0     1001      127     2806 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs
--rw-r--r--   0     1001      127     7713 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs
--rw-r--r--   0     1001      127      956 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap
--rw-r--r--   0     1001      127      465 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_one.snap
--rw-r--r--   0     1001      127      604 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap
--rw-r--r--   0     1001      127    38981 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs
--rw-r--r--   0     1001      127    52612 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs
--rw-r--r--   0     1001      127     3926 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs
--rw-r--r--   0     1001      127     3219 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs
--rw-r--r--   0     1001      127     1738 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs
--rw-r--r--   0     1001      127     2627 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs
--rw-r--r--   0     1001      127     2335 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs
--rw-r--r--   0     1001      127    18116 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs
--rw-r--r--   0     1001      127     8435 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs
--rw-r--r--   0     1001      127     2409 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs
--rw-r--r--   0     1001      127     2377 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs
--rw-r--r--   0     1001      127    13060 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs
--rw-r--r--   0     1001      127     8026 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs
--rw-r--r--   0     1001      127     5798 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs
--rw-r--r--   0     1001      127     6178 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs
--rw-r--r--   0     1001      127     2151 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/lib.rs
--rw-r--r--   0     1001      127     3977 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/reporter.rs
--rw-r--r--   0     1001      127    22540 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs
--rw-r--r--   0     1001      127     2167 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/body.rs
--rw-r--r--   0     1001      127     2718 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs
--rw-r--r--   0     1001      127    13393 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs
--rw-r--r--   0     1001      127     1715 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs
--rw-r--r--   0     1001      127     2609 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/Cargo.toml
--rw-r--r--   0     1001      127      987 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/CHANGELOG.md
--rw-r--r--   0     1001      127     2664 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/src/lib.rs
--rw-r--r--   0     1001      127      113 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/01-sorted-enum.rs
--rw-r--r--   0     1001      127      155 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/02-sorted-struct.rs
--rw-r--r--   0     1001      127      113 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/03-out-of-order-enum.rs
--rw-r--r--   0     1001      127      127 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/03-out-of-order-enum.stderr
--rw-r--r--   0     1001      127      155 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/04-out-of-order-struct.rs
--rw-r--r--   0     1001      127      137 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/04-out-of-order-struct.stderr
--rw-r--r--   0     1001      127      251 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/tests.rs
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/Cargo.toml
--rw-r--r--   0     1001      127     3232 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/CHANGELOG.md
--rw-r--r--   0     1001      127    11042 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/cuda.rs
--rw-r--r--   0     1001      127    12929 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/lib.rs
--rw-r--r--   0     1001      127     3047 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/libc.rs
--rw-r--r--   0     1001      127     3969 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/linux.rs
--rw-r--r--   0     1001      127     2381 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/osx.rs
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/file_url/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/file_url/.gitignore
--rw-r--r--   0     1001      127      486 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/file_url/CHANGELOG.md
--rw-r--r--   0     1001      127     7791 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/file_url/src/lib.rs
--rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/.gitignore
--rw-r--r--   0     1001      127     5482 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/CHANGELOG.md
--rw-r--r--   0     1001      127    74752 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/resources/launcher64.exe
--rw-r--r--   0     1001      127    99068 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/resources/versions.txt
--rw-r--r--   0     1001      127     4794 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/cli/auth.rs
--rw-r--r--   0     1001      127      122 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/cli/mod.rs
--rw-r--r--   0     1001      127     1358 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/apple_codesign.rs
--rw-r--r--   0     1001      127    35510 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/clobber_registry.rs
--rw-r--r--   0     1001      127     9786 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/driver.rs
--rw-r--r--   0     1001      127     8511 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/entry_point.rs
--rw-r--r--   0     1001      127     1666 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/error.rs
--rw-r--r--   0     1001      127    27383 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/indicatif.rs
--rw-r--r--   0     1001      127    20030 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/mod.rs
--rw-r--r--   0     1001      127     4261 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/reporter.rs
--rw-r--r--   0     1001      127    33225 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/link.rs
--rw-r--r--   0     1001      127     9691 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/link_script.rs
--rw-r--r--   0     1001      127    33679 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/mod.rs
--rw-r--r--   0     1001      127     3839 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/python.rs
--rw-r--r--   0     1001      127      609 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap
--rw-r--r--   0     1001      127      190 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-3.snap
--rw-r--r--   0     1001      127      727 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap
--rw-r--r--   0     1001      127      142 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-5.snap
--rw-r--r--   0     1001      127      609 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap
--rw-r--r--   0     1001      127      727 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap
--rw-r--r--   0     1001      127      142 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber.snap
--rw-r--r--   0     1001      127      297 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__entry_point_script.snap
--rw-r--r--   0     1001      127      271 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__windows.snap
--rw-r--r--   0     1001      127      155 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__link__test__replace_long_prefix_in_text_file.snap
--rw-r--r--   0     1001      127     3732 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap
--rw-r--r--   0     1001      127     4688 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/test_utils.rs
--rw-r--r--   0     1001      127     8426 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/transaction.rs
--rw-r--r--   0     1001      127     9414 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/unlink.rs
--rw-r--r--   0     1001      127     2983 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/lib.rs
--rw-r--r--   0     1001      127    22292 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/package_cache.rs
--rw-r--r--   0     1001      127    24363 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/range.rs
--rw-r--r--   0     1001      127    13775 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/validation.rs
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_index/Cargo.toml
--rw-r--r--   0     1001      127     3314 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_index/CHANGELOG.md
--rw-r--r--   0     1001      127     6961 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_index/src/lib.rs
--rw-r--r--   0     1001      127     2162 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_index/tests/test_index.rs
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/Cargo.toml
--rw-r--r--   0     1001      127     4099 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/CHANGELOG.md
--rw-r--r--   0     1001      127     2914 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/benches/bench.rs
--rw-r--r--   0     1001      127     8454 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/lib.rs
--rw-r--r--   0     1001      127    13226 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/input.rs
--rw-r--r--   0     1001      127     1173 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs
--rw-r--r--   0     1001      127     9630 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/mod.rs
--rw-r--r--   0     1001      127     2444 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/output.rs
--rw-r--r--   0     1001      127      561 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs
--rw-r--r--   0     1001      127      864 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs
--rw-r--r--   0     1001      127     1047 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs
--rw-r--r--   0     1001      127    11669 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs
--rw-r--r--   0     1001      127     2720 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs
--rw-r--r--   0     1001      127     6299 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs
--rw-r--r--   0     1001      127     3402 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs
--rw-r--r--   0     1001      127     1262 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs
--rw-r--r--   0     1001      127     3451 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs
--rw-r--r--   0     1001      127     4718 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs
--rw-r--r--   0     1001      127     5589 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs
--rw-r--r--   0     1001      127     2468 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs
--rw-r--r--   0     1001      127     7734 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/resolvo/conda_util.rs
--rw-r--r--   0     1001      127    24305 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/resolvo/mod.rs
--rw-r--r--   0     1001      127    33981 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/backends.rs
--rw-r--r--   0     1001      127      165 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_dummy_repo_install_non_existent.snap
--rw-r--r--   0     1001      127      738 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap
--rw-r--r--   0     1001      127     1105 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap
--rw-r--r--   0     1001      127     3069 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap
--rw-r--r--   0     1001      127     2590 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap
--rw-r--r--   0     1001      127     3631 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap
--rw-r--r--   0     1001      127      216 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_with_error.snap
--rw-r--r--   0     1001      127      411 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_xtensor_xsimd.snap
--rw-r--r--   0     1001      127      369 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__exclude_newer_error.snap
--rw-r--r--   0     1001      127      172 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_dummy_repo_install_non_existent.snap
--rw-r--r--   0     1001      127      412 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_locked.snap
--rw-r--r--   0     1001      127      736 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap
--rw-r--r--   0     1001      127     1103 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap
--rw-r--r--   0     1001      127     3067 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap
--rw-r--r--   0     1001      127     2588 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap
--rw-r--r--   0     1001      127     3629 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap
--rw-r--r--   0     1001      127      588 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap
--rw-r--r--   0     1001      127      400 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_xtensor_xsimd.snap
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/Cargo.toml
--rw-r--r--   0     1001      127     1233 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/CHANGELOG.md
--rw-r--r--   0     1001      127     7607 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/src/lib.rs
--rw-r--r--   0     1001      127     4014 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/src/serde.rs
--rw-r--r--   0     1001      127     2155 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/src/tokio.rs
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/Cargo.toml
--rw-r--r--   0     1001      127     3627 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/CHANGELOG.md
--rw-r--r--   0     1001      127    14736 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_middleware.rs
--rw-r--r--   0     1001      127     1266 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs
--rw-r--r--   0     1001      127     6690 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs
--rw-r--r--   0     1001      127     2852 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs
--rw-r--r--   0     1001      127      103 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/mod.rs
--rw-r--r--   0     1001      127     5769 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs
--rw-r--r--   0     1001      127      270 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/snapshots/rattler_networking__authentication_storage__backends__file__tests__file_storage.snap
--rw-r--r--   0     1001      127      727 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/mod.rs
--rw-r--r--   0     1001      127     6830 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/storage.rs
--rw-r--r--   0     1001      127     2287 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/gcs_middleware.rs
--rw-r--r--   0     1001      127      726 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/lib.rs
--rw-r--r--   0     1001      127    10298 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/mirror_middleware.rs
--rw-r--r--   0     1001      127    10902 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/oci_middleware.rs
--rw-r--r--   0     1001      127     3489 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/redaction.rs
--rw-r--r--   0     1001      127      920 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/retry_policies.rs
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/Cargo.toml
--rw-r--r--   0     1001      127     4351 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/CHANGELOG.md
--rw-r--r--   0     1001      127     1016 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/benches/parse.rs
--rw-r--r--   0     1001      127     3220 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/build_spec/mod.rs
--rw-r--r--   0     1001      127     6519 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/build_spec/parse.rs
--rw-r--r--   0     1001      127    23177 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/channel/mod.rs
--rw-r--r--   0     1001      127     4187 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/channel_data.rs
--rw-r--r--   0     1001      127    11580 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs
--rw-r--r--   0     1001      127      770 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs
--rw-r--r--   0     1001      127     2279 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/lib.rs
--rw-r--r--   0     1001      127     6012 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs
--rw-r--r--   0     1001      127    20372 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/mod.rs
--rw-r--r--   0     1001      127    28532 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/parse.rs
--rw-r--r--   0     1001      127      506 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__parse__tests__parsed matchspecs.snap
--rw-r--r--   0     1001      127      537 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap
--rw-r--r--   0     1001      127     5728 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/no_arch_type.rs
--rw-r--r--   0     1001      127     3206 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/about.rs
--rw-r--r--   0     1001      127     4183 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs
--rw-r--r--   0     1001      127     1400 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/archive_type.rs
--rw-r--r--   0     1001      127     3244 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/entry_point.rs
--rw-r--r--   0     1001      127     1348 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/files.rs
--rw-r--r--   0     1001      127     6460 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/has_prefix.rs
--rw-r--r--   0     1001      127     3942 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/index.rs
--rw-r--r--   0     1001      127     1977 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/link.rs
--rw-r--r--   0     1001      127     3607 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/mod.rs
--rw-r--r--   0     1001      127     1510 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/no_link.rs
--rw-r--r--   0     1001      127     1495 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/no_softlink.rs
--rw-r--r--   0     1001      127      507 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/package_metadata.rs
--rw-r--r--   0     1001      127    12387 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/paths.rs
--rw-r--r--   0     1001      127     2334 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/run_exports.rs
--rw-r--r--   0     1001      127      754 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap
--rw-r--r--   0     1001      127     2515 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap
--rw-r--r--   0     1001      127      134 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__entry_point__test__entry_point.snap
--rw-r--r--   0     1001      127      329 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json.snap
--rw-r--r--   0     1001      127      309 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json_with_symlinks.snap
--rw-r--r--   0     1001      127      349 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__jupyterlab-link.json.snap
--rw-r--r--   0     1001      127      137 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__setuptools-link.json.snap
--rw-r--r--   0     1001      127      138 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__tzdata-link.json.snap
--rw-r--r--   0     1001      127     1171 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap
--rw-r--r--   0     1001      127      776 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap
--rw-r--r--   0     1001      127      601 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap
--rw-r--r--   0     1001      127     6782 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap
--rw-r--r--   0     1001      127      185 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__run_exports__test__reconstruct_run_exports_json_with_symlinks.snap
--rw-r--r--   0     1001      127     5305 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package_name.rs
--rw-r--r--   0     1001      127      233 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/parse_mode.rs
--rw-r--r--   0     1001      127    15923 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/platform.rs
--rw-r--r--   0     1001      127    12758 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/prefix_record.rs
--rw-r--r--   0     1001      127    19998 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/mod.rs
--rw-r--r--   0     1001      127    11158 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/patches.rs
--rw-r--r--   0     1001      127     1554 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs
--rw-r--r--   0     1001      127      181 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__null_values.snap
--rw-r--r--   0     1001      127     2154 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap
--rw-r--r--   0     1001      127     2091 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap
--rw-r--r--   0     1001      127      843 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap
--rw-r--r--   0     1001      127     1595 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap
--rw-r--r--   0     1001      127      873 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap
--rw-r--r--   0     1001      127     4832 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap
--rw-r--r--   0     1001      127      232 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize.snap
--rw-r--r--   0     1001      127     6461 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap
--rw-r--r--   0     1001      127     5154 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap
--rw-r--r--   0     1001      127    77589 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs
--rw-r--r--   0     1001      127     1063 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data_record.rs
--rw-r--r--   0     1001      127      455 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/run_export.rs
--rw-r--r--   0     1001      127    53039 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap
--rw-r--r--   0     1001      127      353 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__vs2015_runtime_win-64.txt.snap
--rw-r--r--   0     1001      127      974 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap
--rw-r--r--   0     1001      127     2269 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap
--rw-r--r--   0     1001      127    12047 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap
--rw-r--r--   0     1001      127   269415 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     4590 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap
--rw-r--r--   0     1001      127    12519 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127   345345 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap
--rw-r--r--   0     1001      127    23076 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     1054 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap
--rw-r--r--   0     1001      127    12151 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     7102 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap
--rw-r--r--   0     1001      127       22 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/utils/mod.rs
--rw-r--r--   0     1001      127     6107 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/utils/serde.rs
--rw-r--r--   0     1001      127     1531 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/bump.rs
--rw-r--r--   0     1001      127     3760 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/flags.rs
--rw-r--r--   0     1001      127    53146 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/mod.rs
--rw-r--r--   0     1001      127    18817 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/parse.rs
--rw-r--r--   0     1001      127     6410 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/segment.rs
--rw-r--r--   0     1001      127     2495 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap
--rw-r--r--   0     1001      127     4817 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/with_source.rs
--rw-r--r--   0     1001      127    10418 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs
--rw-r--r--   0     1001      127    18331 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/mod.rs
--rw-r--r--   0     1001      127    16688 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/parse.rs
--rw-r--r--   0     1001      127    14591 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/Cargo.toml
--rw-r--r--   0     1001      127     3029 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/CHANGELOG.md
--rw-r--r--   0     1001      127    27911 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/activation.rs
--rw-r--r--   0     1001      127      196 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/lib.rs
--rw-r--r--   0     1001      127     2232 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/run/mod.rs
--rw-r--r--   0     1001      127    28467 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/mod.rs
--rw-r--r--   0     1001      127      123 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__bash.snap
--rw-r--r--   0     1001      127      128 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__fish.snap
--rw-r--r--   0     1001      127      104 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_bash.snap
--rw-r--r--   0     1001      127      122 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_xsh.snap
--rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_bash.snap
--rw-r--r--   0     1001      127      185 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_cmd.snap
--rw-r--r--   0     1001      127      190 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_fish.snap
--rw-r--r--   0     1001      127      192 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_powershell.snap
--rw-r--r--   0     1001      127      239 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_xonsh.snap
--rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_zsh.snap
--rw-r--r--   0     1001      127      171 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__after_activation.snap
--rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_append.snap
--rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_prepend.snap
--rw-r--r--   0     1001      127      229 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_replace.snap
--rw-r--r--   0     1001      127      202 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_append.snap
--rw-r--r--   0     1001      127      202 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_prepend.snap
--rw-r--r--   0     1001      127      195 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_replace.snap
--rw-r--r--   0     1001      127      311 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_append.snap
--rw-r--r--   0     1001      127      311 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_prepend.snap
--rw-r--r--   0     1001      127      301 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_replace.snap
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 py_rattler-0.6.0/Cargo.toml
--rw-r--r--   0     1001      127      743 2024-05-27 12:39:44.000000 py_rattler-0.6.0/.gitignore
--rw-r--r--   0     1001      127     1502 2024-05-27 12:39:44.000000 py_rattler-0.6.0/LICENSE
--rw-r--r--   0     1001      127     6880 2024-05-27 12:39:44.000000 py_rattler-0.6.0/README.md
--rw-r--r--   0     1001      127       71 2024-05-27 12:39:44.000000 py_rattler-0.6.0/build.rs
--rw-r--r--   0     1001      127       44 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/about_json.md
--rw-r--r--   0     1001      127       45 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/activate.md
--rw-r--r--   0     1001      127       58 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/activation_error.md
--rw-r--r--   0     1001      127       61 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/activation_result.md
--rw-r--r--   0     1001      127       67 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/activation_variables.md
--rw-r--r--   0     1001      127       34 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/arch.md
--rw-r--r--   0     1001      127       62 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/authenticated_client.md
--rw-r--r--   0     1001      127       54 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/cache_dir_error.md
--rw-r--r--   0     1001      127       39 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/channel.md
--rw-r--r--   0     1001      127       52 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/channel_config.md
--rw-r--r--   0     1001      127       79 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/detect_virtual_package_error.md
--rw-r--r--   0     1001      127       44 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/environment.md
--rw-r--r--   0     1001      127       76 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/environment_creation_error.md
--rw-r--r--   0     1001      127       58 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/fetch_repo_data.md
--rw-r--r--   0     1001      127       65 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/fetch_repo_data_error.md
--rw-r--r--   0     1001      127       51 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/file_mode.md
--rw-r--r--   0     1001      127       41 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/gateway.md
--rw-r--r--   0     1001      127       61 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/generic_virtual_package.md
--rw-r--r--   0     1001      127     5592 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/index.md
--rw-r--r--   0     1001      127       44 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/index_json.md
--rw-r--r--   0     1001      127       41 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/installer.md
--rw-r--r--   0     1001      127       67 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_channel_error.md
--rw-r--r--   0     1001      127       71 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_match_spec_error.md
--rw-r--r--   0     1001      127       75 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_package_name_error.md
--rw-r--r--   0     1001      127       59 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_url_error.md
--rw-r--r--   0     1001      127       67 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_version_error.md
--rw-r--r--   0     1001      127       43 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/io_error.md
--rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/link_error.md
--rw-r--r--   0     1001      127       38 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/lock_file.md
--rw-r--r--   0     1001      127       48 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/locked_package.md
--rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/match_spec.md
--rw-r--r--   0     1001      127       64 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/nameless_match_spec.md
--rw-r--r--   0     1001      127       48 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/package_hashes.md
--rw-r--r--   0     1001      127       48 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/package_name.md
--rw-r--r--   0     1001      127       54 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/package_record.md
--rw-r--r--   0     1001      127       57 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/parse_arch_error.md
--rw-r--r--   0     1001      127       65 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/parse_platform_error.md
--rw-r--r--   0     1001      127       62 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/patch_instructions.md
--rw-r--r--   0     1001      127       77 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/path_modification_behavior.md
--rw-r--r--   0     1001      127       52 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/path_type.md
--rw-r--r--   0     1001      127       56 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/paths_entry.md
--rw-r--r--   0     1001      127       55 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/paths_json.md
--rw-r--r--   0     1001      127       42 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/platform.md
--rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/prefix_paths.md
--rw-r--r--   0     1001      127       69 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/prefix_placeholder.md
--rw-r--r--   0     1001      127       49 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/prefix_record.md
--rw-r--r--   0     1001      127       52 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/pypi_package_data.md
--rw-r--r--   0     1001      127       74 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/pypi_package_environment_data.md
--rw-r--r--   0     1001      127       44 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/repo_data.md
--rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/repo_data_record.md
--rw-r--r--   0     1001      127       56 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/run_exports_json.md
--rw-r--r--   0     1001      127       39 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/shell.md
--rw-r--r--   0     1001      127       35 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/solver.md
--rw-r--r--   0     1001      127       51 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/solver_error.md
--rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/sparse_repo_data.md
--rw-r--r--   0     1001      127     2082 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127       61 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/transaction_error.md
--rw-r--r--   0     1001      127       39 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/version.md
--rw-r--r--   0     1001      127       53 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/version_with_source.md
--rw-r--r--   0     1001      127       62 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/virtual_package.md
--rw-r--r--   0     1001      127     5280 2024-05-27 12:39:44.000000 py_rattler-0.6.0/mkdocs.yml
--rw-r--r--   0     1001      127   210327 2024-05-27 12:39:44.000000 py_rattler-0.6.0/pixi.lock
--rw-r--r--   0     1001      127     1898 2024-05-27 12:39:44.000000 py_rattler-0.6.0/pixi.toml
--rw-r--r--   0     1001      127     1863 2024-05-27 12:39:44.000000 py_rattler-0.6.0/pyproject.toml
--rw-r--r--   0     1001      127     2070 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/__init__.py
--rw-r--r--   0     1001      127      221 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/channel/__init__.py
--rw-r--r--   0     1001      127     2295 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/channel/channel.py
--rw-r--r--   0     1001      127     1532 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/channel/channel_config.py
--rw-r--r--   0     1001      127      474 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/channel/channel_priority.py
--rw-r--r--   0     1001      127     3842 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/exceptions.py
--rw-r--r--   0     1001      127       59 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/index/__init__.py
--rw-r--r--   0     1001      127     1133 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/index/index.py
--rw-r--r--   0     1001      127       69 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/install/__init__.py
--rw-r--r--   0     1001      127     3150 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/install/installer.py
--rw-r--r--   0     1001      127      471 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/__init__.py
--rw-r--r--   0     1001      127     1277 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/channel.py
--rw-r--r--   0     1001      127     7624 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/environment.py
--rw-r--r--   0     1001      127      805 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/hash.py
--rw-r--r--   0     1001      127     3264 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/lock_file.py
--rw-r--r--   0     1001      127     5336 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/package.py
--rw-r--r--   0     1001      127     6544 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/pypi.py
--rw-r--r--   0     1001      127      167 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/match_spec/__init__.py
--rw-r--r--   0     1001      127     7953 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/match_spec/match_spec.py
--rw-r--r--   0     1001      127     4293 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/match_spec/nameless_match_spec.py
--rw-r--r--   0     1001      127      189 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/networking/__init__.py
--rw-r--r--   0     1001      127      915 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/networking/authenticated_client.py
--rw-r--r--   0     1001      127     1393 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/networking/fetch_repo_data.py
--rw-r--r--   0     1001      127      518 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/__init__.py
--rw-r--r--   0     1001      127     7060 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/about_json.py
--rw-r--r--   0     1001      127     9422 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/index_json.py
--rw-r--r--   0     1001      127     3672 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/no_arch_type.py
--rw-r--r--   0     1001      127     4111 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/package_name.py
--rw-r--r--   0     1001      127    15226 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/paths_json.py
--rw-r--r--   0     1001      127     6238 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/run_exports_json.py
--rw-r--r--   0     1001      127      154 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/platform/__init__.py
--rw-r--r--   0     1001      127     1145 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/platform/arch.py
--rw-r--r--   0     1001      127     3993 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/platform/platform.py
--rw-r--r--   0     1001      127      221 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/prefix/__init__.py
--rw-r--r--   0     1001      127     8542 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/prefix/prefix_paths.py
--rw-r--r--   0     1001      127     4514 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/prefix/prefix_record.py
--rw-r--r--   0     1001      127        0 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/py.typed
--rw-r--r--   0     1001      127      495 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/__init__.py
--rw-r--r--   0     1001      127     8268 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/gateway.py
--rw-r--r--   0     1001      127    13342 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/package_record.py
--rw-r--r--   0     1001      127      694 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/patch_instructions.py
--rw-r--r--   0     1001      127     2660 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/record.py
--rw-r--r--   0     1001      127     2264 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/repo_data.py
--rw-r--r--   0     1001      127     6245 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/sparse.py
--rw-r--r--   0     1001      127      179 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/shell/__init__.py
--rw-r--r--   0     1001      127     4442 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/shell/shell.py
--rw-r--r--   0     1001      127       61 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/solver/__init__.py
--rw-r--r--   0     1001      127     5197 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/solver/solver.py
--rw-r--r--   0     1001      127      526 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/utils/rattler_version.py
--rw-r--r--   0     1001      127      146 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/version/__init__.py
--rw-r--r--   0     1001      127    14467 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/version/version.py
--rw-r--r--   0     1001      127     2539 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/version/with_source.py
--rw-r--r--   0     1001      127      188 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/virtual_package/__init__.py
--rw-r--r--   0     1001      127     4411 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/virtual_package/generic.py
--rw-r--r--   0     1001      127     1509 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/virtual_package/virtual_package.py
--rw-r--r--   0     1001      127     4356 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/about_json.rs
--rw-r--r--   0     1001      127     2929 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/channel/mod.rs
--rw-r--r--   0     1001      127     7910 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/error.rs
--rw-r--r--   0     1001      127     1743 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/generic_virtual_package.rs
--rw-r--r--   0     1001      127      593 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/index.rs
--rw-r--r--   0     1001      127     5113 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/index_json.rs
--rw-r--r--   0     1001      127     2334 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/installer.rs
--rw-r--r--   0     1001      127     6766 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/lib.rs
--rw-r--r--   0     1001      127    15021 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/lock/mod.rs
--rw-r--r--   0     1001      127     3683 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/match_spec.rs
--rw-r--r--   0     1001      127      147 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/meta.rs
--rw-r--r--   0     1001      127     3550 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/nameless_match_spec.rs
--rw-r--r--   0     1001      127     1017 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/networking/authenticated_client.rs
--rw-r--r--   0     1001      127      804 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/networking/cached_repo_data.rs
--rw-r--r--   0     1001      127     3328 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/networking/mod.rs
--rw-r--r--   0     1001      127     1619 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/no_arch_type.rs
--rw-r--r--   0     1001      127     2124 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/package_name.rs
--rw-r--r--   0     1001      127     9546 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/paths_json.rs
--rw-r--r--   0     1001      127     2521 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/platform.rs
--rw-r--r--   0     1001      127     5691 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/prefix_paths.rs
--rw-r--r--   0     1001      127    13360 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/record.rs
--rw-r--r--   0     1001      127     4735 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/repo_data/gateway.rs
--rw-r--r--   0     1001      127     1672 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/repo_data/mod.rs
--rw-r--r--   0     1001      127      189 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/repo_data/patch_instructions.rs
--rw-r--r--   0     1001      127     2096 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/repo_data/sparse.rs
--rw-r--r--   0     1001      127     4469 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/run_exports_json.rs
--rw-r--r--   0     1001      127     3878 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/shell.rs
--rw-r--r--   0     1001      127     3842 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/solver.rs
--rw-r--r--   0     1001      127      814 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/version/component.rs
--rw-r--r--   0     1001      127     5550 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/version/mod.rs
--rw-r--r--   0     1001      127     1190 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/virtual_package.rs
--rw-r--r--   0     1001      127        0 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/__init__.py
--rw-r--r--   0     1001      127      696 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/conftest.py
--rw-r--r--   0     1001      127        0 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/__init__.py
--rw-r--r--   0     1001      127     2129 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_fetch_repo_data.py
--rw-r--r--   0     1001      127     2159 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_index.py
--rw-r--r--   0     1001      127      730 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_install.py
--rw-r--r--   0     1001      127     1732 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_prefix_record.py
--rw-r--r--   0     1001      127     3531 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_solver.py
--rw-r--r--   0     1001      127      892 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_version.py
--rw-r--r--   0     1001      127   109244 2024-05-27 12:39:44.000000 py_rattler-0.6.0/Cargo.lock
--rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 py_rattler-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/Cargo.toml
+-rw-r--r--   0     1001      127     4319 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/CHANGELOG.md
+-rw-r--r--   0     1001      127     2053 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/fs.rs
+-rw-r--r--   0     1001      127     2392 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/lib.rs
+-rw-r--r--   0     1001      127     3671 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/read.rs
+-rw-r--r--   0     1001      127       98 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/reqwest/mod.rs
+-rw-r--r--   0     1001      127     6148 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs
+-rw-r--r--   0     1001      127     4387 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/seek.rs
+-rw-r--r--   0     1001      127     1732 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs
+-rw-r--r--   0     1001      127     3101 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/fs.rs
+-rw-r--r--   0     1001      127      113 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/mod.rs
+-rw-r--r--   0     1001      127    14225 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/write.rs
+-rw-r--r--   0     1001      127     9266 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/tests/extract.rs
+-rw-r--r--   0     1001      127     7864 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/tests/write.rs
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/Cargo.toml
+-rw-r--r--   0     1001      127     3970 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/CHANGELOG.md
+-rw-r--r--   0     1001      127     8878 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/builder.rs
+-rw-r--r--   0     1001      127      871 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/channel.rs
+-rw-r--r--   0     1001      127     5792 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/conda.rs
+-rw-r--r--   0     1001      127     2006 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/file_format_version.rs
+-rw-r--r--   0     1001      127     4879 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/hash.rs
+-rw-r--r--   0     1001      127    24726 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/lib.rs
+-rw-r--r--   0     1001      127     6083 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/deserialize.rs
+-rw-r--r--   0     1001      127     2613 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/mod.rs
+-rw-r--r--   0     1001      127     9114 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/serialize.rs
+-rw-r--r--   0     1001      127     8677 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/v3.rs
+-rw-r--r--   0     1001      127     5293 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/pypi.rs
+-rw-r--r--   0     1001      127     1480 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/pypi_indexes.rs
+-rw-r--r--   0     1001      127    15803 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap
+-rw-r--r--   0     1001      127    22538 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap
+-rw-r--r--   0     1001      127   487177 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap
+-rw-r--r--   0     1001      127    40002 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap
+-rw-r--r--   0     1001      127    52187 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap
+-rw-r--r--   0     1001      127  1811359 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap
+-rw-r--r--   0     1001      127   487177 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap
+-rw-r--r--   0     1001      127    19608 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap
+-rw-r--r--   0     1001      127    40002 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap
+-rw-r--r--   0     1001      127    52187 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap
+-rw-r--r--   0     1001      127  1811359 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap
+-rw-r--r--   0     1001      127    10278 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap
+-rw-r--r--   0     1001      127   242145 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap
+-rw-r--r--   0     1001      127     6457 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/url_or_path.rs
+-rw-r--r--   0     1001      127       22 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1693 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs
+-rw-r--r--   0     1001      127      372 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/mod.rs
+-rw-r--r--   0     1001      127     2012 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/ordered.rs
+-rw-r--r--   0     1001      127     1609 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs
+-rw-r--r--   0     1001      127     7980 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs
+-rw-r--r--   0     1001      127     1441 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs
+-rw-r--r--   0     1001      127     1407 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/Cargo.toml
+-rw-r--r--   0     1001      127     4535 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/CHANGELOG.md
+-rw-r--r--   0     1001      127     2806 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs
+-rw-r--r--   0     1001      127     7713 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs
+-rw-r--r--   0     1001      127      956 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap
+-rw-r--r--   0     1001      127      465 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_one.snap
+-rw-r--r--   0     1001      127      604 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap
+-rw-r--r--   0     1001      127    38981 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs
+-rw-r--r--   0     1001      127    52612 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs
+-rw-r--r--   0     1001      127     3926 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs
+-rw-r--r--   0     1001      127     3219 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs
+-rw-r--r--   0     1001      127     1738 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs
+-rw-r--r--   0     1001      127     2627 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs
+-rw-r--r--   0     1001      127     2335 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs
+-rw-r--r--   0     1001      127    18116 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs
+-rw-r--r--   0     1001      127     8435 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs
+-rw-r--r--   0     1001      127     2409 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs
+-rw-r--r--   0     1001      127     2377 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs
+-rw-r--r--   0     1001      127    13060 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs
+-rw-r--r--   0     1001      127     8026 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs
+-rw-r--r--   0     1001      127     5798 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs
+-rw-r--r--   0     1001      127     6178 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs
+-rw-r--r--   0     1001      127     2151 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/lib.rs
+-rw-r--r--   0     1001      127     3977 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/reporter.rs
+-rw-r--r--   0     1001      127    22540 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs
+-rw-r--r--   0     1001      127     2167 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/body.rs
+-rw-r--r--   0     1001      127     2718 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs
+-rw-r--r--   0     1001      127    13393 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs
+-rw-r--r--   0     1001      127     1715 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs
+-rw-r--r--   0     1001      127     2609 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/Cargo.toml
+-rw-r--r--   0     1001      127      987 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/CHANGELOG.md
+-rw-r--r--   0     1001      127     2664 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/src/lib.rs
+-rw-r--r--   0     1001      127      113 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/01-sorted-enum.rs
+-rw-r--r--   0     1001      127      155 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/02-sorted-struct.rs
+-rw-r--r--   0     1001      127      113 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/03-out-of-order-enum.rs
+-rw-r--r--   0     1001      127      127 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/03-out-of-order-enum.stderr
+-rw-r--r--   0     1001      127      155 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/04-out-of-order-struct.rs
+-rw-r--r--   0     1001      127      137 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/04-out-of-order-struct.stderr
+-rw-r--r--   0     1001      127      251 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/tests.rs
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/Cargo.toml
+-rw-r--r--   0     1001      127     1233 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/CHANGELOG.md
+-rw-r--r--   0     1001      127     7607 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/src/lib.rs
+-rw-r--r--   0     1001      127     4014 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/src/serde.rs
+-rw-r--r--   0     1001      127     2155 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/src/tokio.rs
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/Cargo.toml
+-rw-r--r--   0     1001      127     3627 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/CHANGELOG.md
+-rw-r--r--   0     1001      127    14736 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_middleware.rs
+-rw-r--r--   0     1001      127     1266 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs
+-rw-r--r--   0     1001      127     6690 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs
+-rw-r--r--   0     1001      127     2852 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs
+-rw-r--r--   0     1001      127      103 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/mod.rs
+-rw-r--r--   0     1001      127     5769 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs
+-rw-r--r--   0     1001      127      270 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/snapshots/rattler_networking__authentication_storage__backends__file__tests__file_storage.snap
+-rw-r--r--   0     1001      127      727 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/mod.rs
+-rw-r--r--   0     1001      127     6830 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/storage.rs
+-rw-r--r--   0     1001      127     2287 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/gcs_middleware.rs
+-rw-r--r--   0     1001      127      726 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/lib.rs
+-rw-r--r--   0     1001      127    10298 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/mirror_middleware.rs
+-rw-r--r--   0     1001      127    10902 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/oci_middleware.rs
+-rw-r--r--   0     1001      127     3489 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/redaction.rs
+-rw-r--r--   0     1001      127      920 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/retry_policies.rs
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/file_url/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/file_url/.gitignore
+-rw-r--r--   0     1001      127      486 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/file_url/CHANGELOG.md
+-rw-r--r--   0     1001      127     7791 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/file_url/src/lib.rs
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_index/Cargo.toml
+-rw-r--r--   0     1001      127     3536 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_index/CHANGELOG.md
+-rw-r--r--   0     1001      127     6989 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_index/src/lib.rs
+-rw-r--r--   0     1001      127     2162 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_index/tests/test_index.rs
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/Cargo.toml
+-rw-r--r--   0     1001      127     1011 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/CHANGELOG.md
+-rw-r--r--   0     1001      127     1394 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/build.rs
+-rw-r--r--   0     1001      127    77341 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/src/lib.rs
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/Cargo.toml
+-rw-r--r--   0     1001      127     5252 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/CHANGELOG.md
+-rw-r--r--   0     1001      127     1016 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/benches/parse.rs
+-rw-r--r--   0     1001      127     3220 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/build_spec/mod.rs
+-rw-r--r--   0     1001      127     6519 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/build_spec/parse.rs
+-rw-r--r--   0     1001      127    23177 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/channel/mod.rs
+-rw-r--r--   0     1001      127     4187 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/channel_data.rs
+-rw-r--r--   0     1001      127    11580 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs
+-rw-r--r--   0     1001      127      770 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs
+-rw-r--r--   0     1001      127     2299 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/lib.rs
+-rw-r--r--   0     1001      127     6012 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs
+-rw-r--r--   0     1001      127    20372 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/mod.rs
+-rw-r--r--   0     1001      127    28472 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/parse.rs
+-rw-r--r--   0     1001      127      506 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__parse__tests__parsed matchspecs.snap
+-rw-r--r--   0     1001      127      537 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap
+-rw-r--r--   0     1001      127     5728 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/no_arch_type.rs
+-rw-r--r--   0     1001      127     3206 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/about.rs
+-rw-r--r--   0     1001      127     4183 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs
+-rw-r--r--   0     1001      127     1400 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/archive_type.rs
+-rw-r--r--   0     1001      127     3244 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/entry_point.rs
+-rw-r--r--   0     1001      127     1348 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/files.rs
+-rw-r--r--   0     1001      127     6460 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/has_prefix.rs
+-rw-r--r--   0     1001      127     3942 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/index.rs
+-rw-r--r--   0     1001      127     1977 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/link.rs
+-rw-r--r--   0     1001      127     3607 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/mod.rs
+-rw-r--r--   0     1001      127     1510 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/no_link.rs
+-rw-r--r--   0     1001      127     1495 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/no_softlink.rs
+-rw-r--r--   0     1001      127      507 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/package_metadata.rs
+-rw-r--r--   0     1001      127    12387 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/paths.rs
+-rw-r--r--   0     1001      127     2780 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/run_exports.rs
+-rw-r--r--   0     1001      127      754 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap
+-rw-r--r--   0     1001      127     2515 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap
+-rw-r--r--   0     1001      127      134 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__entry_point__test__entry_point.snap
+-rw-r--r--   0     1001      127      329 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json.snap
+-rw-r--r--   0     1001      127      309 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json_with_symlinks.snap
+-rw-r--r--   0     1001      127      349 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__jupyterlab-link.json.snap
+-rw-r--r--   0     1001      127      137 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__setuptools-link.json.snap
+-rw-r--r--   0     1001      127      138 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__tzdata-link.json.snap
+-rw-r--r--   0     1001      127     1171 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap
+-rw-r--r--   0     1001      127      776 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap
+-rw-r--r--   0     1001      127      601 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap
+-rw-r--r--   0     1001      127     6782 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap
+-rw-r--r--   0     1001      127      185 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__run_exports__test__reconstruct_run_exports_json_with_symlinks.snap
+-rw-r--r--   0     1001      127     5305 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package_name.rs
+-rw-r--r--   0     1001      127      233 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/parse_mode.rs
+-rw-r--r--   0     1001      127    15923 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/platform.rs
+-rw-r--r--   0     1001      127    12758 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/prefix_record.rs
+-rw-r--r--   0     1001      127    20250 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/mod.rs
+-rw-r--r--   0     1001      127    11158 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/patches.rs
+-rw-r--r--   0     1001      127     1554 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs
+-rw-r--r--   0     1001      127      181 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__null_values.snap
+-rw-r--r--   0     1001      127     2154 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap
+-rw-r--r--   0     1001      127     2091 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap
+-rw-r--r--   0     1001      127      843 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap
+-rw-r--r--   0     1001      127     1595 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap
+-rw-r--r--   0     1001      127      873 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap
+-rw-r--r--   0     1001      127     4832 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap
+-rw-r--r--   0     1001      127      232 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize.snap
+-rw-r--r--   0     1001      127     6461 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap
+-rw-r--r--   0     1001      127     5154 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap
+-rw-r--r--   0     1001      127    77589 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs
+-rw-r--r--   0     1001      127     1063 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data_record.rs
+-rw-r--r--   0     1001      127      455 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/run_export.rs
+-rw-r--r--   0     1001      127    53039 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap
+-rw-r--r--   0     1001      127      353 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__vs2015_runtime_win-64.txt.snap
+-rw-r--r--   0     1001      127      974 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap
+-rw-r--r--   0     1001      127     2269 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap
+-rw-r--r--   0     1001      127    12047 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap
+-rw-r--r--   0     1001      127   269415 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     4590 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap
+-rw-r--r--   0     1001      127    12519 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127   345345 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap
+-rw-r--r--   0     1001      127    23076 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     1054 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap
+-rw-r--r--   0     1001      127    12151 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     7102 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap
+-rw-r--r--   0     1001      127       22 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/utils/mod.rs
+-rw-r--r--   0     1001      127     6107 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/utils/serde.rs
+-rw-r--r--   0     1001      127     8204 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/bump.rs
+-rw-r--r--   0     1001      127     3760 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/flags.rs
+-rw-r--r--   0     1001      127    46846 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/mod.rs
+-rw-r--r--   0     1001      127    18817 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/parse.rs
+-rw-r--r--   0     1001      127     6410 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/segment.rs
+-rw-r--r--   0     1001      127     2495 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap
+-rw-r--r--   0     1001      127     4817 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/with_source.rs
+-rw-r--r--   0     1001      127    10262 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs
+-rw-r--r--   0     1001      127    19332 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/mod.rs
+-rw-r--r--   0     1001      127    18092 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/parse.rs
+-rw-r--r--   0     1001      127    15169 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/Cargo.toml
+-rw-r--r--   0     1001      127     3218 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/CHANGELOG.md
+-rw-r--r--   0     1001      127    27911 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/activation.rs
+-rw-r--r--   0     1001      127      196 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/lib.rs
+-rw-r--r--   0     1001      127     2232 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/run/mod.rs
+-rw-r--r--   0     1001      127    28467 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/mod.rs
+-rw-r--r--   0     1001      127      123 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__bash.snap
+-rw-r--r--   0     1001      127      128 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__fish.snap
+-rw-r--r--   0     1001      127      104 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_bash.snap
+-rw-r--r--   0     1001      127      122 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_xsh.snap
+-rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_bash.snap
+-rw-r--r--   0     1001      127      185 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_cmd.snap
+-rw-r--r--   0     1001      127      190 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_fish.snap
+-rw-r--r--   0     1001      127      192 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_powershell.snap
+-rw-r--r--   0     1001      127      239 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_xonsh.snap
+-rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_zsh.snap
+-rw-r--r--   0     1001      127      171 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__after_activation.snap
+-rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_append.snap
+-rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_prepend.snap
+-rw-r--r--   0     1001      127      229 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_replace.snap
+-rw-r--r--   0     1001      127      202 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_append.snap
+-rw-r--r--   0     1001      127      202 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_prepend.snap
+-rw-r--r--   0     1001      127      195 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_replace.snap
+-rw-r--r--   0     1001      127      311 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_append.snap
+-rw-r--r--   0     1001      127      311 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_prepend.snap
+-rw-r--r--   0     1001      127      301 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_replace.snap
+-rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/.gitignore
+-rw-r--r--   0     1001      127     5659 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/CHANGELOG.md
+-rw-r--r--   0     1001      127    74752 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/resources/launcher64.exe
+-rw-r--r--   0     1001      127    99068 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/resources/versions.txt
+-rw-r--r--   0     1001      127     4794 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/cli/auth.rs
+-rw-r--r--   0     1001      127      122 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/cli/mod.rs
+-rw-r--r--   0     1001      127     1358 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/apple_codesign.rs
+-rw-r--r--   0     1001      127    35510 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/clobber_registry.rs
+-rw-r--r--   0     1001      127     9786 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/driver.rs
+-rw-r--r--   0     1001      127     8511 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/entry_point.rs
+-rw-r--r--   0     1001      127     1666 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/error.rs
+-rw-r--r--   0     1001      127    27383 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/indicatif.rs
+-rw-r--r--   0     1001      127    20030 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/mod.rs
+-rw-r--r--   0     1001      127     4261 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/reporter.rs
+-rw-r--r--   0     1001      127    33225 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/link.rs
+-rw-r--r--   0     1001      127     9691 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/link_script.rs
+-rw-r--r--   0     1001      127    33679 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/mod.rs
+-rw-r--r--   0     1001      127     3839 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/python.rs
+-rw-r--r--   0     1001      127      609 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap
+-rw-r--r--   0     1001      127      190 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-3.snap
+-rw-r--r--   0     1001      127      727 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap
+-rw-r--r--   0     1001      127      142 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-5.snap
+-rw-r--r--   0     1001      127      609 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap
+-rw-r--r--   0     1001      127      727 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap
+-rw-r--r--   0     1001      127      142 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber.snap
+-rw-r--r--   0     1001      127      297 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__entry_point_script.snap
+-rw-r--r--   0     1001      127      271 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__windows.snap
+-rw-r--r--   0     1001      127      155 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__link__test__replace_long_prefix_in_text_file.snap
+-rw-r--r--   0     1001      127     3732 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap
+-rw-r--r--   0     1001      127     4688 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/test_utils.rs
+-rw-r--r--   0     1001      127     8426 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/transaction.rs
+-rw-r--r--   0     1001      127     9414 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/unlink.rs
+-rw-r--r--   0     1001      127     2983 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/lib.rs
+-rw-r--r--   0     1001      127    22292 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/package_cache.rs
+-rw-r--r--   0     1001      127    24363 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/range.rs
+-rw-r--r--   0     1001      127    13775 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/validation.rs
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/Cargo.toml
+-rw-r--r--   0     1001      127     4417 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/CHANGELOG.md
+-rw-r--r--   0     1001      127     2914 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/benches/bench.rs
+-rw-r--r--   0     1001      127     8738 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/lib.rs
+-rw-r--r--   0     1001      127    13226 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/input.rs
+-rw-r--r--   0     1001      127     1173 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs
+-rw-r--r--   0     1001      127     9630 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/mod.rs
+-rw-r--r--   0     1001      127     2444 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/output.rs
+-rw-r--r--   0     1001      127      561 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs
+-rw-r--r--   0     1001      127      864 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs
+-rw-r--r--   0     1001      127     1047 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs
+-rw-r--r--   0     1001      127    11669 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs
+-rw-r--r--   0     1001      127     2720 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs
+-rw-r--r--   0     1001      127     6299 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs
+-rw-r--r--   0     1001      127     3402 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs
+-rw-r--r--   0     1001      127     1262 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs
+-rw-r--r--   0     1001      127     3451 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs
+-rw-r--r--   0     1001      127     4718 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs
+-rw-r--r--   0     1001      127     5589 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs
+-rw-r--r--   0     1001      127     2468 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs
+-rw-r--r--   0     1001      127     7734 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/resolvo/conda_util.rs
+-rw-r--r--   0     1001      127    24305 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/resolvo/mod.rs
+-rw-r--r--   0     1001      127    34012 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/backends.rs
+-rw-r--r--   0     1001      127      165 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_dummy_repo_install_non_existent.snap
+-rw-r--r--   0     1001      127      738 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap
+-rw-r--r--   0     1001      127     1105 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap
+-rw-r--r--   0     1001      127     3069 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap
+-rw-r--r--   0     1001      127     2590 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap
+-rw-r--r--   0     1001      127     3631 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap
+-rw-r--r--   0     1001      127      216 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_with_error.snap
+-rw-r--r--   0     1001      127      411 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_xtensor_xsimd.snap
+-rw-r--r--   0     1001      127      369 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__exclude_newer_error.snap
+-rw-r--r--   0     1001      127      172 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_dummy_repo_install_non_existent.snap
+-rw-r--r--   0     1001      127      412 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_locked.snap
+-rw-r--r--   0     1001      127      736 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap
+-rw-r--r--   0     1001      127     1103 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap
+-rw-r--r--   0     1001      127     3067 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap
+-rw-r--r--   0     1001      127     2588 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap
+-rw-r--r--   0     1001      127     3629 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap
+-rw-r--r--   0     1001      127      588 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap
+-rw-r--r--   0     1001      127      400 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_xtensor_xsimd.snap
+-rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/simple_spawn_blocking/Cargo.toml
+-rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/simple_spawn_blocking/src/lib.rs
+-rw-r--r--   0     1001      127      692 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/simple_spawn_blocking/src/tokio.rs
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/Cargo.toml
+-rw-r--r--   0     1001      127     3446 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/CHANGELOG.md
+-rw-r--r--   0     1001      127    11042 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/cuda.rs
+-rw-r--r--   0     1001      127    12929 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/lib.rs
+-rw-r--r--   0     1001      127     3047 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/libc.rs
+-rw-r--r--   0     1001      127     3969 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/linux.rs
+-rw-r--r--   0     1001      127     2381 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/osx.rs
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 py_rattler-0.6.1/Cargo.toml
+-rw-r--r--   0     1001      127      743 2024-05-28 14:47:59.000000 py_rattler-0.6.1/.gitignore
+-rw-r--r--   0     1001      127     1502 2024-05-28 14:47:59.000000 py_rattler-0.6.1/LICENSE
+-rw-r--r--   0     1001      127     6880 2024-05-28 14:47:59.000000 py_rattler-0.6.1/README.md
+-rw-r--r--   0     1001      127       71 2024-05-28 14:47:59.000000 py_rattler-0.6.1/build.rs
+-rw-r--r--   0     1001      127       44 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/about_json.md
+-rw-r--r--   0     1001      127       45 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/activate.md
+-rw-r--r--   0     1001      127       58 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/activation_error.md
+-rw-r--r--   0     1001      127       61 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/activation_result.md
+-rw-r--r--   0     1001      127       67 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/activation_variables.md
+-rw-r--r--   0     1001      127       34 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/arch.md
+-rw-r--r--   0     1001      127       62 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/authenticated_client.md
+-rw-r--r--   0     1001      127       54 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/cache_dir_error.md
+-rw-r--r--   0     1001      127       39 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/channel.md
+-rw-r--r--   0     1001      127       52 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/channel_config.md
+-rw-r--r--   0     1001      127       79 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/detect_virtual_package_error.md
+-rw-r--r--   0     1001      127       44 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/environment.md
+-rw-r--r--   0     1001      127       76 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/environment_creation_error.md
+-rw-r--r--   0     1001      127       58 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/fetch_repo_data.md
+-rw-r--r--   0     1001      127       65 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/fetch_repo_data_error.md
+-rw-r--r--   0     1001      127       51 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/file_mode.md
+-rw-r--r--   0     1001      127       41 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/gateway.md
+-rw-r--r--   0     1001      127       61 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/generic_virtual_package.md
+-rw-r--r--   0     1001      127     5592 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/index.md
+-rw-r--r--   0     1001      127       44 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/index_json.md
+-rw-r--r--   0     1001      127       41 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/installer.md
+-rw-r--r--   0     1001      127       67 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_channel_error.md
+-rw-r--r--   0     1001      127       71 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_match_spec_error.md
+-rw-r--r--   0     1001      127       75 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_package_name_error.md
+-rw-r--r--   0     1001      127       59 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_url_error.md
+-rw-r--r--   0     1001      127       67 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_version_error.md
+-rw-r--r--   0     1001      127       43 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/io_error.md
+-rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/link_error.md
+-rw-r--r--   0     1001      127       38 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/lock_file.md
+-rw-r--r--   0     1001      127       48 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/locked_package.md
+-rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/match_spec.md
+-rw-r--r--   0     1001      127       64 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/nameless_match_spec.md
+-rw-r--r--   0     1001      127       48 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/package_hashes.md
+-rw-r--r--   0     1001      127       48 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/package_name.md
+-rw-r--r--   0     1001      127       54 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/package_record.md
+-rw-r--r--   0     1001      127       57 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/parse_arch_error.md
+-rw-r--r--   0     1001      127       65 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/parse_platform_error.md
+-rw-r--r--   0     1001      127       62 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/patch_instructions.md
+-rw-r--r--   0     1001      127       77 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/path_modification_behavior.md
+-rw-r--r--   0     1001      127       52 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/path_type.md
+-rw-r--r--   0     1001      127       56 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/paths_entry.md
+-rw-r--r--   0     1001      127       55 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/paths_json.md
+-rw-r--r--   0     1001      127       42 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/platform.md
+-rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/prefix_paths.md
+-rw-r--r--   0     1001      127       69 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/prefix_placeholder.md
+-rw-r--r--   0     1001      127       49 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/prefix_record.md
+-rw-r--r--   0     1001      127       52 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/pypi_package_data.md
+-rw-r--r--   0     1001      127       74 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/pypi_package_environment_data.md
+-rw-r--r--   0     1001      127       44 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/repo_data.md
+-rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/repo_data_record.md
+-rw-r--r--   0     1001      127       56 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/run_exports_json.md
+-rw-r--r--   0     1001      127       39 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/shell.md
+-rw-r--r--   0     1001      127       35 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/solver.md
+-rw-r--r--   0     1001      127       51 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/solver_error.md
+-rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/sparse_repo_data.md
+-rw-r--r--   0     1001      127     2082 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127       61 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/transaction_error.md
+-rw-r--r--   0     1001      127       39 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/version.md
+-rw-r--r--   0     1001      127       53 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/version_with_source.md
+-rw-r--r--   0     1001      127       62 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/virtual_package.md
+-rw-r--r--   0     1001      127     5280 2024-05-28 14:47:59.000000 py_rattler-0.6.1/mkdocs.yml
+-rw-r--r--   0     1001      127   210327 2024-05-28 14:47:59.000000 py_rattler-0.6.1/pixi.lock
+-rw-r--r--   0     1001      127     1898 2024-05-28 14:47:59.000000 py_rattler-0.6.1/pixi.toml
+-rw-r--r--   0     1001      127     1863 2024-05-28 14:47:59.000000 py_rattler-0.6.1/pyproject.toml
+-rw-r--r--   0     1001      127     2070 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/__init__.py
+-rw-r--r--   0     1001      127      221 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/channel/__init__.py
+-rw-r--r--   0     1001      127     2295 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/channel/channel.py
+-rw-r--r--   0     1001      127     1532 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/channel/channel_config.py
+-rw-r--r--   0     1001      127      474 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/channel/channel_priority.py
+-rw-r--r--   0     1001      127     3842 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/exceptions.py
+-rw-r--r--   0     1001      127       59 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/index/__init__.py
+-rw-r--r--   0     1001      127     1133 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/index/index.py
+-rw-r--r--   0     1001      127       69 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/install/__init__.py
+-rw-r--r--   0     1001      127     3407 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/install/installer.py
+-rw-r--r--   0     1001      127      471 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/__init__.py
+-rw-r--r--   0     1001      127     1277 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/channel.py
+-rw-r--r--   0     1001      127     7624 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/environment.py
+-rw-r--r--   0     1001      127      805 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/hash.py
+-rw-r--r--   0     1001      127     3264 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/lock_file.py
+-rw-r--r--   0     1001      127     5336 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/package.py
+-rw-r--r--   0     1001      127     6544 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/pypi.py
+-rw-r--r--   0     1001      127      167 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/match_spec/__init__.py
+-rw-r--r--   0     1001      127     7953 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/match_spec/match_spec.py
+-rw-r--r--   0     1001      127     4293 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/match_spec/nameless_match_spec.py
+-rw-r--r--   0     1001      127      189 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/networking/__init__.py
+-rw-r--r--   0     1001      127      915 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/networking/authenticated_client.py
+-rw-r--r--   0     1001      127     1393 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/networking/fetch_repo_data.py
+-rw-r--r--   0     1001      127      518 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/__init__.py
+-rw-r--r--   0     1001      127     7060 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/about_json.py
+-rw-r--r--   0     1001      127     9422 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/index_json.py
+-rw-r--r--   0     1001      127     3672 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/no_arch_type.py
+-rw-r--r--   0     1001      127     4111 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/package_name.py
+-rw-r--r--   0     1001      127    15226 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/paths_json.py
+-rw-r--r--   0     1001      127     6238 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/run_exports_json.py
+-rw-r--r--   0     1001      127      154 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/platform/__init__.py
+-rw-r--r--   0     1001      127     1145 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/platform/arch.py
+-rw-r--r--   0     1001      127     3993 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/platform/platform.py
+-rw-r--r--   0     1001      127      221 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/prefix/__init__.py
+-rw-r--r--   0     1001      127     8542 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/prefix/prefix_paths.py
+-rw-r--r--   0     1001      127     4514 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/prefix/prefix_record.py
+-rw-r--r--   0     1001      127        0 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/py.typed
+-rw-r--r--   0     1001      127      495 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/__init__.py
+-rw-r--r--   0     1001      127     8268 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/gateway.py
+-rw-r--r--   0     1001      127    13342 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/package_record.py
+-rw-r--r--   0     1001      127      694 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/patch_instructions.py
+-rw-r--r--   0     1001      127     2660 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/record.py
+-rw-r--r--   0     1001      127     2264 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/repo_data.py
+-rw-r--r--   0     1001      127     6245 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/sparse.py
+-rw-r--r--   0     1001      127      179 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/shell/__init__.py
+-rw-r--r--   0     1001      127     4442 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/shell/shell.py
+-rw-r--r--   0     1001      127       61 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/solver/__init__.py
+-rw-r--r--   0     1001      127     5197 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/solver/solver.py
+-rw-r--r--   0     1001      127      526 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/utils/rattler_version.py
+-rw-r--r--   0     1001      127      146 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/version/__init__.py
+-rw-r--r--   0     1001      127    14868 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/version/version.py
+-rw-r--r--   0     1001      127     2539 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/version/with_source.py
+-rw-r--r--   0     1001      127      188 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/virtual_package/__init__.py
+-rw-r--r--   0     1001      127     4411 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/virtual_package/generic.py
+-rw-r--r--   0     1001      127     1509 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/virtual_package/virtual_package.py
+-rw-r--r--   0     1001      127     4356 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/about_json.rs
+-rw-r--r--   0     1001      127     2929 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/channel/mod.rs
+-rw-r--r--   0     1001      127     8225 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/error.rs
+-rw-r--r--   0     1001      127     1743 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/generic_virtual_package.rs
+-rw-r--r--   0     1001      127      593 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/index.rs
+-rw-r--r--   0     1001      127     5113 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/index_json.rs
+-rw-r--r--   0     1001      127     2334 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/installer.rs
+-rw-r--r--   0     1001      127     6766 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/lib.rs
+-rw-r--r--   0     1001      127    15021 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/lock/mod.rs
+-rw-r--r--   0     1001      127     3683 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/match_spec.rs
+-rw-r--r--   0     1001      127      147 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/meta.rs
+-rw-r--r--   0     1001      127     3550 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/nameless_match_spec.rs
+-rw-r--r--   0     1001      127     1017 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/networking/authenticated_client.rs
+-rw-r--r--   0     1001      127      804 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/networking/cached_repo_data.rs
+-rw-r--r--   0     1001      127     3328 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/networking/mod.rs
+-rw-r--r--   0     1001      127     1619 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/no_arch_type.rs
+-rw-r--r--   0     1001      127     2124 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/package_name.rs
+-rw-r--r--   0     1001      127     9546 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/paths_json.rs
+-rw-r--r--   0     1001      127     2521 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/platform.rs
+-rw-r--r--   0     1001      127     5691 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/prefix_paths.rs
+-rw-r--r--   0     1001      127    13360 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/record.rs
+-rw-r--r--   0     1001      127     4735 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/repo_data/gateway.rs
+-rw-r--r--   0     1001      127     1672 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/repo_data/mod.rs
+-rw-r--r--   0     1001      127      189 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/repo_data/patch_instructions.rs
+-rw-r--r--   0     1001      127     2096 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/repo_data/sparse.rs
+-rw-r--r--   0     1001      127     4469 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/run_exports_json.rs
+-rw-r--r--   0     1001      127     3878 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/shell.rs
+-rw-r--r--   0     1001      127     3842 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/solver.rs
+-rw-r--r--   0     1001      127      814 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/version/component.rs
+-rw-r--r--   0     1001      127     5899 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/version/mod.rs
+-rw-r--r--   0     1001      127     1190 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/virtual_package.rs
+-rw-r--r--   0     1001      127        0 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/__init__.py
+-rw-r--r--   0     1001      127      696 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/conftest.py
+-rw-r--r--   0     1001      127        0 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/__init__.py
+-rw-r--r--   0     1001      127     2129 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_fetch_repo_data.py
+-rw-r--r--   0     1001      127     2159 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_index.py
+-rw-r--r--   0     1001      127      730 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_install.py
+-rw-r--r--   0     1001      127     1732 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_prefix_record.py
+-rw-r--r--   0     1001      127     3531 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_solver.py
+-rw-r--r--   0     1001      127      892 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_version.py
+-rw-r--r--   0     1001      127   109244 2024-05-28 14:47:59.000000 py_rattler-0.6.1/Cargo.lock
+-rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 py_rattler-0.6.1/PKG-INFO
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/build.rs` & `py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/build.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_package_streaming"
-version = "0.21.0"
+version = "0.21.1"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Extract and stream of Conda package archives"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
 rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
 rattler_networking = { path= "../rattler_networking", version = "0.20.8", default-features = false }
 bzip2 = "0.4.4"
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.21.1](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.21.0...rattler_package_streaming-v0.21.1) - 2024-05-28
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.21.0](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.10...rattler_package_streaming-v0.21.0) - 2024-05-27
 
 ### Other
 - introducing the installer ([#664](https://github.com/mamba-org/rattler/pull/664))
 
 ## [0.20.10](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.9...rattler_package_streaming-v0.20.10) - 2024-05-14
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/fs.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/fs.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/read.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/read.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/seek.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/seek.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/fs.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/fs.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/write.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/write.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/tests/extract.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/tests/extract.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/tests/write.rs` & `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/tests/write.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_lock/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [package]
 name = "rattler_lock"
-version = "0.22.8"
+version = "0.22.9"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Rust data types for conda lock"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path = "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.0", default-features = false }
 rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false }
 file_url = { path = "../file_url", version = "0.1.1" }
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
 fxhash = "0.2.1"
 indexmap = { version = "2.2.6", features = ["serde"] }
 itertools = "0.12.1"
-pep508_rs = { version = "0.4.2" , features = ["serde"] }
-pep440_rs = { version = "0.5.0" , features = ["serde"] }
+pep508_rs = { version = "0.6.0" , features = ["serde"] }
+pep440_rs = { version = "0.6.0" , features = ["serde"] }
 serde = { version = "1.0.198" , features = ["derive"] }
 serde_json = { version = "1.0.116" }
 serde_yaml = "0.9.34"
 serde_with = { version = "3.7.0", features = ["indexmap_2"] }
 serde_repr = "0.1"
 thiserror = "1.0"
 url = { version = "2.5.0" , features = ["serde"] }
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_lock/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.22.9](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.8...rattler_lock-v0.22.9) - 2024-05-28
+
+### Added
+- add run exports to package data ([#671](https://github.com/mamba-org/rattler/pull/671))
+
+### Other
+- bump ([#683](https://github.com/mamba-org/rattler/pull/683))
+
 ## [0.22.8](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.7...rattler_lock-v0.22.8) - 2024-05-27
 
 ### Added
 - removed Ord and more ([#673](https://github.com/mamba-org/rattler/pull/673))
 - always store purls as a key in lock file ([#669](https://github.com/mamba-org/rattler/pull/669))
 
 ## [0.22.7](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.6...rattler_lock-v0.22.7) - 2024-05-14
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/builder.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/builder.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/channel.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/channel.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/conda.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/conda.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/file_format_version.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/file_format_version.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/hash.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/hash.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/deserialize.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/deserialize.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/serialize.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/serialize.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/v3.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/v3.rs`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,15 @@
                             sha256,
                             size: value.size,
                             subdir: value.subdir.unwrap_or(platform.to_string()),
                             timestamp: value.timestamp,
                             track_features: value.track_features,
                             version: value.version,
                             purls: value.purls.is_empty().not().then_some(value.purls),
+                            run_exports: None,
                         },
                         url: value.url,
                         file_name: None,
                         channel: None,
                     })
                     .0;
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/pypi.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/pypi.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/pypi_indexes.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/pypi_indexes.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/url_or_path.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/url_or_path.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/ordered.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/ordered.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                         extras: Vec::new(),
                         version_or_url: if spec.is_empty() {
                             None
                         } else {
                             Some(VersionOrUrl::VersionSpecifier(spec))
                         },
                         marker: None,
+                        origin: None,
                     })
                 })
                 .collect::<Result<Vec<_>, _>>()
                 .map_err(serde::de::Error::custom)?,
         })
     }
 }
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,15 @@
                 purls: value.purls.into_owned(),
                 sha256: value.sha256,
                 size: value.size.into_owned(),
                 subdir: value.subdir.into_owned(),
                 timestamp: value.timestamp,
                 track_features: value.track_features.into_owned(),
                 version: value.version.into_owned(),
+                run_exports: None,
             },
             url: value.url.into_owned(),
             file_name: value.file_name.into_owned(),
             channel: value.channel.into_owned(),
         }
     }
 }
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs` & `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/simple_spawn_blocking/src/tokio.rs` & `py_rattler-0.6.1/local_dependencies/simple_spawn_blocking/src/tokio.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "rattler_repodata_gateway"
-version = "0.20.2"
+version = "0.20.3"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "A crate to interact with Conda repodata"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
 file_url = { path = "../file_url", version = "0.1.1" }
-rattler_conda_types = { path = "../rattler_conda_types", version = "0.24.0", default-features = false, optional = true }
+rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.0", default-features = false, optional = true }
 rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false, features = ["tokio", "serde"] }
 rattler_networking = { path = "../rattler_networking", version = "0.20.8", default-features = false }
 simple_spawn_blocking = { path = "../simple_spawn_blocking", version = "1.0", features = ["tokio"] }
 anyhow = "1.0.82"
 async-compression = { version = "0.4.8", features = [
     "gzip",
     "tokio",
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.20.3](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.20.2...rattler_repodata_gateway-v0.20.3) - 2024-05-28
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_conda_types
+
 ## [0.20.2](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.20.1...rattler_repodata_gateway-v0.20.2) - 2024-05-27
 
 ### Fixed
 - result grouped by subdir instead of channel ([#666](https://github.com/mamba-org/rattler/pull/666))
 
 ### Other
 - introducing the installer ([#664](https://github.com/mamba-org/rattler/pull/664))
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/reporter.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/reporter.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/body.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/body.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs` & `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_macros/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_macros/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_macros/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_macros/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_virtual_packages"
-version = "0.19.12"
+version = "0.19.13"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Library to work with and detect Conda virtual packages"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
 libloading = "0.8.3"
 nom = "7.1.3"
 once_cell = "1.19.0"
 regex = "1.10.4"
 serde = { version = "1.0.198" , features = ["derive"] }
 thiserror = "1.0"
 tracing = "0.1.40"
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.19.13](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.12...rattler_virtual_packages-v0.19.13) - 2024-05-28
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.19.12](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.11...rattler_virtual_packages-v0.19.12) - 2024-05-27
 
 ### Other
 - updated the following local packages: rattler_conda_types
 
 ## [0.19.11](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.10...rattler_virtual_packages-v0.19.11) - 2024-05-14
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/cuda.rs` & `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/cuda.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/libc.rs` & `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/libc.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/linux.rs` & `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/linux.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/osx.rs` & `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/osx.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/file_url/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/file_url/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rattler"
-version = "0.26.0"
+version = "0.26.1"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Rust library to install conda environments"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
@@ -15,19 +15,19 @@
 default = ['native-tls']
 native-tls = ['reqwest/native-tls', 'rattler_package_streaming/native-tls']
 rustls-tls = ['reqwest/rustls-tls', 'rattler_package_streaming/rustls-tls']
 cli-tools = ['dep:clap']
 indicatif = ['dep:indicatif', 'dep:console']
 
 [dependencies]
-rattler_conda_types = { path = "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.0", default-features = false }
 rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false }
 rattler_networking = { path = "../rattler_networking", version = "0.20.8", default-features = false }
-rattler_shell = { path = "../rattler_shell", version = "0.20.5", default-features = false }
-rattler_package_streaming = { path = "../rattler_package_streaming", version = "0.21.0", default-features = false, features = ["reqwest"] }
+rattler_shell = { path = "../rattler_shell", version = "0.20.6", default-features = false }
+rattler_package_streaming = { path = "../rattler_package_streaming", version = "0.21.1", default-features = false, features = ["reqwest"] }
 simple_spawn_blocking = { path = "../simple_spawn_blocking", version = "1.0", default-features = false, features = ["tokio"] }
 anyhow = "1.0.82"
 bytes = "1.6.0"
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.26.1](https://github.com/mamba-org/rattler/compare/rattler-v0.26.0...rattler-v0.26.1) - 2024-05-28
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.26.0](https://github.com/mamba-org/rattler/compare/rattler-v0.25.0...rattler-v0.26.0) - 2024-05-27
 
 ### Fixed
 - improve progress bar duration display ([#680](https://github.com/mamba-org/rattler/pull/680))
 
 ### Other
 - introducing the installer ([#664](https://github.com/mamba-org/rattler/pull/664))
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/resources/launcher64.exe` & `py_rattler-0.6.1/local_dependencies/rattler/resources/launcher64.exe`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/resources/versions.txt` & `py_rattler-0.6.1/local_dependencies/rattler/resources/versions.txt`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/cli/auth.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/cli/auth.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/apple_codesign.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/apple_codesign.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/clobber_registry.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/clobber_registry.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/driver.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/driver.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/entry_point.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/entry_point.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/error.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/error.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/indicatif.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/indicatif.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/reporter.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/reporter.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/link.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/link.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/link_script.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/link_script.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/python.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/python.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/test_utils.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/test_utils.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/transaction.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/transaction.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/install/unlink.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/install/unlink.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/package_cache.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/package_cache.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/range.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/range.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler/src/validation.rs` & `py_rattler-0.6.1/local_dependencies/rattler/src/validation.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_index/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_solve/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,40 @@
 [package]
-name = "rattler_index"
-version = "0.19.13"
+name = "rattler_solve"
+version = "0.23.1"
 edition= "2021"
-authors = []
-description = "A crate that indexes directories containing conda packages to create local conda channels"
+authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
+description = "A crate to solve conda environments"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
 rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
-rattler_package_streaming = { path= "../rattler_package_streaming", version = "0.21.0", default-features = false }
-fs-err = "2.11.0"
-serde_json = { version = "1.0.116" }
+rattler_libsolv_c = { path= "../rattler_libsolv_c", version = "0.19.3", default-features = false, optional = true }
+libc = { version = "0.2" , optional = true }
+chrono = { version = "0.4.38", default-features = false, features = [
+    "std",
+    "serde",
+    "alloc",
+] }
+thiserror = "1.0"
 tracing = "0.1.40"
-walkdir = "2.5.0"
+itertools = "0.12.1"
+url = { version = "2.5.0" }
+tempfile = "3.10.1"
+resolvo = { version = "0.4.1" , optional = true }
+futures = { version = "0.3.30", optional = true }
+serde = { version = "1.0.198" , optional = true }
+
+[features]
+default = ["resolvo"]
+libsolv_c = ["rattler_libsolv_c", "libc"]
+resolvo = ["dep:resolvo", "dep:futures"]
+
+[[bench]]
+name = "bench"
+harness = false
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_index/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_index/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.19.14](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.13...rattler_index-v0.19.14) - 2024-05-28
+
+### Added
+- add run exports to package data ([#671](https://github.com/mamba-org/rattler/pull/671))
+
 ## [0.19.13](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.12...rattler_index-v0.19.13) - 2024-05-27
 
 ### Added
 - always store purls as a key in lock file ([#669](https://github.com/mamba-org/rattler/pull/669))
 
 ## [0.19.12](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.11...rattler_index-v0.19.12) - 2024-05-14
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_index/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_index/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         noarch: index.noarch,
         license: index.license,
         license_family: index.license_family,
         timestamp: index.timestamp,
         legacy_bz2_md5: None,
         legacy_bz2_size: None,
         purls: None,
+        run_exports: None,
     };
+
     Ok(package_record)
 }
 
 fn package_record_from_tar_bz2(file: &Path) -> Result<PackageRecord, std::io::Error> {
     let reader = std::fs::File::open(file)?;
     let mut archive = read::stream_tar_bz2(reader);
     for entry in archive.entries()?.flatten() {
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_index/tests/test_index.rs` & `py_rattler-0.6.1/local_dependencies/rattler_index/tests/test_index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 [package]
-name = "rattler_solve"
-version = "0.23.0"
+name = "rattler_conda_types"
+version = "0.25.0"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
-description = "A crate to solve conda environments"
+description = "Rust data types for common types used within the Conda ecosystem"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
-rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
-rattler_libsolv_c = { path= "../rattler_libsolv_c", version = "0.19.3", default-features = false, optional = true }
-libc = { version = "0.2" , optional = true }
+file_url = { path = "../file_url", version = "0.1.1" }
+rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false, features = ["serde"] }
+rattler_macros = { path = "../rattler_macros", version = "0.19.3", default-features = false }
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
+fxhash = "0.2.1"
+glob = "0.3.1"
+hex = "0.4.3"
+itertools = "0.12.1"
+lazy-regex = "3.1.0"
+nom = "7.1.3"
+purl = { version = "0.1.2", features = ["serde","serde"] }
+regex = "1.10.4"
+serde = { version = "1.0.198" , features = ["derive", "rc"] }
+serde_json = { version = "1.0.116" }
+serde_repr = "0.1"
+serde_with = { version = "3.7.0", features = ["indexmap_2"] }
+smallvec = { version = "1.13.2", features = [
+    "serde",
+    "const_new",
+    "const_generics",
+    "union","serde", "const_new", "const_generics", "union",
+] }
+strum = { version = "0.26.2", features = ["derive","derive"] }
 thiserror = "1.0"
 tracing = "0.1.40"
-itertools = "0.12.1"
-url = { version = "2.5.0" }
-tempfile = "3.10.1"
-resolvo = { version = "0.4.1" , optional = true }
-futures = { version = "0.3.30", optional = true }
-
-[features]
-default = ["resolvo"]
-libsolv_c = ["rattler_libsolv_c", "libc"]
-resolvo = ["dep:resolvo", "dep:futures"]
+typed-path = { version = "0.8.0" }
+url = { version = "2.5.0" , features = ["serde"] }
 
 [[bench]]
-name = "bench"
+name = "parse"
 harness = false
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_solve/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.23.1](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.23.0...rattler_solve-v0.23.1) - 2024-05-28
+
+### Added
+- add run exports to package data ([#671](https://github.com/mamba-org/rattler/pull/671))
+
+### Other
+- enable serialization of enums ([#698](https://github.com/mamba-org/rattler/pull/698))
+
 ## [0.23.0](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.22.0...rattler_solve-v0.23.0) - 2024-05-27
 
 ### Added
 - removed Ord and more ([#673](https://github.com/mamba-org/rattler/pull/673))
 - always store purls as a key in lock file ([#669](https://github.com/mamba-org/rattler/pull/669))
 - add solve strategies ([#660](https://github.com/mamba-org/rattler/pull/660))
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/benches/bench.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -77,14 +77,16 @@
             }
         }
     }
 }
 
 /// Represents the channel priority option to use during solves.
 #[derive(Clone, Copy, PartialEq, Eq, Default)]
+#[cfg_attr(feature = "serde", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "serde", serde(rename_all = "kebab-case"))]
 pub enum ChannelPriority {
     /// The channel that the package is first found in will be used as the only
     /// channel for that package.
     #[default]
     Strict,
 
     // Conda also has "Flexible" as an option, where packages present in multiple channels
@@ -160,14 +162,16 @@
             strategy: SolveStrategy::default(),
         }
     }
 }
 
 /// Represents the strategy to use when solving dependencies
 #[derive(Debug, Clone, Copy, Default, Eq, PartialEq)]
+#[cfg_attr(feature = "serde", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "serde", serde(rename_all = "kebab-case"))]
 pub enum SolveStrategy {
     /// Resolve the highest version of each package.
     #[default]
     Highest,
 
     /// Resolve the lowest compatible version for each package.
     ///
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/input.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/input.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/output.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/output.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/resolvo/conda_util.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/resolvo/conda_util.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/src/resolvo/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/src/resolvo/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/backends.rs` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/backends.rs`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
             noarch: NoArchType::default(),
             license: None,
             license_family: None,
             timestamp: None,
             legacy_bz2_size: None,
             legacy_bz2_md5: None,
             purls: None,
+            run_exports: None,
         },
     }
 }
 
 fn solve_real_world<T: SolverImpl + Default>(specs: Vec<&str>) -> Vec<String> {
     let specs = specs
         .iter()
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap` & `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_digest/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_digest/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_digest/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_digest/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_digest/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_digest/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_digest/src/serde.rs` & `py_rattler-0.6.1/local_dependencies/rattler_digest/src/serde.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_digest/src/tokio.rs` & `py_rattler-0.6.1/local_dependencies/rattler_digest/src/tokio.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_networking/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_networking/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_middleware.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/storage.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/storage.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/gcs_middleware.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/gcs_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/mirror_middleware.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/mirror_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/oci_middleware.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/oci_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/redaction.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/redaction.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_networking/src/retry_policies.rs` & `py_rattler-0.6.1/local_dependencies/rattler_networking/src/retry_policies.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/CHANGELOG.md` & `py_rattler-0.6.1/local_dependencies/rattler_shell/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,93 +2,76 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.24.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.23.1...rattler_conda_types-v0.24.0) - 2024-05-27
+## [0.20.6](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.5...rattler_shell-v0.20.6) - 2024-05-28
 
-### Added
-- removed Ord and more ([#673](https://github.com/mamba-org/rattler/pull/673))
-- always store purls as a key in lock file ([#669](https://github.com/mamba-org/rattler/pull/669))
-- add solve strategies ([#660](https://github.com/mamba-org/rattler/pull/660))
+### Other
+- updated the following local packages: rattler_conda_types
 
-### Fixed
-- make topological sorting support fully cyclic dependencies ([#678](https://github.com/mamba-org/rattler/pull/678))
+## [0.20.5](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.4...rattler_shell-v0.20.5) - 2024-05-27
 
-## [0.23.1](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.23.0...rattler_conda_types-v0.23.1) - 2024-05-14
+### Other
+- updated the following local packages: rattler_conda_types
+
+## [0.20.4](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.3...rattler_shell-v0.20.4) - 2024-05-14
 
 ### Added
 - exclude repodata records based on timestamp ([#654](https://github.com/mamba-org/rattler/pull/654))
 
-## [0.23.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.22.1...rattler_conda_types-v0.23.0) - 2024-05-13
-
-### Added
-- high level repodata access ([#560](https://github.com/mamba-org/rattler/pull/560))
+## [0.20.3](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.2...rattler_shell-v0.20.3) - 2024-05-13
 
 ### Other
-- update README.md
-
-## [0.22.1](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.22.0...rattler_conda_types-v0.22.1) - 2024-05-06
+- updated the following local packages: rattler_conda_types
 
-### Added
-- expose `*Record.noarch` in Python bindings ([#635](https://github.com/mamba-org/rattler/pull/635))
+## [0.20.2](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.1...rattler_shell-v0.20.2) - 2024-05-06
 
-## [0.22.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.21.0...rattler_conda_types-v0.22.0) - 2024-04-25
+### Other
+- updated the following local packages: rattler_conda_types
 
-### Added
-- add support for extracting prefix placeholder data to PathsEntry ([#614](https://github.com/mamba-org/rattler/pull/614))
+## [0.20.1](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.0...rattler_shell-v0.20.1) - 2024-04-25
 
-## [0.21.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.20.5...rattler_conda_types-v0.21.0) - 2024-04-19
+### Fixed
+- compare `UrlOrPath` ([#618](https://github.com/mamba-org/rattler/pull/618))
 
-### Added
-- make root dir configurable in channel config ([#602](https://github.com/mamba-org/rattler/pull/602))
+## [0.20.0](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.19.6...rattler_shell-v0.20.0) - 2024-04-19
 
 ### Fixed
-- better value for `link` field ([#610](https://github.com/mamba-org/rattler/pull/610))
-
-### Other
-- update dependencies incl. reqwest ([#606](https://github.com/mamba-org/rattler/pull/606))
+- unicode activation issues on windows ([#604](https://github.com/mamba-org/rattler/pull/604))
 
-## [0.20.5](https://github.com/baszalmstra/rattler/compare/rattler_conda_types-v0.20.4...rattler_conda_types-v0.20.5) - 2024-04-05
+## [0.19.6](https://github.com/baszalmstra/rattler/compare/rattler_shell-v0.19.5...rattler_shell-v0.19.6) - 2024-04-05
 
 ### Fixed
 - run post-link scripts ([#574](https://github.com/baszalmstra/rattler/pull/574))
 
-## [0.20.4](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.20.3...rattler_conda_types-v0.20.4) - 2024-03-30
+## [0.19.5](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.19.4...rattler_shell-v0.19.5) - 2024-03-30
 
-### Fixed
-- matchspec empty namespace and channel cannonical name ([#582](https://github.com/mamba-org/rattler/pull/582))
+### Other
+- updated the following local packages: rattler_conda_types
 
-## [0.20.3](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.20.2...rattler_conda_types-v0.20.3) - 2024-03-21
+## [0.19.4](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.19.3...rattler_shell-v0.19.4) - 2024-03-21
 
-### Fixed
-- allow not starts with in strict mode ([#577](https://github.com/mamba-org/rattler/pull/577))
+### Other
+- updated the following local packages: rattler_conda_types
 
-## [0.20.2](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.20.1...rattler_conda_types-v0.20.2) - 2024-03-14
+## [0.19.3](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.19.2...rattler_shell-v0.19.3) - 2024-03-14
 
 ### Other
 - add pixi badge ([#563](https://github.com/mamba-org/rattler/pull/563))
 
-## [0.20.1](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.20.0...rattler_conda_types-v0.20.1) - 2024-03-08
+## [0.19.2](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.19.1...rattler_shell-v0.19.2) - 2024-03-08
 
 ### Fixed
-- chrono deprecation warnings ([#558](https://github.com/mamba-org/rattler/pull/558))
-
-## [0.20.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.19.0...rattler_conda_types-v0.20.0) - 2024-03-06
+- better handle utf8 paths in CmdExe and Powershell ([#561](https://github.com/mamba-org/rattler/pull/561))
 
-### Added
-- [**breaking**] optional strict parsing of matchspec and versionspec ([#552](https://github.com/mamba-org/rattler/pull/552))
+## [0.19.1](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.19.0...rattler_shell-v0.19.1) - 2024-03-06
 
 ### Fixed
-- patch unsupported glob operators ([#551](https://github.com/mamba-org/rattler/pull/551))
 - dont use workspace dependencies for local crates ([#546](https://github.com/mamba-org/rattler/pull/546))
 
 ### Other
 - every crate should have its own version ([#557](https://github.com/mamba-org/rattler/pull/557))
 
-## [0.19.0](https://github.com/baszalmstra/rattler/compare/rattler_conda_types-v0.18.0...rattler_conda_types-v0.19.0) - 2024-02-26
-
-### Fixed
-- Fix arch for osx-arm64 and win-arm64 ([#528](https://github.com/baszalmstra/rattler/pull/528))
-- Channel name display ([#531](https://github.com/baszalmstra/rattler/pull/531))
+## [0.19.0](https://github.com/baszalmstra/rattler/compare/rattler_shell-v0.18.0...rattler_shell-v0.19.0) - 2024-02-26
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/benches/parse.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/benches/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/build_spec/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/build_spec/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/build_spec/parse.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/build_spec/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/channel/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/channel/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/channel_data.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/channel_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/lib.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 pub use repo_data::{
     compute_package_url, ChannelInfo, ConvertSubdirError, PackageRecord, RepoData,
 };
 pub use repo_data_record::RepoDataRecord;
 pub use run_export::RunExportKind;
 pub use version::{
     Component, ParseVersionError, ParseVersionErrorKind, StrictVersion, Version, VersionBumpError,
-    VersionBumpType, VersionWithSource,
+    VersionBumpType, VersionExtendError, VersionWithSource,
 };
 pub use version_spec::VersionSpec;
 
 #[cfg(test)]
 use std::path::{Path, PathBuf};
 
 /// An package identifier that can be used to identify packages across package ecosystems.
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/parse.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/parse.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,40 @@
-use super::matcher::{StringMatcher, StringMatcherParseError};
-use super::MatchSpec;
-use crate::build_spec::{BuildNumberSpec, ParseBuildNumberSpecError};
-use crate::package::ArchiveType;
-use crate::version_spec::version_tree::{recognize_constraint, recognize_version};
-use crate::version_spec::{is_start_of_version_constraint, ParseVersionSpecError};
-use crate::{
-    Channel, ChannelConfig, InvalidPackageNameError, NamelessMatchSpec, PackageName,
-    ParseChannelError, ParseStrictness, VersionSpec,
+use std::{borrow::Cow, path::PathBuf, str::FromStr};
+
+use nom::{
+    branch::alt,
+    bytes::complete::{tag, take_till1, take_until, take_while, take_while1},
+    character::complete::{char, multispace0, one_of},
+    combinator::{opt, recognize},
+    error::{context, ContextError, ParseError},
+    multi::{separated_list0, separated_list1},
+    sequence::{delimited, preceded, separated_pair, terminated},
+    Finish, IResult,
 };
-use nom::branch::alt;
-use nom::bytes::complete::{tag, take_till1, take_until, take_while, take_while1};
-use nom::character::complete::{char, multispace0, one_of};
-use nom::combinator::{opt, recognize};
-use nom::error::{context, ContextError, ParseError};
-use nom::multi::{separated_list0, separated_list1};
-use nom::sequence::{delimited, preceded, separated_pair, terminated};
-use nom::{Finish, IResult};
 use rattler_digest::{parse_digest_from_hex, Md5, Sha256};
 use smallvec::SmallVec;
-use std::borrow::Cow;
-use std::path::PathBuf;
-use std::str::FromStr;
 use thiserror::Error;
 use url::Url;
 
+use super::{
+    matcher::{StringMatcher, StringMatcherParseError},
+    MatchSpec,
+};
+use crate::{
+    build_spec::{BuildNumberSpec, ParseBuildNumberSpecError},
+    package::ArchiveType,
+    version_spec::{
+        is_start_of_version_constraint,
+        version_tree::{recognize_constraint, recognize_version},
+        ParseVersionSpecError,
+    },
+    Channel, ChannelConfig, InvalidPackageNameError, NamelessMatchSpec, PackageName,
+    ParseChannelError, ParseStrictness, VersionSpec,
+};
+
 /// The type of parse error that occurred when parsing match spec.
 #[derive(Debug, Clone, Error)]
 pub enum ParseMatchSpecError {
     /// The path or url of the package was invalid
     #[error("invalid package path or url")]
     InvalidPackagePathOrUrl,
 
@@ -94,41 +101,42 @@
         source: &str,
         strictness: ParseStrictness,
     ) -> Result<Self, ParseMatchSpecError> {
         matchspec_parser(source, strictness)
     }
 }
 
-/// Strips a comment from a match spec. A comment is preceded by a '#' followed by the comment
-/// itself. This functions splits the matchspec into the matchspec and comment part.
+/// Strips a comment from a match spec. A comment is preceded by a '#' followed
+/// by the comment itself. This functions splits the matchspec into the
+/// matchspec and comment part.
 fn strip_comment(input: &str) -> (&str, Option<&str>) {
     input
         .split_once('#')
         .map_or_else(|| (input, None), |(spec, comment)| (spec, Some(comment)))
 }
 
-/// Strips any if statements from the matchspec. `if` statements in matchspec are "anticipating
-/// future compatibility issues".
+/// Strips any if statements from the matchspec. `if` statements in matchspec
+/// are "anticipating future compatibility issues".
 fn strip_if(input: &str) -> (&str, Option<&str>) {
     // input
     //     .split_once("if")
     //     .map(|(spec, if_statement)| (spec, Some(if_statement)))
     //     .unwrap_or_else(|| (input, None))
     (input, None)
 }
 
 /// Returns true if the specified string represents a package path.
 fn is_package_file(input: &str) -> bool {
     ArchiveType::try_from(input).is_some()
 }
 
-/// An optimized data structure to store key value pairs in between a bracket string
-/// `[key1=value1, key2=value2]`. The optimization stores two such values on the stack and otherwise
-/// allocates a vector on the heap. Two is chosen because that seems to be more than enough for
-/// most use cases.
+/// An optimized data structure to store key value pairs in between a bracket
+/// string `[key1=value1, key2=value2]`. The optimization stores two such values
+/// on the stack and otherwise allocates a vector on the heap. Two is chosen
+/// because that seems to be more than enough for most use cases.
 type BracketVec<'a> = SmallVec<[(&'a str, &'a str); 2]>;
 
 /// A parse combinator to filter whitespace if front and after another parser.
 fn whitespace_enclosed<'a, F, O, E: ParseError<&'a str>>(
     mut inner: F,
 ) -> impl FnMut(&'a str) -> IResult<&'a str, O, E>
 where
@@ -180,16 +188,16 @@
 
     match parse_bracket_list(input).finish() {
         Ok((_remaining, values)) => Ok(values.into()),
         Err(nom::error::Error { .. }) => Err(ParseMatchSpecError::InvalidBracket),
     }
 }
 
-/// Strips the brackets part of the matchspec returning the rest of the matchspec and  the contents
-/// of the brackets as a `Vec<&str>`.
+/// Strips the brackets part of the matchspec returning the rest of the
+/// matchspec and  the contents of the brackets as a `Vec<&str>`.
 fn strip_brackets(input: &str) -> Result<(Cow<'_, str>, BracketVec<'_>), ParseMatchSpecError> {
     if let Some(matches) = lazy_regex::regex!(r#".*(?:(\[.*\]))"#).captures(input) {
         let bracket_str = matches.get(1).unwrap().as_str();
         let bracket_contents = parse_bracket_list(bracket_str)?;
 
         let input = if let Some(input) = input.strip_suffix(bracket_str) {
             Cow::Borrowed(input)
@@ -271,15 +279,15 @@
     fn parse_special_equality<'a, E: ParseError<&'a str> + ContextError<&'a str>>(
         input: &'a str,
     ) -> IResult<&'a str, &'a str, E> {
         // Matches ".*" or "*" but not "."
         let version_glob = terminated(opt(tag(".")), tag("*"));
 
         // Matches a version followed by an optional version glob
-        let version_followed_by_glob = terminated(recognize_version, opt(version_glob));
+        let version_followed_by_glob = terminated(recognize_version(true), opt(version_glob));
 
         // Just matches the glob operator ("*")
         let just_star = tag("*");
 
         recognize(preceded(
             tag("="),
             alt((version_followed_by_glob, just_star)),
@@ -452,21 +460,22 @@
             Cow::Borrowed(version_str)
         };
 
         // Special case handling for version strings that start with `=`.
         let version_str = if let (Some(version_str), true) =
             (version_str.strip_prefix("=="), build_str.is_none())
         {
-            // If the version starts with `==` and the build string is none we strip the `==` part.
+            // If the version starts with `==` and the build string is none we strip the
+            // `==` part.
             Cow::Borrowed(version_str)
         } else if let Some(version_str_part) = version_str.strip_prefix('=') {
             let not_a_group = !version_str_part.contains(['=', ',', '|']);
             if not_a_group {
-                // If the version starts with `=`, is not part of a group (e.g. 1|2) we append a *
-                // if it doesnt have one already.
+                // If the version starts with `=`, is not part of a group (e.g. 1|2) we append a
+                // * if it doesnt have one already.
                 if build_str.is_none() && !version_str_part.ends_with('*') {
                     Cow::Owned(format!("{version_str_part}*"))
                 } else {
                     Cow::Borrowed(version_str_part)
                 }
             } else {
                 // Version string is part of a group, return the non-stripped version string
@@ -488,29 +497,29 @@
     }
 
     Ok(match_spec)
 }
 
 #[cfg(test)]
 mod tests {
-    use crate::ParseStrictness::*;
+    use std::{collections::BTreeMap, str::FromStr, sync::Arc};
+
     use assert_matches::assert_matches;
     use rattler_digest::{parse_digest_from_hex, Md5, Sha256};
     use serde::Serialize;
-    use std::collections::BTreeMap;
-    use std::str::FromStr;
-    use std::sync::Arc;
+    use smallvec::smallvec;
 
     use super::{
         split_version_and_build, strip_brackets, strip_package_name, BracketVec, MatchSpec,
         ParseMatchSpecError,
     };
-    use crate::match_spec::parse::parse_bracket_list;
-    use crate::{BuildNumberSpec, Channel, ChannelConfig, NamelessMatchSpec, VersionSpec};
-    use smallvec::smallvec;
+    use crate::{
+        match_spec::parse::parse_bracket_list, BuildNumberSpec, Channel, ChannelConfig,
+        NamelessMatchSpec, ParseStrictness::*, VersionSpec,
+    };
 
     fn channel_config() -> ChannelConfig {
         ChannelConfig::default_with_root_dir(
             std::env::current_dir().expect("Could not get current directory"),
         )
     }
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/no_arch_type.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/no_arch_type.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/about.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/about.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/archive_type.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/archive_type.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/entry_point.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/entry_point.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/files.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/files.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/has_prefix.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/has_prefix.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/index.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/link.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/link.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/no_link.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/no_link.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/no_softlink.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/no_softlink.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/paths.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/paths.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/run_exports.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/run_exports.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,70 @@
 use std::path::Path;
 
-use super::PackageFile;
 use serde::{Deserialize, Serialize};
 use serde_with::{serde_as, skip_serializing_none};
 
+use super::PackageFile;
+
 /// A representation of the `run_exports.json` file found in package archives.
 ///
-/// The `run_exports.json` file contains information about the run exports of a package
+/// The `run_exports.json` file contains information about the run exports of a
+/// package
 #[serde_as]
 #[skip_serializing_none]
-#[derive(Debug, Deserialize, Serialize, Eq, PartialEq, Hash, Clone)]
+#[derive(Debug, Default, Deserialize, Serialize, Eq, PartialEq, Hash, Clone)]
 pub struct RunExportsJson {
     /// weak run exports apply a dependency from host to run
     #[serde(skip_serializing_if = "Vec::is_empty", default)]
     pub weak: Vec<String>,
     /// strong run exports apply a dependency from build to host and run
     #[serde(skip_serializing_if = "Vec::is_empty", default)]
     pub strong: Vec<String>,
-    /// noarch run exports apply a run export only to noarch packages (other run exports are ignored)
-    /// for example, python uses this to apply a dependency on python to all noarch packages, but not to
+    /// noarch run exports apply a run export only to noarch packages (other run
+    /// exports are ignored) for example, python uses this to apply a
+    /// dependency on python to all noarch packages, but not to
     /// the python_abi package
     #[serde(skip_serializing_if = "Vec::is_empty", default)]
     pub noarch: Vec<String>,
-    /// weak constrains apply a constrain dependency from host to build, or run to host
+    /// weak constrains apply a constrain dependency from host to build, or run
+    /// to host
     #[serde(skip_serializing_if = "Vec::is_empty", default)]
     pub weak_constrains: Vec<String>,
-    /// strong constrains apply a constrain dependency from build to host and run
+    /// strong constrains apply a constrain dependency from build to host and
+    /// run
     #[serde(skip_serializing_if = "Vec::is_empty", default)]
     pub strong_constrains: Vec<String>,
 }
 
 impl PackageFile for RunExportsJson {
     fn package_path() -> &'static Path {
         Path::new("info/run_exports.json")
     }
 
     fn from_str(str: &str) -> Result<Self, std::io::Error> {
         serde_json::from_str(str).map_err(Into::into)
     }
 }
 
+impl RunExportsJson {
+    /// Construct an empty `RunExportsJson`
+    pub fn new() -> Self {
+        Self::default()
+    }
+
+    /// Test if all fields are empty
+    pub fn is_empty(&self) -> bool {
+        self.weak.is_empty()
+            && self.strong.is_empty()
+            && self.noarch.is_empty()
+            && self.weak_constrains.is_empty()
+            && self.strong_constrains.is_empty()
+    }
+}
+
 #[cfg(all(unix, test))]
 mod test {
     use super::{PackageFile, RunExportsJson};
 
     #[test]
     pub fn test_reconstruct_run_exports_json_with_symlinks() {
         let package_dir = tempfile::tempdir().unwrap();
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package_name.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/platform.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/platform.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/prefix_record.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/prefix_record.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 use rattler_macros::sorted;
 use serde::{Deserialize, Serialize};
 use serde_with::{serde_as, skip_serializing_none, OneOrMany};
 use thiserror::Error;
 use url::Url;
 
 use crate::{
-    build_spec::BuildNumber, package::IndexJson, utils::serde::DeserializeFromStrUnchecked,
+    build_spec::BuildNumber,
+    package::{IndexJson, RunExportsJson},
+    utils::serde::DeserializeFromStrUnchecked,
     Channel, NoArchType, PackageName, PackageUrl, Platform, RepoDataRecord, VersionWithSource,
 };
 
 /// [`RepoData`] is an index of package binaries available on in a subdirectory
 /// of a Conda channel.
 // Note: we cannot use the sorted macro here, because the `packages` and `conda_packages` fields are
 // serialized in a special way. Therefore we do it manually.
@@ -143,14 +145,18 @@
     /// Now, None:: means that the purl is missing, and it will be tried to
     /// filled in. So later it can be one of the following:
     /// [`Some(vec![])`] means that the purl is empty and package is not pypi
     /// one. [`Some([`PackageUrl`])`] means that it is a pypi package.
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub purls: Option<BTreeSet<PackageUrl>>,
 
+    /// Run exports that are specified in the package.
+    #[serde(default, skip_serializing_if = "Option::is_none")]
+    pub run_exports: Option<RunExportsJson>,
+
     /// Optionally a SHA256 hash of the package archive
     #[serde_as(as = "Option<SerializableHash::<rattler_digest::Sha256>>")]
     pub sha256: Option<Sha256Hash>,
 
     /// Optionally the size of the package archive in bytes
     pub size: Option<u64>,
 
@@ -300,14 +306,15 @@
             sha256: None,
             size: None,
             subdir: Platform::current().to_string(),
             timestamp: None,
             track_features: vec![],
             version: version.into(),
             purls: None,
+            run_exports: None,
         }
     }
 
     /// Sorts the records topologically.
     ///
     /// This function is deterministic, meaning that it will return the same
     /// result regardless of the order of `records` and of the `depends`
@@ -417,14 +424,15 @@
             sha256,
             size,
             subdir,
             timestamp: index.timestamp,
             track_features: index.track_features,
             version: index.version,
             purls: None,
+            run_exports: None,
         })
     }
 }
 
 fn sort_map_alphabetically<T: Serialize, S: serde::Serializer>(
     value: &FxHashMap<String, T>,
     serializer: S,
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/patches.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/patches.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data_record.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data_record.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/utils/serde.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/utils/serde.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/flags.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/flags.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 pub(crate) mod bump;
 pub use bump::{VersionBumpError, VersionBumpType};
 
 use flags::Flags;
 use segment::Segment;
 
+use thiserror::Error;
 pub use with_source::VersionWithSource;
 
 /// This class implements an order relation between version strings. Version strings can contain the
 /// usual alphanumeric characters (A-Za-z0-9), separated into segments by dots and underscores.
 /// Empty segments (i.e. two consecutive dots, a leading/trailing underscore) are not permitted. An
 /// optional epoch number - an integer followed by '!' - can precede the actual version string (this
 /// is useful to indicate a change in the versioning scheme itself). Version comparison is
@@ -164,14 +165,23 @@
     /// no local version.
     flags: Flags,
 }
 
 type ComponentVec = SmallVec<[Component; 3]>;
 type SegmentVec = SmallVec<[Segment; 4]>;
 
+/// Error that can occur when extending a version to a certain length.
+#[derive(Error, Debug, PartialEq)]
+
+pub enum VersionExtendError {
+    /// The version is too long (there is a maximum number of segments allowed)
+    #[error("the version is too long")]
+    VersionTooLong,
+}
+
 impl Version {
     /// Constructs a version with just a major component and no other components, e.g. "1".
     pub fn major(major: u64) -> Version {
         Version {
             components: smallvec::smallvec![Component::Numeral(major)],
             segments: smallvec::smallvec![Segment::new(1).unwrap()],
             flags: Flags(0),
@@ -235,133 +245,14 @@
                 offset: start,
                 version: self,
                 segment,
             }
         })
     }
 
-    /// Returns a new version after bumping it according to the specified bump type.
-    pub fn bump(&self, bump_type: VersionBumpType) -> Result<Self, VersionBumpError> {
-        let mut components = ComponentVec::new();
-        let mut segments = SegmentVec::new();
-        let mut flags = Flags::default();
-
-        // Copy the optional epoch.
-        if let Some(epoch) = self.epoch_opt() {
-            components.push(Component::Numeral(epoch));
-            flags = flags.with_has_epoch(true);
-        }
-
-        // Sanity check whether the version has enough segments for this bump type.
-        let segment_count = self.segment_count();
-        match bump_type {
-            VersionBumpType::Major => {
-                if segment_count < 1 {
-                    return Err(VersionBumpError::NoMajorSegment);
-                }
-            }
-            VersionBumpType::Minor => {
-                if segment_count < 2 {
-                    return Err(VersionBumpError::NoMinorSegment);
-                }
-            }
-            VersionBumpType::Patch => {
-                if segment_count < 3 {
-                    return Err(VersionBumpError::NoPatchSegment);
-                }
-            }
-            VersionBumpType::Last => {
-                if segment_count == 0 {
-                    return Err(VersionBumpError::NoLastSegment);
-                }
-            }
-            VersionBumpType::Segment(index) => {
-                let uindex = if index < 0 {
-                    segment_count as i32 + index
-                } else {
-                    index
-                };
-
-                if uindex < 0 || uindex >= segment_count as i32 {
-                    return Err(VersionBumpError::InvalidSegment { index });
-                }
-            }
-        }
-
-        // Copy over all the segments and bump the last segment.
-        let segment_count = self.segment_count();
-        for (idx, segment_iter) in self.segments().enumerate() {
-            let segment = segment_iter.segment;
-
-            let mut segment_components =
-                segment_iter.components().cloned().collect::<ComponentVec>();
-
-            // Determine whether this is the segment that needs to be bumped.
-            let is_segment_to_bump = match bump_type {
-                VersionBumpType::Major => idx == 0,
-                VersionBumpType::Minor => idx == 1,
-                VersionBumpType::Patch => idx == 2,
-                VersionBumpType::Last => idx == (segment_count - 1),
-                VersionBumpType::Segment(mut index_to_bump) => {
-                    if index_to_bump < 0 {
-                        index_to_bump += segment_count as i32;
-                    }
-
-                    idx == index_to_bump as usize
-                }
-            };
-
-            // Bump the segment if we need to. Each segment must at least start with a number so this should always work.
-            if is_segment_to_bump {
-                let last_numeral_component = segment_components
-                    .iter_mut()
-                    .filter_map(Component::as_number_mut)
-                    .next_back()
-                    .expect("every segment must at least contain a single numeric component");
-                *last_numeral_component += 1;
-            }
-
-            let has_implicit_default =
-                segment.has_implicit_default() && segment_components[0] == Component::default();
-            let start_idx = usize::from(has_implicit_default);
-
-            let component_count = segment_components.len();
-            for component in segment_components.into_iter().skip(start_idx) {
-                components.push(component);
-            }
-
-            let segment = Segment::new((component_count - start_idx) as _)
-                .expect("there will be no more components than in the previous segment")
-                .with_implicit_default(has_implicit_default)
-                .with_separator(segment.separator())
-                .expect("copying the segment should just work");
-
-            segments.push(segment);
-        }
-
-        if self.has_local() {
-            let segment_idx = segments.len() as u8;
-            for segment_iter in self.local_segments() {
-                for component in segment_iter.components().cloned() {
-                    components.push(component);
-                }
-                segments.push(segment_iter.segment);
-            }
-            flags = flags
-                .with_local_segment_index(segment_idx)
-                .expect("this should never fail because no new segments are added");
-        }
-
-        Ok(Self {
-            components,
-            segments,
-            flags,
-        })
-    }
-
     /// Returns the segments that belong the local part of the version.
     ///
     /// The local part of a a version is the part behind the (optional) `+`. E.g.:
     ///
     /// ```text
     /// 1.2+3.2.1-alpha0
     ///     ^^^^^^^^^^^^ This is the local part of the version
@@ -563,14 +454,59 @@
                 segments,
                 flags,
             })
         } else {
             Cow::Borrowed(self)
         }
     }
+
+    /// Extend the version to the specified length by adding default components (0s).
+    /// If the version is already longer than the specified length it is returned as is.
+    pub fn extend_to_length(&self, length: usize) -> Result<Cow<'_, Version>, VersionExtendError> {
+        if self.segment_count() >= length {
+            return Ok(Cow::Borrowed(self));
+        }
+
+        // copy everything up to local version
+        let mut segments = self.segments[..self.segment_count()].to_vec();
+        let components_end = segments.iter().map(|s| s.len() as usize).sum::<usize>()
+            + usize::from(self.has_epoch());
+        let mut components = self.components.clone()[..components_end].to_vec();
+
+        // unwrap is OK here because these should be fine to construct
+        let segment = Segment::new(1).unwrap().with_separator(Some('.')).unwrap();
+
+        for _ in 0..(length - self.segment_count()) {
+            components.push(Component::Numeral(0));
+            segments.push(segment);
+        }
+
+        // add local version if it exists
+        let flags = if self.has_local() {
+            let flags = self
+                .flags
+                .with_local_segment_index(segments.len() as u8)
+                .ok_or(VersionExtendError::VersionTooLong)?;
+            for segment_iter in self.local_segments() {
+                for component in segment_iter.components().cloned() {
+                    components.push(component);
+                }
+                segments.push(segment_iter.segment);
+            }
+            flags
+        } else {
+            self.flags
+        };
+
+        Ok(Cow::Owned(Version {
+            components: components.into(),
+            segments: segments.into(),
+            flags,
+        }))
+    }
 }
 
 /// Returns true if the specified segments are considered to start with the other segments.
 fn segments_starts_with<
     'a,
     'b,
     A: Iterator<Item = SegmentIter<'a>> + 'a,
@@ -579,15 +515,23 @@
     a: A,
     b: B,
 ) -> bool {
     for ranges in a.zip_longest(b) {
         let (left, right) = match ranges {
             EitherOrBoth::Both(left, right) => (left, right),
             EitherOrBoth::Left(_) => return true,
-            EitherOrBoth::Right(_) => return false,
+            EitherOrBoth::Right(segment) => {
+                // If the segment is zero we can skip it. As long as there are
+                // only zeros, the version is still considered to start with
+                // the other version.
+                if segment.is_zero() {
+                    continue;
+                }
+                return false;
+            }
         };
         for values in left.components().zip_longest(right.components()) {
             if !match values {
                 EitherOrBoth::Both(a, b) => a == b,
                 EitherOrBoth::Left(_) => return true,
                 EitherOrBoth::Right(_) => return false,
             } {
@@ -766,14 +710,30 @@
     pub fn as_number_mut(&mut self) -> Option<&mut u64> {
         match self {
             Component::Numeral(value) => Some(value),
             _ => None,
         }
     }
 
+    /// Returns a component as iden value
+    pub fn as_iden(&self) -> Option<&str> {
+        match self {
+            Component::Iden(value) => Some(value),
+            _ => None,
+        }
+    }
+
+    /// Returns a component as mutable iden value
+    pub fn as_iden_mut(&mut self) -> Option<&mut Box<str>> {
+        match self {
+            Component::Iden(value) => Some(value),
+            _ => None,
+        }
+    }
+
     /// Returns a component as string value.
     #[allow(dead_code)]
     pub fn as_string(&self) -> Option<&str> {
         match self {
             Component::Iden(value) => Some(value.as_ref()),
             _ => None,
         }
@@ -791,14 +751,19 @@
         matches!(self, Component::Dev)
     }
 
     /// Checks whether a component is [`Component::Numeral`]
     pub fn is_numeric(&self) -> bool {
         matches!(self, Component::Numeral(_))
     }
+
+    /// Checks whether the component is a zero.
+    pub fn is_zero(&self) -> bool {
+        matches!(self, Component::Numeral(0))
+    }
 }
 
 impl From<u64> for Component {
     fn from(num: u64) -> Self {
         Component::Numeral(num)
     }
 }
@@ -964,14 +929,19 @@
     offset: usize,
 
     /// The version to which the segment belongs
     version: &'v Version,
 }
 
 impl<'v> SegmentIter<'v> {
+    /// Returns true if the
+    pub fn is_zero(&self) -> bool {
+        self.components().all(Component::is_zero)
+    }
+
     /// Returns true if the first component is an implicit default added while parsing the version.
     /// E.g. `2.a` is represented as `2.0a`. The `0` is added implicitly.
     pub fn has_implicit_default(&self) -> bool {
         self.segment.has_implicit_default()
     }
 
     /// Returns the separator that is found in from of this segment or `None` if this segment was
@@ -1054,16 +1024,17 @@
     use std::cmp::Ordering;
     use std::str::FromStr;
 
     use std::collections::hash_map::DefaultHasher;
     use std::hash::{Hash, Hasher};
 
     use rand::seq::SliceRandom;
+    use rstest::rstest;
 
-    use crate::version::{StrictVersion, VersionBumpError, VersionBumpType};
+    use crate::version::StrictVersion;
 
     use super::Version;
 
     // Tests are inspired by: https://github.com/conda/conda/blob/33a142c16530fcdada6c377486f1c1a385738a96/tests/models/test_version.py
 
     #[test]
     fn valid_versions() {
@@ -1263,39 +1234,14 @@
 
         // Hashing should consider v_1_0 and v_1_0_0 as unequal
         assert_eq!(get_hash(&v_1_0), get_hash(&v_1_0));
         assert_ne!(get_hash(&v_1_0), get_hash(&v_1_0_0));
     }
 
     #[test]
-    fn bump_last() {
-        assert_eq!(
-            Version::from_str("1.1")
-                .unwrap()
-                .bump(VersionBumpType::Last)
-                .unwrap(),
-            Version::from_str("1.2").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("1.1l")
-                .unwrap()
-                .bump(VersionBumpType::Last)
-                .unwrap(),
-            Version::from_str("1.2l").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("5!1.alpha+3.4")
-                .unwrap()
-                .bump(VersionBumpType::Last)
-                .unwrap(),
-            Version::from_str("5!1.1alpha+3.4").unwrap()
-        );
-    }
-
-    #[test]
     fn starts_with() {
         assert!(Version::from_str("1.2.3")
             .unwrap()
             .starts_with(&Version::from_str("1.2").unwrap()));
     }
 
     fn get_hash(spec: &impl Hash) -> u64 {
@@ -1418,167 +1364,25 @@
                 .unwrap()
                 .strip_local()
                 .into_owned(),
             Version::from_str("3!4.5a.6b").unwrap()
         );
     }
 
+    #[rstest]
+    #[case("1", 3, "1.0.0")]
+    #[case("1.2", 3, "1.2.0")]
+    #[case("1.2+3.4", 3, "1.2.0+3.4")]
+    #[case("4!1.2+3.4", 3, "4!1.2.0+3.4")]
+    #[case("4!1.2+3.4", 5, "4!1.2.0.0.0+3.4")]
     #[test]
-    fn bump_major() {
-        assert_eq!(
-            Version::from_str("1.1")
-                .unwrap()
-                .bump(VersionBumpType::Major)
-                .unwrap(),
-            Version::from_str("2.1").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("2.1l")
-                .unwrap()
-                .bump(VersionBumpType::Major)
-                .unwrap(),
-            Version::from_str("3.1l").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("5!1.alpha+3.4")
-                .unwrap()
-                .bump(VersionBumpType::Major)
-                .unwrap(),
-            Version::from_str("5!2.alpha+3.4").unwrap()
-        );
-    }
-
-    #[test]
-    fn bump_minor() {
+    fn extend_to_length(#[case] version: &str, #[case] elements: usize, #[case] expected: &str) {
         assert_eq!(
-            Version::from_str("1.1")
+            Version::from_str(version)
                 .unwrap()
-                .bump(VersionBumpType::Minor)
-                .unwrap(),
-            Version::from_str("1.2").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("2.1l")
-                .unwrap()
-                .bump(VersionBumpType::Minor)
-                .unwrap(),
-            Version::from_str("2.2l").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("5!1.alpha+3.4")
-                .unwrap()
-                .bump(VersionBumpType::Minor)
-                .unwrap(),
-            Version::from_str("5!1.1alpha+3.4").unwrap()
-        );
-    }
-
-    #[test]
-    fn bump_minor_fail() {
-        let err = Version::from_str("1")
-            .unwrap()
-            .bump(VersionBumpType::Minor)
-            .unwrap_err();
-
-        assert_eq!(err, VersionBumpError::NoMinorSegment);
-    }
-
-    #[test]
-    fn bump_patch() {
-        assert_eq!(
-            Version::from_str("1.1.9")
-                .unwrap()
-                .bump(VersionBumpType::Patch)
-                .unwrap(),
-            Version::from_str("1.1.10").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("2.1l.5alpha")
+                .extend_to_length(elements)
                 .unwrap()
-                .bump(VersionBumpType::Patch)
-                .unwrap(),
-            Version::from_str("2.1l.6alpha").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("5!1.8.alpha+3.4")
-                .unwrap()
-                .bump(VersionBumpType::Patch)
-                .unwrap(),
-            Version::from_str("5!1.8.1alpha+3.4").unwrap()
-        );
-    }
-
-    #[test]
-    fn bump_patch_fail() {
-        let err = Version::from_str("1.3")
-            .unwrap()
-            .bump(VersionBumpType::Patch)
-            .unwrap_err();
-
-        assert_eq!(err, VersionBumpError::NoPatchSegment);
-    }
-
-    #[test]
-    fn bump_segment() {
-        // Positive index
-        assert_eq!(
-            Version::from_str("1.1.9")
-                .unwrap()
-                .bump(VersionBumpType::Segment(0))
-                .unwrap(),
-            Version::from_str("2.1.9").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("1.1.9")
-                .unwrap()
-                .bump(VersionBumpType::Segment(1))
-                .unwrap(),
-            Version::from_str("1.2.9").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("1.1.9")
-                .unwrap()
-                .bump(VersionBumpType::Segment(2))
-                .unwrap(),
-            Version::from_str("1.1.10").unwrap()
-        );
-        // Negative index
-        assert_eq!(
-            Version::from_str("1.1.9")
-                .unwrap()
-                .bump(VersionBumpType::Segment(-1))
-                .unwrap(),
-            Version::from_str("1.1.10").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("1.1.9")
-                .unwrap()
-                .bump(VersionBumpType::Segment(-2))
-                .unwrap(),
-            Version::from_str("1.2.9").unwrap()
-        );
-        assert_eq!(
-            Version::from_str("1.1.9")
-                .unwrap()
-                .bump(VersionBumpType::Segment(-3))
-                .unwrap(),
-            Version::from_str("2.1.9").unwrap()
+                .to_string(),
+            expected
         );
     }
-
-    #[test]
-    fn bump_segment_fail() {
-        let err = Version::from_str("1.3")
-            .unwrap()
-            .bump(VersionBumpType::Segment(3))
-            .unwrap_err();
-
-        assert_eq!(err, VersionBumpError::InvalidSegment { index: 3 });
-
-        let err = Version::from_str("1.3")
-            .unwrap()
-            .bump(VersionBumpType::Segment(-3))
-            .unwrap_err();
-
-        assert_eq!(err, VersionBumpError::InvalidSegment { index: -3 });
-    }
 }
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/parse.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/segment.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/segment.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/with_source.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/with_source.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs`

 * *Files 1% similar despite different names*

```diff
@@ -270,18 +270,14 @@
         assert_eq!(
             Constraint::from_str("1.2.*", strictness),
             Ok(Constraint::StrictComparison(
                 StrictRangeOperator::StartsWith,
                 Version::from_str("1.2").unwrap(),
             ))
         );
-        assert_eq!(
-            Constraint::from_str("1.2.*.*", strictness),
-            Err(ParseConstraintError::RegexConstraintsNotSupported)
-        );
     }
 
     #[rstest]
     fn test_exact(#[values(Lenient, Strict)] strictness: ParseStrictness) {
         assert_eq!(
             Constraint::from_str("1.2.3", strictness),
             Ok(Constraint::Exact(
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-//! This module contains code to work with "versionspec". It represents the version part of
-//! [`crate::MatchSpec`], e.g.: `>=3.4,<4.0`.
+//! This module contains code to work with "versionspec". It represents the
+//! version part of [`crate::MatchSpec`], e.g.: `>=3.4,<4.0`.
 
 mod constraint;
 pub(crate) mod parse;
 pub(crate) mod version_tree;
 
-use crate::version_spec::version_tree::ParseVersionTreeError;
-use crate::{ParseStrictness, ParseVersionError, Version};
+use std::{
+    convert::TryFrom,
+    fmt::{Display, Formatter},
+    str::FromStr,
+};
+
+pub(crate) use constraint::is_start_of_version_constraint;
 use constraint::Constraint;
+use parse::ParseConstraintError;
 use serde::{Deserialize, Serialize, Serializer};
-use std::convert::TryFrom;
-use std::fmt::{Display, Formatter};
-use std::str::FromStr;
 use thiserror::Error;
 use version_tree::VersionTree;
 
-use crate::version::StrictVersion;
-pub(crate) use constraint::is_start_of_version_constraint;
-use parse::ParseConstraintError;
+use crate::{
+    version::StrictVersion, version_spec::version_tree::ParseVersionTreeError, ParseStrictness,
+    ParseVersionError, Version,
+};
 
 /// An operator to compare two versions.
 #[allow(missing_docs)]
 #[derive(Debug, Copy, Clone, Eq, PartialEq, Hash, Ord, PartialOrd, Serialize, Deserialize)]
 pub enum RangeOperator {
     Greater,
     GreaterEquals,
@@ -87,16 +91,16 @@
     Range(RangeOperator),
     /// Specifies a range of versions using the strict operator
     StrictRange(StrictRangeOperator),
     /// Specifies an exact version
     Exact(EqualityOperator),
 }
 
-/// Logical operator used two compare groups of version comparisions. E.g. `>=3.4,<4.0` or
-/// `>=3.4|<4.0`,
+/// Logical operator used two compare groups of version comparisions. E.g.
+/// `>=3.4,<4.0` or `>=3.4|<4.0`,
 #[derive(Debug, Copy, Clone, Eq, PartialEq, Hash, Ord, PartialOrd, Serialize, Deserialize)]
 pub enum LogicalOperator {
     /// All comparators must evaluate to true for the group to evaluate to true.
     And,
 
     /// Any comparators must evaluate to true for the group to evaluate to true.
     Or,
@@ -326,22 +330,26 @@
             }
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
+    use std::str::FromStr;
+
     use assert_matches::assert_matches;
+    use rstest::rstest;
 
-    use crate::version_spec::parse::ParseConstraintError;
-    use crate::version_spec::{
-        EqualityOperator, LogicalOperator, ParseVersionSpecError, RangeOperator,
+    use crate::{
+        version_spec::{
+            parse::ParseConstraintError, EqualityOperator, LogicalOperator, ParseVersionSpecError,
+            RangeOperator,
+        },
+        ParseStrictness, Version, VersionSpec,
     };
-    use crate::{ParseStrictness, Version, VersionSpec};
-    use std::str::FromStr;
 
     #[test]
     fn test_simple() {
         assert_eq!(
             VersionSpec::from_str("1.2.3", ParseStrictness::Strict),
             Ok(VersionSpec::Exact(
                 EqualityOperator::Equals,
@@ -424,14 +432,25 @@
     }
 
     #[test]
     fn issue_204() {
         assert!(VersionSpec::from_str(">=3.8<3.9", ParseStrictness::Strict).is_err());
     }
 
+    #[rstest]
+    #[case("2.38.*", true)]
+    #[case("2.38.0.*", true)]
+    #[case("2.38.0.1*", false)]
+    #[case("2.38.0a.*", false)]
+    fn issue_685(#[case] spec: &str, #[case] starts_with: bool) {
+        let spec = VersionSpec::from_str(spec, ParseStrictness::Strict).unwrap();
+        let version = &Version::from_str("2.38").unwrap();
+        assert_eq!(spec.matches(version), starts_with);
+    }
+
     #[test]
     fn issue_225() {
         let spec = VersionSpec::from_str("~=2.4", ParseStrictness::Strict).unwrap();
         assert!(!spec.matches(&Version::from_str("3.1").unwrap()));
         assert!(spec.matches(&Version::from_str("2.4").unwrap()));
         assert!(spec.matches(&Version::from_str("2.5").unwrap()));
         assert!(!spec.matches(&Version::from_str("2.1").unwrap()));
@@ -442,14 +461,29 @@
         assert_eq!(
             VersionSpec::from_str(">2.10*", ParseStrictness::Lenient).unwrap(),
             VersionSpec::from_str(">=2.10", ParseStrictness::Strict).unwrap()
         );
     }
 
     #[test]
+    fn issue_mkl_double() {
+        assert_eq!(
+            VersionSpec::from_str("2023.*.*", ParseStrictness::Lenient).unwrap(),
+            VersionSpec::from_str("2023.*", ParseStrictness::Lenient).unwrap()
+        );
+        assert!(VersionSpec::from_str("2023.*.*", ParseStrictness::Strict).is_err());
+        assert_matches!(
+            VersionSpec::from_str("2023.*.0", ParseStrictness::Lenient).unwrap_err(),
+            ParseVersionSpecError::InvalidConstraint(
+                ParseConstraintError::RegexConstraintsNotSupported
+            )
+        );
+    }
+
+    #[test]
     fn issue_star_operator() {
         assert_eq!(
             VersionSpec::from_str(">=*", ParseStrictness::Lenient).unwrap(),
             VersionSpec::from_str("*", ParseStrictness::Lenient).unwrap()
         );
         assert_eq!(
             VersionSpec::from_str("==*", ParseStrictness::Lenient).unwrap(),
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/parse.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/parse.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-use crate::version::parse::version_parser;
-use crate::version_spec::constraint::Constraint;
-use crate::version_spec::{EqualityOperator, RangeOperator, StrictRangeOperator, VersionOperators};
-use crate::{ParseStrictness, ParseVersionError, ParseVersionErrorKind};
 use nom::{
     branch::alt,
     bytes::complete::{tag, take_while, take_while1},
     character::complete::char,
     combinator::opt,
     error::{ErrorKind, ParseError},
     sequence::tuple,
     IResult,
 };
 use thiserror::Error;
 
+use crate::{
+    version::parse::version_parser,
+    version_spec::{
+        constraint::Constraint, EqualityOperator, RangeOperator, StrictRangeOperator,
+        VersionOperators,
+    },
+    ParseStrictness, ParseVersionError, ParseVersionErrorKind,
+};
+
 #[derive(Debug, Clone, Error, Eq, PartialEq)]
 enum ParseVersionOperatorError<'i> {
     #[error("invalid operator '{0}'")]
     InvalidOperator(&'i str),
     #[error("expected version operator")]
     ExpectedOperator,
 }
 
-/// Parses a version operator, returns an error if the operator is not recognized or not found.
+/// Parses a version operator, returns an error if the operator is not
+/// recognized or not found.
 fn operator_parser(input: &str) -> IResult<&str, VersionOperators, ParseVersionOperatorError<'_>> {
     // Take anything that looks like an operator.
     let (rest, operator_str) = take_while1(|c| "=!<>~".contains(c))(input).map_err(
         |_err: nom::Err<nom::error::Error<&str>>| {
             nom::Err::Error(ParseVersionOperatorError::ExpectedOperator)
         },
     )?;
@@ -138,29 +144,31 @@
                 )));
             }
             Err(nom::Err::Error(_)) => (input, None),
             Ok((rest, op)) => (rest, Some(op)),
             _ => unreachable!(),
         };
 
-        // Take everything that looks like a version and use that to parse the version. Any error means
-        // no characters were detected that belong to the version.
+        // Take everything that looks like a version and use that to parse the version.
+        // Any error means no characters were detected that belong to the
+        // version.
         let (rest, version_str) = take_while1::<_, _, (&str, ErrorKind)>(|c: char| {
             c.is_alphanumeric() || "!-_.*+".contains(c)
         })(input)
         .map_err(|_err| {
             nom::Err::Error(ParseConstraintError::InvalidVersion(ParseVersionError {
                 kind: ParseVersionErrorKind::Empty,
                 version: String::from(""),
             }))
         })?;
 
-        // Handle the case where no version was specified. These cases don't make any sense (e.g.
-        // ``>=*``) but they do exist in the wild. This code here tries to map it to something that at
-        // least makes some sort of sense. But this is not the case for everything, for instance what
+        // Handle the case where no version was specified. These cases don't make any
+        // sense (e.g. ``>=*``) but they do exist in the wild. This code here
+        // tries to map it to something that at least makes some sort of sense.
+        // But this is not the case for everything, for instance what
         // what is ment with `!=*` or `<*`?
         // See: https://github.com/AnacondaRecipes/repodata-hotfixes/issues/220
         if version_str == "*" {
             let op = op.expect(
                 "if no operator was specified for the star then this is not a logical constraint",
             );
 
@@ -226,14 +234,21 @@
             ("*" | ".*", Some(op), Strict) => {
                 return Err(nom::Err::Failure(
                     ParseConstraintError::GlobVersionIncompatibleWithOperator(op),
                 ));
             }
             ("*" | ".*", None, _) => VersionOperators::StrictRange(StrictRangeOperator::StartsWith),
 
+            // Support for edge case version spec that looks like `2023.*.*`.
+            (version_remainder, None, Lenient)
+                if looks_like_infinite_starts_with(version_remainder) =>
+            {
+                VersionOperators::StrictRange(StrictRangeOperator::StartsWith)
+            }
+
             // The version string kinda looks like a regular expression.
             (version_remainder, _, _)
                 if version_str.contains('*') || version_remainder.ends_with('$') =>
             {
                 return Err(nom::Err::Failure(
                     ParseConstraintError::RegexConstraintsNotSupported,
                 ));
@@ -256,14 +271,35 @@
             VersionOperators::StrictRange(s) => {
                 Ok((rest, Constraint::StrictComparison(s, version)))
             }
         }
     }
 }
 
+/// Returns true if the input looks like a version constraint with repeated
+/// starts with pattern. E.g: `.*.*`
+///
+/// This is an edge case found in the anaconda main repodata as `mkl 2023.*.*`.
+pub fn looks_like_infinite_starts_with(input: &str) -> bool {
+    let mut input = input;
+    while !input.is_empty() {
+        match input.strip_suffix(".*") {
+            Some(rest) if rest.is_empty() => {
+                // If we were able to continuously strip the `.*` pattern, then we found a
+                // match.
+                return true;
+            }
+            Some(rest) => input = rest,
+            None => return false,
+        }
+    }
+
+    false
+}
+
 /// Parses a version constraint.
 pub fn constraint_parser(
     strictness: ParseStrictness,
 ) -> impl FnMut(&str) -> IResult<&str, Constraint, ParseConstraintError> {
     move |input| {
         alt((
             regex_constraint_parser(strictness),
@@ -271,19 +307,21 @@
             logical_constraint_parser(strictness),
         ))(input)
     }
 }
 
 #[cfg(test)]
 mod test {
-    use super::*;
-    use crate::{ParseStrictness::*, Version, VersionSpec};
+    use std::str::FromStr;
+
     use assert_matches::assert_matches;
     use rstest::rstest;
-    use std::str::FromStr;
+
+    use super::*;
+    use crate::{ParseStrictness::*, Version, VersionSpec};
 
     #[test]
     fn test_operator_parser() {
         assert_eq!(
             operator_parser(">3.1"),
             Ok(("3.1", VersionOperators::Range(RangeOperator::Greater)))
         );
@@ -468,8 +506,18 @@
         );
     }
 
     #[test]
     fn pixi_issue_278() {
         assert!(VersionSpec::from_str("1.8.1+g6b29558", Strict).is_ok());
     }
+
+    #[test]
+    fn test_looks_like_infinite_starts_with() {
+        assert!(looks_like_infinite_starts_with(".*"));
+        assert!(looks_like_infinite_starts_with(".*.*"));
+        assert!(!looks_like_infinite_starts_with(".0.*"));
+        assert!(!looks_like_infinite_starts_with(""));
+        assert!(!looks_like_infinite_starts_with(""));
+        assert!(!looks_like_infinite_starts_with(".* .*"));
+    }
 }
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs` & `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-use crate::version_spec::{
-    EqualityOperator, LogicalOperator, RangeOperator, StrictRangeOperator, VersionOperators,
-};
+use std::convert::TryFrom;
+
 use nom::{
     branch::alt,
     bytes::complete::{tag, take_while},
     character::complete::{alpha1, digit1, multispace0, u32},
     combinator::{all_consuming, cut, map, not, opt, recognize, value},
     error::{context, convert_error, ContextError, ParseError},
     multi::{many0, separated_list1},
     sequence::{delimited, preceded, terminated, tuple},
+    IResult,
 };
-use std::convert::TryFrom;
 use thiserror::Error;
 
-/// A representation of an hierarchy of version constraints e.g. `1.3.4,>=5.0.1|(1.2.4,>=3.0.1)`.
+use crate::version_spec::{
+    EqualityOperator, LogicalOperator, RangeOperator, StrictRangeOperator, VersionOperators,
+};
+
+/// A representation of an hierarchy of version constraints e.g.
+/// `1.3.4,>=5.0.1|(1.2.4,>=3.0.1)`.
 #[derive(Debug, Eq, PartialEq)]
 pub(super) enum VersionTree<'a> {
     Term(&'a str),
     Group(LogicalOperator, Vec<VersionTree<'a>>),
 }
 
 #[derive(Debug, Clone, Error, Eq, PartialEq)]
@@ -62,58 +66,72 @@
     input: &'a str,
 ) -> Result<(&'a str, u32), nom::Err<E>> {
     terminated(u32, tag("!"))(input)
 }
 
 /// A parser that recognizes a version
 pub(crate) fn recognize_version<'a, E: ParseError<&'a str> + ContextError<&'a str>>(
-    input: &'a str,
-) -> Result<(&'a str, &'a str), nom::Err<E>> {
+    allow_glob: bool,
+) -> impl FnMut(&'a str) -> IResult<&'a str, &'a str, E> {
     /// Recognizes a single version component (`1`, `a`, `alpha`, `grub`)
     fn recognize_version_component<'a, E: ParseError<&'a str> + ContextError<&'a str>>(
-        input: &'a str,
-    ) -> Result<(&'a str, &'a str), nom::Err<E>> {
-        let ident = alpha1;
-        let num = digit1;
-        alt((ident, num))(input)
+        allow_glob: bool,
+    ) -> impl FnMut(&'a str) -> IResult<&'a str, &'a str, E> {
+        move |input: &'a str| {
+            let ident = alpha1;
+            let num = digit1;
+            let glob = tag("*");
+            if allow_glob {
+                alt((ident, num, glob))(input)
+            } else {
+                alt((ident, num))(input)
+            }
+        }
     }
 
     /// Recognize one or more version components (`1.2.3`)
     fn recognize_version_components<'a, E: ParseError<&'a str> + ContextError<&'a str>>(
-        input: &'a str,
-    ) -> Result<(&'a str, &'a str), nom::Err<E>> {
+        allow_glob: bool,
+    ) -> impl FnMut(&'a str) -> IResult<&'a str, &'a str, E> {
+        move |input: &'a str| {
+            recognize(tuple((
+                recognize_version_component(allow_glob),
+                many0(preceded(
+                    opt(take_while(|c: char| c == '.' || c == '-' || c == '_')),
+                    recognize_version_component(allow_glob),
+                )),
+            )))(input)
+        }
+    }
+
+    move |input: &'a str| {
         recognize(tuple((
-            recognize_version_component,
-            many0(preceded(
-                opt(take_while(|c: char| c == '.' || c == '-' || c == '_')),
-                recognize_version_component,
+            // Optional version epoch
+            opt(context("epoch", parse_version_epoch)),
+            // Version components
+            context("components", recognize_version_components(allow_glob)),
+            // Local version
+            opt(preceded(
+                tag("+"),
+                cut(context("local", recognize_version_components(allow_glob))),
             )),
         )))(input)
     }
-
-    recognize(tuple((
-        // Optional version epoch
-        opt(context("epoch", parse_version_epoch)),
-        // Version components
-        context("components", recognize_version_components),
-        // Local version
-        opt(preceded(
-            tag("+"),
-            cut(context("local", recognize_version_components)),
-        )),
-    )))(input)
 }
 
 /// Recognize a version followed by a .* or *, or just a *
 pub(crate) fn recognize_version_with_star<'a, E: ParseError<&'a str> + ContextError<&'a str>>(
     input: &'a str,
 ) -> Result<(&'a str, &'a str), nom::Err<E>> {
     alt((
         // A version with an optional * or .*.
-        terminated(recognize_version, opt(alt((tag(".*"), tag("*"))))),
+        terminated(
+            recognize_version(true),
+            take_while(|c: char| c == '.' || c == '*'),
+        ),
         // Just a *
         tag("*"),
     ))(input)
 }
 
 /// A parser that recognized a constraint but does not actually parse it.
 pub(crate) fn recognize_constraint<'a, E: ParseError<&'a str> + ContextError<&'a str>>(
@@ -152,15 +170,16 @@
                 ),
                 map(recognize_constraint, |constraint| {
                     VersionTree::Term(constraint)
                 }),
             ))(input)
         }
 
-        /// Given multiple version tree components, flatten the structure as much as possible.
+        /// Given multiple version tree components, flatten the structure as
+        /// much as possible.
         fn flatten_group(operator: LogicalOperator, args: Vec<VersionTree<'_>>) -> VersionTree<'_> {
             if args.len() == 1 {
                 args.into_iter().next().unwrap()
             } else {
                 let mut result = Vec::new();
                 for term in args {
                     match term {
@@ -203,20 +222,21 @@
             _ => unreachable!("with all_consuming the only error can be Error"),
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
+    use std::convert::TryFrom;
+
     use super::{parse_operator, recognize_version, LogicalOperator, VersionTree};
-    use crate::version_spec::version_tree::{parse_version_epoch, recognize_constraint};
     use crate::version_spec::{
+        version_tree::{parse_version_epoch, recognize_constraint},
         EqualityOperator, RangeOperator, StrictRangeOperator, VersionOperators,
     };
-    use std::convert::TryFrom;
 
     #[test]
     fn test_treeify() {
         use LogicalOperator::{And, Or};
         use VersionTree::{Group, Term};
 
         assert_eq!(VersionTree::try_from("1.2.3").unwrap(), Term("1.2.3"));
@@ -318,22 +338,25 @@
         );
     }
 
     #[test]
     fn test_recognize_version() {
         type Err<'a> = nom::error::Error<&'a str>;
 
-        assert_eq!(recognize_version::<Err<'_>>("3.8.9"), Ok(("", "3.8.9")));
-        assert_eq!(recognize_version::<Err<'_>>("3"), Ok(("", "3")));
         assert_eq!(
-            recognize_version::<Err<'_>>("1!3.8.9+3.4-alpha.2"),
+            recognize_version::<Err<'_>>(false)("3.8.9"),
+            Ok(("", "3.8.9"))
+        );
+        assert_eq!(recognize_version::<Err<'_>>(false)("3"), Ok(("", "3")));
+        assert_eq!(
+            recognize_version::<Err<'_>>(false)("1!3.8.9+3.4-alpha.2"),
             Ok(("", "1!3.8.9+3.4-alpha.2"))
         );
-        assert_eq!(recognize_version::<Err<'_>>("3."), Ok((".", "3")));
-        assert_eq!(recognize_version::<Err<'_>>("3.*"), Ok((".*", "3")));
+        assert_eq!(recognize_version::<Err<'_>>(false)("3."), Ok((".", "3")));
+        assert_eq!(recognize_version::<Err<'_>>(false)("3.*"), Ok((".*", "3")));
 
         let versions = [
             // Implicit epoch of 0
             "1.0a1",
             "1.0a2.dev456",
             "1.0a12.dev456",
             "1.0a12",
@@ -386,15 +409,15 @@
             "1!1.2+123abc456",
             "1!1.2+1234.abc",
             "1!1.2+123456",
         ];
 
         for version_str in versions {
             assert_eq!(
-                recognize_version::<Err<'_>>(version_str),
+                recognize_version::<Err<'_>>(false)(version_str),
                 Ok(("", version_str))
             );
         }
     }
 
     #[test]
     fn test_parse_version_epoch() {
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_shell/Cargo.toml` & `py_rattler-0.6.1/local_dependencies/rattler_shell/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_shell"
-version = "0.20.5"
+version = "0.20.6"
 edition= "2021"
 authors = ["Wolf Vollprecht <w.vollprecht@gmail.com>"]
 description = "A crate to help with activation and deactivation of a conda environment"
 categories = ["conda", "mamba", "package_management", "virtual_environment"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
 enum_dispatch = "0.3.13"
 indexmap = "2.2.6"
 itertools = "0.12.1"
 serde_json = { version = "1.0.116" , features = ["preserve_order"] }
 shlex = "1.3.0"
 sysinfo = { version = "0.30.10", optional = true }
 tempfile = "3.10.1"
```

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_shell/src/activation.rs` & `py_rattler-0.6.1/local_dependencies/rattler_shell/src/activation.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_shell/src/run/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_shell/src/run/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/mod.rs` & `py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/Cargo.toml` & `py_rattler-0.6.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-rattler"
-version = "0.6.0"
+version = "0.6.1"
 edition = "2021"
 license = "BSD-3-Clause"
 publish = false
 
 [lib]
 name = "rattler"
 crate-type = ["cdylib"]
@@ -48,15 +48,15 @@
 reqwest = { version = "0.12.3", default-features = false }
 reqwest-middleware = "0.3.0"
 
 thiserror = "1.0.61"
 url = "2.5.0"
 
 openssl = { version = "0.10", optional = true }
-pep508_rs = "0.4.2"
+pep508_rs = "0.6.0"
 
 [build-dependencies]
 pyo3-build-config = "0.21"
 
 
 [patch.crates-io]
```

### Comparing `py_rattler-0.6.0/.gitignore` & `py_rattler-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/LICENSE` & `py_rattler-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/README.md` & `py_rattler-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/docs/index.md` & `py_rattler-0.6.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/docs/stylesheets/extra.css` & `py_rattler-0.6.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/mkdocs.yml` & `py_rattler-0.6.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/pixi.lock` & `py_rattler-0.6.1/pixi.lock`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/pixi.toml` & `py_rattler-0.6.1/pixi.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/pyproject.toml` & `py_rattler-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/__init__.py` & `py_rattler-0.6.1/rattler/__init__.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/channel/channel.py` & `py_rattler-0.6.1/rattler/channel/channel.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/channel/channel_config.py` & `py_rattler-0.6.1/rattler/channel/channel_config.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/exceptions.py` & `py_rattler-0.6.1/rattler/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/index/index.py` & `py_rattler-0.6.1/rattler/index/index.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/install/installer.py` & `py_rattler-0.6.1/rattler/install/installer.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,22 +31,26 @@
         arbitraty code. It is therefor discouraged to enable executing link scripts.
 
     Example
     -------
     ```python
     >>> import asyncio
     >>> from rattler import solve, install
+    >>> from tempfile import TemporaryDirectory
+    >>> temp_dir = TemporaryDirectory()
+    >>>
     >>> async def main():
     ...     # Solve an environment with python 3.9 for the current platform
     ...     records = await solve(channels=["conda-forge"], specs=["python=3.9"])
     ...
-    ...     # Link the environment in the directory `my-env`.
-    ...     await install(records, target_prefix="my-env")
+    ...     # Link the environment in a temporary directory (you can pass any kind of path here).
+    ...     await install(records, target_prefix=temp_dir.name)
     ...
     ...     # That's it! The environment is now created.
+    ...     # You will find Python under `f"{temp_dir.name}/bin/python"` or `f"{temp_dir.name}/python.exe"` on Windows.
     >>> asyncio.run(main())
 
     ```
 
     Arguments:
         records: A list of solved `RepoDataRecord`s.
         target_prefix: Path to the directory where the environment should
```

### Comparing `py_rattler-0.6.0/rattler/lock/channel.py` & `py_rattler-0.6.1/rattler/lock/channel.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/lock/environment.py` & `py_rattler-0.6.1/rattler/lock/environment.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/lock/hash.py` & `py_rattler-0.6.1/rattler/lock/hash.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/lock/lock_file.py` & `py_rattler-0.6.1/rattler/lock/lock_file.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/lock/package.py` & `py_rattler-0.6.1/rattler/lock/package.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/lock/pypi.py` & `py_rattler-0.6.1/rattler/lock/pypi.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/match_spec/match_spec.py` & `py_rattler-0.6.1/rattler/match_spec/match_spec.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/match_spec/nameless_match_spec.py` & `py_rattler-0.6.1/rattler/match_spec/nameless_match_spec.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/networking/authenticated_client.py` & `py_rattler-0.6.1/rattler/networking/authenticated_client.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/networking/fetch_repo_data.py` & `py_rattler-0.6.1/rattler/networking/fetch_repo_data.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/package/__init__.py` & `py_rattler-0.6.1/rattler/package/__init__.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/package/about_json.py` & `py_rattler-0.6.1/rattler/package/about_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/package/index_json.py` & `py_rattler-0.6.1/rattler/package/index_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/package/no_arch_type.py` & `py_rattler-0.6.1/rattler/package/no_arch_type.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/package/package_name.py` & `py_rattler-0.6.1/rattler/package/package_name.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/package/paths_json.py` & `py_rattler-0.6.1/rattler/package/paths_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/package/run_exports_json.py` & `py_rattler-0.6.1/rattler/package/run_exports_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/platform/arch.py` & `py_rattler-0.6.1/rattler/platform/arch.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/platform/platform.py` & `py_rattler-0.6.1/rattler/platform/platform.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/prefix/prefix_paths.py` & `py_rattler-0.6.1/rattler/prefix/prefix_paths.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/prefix/prefix_record.py` & `py_rattler-0.6.1/rattler/prefix/prefix_record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/repo_data/gateway.py` & `py_rattler-0.6.1/rattler/repo_data/gateway.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/repo_data/package_record.py` & `py_rattler-0.6.1/rattler/repo_data/package_record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/repo_data/patch_instructions.py` & `py_rattler-0.6.1/rattler/repo_data/patch_instructions.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/repo_data/record.py` & `py_rattler-0.6.1/rattler/repo_data/record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/repo_data/repo_data.py` & `py_rattler-0.6.1/rattler/repo_data/repo_data.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/repo_data/sparse.py` & `py_rattler-0.6.1/rattler/repo_data/sparse.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/shell/shell.py` & `py_rattler-0.6.1/rattler/shell/shell.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/solver/solver.py` & `py_rattler-0.6.1/rattler/solver/solver.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/utils/rattler_version.py` & `py_rattler-0.6.1/rattler/utils/rattler_version.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/version/version.py` & `py_rattler-0.6.1/rattler/version/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
         Examples
         --------
         ```python
         >>> v = Version('1.0')
         >>> v.bump_major()
         Version("2.0")
+        >>> v = Version('9d')
+        >>> v.bump_major()
+        Version("10a")
         >>>
         ```
         """
         return Version._from_py_version(self._version.bump_major())
 
     def bump_minor(self) -> Version:
         """
@@ -75,17 +78,16 @@
         Examples
         --------
         ```python
         >>> v = Version('1.0')
         >>> v.bump_minor()
         Version("1.1")
         >>>
-        >>> Version("1").bump_minor() # doctest: +IGNORE_EXCEPTION_DETAIL
-        Traceback (most recent call last):
-        exceptions.VersionBumpException
+        >>> Version("1").bump_minor()
+        Version("1.1")
         >>>
         ```
         """
         return Version._from_py_version(self._version.bump_minor())
 
     def bump_patch(self) -> Version:
         """
@@ -94,18 +96,20 @@
 
         Examples
         --------
         ```python
         >>> v = Version('1.0.5')
         >>> v.bump_patch()
         Version("1.0.6")
+        >>> v = Version('1.1.1e')
+        >>> v.bump_patch()
+        Version("1.1.2a")
         >>>
-        >>> Version("1.5").bump_patch() # doctest: +IGNORE_EXCEPTION_DETAIL
-        Traceback (most recent call last):
-        exceptions.VersionBumpException
+        >>> Version("1.5").bump_patch()
+        Version("1.5.1")
         >>>
         ```
         """
         return Version._from_py_version(self._version.bump_patch())
 
     def bump_last(self) -> Version:
         """
@@ -134,22 +138,39 @@
         >>> v = Version('1.0')
         >>> v.bump_segment(index=1)
         Version("1.1")
         >>>
         >>> Version("1.5").bump_segment(-5) # doctest: +IGNORE_EXCEPTION_DETAIL
         Traceback (most recent call last):
         exceptions.VersionBumpException
-        >>> Version("1.5").bump_segment(5) # doctest: +IGNORE_EXCEPTION_DETAIL
-        Traceback (most recent call last):
-        exceptions.VersionBumpException
+        >>> Version("1.5").bump_segment(5)
+        Version("1.5.0.0.0.1")
         >>>
         ```
         """
         return Version._from_py_version(self._version.bump_segment(index))
 
+    def extend_to_length(self, length: int) -> Version:
+        """
+        Returns a new version that is extended with `0s` to the specified length.
+
+        Examples
+        --------
+        ```python
+        >>> v = Version('1')
+        >>> v.extend_to_length(3)
+        Version("1.0.0")
+        >>> v = Version('4!1.2+3.4')
+        >>> v.extend_to_length(4)
+        Version("4!1.2.0.0+3.4")
+        >>>
+        ```
+        """
+        return Version._from_py_version(self._version.extend_to_length(length))
+
     @property
     def has_local(self) -> bool:
         """
         Returns true if this version has a local segment defined.
         The local part of a version is the part behind the (optional) `+`.
 
         Examples
```

### Comparing `py_rattler-0.6.0/rattler/version/with_source.py` & `py_rattler-0.6.1/rattler/version/with_source.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/virtual_package/generic.py` & `py_rattler-0.6.1/rattler/virtual_package/generic.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/rattler/virtual_package/virtual_package.py` & `py_rattler-0.6.1/rattler/virtual_package/virtual_package.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/about_json.rs` & `py_rattler-0.6.1/src/about_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/channel/mod.rs` & `py_rattler-0.6.1/src/channel/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/error.rs` & `py_rattler-0.6.1/src/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use std::{error::Error, io};
 
 use pyo3::{create_exception, exceptions::PyException, PyErr};
 use rattler::install::TransactionError;
 use rattler_conda_types::{
     ConvertSubdirError, InvalidPackageNameError, ParseArchError, ParseChannelError,
     ParseMatchSpecError, ParsePlatformError, ParseVersionError, VersionBumpError,
+    VersionExtendError,
 };
 use rattler_lock::{ConversionError, ParseCondaLockError};
 use rattler_package_streaming::ExtractError;
 use rattler_repodata_gateway::{fetch::FetchRepoDataError, GatewayError};
 use rattler_shell::activation::ActivationError;
 use rattler_solve::SolveError;
 use rattler_virtual_packages::DetectVirtualPackageError;
@@ -48,14 +49,16 @@
     #[error("{0}")]
     LinkError(String),
     #[error(transparent)]
     ConverSubdirError(#[from] ConvertSubdirError),
     #[error(transparent)]
     VersionBumpError(#[from] VersionBumpError),
     #[error(transparent)]
+    VersionExtendError(#[from] VersionExtendError),
+    #[error(transparent)]
     ParseCondaLockError(#[from] ParseCondaLockError),
     #[error(transparent)]
     ConversionError(#[from] ConversionError),
     #[error("{0}")]
     RequirementError(String),
     #[error("{0}")]
     EnvironmentCreationError(String),
@@ -122,14 +125,17 @@
             PyRattlerError::LinkError(err) => LinkException::new_err(err),
             PyRattlerError::ConverSubdirError(err) => {
                 ConvertSubdirException::new_err(pretty_print_error(&err))
             }
             PyRattlerError::VersionBumpError(err) => {
                 VersionBumpException::new_err(pretty_print_error(&err))
             }
+            PyRattlerError::VersionExtendError(err) => {
+                VersionExtendException::new_err(pretty_print_error(&err))
+            }
             PyRattlerError::ParseCondaLockError(err) => {
                 ParseCondaLockException::new_err(pretty_print_error(&err))
             }
             PyRattlerError::ConversionError(err) => {
                 ConversionException::new_err(pretty_print_error(&err))
             }
             PyRattlerError::RequirementError(err) => RequirementException::new_err(err),
@@ -165,14 +171,15 @@
 create_exception!(exceptions, DetectVirtualPackageException, PyException);
 create_exception!(exceptions, IoException, PyException);
 create_exception!(exceptions, SolverException, PyException);
 create_exception!(exceptions, TransactionException, PyException);
 create_exception!(exceptions, LinkException, PyException);
 create_exception!(exceptions, ConvertSubdirException, PyException);
 create_exception!(exceptions, VersionBumpException, PyException);
+create_exception!(exceptions, VersionExtendException, PyException);
 create_exception!(exceptions, ParseCondaLockException, PyException);
 create_exception!(exceptions, ConversionException, PyException);
 create_exception!(exceptions, RequirementException, PyException);
 create_exception!(exceptions, EnvironmentCreationException, PyException);
 create_exception!(exceptions, ExtractException, PyException);
 create_exception!(exceptions, ActivationScriptFormatException, PyException);
 create_exception!(exceptions, GatewayException, PyException);
```

### Comparing `py_rattler-0.6.0/src/generic_virtual_package.rs` & `py_rattler-0.6.1/src/generic_virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/index.rs` & `py_rattler-0.6.1/src/index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/index_json.rs` & `py_rattler-0.6.1/src/index_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/installer.rs` & `py_rattler-0.6.1/src/installer.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/lib.rs` & `py_rattler-0.6.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/lock/mod.rs` & `py_rattler-0.6.1/src/lock/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/match_spec.rs` & `py_rattler-0.6.1/src/match_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/nameless_match_spec.rs` & `py_rattler-0.6.1/src/nameless_match_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/networking/authenticated_client.rs` & `py_rattler-0.6.1/src/networking/authenticated_client.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/networking/cached_repo_data.rs` & `py_rattler-0.6.1/src/networking/cached_repo_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/networking/mod.rs` & `py_rattler-0.6.1/src/networking/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/no_arch_type.rs` & `py_rattler-0.6.1/src/no_arch_type.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/package_name.rs` & `py_rattler-0.6.1/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/paths_json.rs` & `py_rattler-0.6.1/src/paths_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/platform.rs` & `py_rattler-0.6.1/src/platform.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/prefix_paths.rs` & `py_rattler-0.6.1/src/prefix_paths.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/record.rs` & `py_rattler-0.6.1/src/record.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/repo_data/gateway.rs` & `py_rattler-0.6.1/src/repo_data/gateway.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/repo_data/mod.rs` & `py_rattler-0.6.1/src/repo_data/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/repo_data/sparse.rs` & `py_rattler-0.6.1/src/repo_data/sparse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/run_exports_json.rs` & `py_rattler-0.6.1/src/run_exports_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/shell.rs` & `py_rattler-0.6.1/src/shell.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/solver.rs` & `py_rattler-0.6.1/src/solver.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/version/component.rs` & `py_rattler-0.6.1/src/version/component.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/src/version/mod.rs` & `py_rattler-0.6.1/src/version/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -79,14 +79,25 @@
     /// invalid due to the operation.
     pub fn pop_segments(&self, n: usize) -> Option<Self> {
         Some(Self {
             inner: self.inner.pop_segments(n)?,
         })
     }
 
+    /// Extend a version to a specified length by adding `0s` if necessary
+    pub fn extend_to_length(&self, length: usize) -> PyResult<Self> {
+        Ok(Self {
+            inner: self
+                .inner
+                .extend_to_length(length)
+                .map_err(PyRattlerError::from)?
+                .into_owned(),
+        })
+    }
+
     /// Returns a list of segments of the version. It does not contain
     /// the local segment of the version. See `local_segments` for
     /// local segments in version.
     pub fn segments(&self) -> Vec<Vec<PyComponent>> {
         self.inner
             .segments()
             .map(|s| s.components().map(|c| c.clone().into()).collect::<Vec<_>>())
```

### Comparing `py_rattler-0.6.0/src/virtual_package.rs` & `py_rattler-0.6.1/src/virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/tests/conftest.py` & `py_rattler-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/tests/unit/test_fetch_repo_data.py` & `py_rattler-0.6.1/tests/unit/test_fetch_repo_data.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/tests/unit/test_index.py` & `py_rattler-0.6.1/tests/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/tests/unit/test_install.py` & `py_rattler-0.6.1/tests/unit/test_install.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/tests/unit/test_prefix_record.py` & `py_rattler-0.6.1/tests/unit/test_prefix_record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/tests/unit/test_solver.py` & `py_rattler-0.6.1/tests/unit/test_solver.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/tests/unit/test_version.py` & `py_rattler-0.6.1/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.0/Cargo.lock` & `py_rattler-0.6.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2097,29 +2097,29 @@
 dependencies = [
  "base64 0.22.1",
  "serde",
 ]
 
 [[package]]
 name = "pep440_rs"
-version = "0.5.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15efd4d885c29126cc93e12af3087896e2518bd5ca0fb328c19c4ef9cecfa8be"
+checksum = "ca0a570e7ec9171250cac57614e901f62408094b54b3798bb920d3cf0d4a0e09"
 dependencies = [
  "once_cell",
  "serde",
  "unicode-width",
  "unscanny",
 ]
 
 [[package]]
 name = "pep508_rs"
-version = "0.4.2"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1455babf8edd3eedcdfcb39700e455a4bb189e71b4f1fa0eacc9b244cc5a55e6"
+checksum = "581c27e97a3f38c5d691962af7da93c2672b5227d59cf165b87a9b1fd53dd724"
 dependencies = [
  "derivative",
  "once_cell",
  "pep440_rs",
  "regex",
  "serde",
  "thiserror",
@@ -2345,15 +2345,15 @@
  "smartstring",
  "thiserror",
  "unicase",
 ]
 
 [[package]]
 name = "py-rattler"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "anyhow",
  "chrono",
  "futures",
  "openssl",
  "pep508_rs",
  "pyo3",
@@ -2517,15 +2517,15 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rattler"
-version = "0.26.0"
+version = "0.26.1"
 dependencies = [
  "anyhow",
  "bytes",
  "chrono",
  "console",
  "digest",
  "dirs",
@@ -2558,15 +2558,15 @@
  "tracing",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "rattler_conda_types"
-version = "0.24.0"
+version = "0.25.0"
 dependencies = [
  "chrono",
  "file_url",
  "fxhash",
  "glob",
  "hex",
  "itertools 0.12.1",
@@ -2601,28 +2601,28 @@
  "serde_with",
  "sha2",
  "tokio",
 ]
 
 [[package]]
 name = "rattler_index"
-version = "0.19.13"
+version = "0.19.14"
 dependencies = [
  "fs-err",
  "rattler_conda_types",
  "rattler_digest",
  "rattler_package_streaming",
  "serde_json",
  "tracing",
  "walkdir",
 ]
 
 [[package]]
 name = "rattler_lock"
-version = "0.22.8"
+version = "0.22.9"
 dependencies = [
  "chrono",
  "file_url",
  "fxhash",
  "indexmap 2.2.6",
  "itertools 0.12.1",
  "pep440_rs",
@@ -2674,15 +2674,15 @@
  "thiserror",
  "tracing",
  "url",
 ]
 
 [[package]]
 name = "rattler_package_streaming"
-version = "0.21.0"
+version = "0.21.1"
 dependencies = [
  "bzip2",
  "chrono",
  "futures-util",
  "num_cpus",
  "rattler_conda_types",
  "rattler_digest",
@@ -2698,15 +2698,15 @@
  "url",
  "zip",
  "zstd",
 ]
 
 [[package]]
 name = "rattler_repodata_gateway"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "anyhow",
  "async-compression",
  "async-trait",
  "blake2",
  "bytes",
  "cache_control",
@@ -2748,30 +2748,30 @@
  "url",
  "windows-sys 0.52.0",
  "zstd",
 ]
 
 [[package]]
 name = "rattler_shell"
-version = "0.20.5"
+version = "0.20.6"
 dependencies = [
  "enum_dispatch",
  "indexmap 2.2.6",
  "itertools 0.12.1",
  "rattler_conda_types",
  "serde_json",
  "shlex",
  "tempfile",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "rattler_solve"
-version = "0.23.0"
+version = "0.23.1"
 dependencies = [
  "chrono",
  "futures",
  "itertools 0.12.1",
  "rattler_conda_types",
  "rattler_digest",
  "resolvo",
@@ -2779,15 +2779,15 @@
  "thiserror",
  "tracing",
  "url",
 ]
 
 [[package]]
 name = "rattler_virtual_packages"
-version = "0.19.12"
+version = "0.19.13"
 dependencies = [
  "archspec",
  "libloading",
  "nom",
  "once_cell",
  "plist",
  "rattler_conda_types",
```

### Comparing `py_rattler-0.6.0/PKG-INFO` & `py_rattler-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-rattler
-Version: 0.6.0
+Version: 0.6.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-rattler Version: 0.6.0 Classifier: Development
+Metadata-Version: 2.1 Name: py-rattler Version: 0.6.1 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed License-File: LICENSE Summary: A blazing fast
 library to work with the conda ecosystem Author-email: Bas Zalmstra
 gmail.com>, Tarun Pratap Singh
```

