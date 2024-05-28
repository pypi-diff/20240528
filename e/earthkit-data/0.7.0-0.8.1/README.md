# Comparing `tmp/earthkit_data-0.7.0.tar.gz` & `tmp/earthkit_data-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit_data-0.7.0.tar", last modified: Thu Apr 18 11:33:33 2024, max compression
+gzip compressed data, was "earthkit_data-0.8.1.tar", last modified: Tue May 28 20:50:26 2024, max compression
```

## Comparing `earthkit_data-0.7.0.tar` & `earthkit_data-0.8.1.tar`

### file list

```diff
@@ -1,494 +1,509 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/ci-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/ci-hpc-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/ci_other.yml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/label-public-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/notify-new-issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.github/workflows/notify-new-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)    65385 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/_static/earthkit-data.png
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.304596 earthkit_data-0.7.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/development.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/ads.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25628 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/bufr_synop.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    80839 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/bufr_temp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13363 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/cache.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/cds.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    51752 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/data_from_stream.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/default_fdb_schema
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/demo_sources_plugin.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/ecmwf_open_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    57129 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/fdb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30675 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/file_parts.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/files.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    27906 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/from_object.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22543 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/geojson_geopandas.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25900 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_array_backends.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_fdb_write.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23026 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_indexing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20668 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_lat_lon_value.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    88655 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_missing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_nearest_gridpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   105060 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    47388 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_time_series.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/grib_to_netcdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34283 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/list_of_dict.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/mars.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    49512 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/missing.grib
--rw-r--r--   0 runner    (1001) docker     (127)    16882 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/multi_files.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    39146 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/netcdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    65479 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/netcdf_fieldlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    35982 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/netcdf_opendap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/numpy_fieldlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/odb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/pandas.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/polytope.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   442939 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/projection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/settings.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    45359 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/shapefile.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/synop_10.bufr
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/tar_files.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/temp_10.bufr
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test.grib
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test.nc
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test.odb
--rw-r--r--   0 runner    (1001) docker     (127)   521712 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test4.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/test6.grib
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/time_series.grib
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/tuv_pl.grib
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/tuv_pl.nc
--rw-r--r--   0 runner    (1001) docker     (127)    28753 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/url.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/url_parts.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/url_stream.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    35809 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/examples/wekeo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/caching.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/guide/data_format/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/bufr.rst
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/csv.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/netcdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/data_format/odb.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/guide/include/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/include/settings-get.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/include/settings-reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/include/settings-set.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/include/settings-temporary.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.316596 earthkit_data-0.7.0/docs/guide/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/misc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/misc/parts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/misc/split_on.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)    36947 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/guide/sources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/howtos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/licence.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/docs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/plugins/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/plugins/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/plugins/sources_plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/docs/release_notes/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.2_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.3_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.4_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.5_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.6_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/release_notes/version_0.7_updates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/docs/skip_api_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.296596 earthkit_data-0.7.0/earthkit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/earthkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/earthkit/data/arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/args_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/earthkit_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/input_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/arguments/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/earthkit/data/conf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.320597 earthkit_data-0.7.0/earthkit/data/conf/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/css/tab.css
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/css/table.css
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/css/tree.css
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/global_grids.json
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/gridspec.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/conf/gridspec_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    47136 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/fieldlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/geography.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    21054 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/ipython.py
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/select.py
--rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/temporary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/core/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/indexing/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/indexing/database/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/database/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/database/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/indexing/database/stdout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/mergers/
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mergers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mergers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mergers/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.324597 earthkit_data-0.7.0/earthkit/data/mirrors/
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mirrors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/mirrors/directory_mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.328596 earthkit_data-0.7.0/earthkit/data/readers/
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.328596 earthkit_data-0.7.0/earthkit/data/readers/bufr/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/bufr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/bufr/bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/bufr/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/covjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/geojson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.328596 earthkit_data-0.7.0/earthkit/data/readers/grib/
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17730 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/gridspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.328596 earthkit_data-0.7.0/earthkit/data/readers/grib/index/
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/index/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/grib/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.332597 earthkit_data-0.7.0/earthkit/data/readers/netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/field.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/netcdf/fieldlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/odb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/shapefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/readers/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.336597 earthkit_data-0.7.0/earthkit/data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/ads.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/array_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/cds.py
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/dummy.grib
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/dummy_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/ecmwf_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/ecmwf_open_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/fdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/file_indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/file_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/list_of_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/numpy_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/opendap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/polytope.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/virtual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/virtual_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/wekeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sources/wekeocds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.336597 earthkit_data-0.7.0/earthkit/data/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sphinxext/generate_settings_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sphinxext/module_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/sphinxext/xref.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.336597 earthkit_data-0.7.0/earthkit/data/translators/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/translators/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/utils/array/
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/array/cupy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/array/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/array/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/conventions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    19711 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/factorise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/module_inputs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/parts.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/progbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/utils/projections/
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/projections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/projections/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/projections/proj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/serialise.py
--rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/grib-paramid.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/vocabularies/grib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/wrappers/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.340597 earthkit_data-0.7.0/earthkit/data/writers/
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/earthkit/data/writers/grib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/earthkit_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 11:33:33.000000 earthkit_data-0.7.0/earthkit_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-18 11:33:33.372597 earthkit_data-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.344597 earthkit_data-0.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.344597 earthkit_data-0.7.0/tests/array_fieldlist/
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/array_fl_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fl_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.344597 earthkit_data-0.7.0/tests/bufr/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_file_parts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/bufr/test_bufr_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.344597 earthkit_data-0.7.0/tests/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/constants_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_constants_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/constants/test_contants_proc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.348597 earthkit_data-0.7.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/core/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.352597 earthkit_data-0.7.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)  2542596 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/NUTS_RG_20M_2021_3035.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   640295 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/NUTS_RG_20M_2021_3035.shp.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.352597 earthkit_data-0.7.0/tests/data/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/constants/proc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/empty_file.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/era5_2t_1.nc
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/era5_2t_2.nc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.356597 earthkit_data-0.7.0/tests/data/gridspec/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/healpix.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/reduced_gg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/reduced_ll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/reduced_rotated_gg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/regular_gg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/regular_ll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/rotated_gg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/rotated_ll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/sh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/gridspec/t_75_-60_10_40_5x5.grib1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1308 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/hovexp_vert_area.nc
--rw-r--r--   0 runner    (1001) docker     (127)    22138 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/mercator.grib
--rw-r--r--   0 runner    (1001) docker     (127)    47520 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/ml_data.grib
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/rgg_small_subarea_cellarea_ref.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/t_pl.grib
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/t_time_series.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/test_icon.grib
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/test_single.grib
--rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/test_single.nc
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/test_single_with_missing.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/time_series.covjson
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/u_pl.grib
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/data/v_pl.grib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.356597 earthkit_data-0.7.0/tests/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/documentation/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/documentation/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/downstream-ci-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/environment-unit-tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.356597 earthkit_data-0.7.0/tests/grib/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/grib_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_file_parts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_geography.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_inidces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    17347 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_url.py
--rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_url_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/grib/test_grib_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.360597 earthkit_data-0.7.0/tests/indexing/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/indexing_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_indexing_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_indexing_isel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_indexing_order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_indexing_serialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_order_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/indexing/test_selection_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.360597 earthkit_data-0.7.0/tests/netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_fieldlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_geography.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_opendap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/netcdf/test_netcdf_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.360597 earthkit_data-0.7.0/tests/normalize/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/aliases.json
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/availability.json
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_aliases_grib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_normalize_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/normalize/test_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.360597 earthkit_data-0.7.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/plugins/test_sources_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.364597 earthkit_data-0.7.0/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_covjson_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_geojson_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_grib_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_netcdf_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_odb_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_reader_padding_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_shapefile_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_tar_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_unknown_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/test_zip_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/unknown_file.unknown_ext
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/readers/unknown_text_file.unknown_ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.364597 earthkit_data-0.7.0/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_cds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_ecmwf_open_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_fdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_list_of_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_polytope.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_wekeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/sources/test_wekeocds.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/test_00_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.364597 earthkit_data-0.7.0/tests/translators/
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/translators/test_translators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_download_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_module_inputs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_parts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/utils/test_projections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:33:33.368597 earthkit_data-0.7.0/tests/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/wrappers/test_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/wrappers/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/wrappers/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-18 11:33:24.000000 earthkit_data-0.7.0/tests/wrappers/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.148332 earthkit_data-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.068332 earthkit_data-0.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.github/ci-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.github/ci-hpc-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.068332 earthkit_data-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.github/workflows/cd-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.github/workflows/legacy-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.github/workflows/notify-new-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.github/workflows/notify-new-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-28 20:50:26.148332 earthkit_data-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.072332 earthkit_data-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.072332 earthkit_data-0.8.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    65385 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/_static/earthkit-data.png
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.072332 earthkit_data-0.8.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/development.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.084332 earthkit_data-0.8.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/ads.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25628 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/bufr_synop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    80839 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/bufr_temp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13363 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/cache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/cds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    50147 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/data_from_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/default_fdb_schema
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/demo_sources_plugin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/ecmwf_open_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    55431 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/fdb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30675 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/file_parts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27906 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/from_object.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22543 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/geojson_geopandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25900 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_array_backends.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_fdb_write.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23026 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_indexing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20668 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_lat_lon_value.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    88655 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_missing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_nearest_gridpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   105060 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    47388 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_time_series.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/grib_to_netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34283 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/list_of_dict.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/mars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    49512 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/missing.grib
+-rw-r--r--   0 runner    (1001) docker     (127)    16882 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/multi_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    39146 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    65479 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/netcdf_fieldlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    35982 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/netcdf_opendap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/numpy_fieldlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/odb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/pandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/polytope.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   442939 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/projection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/settings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    45408 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/shapefile.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/synop_10.bufr
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/tar_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/temp_10.bufr
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/test.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/test.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/test.odb
+-rw-r--r--   0 runner    (1001) docker     (127)   521712 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/test4.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/test6.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/time_series.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/tuv_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/tuv_pl.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    28753 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/url.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/url_parts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/url_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    35809 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/examples/wekeo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.084332 earthkit_data-0.8.1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12485 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/data.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.084332 earthkit_data-0.8.1/docs/guide/data_format/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/data_format/bufr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/data_format/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/data_format/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/data_format/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/data_format/netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/data_format/odb.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.084332 earthkit_data-0.8.1/docs/guide/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/include/settings-get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/include/settings-reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/include/settings-set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/include/settings-temporary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.084332 earthkit_data-0.8.1/docs/guide/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/misc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/misc/parts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/misc/split_on.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34996 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/guide/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/howtos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.088332 earthkit_data-0.8.1/docs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/plugins/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/plugins/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/plugins/sources_plugin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.088332 earthkit_data-0.8.1/docs/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/release_notes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/release_notes/version_0.2_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/release_notes/version_0.3_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/release_notes/version_0.4_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/release_notes/version_0.5_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/release_notes/version_0.6_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/release_notes/version_0.7_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/release_notes/version_0.8_updates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/docs/skip_api_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:50:26.152333 earthkit_data-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.064332 earthkit_data-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.060332 earthkit_data-0.8.1/src/earthkit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.088332 earthkit_data-0.8.1/src/earthkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 20:50:25.000000 earthkit_data-0.8.1/src/earthkit/data/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.088332 earthkit_data-0.8.1/src/earthkit/data/arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/arguments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/arguments/args_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/arguments/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/arguments/earthkit_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/arguments/input_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/arguments/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.088332 earthkit_data-0.8.1/src/earthkit/data/conf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.092332 earthkit_data-0.8.1/src/earthkit/data/conf/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/conf/css/tab.css
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/conf/css/table.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/conf/css/tree.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/conf/global_grids.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/conf/gridspec.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/conf/gridspec_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.092332 earthkit_data-0.8.1/src/earthkit/data/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48574 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/fieldlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/core/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.092332 earthkit_data-0.8.1/src/earthkit/data/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/indexing/cube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.092332 earthkit_data-0.8.1/src/earthkit/data/indexing/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/indexing/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/indexing/database/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/indexing/database/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/indexing/database/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/indexing/fieldlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.096332 earthkit_data-0.8.1/src/earthkit/data/mergers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/mergers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/mergers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/mergers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.096332 earthkit_data-0.8.1/src/earthkit/data/mirrors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/mirrors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/mirrors/directory_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.096332 earthkit_data-0.8.1/src/earthkit/data/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.096332 earthkit_data-0.8.1/src/earthkit/data/readers/bufr/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/bufr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/bufr/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/bufr/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/covjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/geojson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.100332 earthkit_data-0.8.1/src/earthkit/data/readers/grib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17730 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/gridspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.100332 earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19393 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/grib/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.100332 earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/fieldlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/odb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/readers/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.104332 earthkit_data-0.8.1/src/earthkit/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/array_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/dummy.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/dummy_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/ecmwf_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/ecmwf_open_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/fdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/file_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/file_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/list_of_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/numpy_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/polytope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/virtual_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/wekeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sources/wekeocds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.104332 earthkit_data-0.8.1/src/earthkit/data/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sphinxext/generate_settings_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sphinxext/module_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/sphinxext/xref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.108332 earthkit_data-0.8.1/src/earthkit/data/translators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/translators/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/translators/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/translators/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/translators/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.108332 earthkit_data-0.8.1/src/earthkit/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.112332 earthkit_data-0.8.1/src/earthkit/data/utils/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/array/cupy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/array/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/array/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23088 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/factorise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11134 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/module_inputs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/progbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.112332 earthkit_data-0.8.1/src/earthkit/data/utils/projections/
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/projections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/projections/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/projections/proj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.112332 earthkit_data-0.8.1/src/earthkit/data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/vocabularies/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/vocabularies/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/vocabularies/grib-paramid.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/vocabularies/grib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.112332 earthkit_data-0.8.1/src/earthkit/data/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/wrappers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/wrappers/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/wrappers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/wrappers/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/wrappers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.112332 earthkit_data-0.8.1/src/earthkit/data/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/src/earthkit/data/writers/grib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.144333 earthkit_data-0.8.1/src/earthkit_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-28 20:50:25.000000 earthkit_data-0.8.1/src/earthkit_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15260 2024-05-28 20:50:26.000000 earthkit_data-0.8.1/src/earthkit_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:50:25.000000 earthkit_data-0.8.1/src/earthkit_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-28 20:50:25.000000 earthkit_data-0.8.1/src/earthkit_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 20:50:25.000000 earthkit_data-0.8.1/src/earthkit_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.116332 earthkit_data-0.8.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.116332 earthkit_data-0.8.1/tests/array_fieldlist/
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/array_fieldlist/array_fl_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fl_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fs_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fs_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fs_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.116332 earthkit_data-0.8.1/tests/bufr/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/bufr/test_bufr_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/bufr/test_bufr_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/bufr/test_bufr_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/bufr/test_bufr_file_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/bufr/test_bufr_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/bufr/test_bufr_sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/bufr/test_bufr_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.116332 earthkit_data-0.8.1/tests/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/constants/constants_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/constants/test_constants_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/constants/test_constants_sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/constants/test_constants_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/constants/test_constants_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/constants/test_constants_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/constants/test_contants_proc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.116332 earthkit_data-0.8.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/core/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/core/test_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/core/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/core/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/core/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.128332 earthkit_data-0.8.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2542596 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/NUTS_RG_20M_2021_3035.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   640295 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/NUTS_RG_20M_2021_3035.shp.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.128332 earthkit_data-0.8.1/tests/data/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/constants/proc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/empty_file.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/era5_2t_1.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/era5_2t_2.nc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.128332 earthkit_data-0.8.1/tests/data/gridspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/healpix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/reduced_gg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/reduced_ll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/reduced_rotated_gg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/regular_gg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/regular_ll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/rotated_gg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/rotated_ll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/sh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/gridspec/t_75_-60_10_40_5x5.grib1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1308 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/hovexp_vert_area.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    22138 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/mercator.grib
+-rw-r--r--   0 runner    (1001) docker     (127)    47520 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/ml_data.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/rgg_small_subarea_cellarea_ref.grib
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/rotated_N32_subarea.grib
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/rotated_wind_20x20.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/t_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/t_time_series.grib
+-rw-r--r--   0 runner    (1001) docker     (127)   524796 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/test4.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/test6.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/test_icon.grib
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/test_single.grib
+-rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/test_single.nc
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/test_single_with_missing.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/time_series.covjson
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/u_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/v_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/data/wind_20x20.grib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.128332 earthkit_data-0.8.1/tests/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/documentation/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/documentation/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/downstream-ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/environment-unit-tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.132332 earthkit_data-0.8.1/tests/grib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/grib_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_file_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_inidces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17333 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_url_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/grib/test_grib_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.132332 earthkit_data-0.8.1/tests/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/indexing/indexing_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/indexing/test_indexing_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/indexing/test_indexing_isel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/indexing/test_indexing_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/indexing/test_indexing_serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/indexing/test_order_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/indexing/test_selection_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.136332 earthkit_data-0.8.1/tests/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_fieldlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/netcdf/test_netcdf_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.136332 earthkit_data-0.8.1/tests/normalize/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/availability.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_aliases_grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_normalize_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/normalize/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.136332 earthkit_data-0.8.1/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/plugins/test_sources_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.140333 earthkit_data-0.8.1/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_covjson_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_geojson_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_grib_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_netcdf_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_odb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_reader_padding_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_shapefile_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_tar_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_unknown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/test_zip_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/unknown_file.unknown_ext
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/readers/unknown_text_file.unknown_ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.140333 earthkit_data-0.8.1/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_ecmwf_open_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_fdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_list_of_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_polytope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_wekeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/sources/test_wekeocds.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/test_00_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.140333 earthkit_data-0.8.1/tests/translators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/translators/test_translators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.144333 earthkit_data-0.8.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/test_download_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/test_module_inputs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/test_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/utils/test_projections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:50:26.144333 earthkit_data-0.8.1/tests/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/wrappers/test_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/wrappers/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/wrappers/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-28 20:50:16.000000 earthkit_data-0.8.1/tests/wrappers/test_xarray.py
```

### Comparing `earthkit_data-0.7.0/.github/ci-hpc-config.yml` & `earthkit_data-0.8.1/.github/ci-hpc-config.yml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/.github/workflows/ci.yml` & `earthkit_data-0.8.1/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   downstream-ci:
     name: downstream-ci
     if: ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
     uses: ecmwf-actions/downstream-ci/.github/workflows/downstream-ci.yml@main
     with:
       earthkit-data: ecmwf/earthkit-data@${{ github.event.pull_request.head.sha || github.sha }}
       codecov_upload: true
+      python_qa: true
     secrets: inherit
 
 
   # Build downstream packages on HPC
   downstream-ci-hpc:
     name: downstream-ci-hpc
     if: ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
```

### Comparing `earthkit_data-0.7.0/.github/workflows/ci_other.yml` & `earthkit_data-0.8.1/.github/workflows/legacy-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: ci
+name: legacy-ci
 
 on:
   push:
     branches:
     - main
     - develop
     tags:
@@ -61,68 +61,33 @@
         micromamba remove eccodes
     - name: Run tests without eccodes
       run: |
         python -m pytest -v -m 'no_eccodes'
 
 
   documentation:
-    needs: [unit-tests-no-eccodes]
     if: ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
     runs-on: ubuntu-latest
     defaults:
       run:
         shell: bash -l {0}
 
     steps:
     - uses: actions/checkout@v3
       with:
         ref: ${{ github.event.pull_request.head.sha || github.ref }}
     - name: Install Conda environment with Micromamba
       uses: mamba-org/provision-with-micromamba@v12
       with:
-        environment-file: environment.yml
+        environment-file: tests/environment-unit-tests.yml
         environment-name: DEVELOP
         channels: conda-forge
         cache-env: true
         cache-env-key: ubuntu-latest-3.10-no-eccodes
         extra-specs: |
           python=3.10
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Build documentation
       run: |
         make docs-build
-
-  distribution:
-    needs: [documentation]
-    if: ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
-    runs-on: ubuntu-latest
-
-    steps:
-    - uses: actions/checkout@v3
-      with:
-        ref: ${{ github.event.pull_request.head.sha || github.ref }}
-    - name: Build distributions
-      run: |
-        $CONDA/bin/python -m pip install build
-        $CONDA/bin/python -m build
-    - name: Publish a Python distribution to PyPI
-      if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}
-
-  notify:
-    if: always() && ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
-    needs:
-    - pre-commit
-    - unit-tests-no-eccodes
-    - documentation
-    runs-on: ubuntu-latest
-    steps:
-    - name: Trigger Teams notification
-      uses: ecmwf-actions/notify-teams@v1
-      with:
-        incoming_webhook: ${{ secrets.MS_TEAMS_INCOMING_WEBHOOK }}
-        needs_context: ${{ toJSON(needs) }}
```

### Comparing `earthkit_data-0.7.0/.gitignore` & `earthkit_data-0.8.1/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # setuptools-scm
 version.py
+_version.py
 
 # Sphinx automatic generation of API
 docs/_api/
 
 # Created by https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm
 # Edit at https://www.toptal.com/developers/gitignore?templates=python,jupyternotebooks,vim,visualstudiocode,pycharm
```

### Comparing `earthkit_data-0.7.0/.pre-commit-config.yaml` & `earthkit_data-0.8.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   - id: debug-statements
   - id: mixed-line-ending
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/psf/black
-  rev: 23.9.1
+  rev: 24.4.2
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.8
   hooks:
   - id: blackdoc
     additional_dependencies: [black==23.3.0]
```

### Comparing `earthkit_data-0.7.0/LICENSE` & `earthkit_data-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/Makefile` & `earthkit_data-0.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/PKG-INFO` & `earthkit_data-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: earthkit-data
-Version: 0.7.0
+Version: 0.8.1
 Summary: A format-agnostic Python interface for geospatial data
-License: Apache License 2.0
+Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
+License: Apache License Version 2.0
+Project-URL: Documentation, https://earthkit-data.readthedocs.io/
+Project-URL: Homepage, https://github.com/ecmwf/earthkit-data/
+Project-URL: Issues, https://github.com/ecmwf/earthkit-data.issues
+Project-URL: Repository, https://github.com/ecmwf/earthkit-data/
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cfgrib>=0.9.10.1
 Requires-Dist: eccodes>=1.7.0
 Requires-Dist: dask
 Requires-Dist: entrypoints
 Requires-Dist: filelock
@@ -27,54 +33,55 @@
 Requires-Dist: multiurl
 Requires-Dist: netcdf4
 Requires-Dist: pandas
 Requires-Dist: pdbufr>=0.11.0
 Requires-Dist: pyyaml
 Requires-Dist: tqdm>=4.63.0
 Requires-Dist: xarray>=0.19.0
+Requires-Dist: earthkit-geo>=0.2.0
 Requires-Dist: earthkit-meteo>=0.0.1
-Provides-Extra: mars
-Requires-Dist: ecmwf-api-client>=1.6.1; extra == "mars"
-Provides-Extra: cds
-Requires-Dist: cdsapi; extra == "cds"
-Provides-Extra: fdb
-Requires-Dist: pyfdb; extra == "fdb"
-Provides-Extra: polytope
-Requires-Dist: polytope-client>=0.7.4; extra == "polytope"
-Provides-Extra: wekeo
-Requires-Dist: hda; extra == "wekeo"
-Provides-Extra: ecmwf-opendata
-Requires-Dist: ecmwf-opendata>=0.3.3; extra == "ecmwf-opendata"
-Provides-Extra: odb
-Requires-Dist: pyodc; extra == "odb"
-Provides-Extra: projection
-Requires-Dist: cartopy; extra == "projection"
-Provides-Extra: geopandas
-Requires-Dist: geopandas; extra == "geopandas"
-Provides-Extra: eccovjson
-Requires-Dist: eccovjson>=0.0.5; extra == "eccovjson"
 Provides-Extra: all
 Requires-Dist: earthkit-data[mars]; extra == "all"
 Requires-Dist: earthkit-data[cds]; extra == "all"
 Requires-Dist: earthkit-data[ecmwf-opendata]; extra == "all"
 Requires-Dist: earthkit-data[fdb]; extra == "all"
 Requires-Dist: earthkit-data[polytope]; extra == "all"
 Requires-Dist: earthkit-data[wekeo]; extra == "all"
 Requires-Dist: earthkit-data[odb]; extra == "all"
 Requires-Dist: earthkit-data[projection]; extra == "all"
 Requires-Dist: earthkit-data[geopandas]; extra == "all"
 Requires-Dist: earthkit-data[eccovjson]; extra == "all"
+Provides-Extra: cds
+Requires-Dist: cdsapi; extra == "cds"
+Provides-Extra: eccovjson
+Requires-Dist: eccovjson>=0.0.5; extra == "eccovjson"
+Provides-Extra: ecmwf-opendata
+Requires-Dist: ecmwf-opendata>=0.3.3; extra == "ecmwf-opendata"
+Provides-Extra: fdb
+Requires-Dist: pyfdb; extra == "fdb"
+Provides-Extra: geopandas
+Requires-Dist: geopandas; extra == "geopandas"
+Provides-Extra: mars
+Requires-Dist: ecmwf-api-client>=1.6.1; extra == "mars"
+Provides-Extra: odb
+Requires-Dist: pyodc; extra == "odb"
+Provides-Extra: polytope
+Requires-Dist: polytope-client>=0.7.4; extra == "polytope"
+Provides-Extra: projection
+Requires-Dist: cartopy; extra == "projection"
 Provides-Extra: test
 Requires-Dist: earthkit-data[all]; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-forked; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
 Requires-Dist: nbformat; extra == "test"
 Requires-Dist: nbconvert; extra == "test"
+Provides-Extra: wekeo
+Requires-Dist: hda; extra == "wekeo"
 
 # earthkit-data
 
 <img src="docs/_static/earthkit-data.png" width="120">
 
 [![PyPI version fury.io](https://badge.fury.io/py/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
```

### Comparing `earthkit_data-0.7.0/README.md` & `earthkit_data-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/Makefile` & `earthkit_data-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/_static/earthkit-data.png` & `earthkit_data-0.8.1/docs/_static/earthkit-data.png`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/_static/style.css` & `earthkit_data-0.8.1/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/api.rst` & `earthkit_data-0.8.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/conf.py` & `earthkit_data-0.8.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,22 +41,21 @@
     "earthkit.data.sphinxext.module_output",
 ]
 
 # autodoc configuration
 autodoc_typehints = "none"
 
 # autoapi configuration
-autoapi_dirs = ["../earthkit/data"]
-autoapi_ignore = ["*/version.py", "sphinxext/*"]
+autoapi_dirs = ["../src/earthkit/data"]
+autoapi_ignore = ["*/_version.py", "sphinxext/*"]
 autoapi_options = [
     "members",
     "undoc-members",
     "show-inheritance",
     "show-module-summary",
-    "imported-members",
     "inherited-members",
 ]
 autoapi_root = "_api"
 autoapi_member_order = "alphabetical"
 autoapi_add_toctree_entry = False
 
 # napoleon configuration
```

### Comparing `earthkit_data-0.7.0/docs/development.rst` & `earthkit_data-0.8.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/ads.ipynb` & `earthkit_data-0.8.1/docs/examples/ads.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/bufr_synop.ipynb` & `earthkit_data-0.8.1/docs/examples/bufr_synop.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/bufr_temp.ipynb` & `earthkit_data-0.8.1/docs/examples/bufr_temp.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/cache.ipynb` & `earthkit_data-0.8.1/docs/examples/cache.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/cds.ipynb` & `earthkit_data-0.8.1/docs/examples/cds.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/data_from_stream.ipynb` & `earthkit_data-0.8.1/docs/examples/data_from_stream.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9602839595792237%*

 * *Differences: {"'cells'": "{7: {'source': ['We load it into earthkit-data.']}, 9: {'source': ['Using this object "*

 * *            'we can iterate through the stream. As we progressing with the iteration '*

 * *            ':py:class:`~data.readers.grib.codes.GribField` objects are created then get deleted '*

 * *            'when going out of scope. As a result, only one GRIB message is kept in memory at a '*

 * *            "time.']}, 13: {'id': 'judicial-backing', 'source': ['### Using batched']}, 14: {'id': "*

 * *            "'fb4528e4-f64 […]*

```diff
@@ -92,15 +92,15 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "We load it into earthkit-data by using the default settings (:ref:`batch_size <data-sources-stream>`\\=1). With this when we iterate through *ds* it will consume one message from the stream at a time:"
+                "We load it into earthkit-data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "durable-helicopter",
             "metadata": {
@@ -123,15 +123,15 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "At this point nothing is read from the stream. As we progressing with the iteration :py:class:`~data.readers.grib.codes.GribField` objects are created then get deleted when going out of scope. As a result, only one GRIB message is kept in memory at a time."
+                "Using this object we can iterate through the stream. As we progressing with the iteration :py:class:`~data.readers.grib.codes.GribField` objects are created then get deleted when going out of scope. As a result, only one GRIB message is kept in memory at a time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "animated-prayer",
             "metadata": {
@@ -177,238 +177,198 @@
             "outputs": [],
             "source": [
                 "stream.close()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7122a9a4-9ca0-4d75-9194-144074c6dcad",
+            "id": "judicial-backing",
             "metadata": {},
             "source": [
-                "### Using group_by"
+                "### Using batched"
             ]
         },
         {
             "cell_type": "raw",
-            "id": "d970d832-7203-498f-81d6-99434ce42b88",
+            "id": "fb4528e4-f649-4a5b-92b4-e92e9391851b",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "When we use the :ref:`group_by <data-sources-stream>` option :ref:`from_source() <data-sources-stream>` gives us a stream iterator object. Each iteration step results in a :py:class:`FieldList <data.readers.grib.index.GribFieldList>` object, which is built by consuming GRIB messages from the stream until the values of the metadata keys specified in :ref:`group_by <data-sources-stream>` change. The generated :py:class:`FieldList <data.readers.grib.index.GribFieldList>` keeps GRIB messages in memory then gets deleted when going out of scope."
+                "When we use the :py:meth:`batched <data.readers.grib.index.GribFieldList.batched>` method we can iterate throught the stream in batches of fixed size. In this example we create a stream and read 2 fields from it at a time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "8e1be478-6eb6-4732-bb96-9d6fa942c20d",
+            "id": "placed-blues",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
-            "outputs": [],
-            "source": [
-                "stream = open(\"test6.grib\", \"rb\")\n",
-                "ds = earthkit.data.from_source(\"stream\", stream, group_by=\"level\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "id": "810cc3eb-4a3f-4806-b799-23e1bc5523c6",
-            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "len=3\n",
-                        " GribField(t,1000,20180801,1200,0,0)\n",
-                        " GribField(u,1000,20180801,1200,0,0)\n",
-                        " GribField(v,1000,20180801,1200,0,0)\n",
-                        "len=3\n",
-                        " GribField(t,850,20180801,1200,0,0)\n",
-                        " GribField(u,850,20180801,1200,0,0)\n",
-                        " GribField(v,850,20180801,1200,0,0)\n"
+                        "len=2 [('t', 1000), ('u', 1000)]\n",
+                        "len=2 [('v', 1000), ('t', 850)]\n",
+                        "len=2 [('u', 850), ('v', 850)]\n"
                     ]
                 }
             ],
             "source": [
-                "for f in ds:\n",
-                "    # f is a fieldlist\n",
-                "    print(f\"len={len(f)}\")\n",
-                "    for g in f:\n",
-                "        print(f\" {g}\")"
+                "stream = open(\"test6.grib\", \"rb\")\n",
+                "ds = earthkit.data.from_source(\"stream\", stream)\n",
+                "\n",
+                "# f is a fieldlist\n",
+                "for f in ds.batched(2):\n",
+                "    print(f\"len={len(f)} {f.metadata(('param', 'level'))}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "89d33d4c-00d2-4f0b-996e-aaf5a5c9e161",
+            "id": "unavailable-actress",
             "metadata": {},
             "source": [
                 "Having finished the iteration there is no data available in *ds*.  We can close the stream:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
-            "id": "2ac79f14-cb43-40c0-8a56-9bc16943d7e7",
+            "execution_count": 8,
+            "id": "jewish-season",
             "metadata": {},
             "outputs": [],
             "source": [
                 "stream.close()"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "judicial-backing",
-            "metadata": {},
-            "source": [
-                "### Using batch_size"
-            ]
-        },
-        {
             "cell_type": "raw",
-            "id": "fb4528e4-f649-4a5b-92b4-e92e9391851b",
+            "id": "ed0b0e9c-1016-474b-8ea0-c65d864d2427",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "The :ref:`batch_size <data-sources-stream>` option controls how many fields we read from the stream in one go. Please note that :ref:`batch_size <data-sources-stream>` cannot be used together with *group_by*. In this example we create a stream and read 2 fields from it at a time by using :ref:`batch_size <data-sources-stream>`\\=2 in :ref:`from_source() <data-sources-stream>`:"
+                "It is possible to use a batch size that is not a factor of the total number fields in the stream. In this case the last batch will simply contain less fields than the specified batch size."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "id": "placed-blues",
+            "execution_count": 9,
+            "id": "bf94a190-ec0e-4172-8e75-6518e48f50a4",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
-            "outputs": [],
-            "source": [
-                "stream = open(\"test6.grib\", \"rb\")\n",
-                "ds = earthkit.data.from_source(\"stream\", stream, batch_size=2)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 11,
-            "id": "outside-tennis",
-            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "len=2\n",
-                        " GribField(t,1000,20180801,1200,0,0)\n",
-                        " GribField(u,1000,20180801,1200,0,0)\n",
-                        "len=2\n",
-                        " GribField(v,1000,20180801,1200,0,0)\n",
-                        " GribField(t,850,20180801,1200,0,0)\n",
-                        "len=2\n",
-                        " GribField(u,850,20180801,1200,0,0)\n",
-                        " GribField(v,850,20180801,1200,0,0)\n"
+                        "len=4 [('t', 1000), ('u', 1000), ('v', 1000), ('t', 850)]\n",
+                        "len=2 [('u', 850), ('v', 850)]\n"
                     ]
                 }
             ],
             "source": [
-                "for f in ds:\n",
-                "    # f is a fieldlist\n",
-                "    print(f\"len={len(f)}\")\n",
-                "    for g in f:\n",
-                "        print(f\" {g}\")"
+                "stream = open(\"test6.grib\", \"rb\")\n",
+                "ds = earthkit.data.from_source(\"stream\", stream)\n",
+                "\n",
+                "# f is a fieldlist\n",
+                "for f in ds.batched(4):\n",
+                "    print(f\"len={len(f)} {f.metadata(('param', 'level'))}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "unavailable-actress",
-            "metadata": {},
-            "source": [
-                "Having finished the iteration there is no data available in *ds*.  We can close the stream:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 12,
-            "id": "jewish-season",
+            "id": "7122a9a4-9ca0-4d75-9194-144074c6dcad",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "stream.close()"
+                "### Using group_by"
             ]
         },
         {
             "cell_type": "raw",
-            "id": "ed0b0e9c-1016-474b-8ea0-c65d864d2427",
+            "id": "d970d832-7203-498f-81d6-99434ce42b88",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "It is possible to set a batch size that is not a factor of the total number fields in the stream. In this case the last batch will simply contain less fields than prescribed by :ref:`batch_size <data-sources-stream>`."
+                "When we use the :py:meth:`group_by <data.readers.grib.index.GribFieldList.group_by>` method we can iterate throught the stream in groups defined by metadata keys. Each iteration step results in a :py:class:`FieldList <data.readers.grib.index.GribFieldList>` object, which is built by consuming GRIB messages from the stream until the values of the metadata keys change. The generated :py:class:`FieldList <data.readers.grib.index.GribFieldList>` keeps GRIB messages in memory then gets deleted when going out of scope."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "id": "bf94a190-ec0e-4172-8e75-6518e48f50a4",
+            "execution_count": 10,
+            "id": "8e1be478-6eb6-4732-bb96-9d6fa942c20d",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "len=4\n",
-                        " GribField(t,1000,20180801,1200,0,0)\n",
-                        " GribField(u,1000,20180801,1200,0,0)\n",
-                        " GribField(v,1000,20180801,1200,0,0)\n",
-                        " GribField(t,850,20180801,1200,0,0)\n",
-                        "len=2\n",
-                        " GribField(u,850,20180801,1200,0,0)\n",
-                        " GribField(v,850,20180801,1200,0,0)\n"
+                        "len=3 [('t', 1000), ('u', 1000), ('v', 1000)]\n",
+                        "len=3 [('t', 850), ('u', 850), ('v', 850)]\n"
                     ]
                 }
             ],
             "source": [
                 "stream = open(\"test6.grib\", \"rb\")\n",
-                "ds = earthkit.data.from_source(\"stream\", stream, batch_size=4)\n",
+                "ds = earthkit.data.from_source(\"stream\", stream)\n",
                 "\n",
-                "for f in ds:\n",
-                "    # f is a fieldlist\n",
-                "    print(f\"len={len(f)}\")\n",
-                "    for g in f:\n",
-                "        print(f\" {g}\")"
+                "# f is a fieldlist\n",
+                "for f in ds.group_by(\"level\"):\n",
+                "    print(f\"len={len(f)} {f.metadata(('param', 'level'))}\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "89d33d4c-00d2-4f0b-996e-aaf5a5c9e161",
+            "metadata": {},
+            "source": [
+                "Having finished the iteration there is no data available in *ds*.  We can close the stream:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "2ac79f14-cb43-40c0-8a56-9bc16943d7e7",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "stream.close()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "permanent-uncertainty",
             "metadata": {},
             "source": [
@@ -423,70 +383,66 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "We can also set :ref:`batch_size <data-sources-stream>`\\=0 in  :ref:`from_source() <data-sources-stream>`."
+                "We can load the whole stream into memory by using ``read_all=True`` in :ref:`from_source() <data-sources-stream>`. The resulting object will be a :py:class:`FieldList` storing all the GRIB messages in memory."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 12,
             "id": "simple-london",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "stream = open(\"test6.grib\", \"rb\")\n",
-                "ds = earthkit.data.from_source(\"stream\", stream, batch_size=0)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "seeing-freight",
-            "metadata": {},
-            "source": [
-                "The resulting earthkit-data object is empty at this point. However, as soon as we call any method on it it will consume the whole stream and load all the GRIB messages into memory. They will be stored in memory as long as *ds* exists.\n",
-                "\n",
-                "We can call all the standard earthkit-data methods on *ds*:"
+                "ds = earthkit.data.from_source(\"stream\", stream, read_all=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 13,
             "id": "meaning-oxide",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "6"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "len(ds)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 14,
             "id": "copyrighted-walnut",
-            "metadata": {},
+            "metadata": {
+                "editable": true,
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
@@ -614,26 +570,26 @@
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  \n",
                             "3       an       0  regular_ll  \n",
                             "4       an       0  regular_ll  \n",
                             "5       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 15,
             "id": "static-reasoning",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -703,27 +659,27 @@
                             "1   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = ds.sel(param=\"t\")\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 16,
             "id": "spanish-wagon",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -1105,17 +1061,17 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2024-01-02T11:25 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-2b6366e3-a8a7-4329-afeb-8d7c60cd86d5' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-2b6366e3-a8a7-4329-afeb-8d7c60cd86d5' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-a7eac6c6-aa02-4171-886e-e66d33d35f24' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a7eac6c6-aa02-4171-886e-e66d33d35f24' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-e33ea9dd-6e7b-42ae-8e7a-e54b2053841d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e33ea9dd-6e7b-42ae-8e7a-e54b2053841d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-5059bdce-f75e-4b9c-8d41-789ab1dfaa5b' class='xr-var-data-in' type='checkbox'><label for='data-5059bdce-f75e-4b9c-8d41-789ab1dfaa5b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-50a7a563-83df-4a9c-a7f1-9c6a1dbbb921' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-50a7a563-83df-4a9c-a7f1-9c6a1dbbb921' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-63f86500-922e-49d2-bfbe-4f42cfe8f798' class='xr-var-data-in' type='checkbox'><label for='data-63f86500-922e-49d2-bfbe-4f42cfe8f798' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-14b996b3-cd4d-45a0-b8ac-ae26b0e52d40' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-14b996b3-cd4d-45a0-b8ac-ae26b0e52d40' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-64fd0845-29a1-409f-8088-47adfdb5ac56' class='xr-var-data-in' type='checkbox'><label for='data-64fd0845-29a1-409f-8088-47adfdb5ac56' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>1e+03 850.0</div><input id='attrs-c4af0352-49c7-4a64-be7e-b682e197c219' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-c4af0352-49c7-4a64-be7e-b682e197c219' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-7fc64dc7-6872-4c13-8655-bdeb8a7a3f7e' class='xr-var-data-in' type='checkbox'><label for='data-7fc64dc7-6872-4c13-8655-bdeb8a7a3f7e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000.,  850.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-8ee8154b-5dc2-402f-83ab-8b3fbd5267db' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-8ee8154b-5dc2-402f-83ab-8b3fbd5267db' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e848f2b9-dac3-438c-afd8-7e40a6c641b8' class='xr-var-data-in' type='checkbox'><label for='data-e848f2b9-dac3-438c-afd8-7e40a6c641b8' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-ef413f70-07b8-42c1-892e-f1a3f57ebe26' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ef413f70-07b8-42c1-892e-f1a3f57ebe26' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-257f8190-b5e9-49b3-8a81-36406f1d72be' class='xr-var-data-in' type='checkbox'><label for='data-257f8190-b5e9-49b3-8a81-36406f1d72be' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-17f1768b-794c-40c1-9a57-b8481f6c46ff' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-17f1768b-794c-40c1-9a57-b8481f6c46ff' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-81984098-190c-4d74-9157-9d2ecf2112c2' class='xr-var-data-in' type='checkbox'><label for='data-81984098-190c-4d74-9157-9d2ecf2112c2' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-bea46411-fb89-4567-b825-edc4ed7c5d50' class='xr-section-summary-in' type='checkbox'  checked><label for='section-bea46411-fb89-4567-b825-edc4ed7c5d50' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-cbe2446d-f0d7-4600-bd9c-c89a99ac5433' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-cbe2446d-f0d7-4600-bd9c-c89a99ac5433' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d7167053-4c06-4230-8bd1-3e7c6bcad833' class='xr-var-data-in' type='checkbox'><label for='data-d7167053-4c06-4230-8bd1-3e7c6bcad833' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-879b4eb2-98be-4a35-8940-d7401dcd153f' class='xr-section-summary-in' type='checkbox'  ><label for='section-879b4eb2-98be-4a35-8940-d7401dcd153f' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e96e7475-ded6-4e66-b16d-2ff1b0566f9d' class='xr-index-data-in' type='checkbox'/><label for='index-e96e7475-ded6-4e66-b16d-2ff1b0566f9d' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1f4de1ec-d805-4b58-9ac8-07d0af42a271' class='xr-index-data-in' type='checkbox'/><label for='index-1f4de1ec-d805-4b58-9ac8-07d0af42a271' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-d98c7386-5553-4ea4-ac0b-682239f9678e' class='xr-index-data-in' type='checkbox'/><label for='index-d98c7386-5553-4ea4-ac0b-682239f9678e' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1988c873-2505-4f89-8e28-51160ad38a1d' class='xr-index-data-in' type='checkbox'/><label for='index-1988c873-2505-4f89-8e28-51160ad38a1d' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1000.0, 850.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-11b310dc-6319-4b19-ac01-96b99624bcd7' class='xr-index-data-in' type='checkbox'/><label for='index-11b310dc-6319-4b19-ac01-96b99624bcd7' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c9c694fe-0537-4ce8-9c4b-9a57887113b3' class='xr-index-data-in' type='checkbox'/><label for='index-c9c694fe-0537-4ce8-9c4b-9a57887113b3' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0, 300.0,\n",
+                            "    history:                 2024-04-23T17:21 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-a47d76ba-66ad-4a2a-a111-e4d676370ddc' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-a47d76ba-66ad-4a2a-a111-e4d676370ddc' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-fe4e2d0e-2360-4e8f-a80a-dd77500ce15c' class='xr-section-summary-in' type='checkbox'  checked><label for='section-fe4e2d0e-2360-4e8f-a80a-dd77500ce15c' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-67f4a3b3-679d-4c4c-b859-3f1c641e28a3' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-67f4a3b3-679d-4c4c-b859-3f1c641e28a3' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-46472886-138e-4d6e-81a3-0333b6717851' class='xr-var-data-in' type='checkbox'><label for='data-46472886-138e-4d6e-81a3-0333b6717851' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-adea931c-4186-4833-a1fe-ab4c2a4c0775' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-adea931c-4186-4833-a1fe-ab4c2a4c0775' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-89dd04b7-7082-48c5-b38c-1fc78c3e6688' class='xr-var-data-in' type='checkbox'><label for='data-89dd04b7-7082-48c5-b38c-1fc78c3e6688' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-a5fb9bf4-60fd-4b9f-8e5e-586fc607d2fd' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a5fb9bf4-60fd-4b9f-8e5e-586fc607d2fd' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-19a34a8a-d7f5-436e-8f1d-5ba45dab6574' class='xr-var-data-in' type='checkbox'><label for='data-19a34a8a-d7f5-436e-8f1d-5ba45dab6574' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>1e+03 850.0</div><input id='attrs-3b94023e-43e4-41c3-85e3-6ff7b102c517' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-3b94023e-43e4-41c3-85e3-6ff7b102c517' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f4b2b9e4-e814-44e6-a91b-8bdbd42fea49' class='xr-var-data-in' type='checkbox'><label for='data-f4b2b9e4-e814-44e6-a91b-8bdbd42fea49' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000.,  850.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-1384986a-358a-40bc-9240-b5c803686078' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1384986a-358a-40bc-9240-b5c803686078' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-70adce6a-88bb-4950-a812-314913789f91' class='xr-var-data-in' type='checkbox'><label for='data-70adce6a-88bb-4950-a812-314913789f91' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-4c9560ca-d325-490f-923f-befd21aff2f0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-4c9560ca-d325-490f-923f-befd21aff2f0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d4c7d721-1e92-4bbc-aabe-a7d1110d96ce' class='xr-var-data-in' type='checkbox'><label for='data-d4c7d721-1e92-4bbc-aabe-a7d1110d96ce' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-3b03ad76-2023-4b2a-8b52-e7d605a6e9dc' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-3b03ad76-2023-4b2a-8b52-e7d605a6e9dc' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e6b9fb6e-f380-4edc-9528-e5237d591a96' class='xr-var-data-in' type='checkbox'><label for='data-e6b9fb6e-f380-4edc-9528-e5237d591a96' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-3cc47aae-6ce7-4c1d-b687-16c41aec648b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-3cc47aae-6ce7-4c1d-b687-16c41aec648b' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-ae33e165-9d94-488f-afd0-9a9bc8377be8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ae33e165-9d94-488f-afd0-9a9bc8377be8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-84e62f11-cdfd-457d-94ac-b356fa63d238' class='xr-var-data-in' type='checkbox'><label for='data-84e62f11-cdfd-457d-94ac-b356fa63d238' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-9baa4ba1-c488-4b2c-a95a-42ed1557b710' class='xr-section-summary-in' type='checkbox'  ><label for='section-9baa4ba1-c488-4b2c-a95a-42ed1557b710' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-3a569b72-299d-4222-9068-d804d762fc75' class='xr-index-data-in' type='checkbox'/><label for='index-3a569b72-299d-4222-9068-d804d762fc75' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-4bf4263e-bc24-4cdd-b24d-7ae3d16f138b' class='xr-index-data-in' type='checkbox'/><label for='index-4bf4263e-bc24-4cdd-b24d-7ae3d16f138b' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0a1ac57a-c711-4e0f-aec3-9f7a8436fe51' class='xr-index-data-in' type='checkbox'/><label for='index-0a1ac57a-c711-4e0f-aec3-9f7a8436fe51' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c7b72de6-b478-4855-b8aa-219750039f87' class='xr-index-data-in' type='checkbox'/><label for='index-c7b72de6-b478-4855-b8aa-219750039f87' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1000.0, 850.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-decb1328-511f-47e2-8398-7551d478f6f5' class='xr-index-data-in' type='checkbox'/><label for='index-decb1328-511f-47e2-8398-7551d478f6f5' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-2c81760b-834b-49cd-9179-b8c1f7085f17' class='xr-index-data-in' type='checkbox'/><label for='index-2c81760b-834b-49cd-9179-b8c1f7085f17' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0, 300.0,\n",
                             "       330.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-d1e2fb57-df40-40db-9b0e-457fac32c1d8' class='xr-section-summary-in' type='checkbox'  checked><label for='section-d1e2fb57-df40-40db-9b0e-457fac32c1d8' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2024-01-02T11:25 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.32.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-775bed68-8fc5-42ab-864d-f62e22605f6b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-775bed68-8fc5-42ab-864d-f62e22605f6b' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2024-04-23T17:21 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.36.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * number         (number) int64 0\n",
@@ -1130,18 +1086,18 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2024-01-02T11:25 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2024-04-23T17:21 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = a.to_xarray()\n",
                 "a"
@@ -1153,15 +1109,15 @@
             "metadata": {},
             "source": [
                 "We close the stream:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 17,
             "id": "through-mistress",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
@@ -1170,17 +1126,17 @@
             "source": [
                 "stream.close()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "dev",
+            "display_name": "dev_ecc",
             "language": "python",
-            "name": "dev"
+            "name": "dev_ecc"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `earthkit_data-0.7.0/docs/examples/default_fdb_schema` & `earthkit_data-0.8.1/docs/examples/default_fdb_schema`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/demo_sources_plugin.ipynb` & `earthkit_data-0.8.1/docs/examples/demo_sources_plugin.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/ecmwf_open_data.ipynb` & `earthkit_data-0.8.1/docs/examples/ecmwf_open_data.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/fdb.ipynb` & `earthkit_data-0.8.1/docs/examples/fdb.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9665640856207334%*

 * *Differences: {"'cells'": '{4: {\'execution_count\': 2, \'source\': {insert: [(4, "    \'date\': '*

 * *            '\'20240421\',\\n")], delete: [4]}}, 7: {\'source\': [\'#### Iteration with one field '*

 * *            "at a time in memory']}, 9: {'outputs': {0: {'text': "*

 * *            "['GribField(msl,None,20240421,0,0,0)\\n', 'GribField(2t,None,20240421,0,0,0)\\n', "*

 * *            "'GribField(2d,None,20240421,0,0,0)\\n', 'GribField(msl,None,20240421,1200,0,0)\\n', "*

 * *            "'GribField(2t,None,20240421,1200,0,0)\\n', "*

 * *       […]*

```diff
@@ -43,24 +43,24 @@
             "metadata": {},
             "source": [
                 "The following request was  written to retrieve data from the operational FDB at ECMWF.  Please note that the **date** must be adjusted since FDB at ECMWF only stores the most recent dates."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 2,
             "id": "drawn-renewal",
             "metadata": {},
             "outputs": [],
             "source": [
                 "request = {\n",
                 "    'class': 'od',\n",
                 "    'expver': '0001',\n",
                 "    'stream': 'oper',\n",
-                "    'date': '20230607',\n",
+                "    'date': '20240421',\n",
                 "    'time': [0, 12],\n",
                 "    'domain': 'g',\n",
                 "    'type': 'an',\n",
                 "    'levtype': 'sfc',\n",
                 "    'step': 0,\n",
                 "    'param': [151, 167, 168]\n",
                 "}"
@@ -97,15 +97,15 @@
                 "raw_mimetype": "",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "#### Stream: iteration with one field at a time in memory"
+                "#### Iteration with one field at a time in memory"
             ]
         },
         {
             "cell_type": "raw",
             "id": "eccee7c9-7769-436a-b764-18045c04d86b",
             "metadata": {
                 "editable": true,
@@ -131,20 +131,20 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "GribField(msl,None,20230607,0,0,0)\n",
-                        "GribField(2t,None,20230607,0,0,0)\n",
-                        "GribField(2d,None,20230607,0,0,0)\n",
-                        "GribField(msl,None,20230607,1200,0,0)\n",
-                        "GribField(2t,None,20230607,1200,0,0)\n",
-                        "GribField(2d,None,20230607,1200,0,0)\n"
+                        "GribField(msl,None,20240421,0,0,0)\n",
+                        "GribField(2t,None,20240421,0,0,0)\n",
+                        "GribField(2d,None,20240421,0,0,0)\n",
+                        "GribField(msl,None,20240421,1200,0,0)\n",
+                        "GribField(2t,None,20240421,1200,0,0)\n",
+                        "GribField(2d,None,20240421,1200,0,0)\n"
                     ]
                 }
             ],
             "source": [
                 "ds = earthkit.data.from_source(\"fdb\", request)\n",
                 "for f in ds:\n",
                 "    print(f)"
@@ -182,30 +182,30 @@
         {
             "cell_type": "markdown",
             "id": "7e63bb45-b15d-4a89-b882-bf4db27d4f39",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "#### Stream: using group_by"
+                "#### Iteration with group_by"
             ]
         },
         {
             "cell_type": "raw",
             "id": "1f3f2802-7af9-48da-a964-7769c951ce48",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "When we use the :ref:`group_by <data-sources-fdb>` option :ref:`from_source() <data-sources-fdb>` gives us a stream iterator object. Each iteration step results in a Fieldlist object, which is built by consuming GRIB messages from the stream until the values of the metadata keys specified in :ref:`group_by <data-sources-fdb>` change. The generated Fieldlist keeps GRIB messages in memory then gets deleted when going out of scope."
+                "When we use the :py:meth:`group_by <data.readers.grib.index.GribFieldList.group_by>` method we can iterate throught the stream in groups defined by metadata keys. Each iteration step results in a :py:class:`FieldList <data.readers.grib.index.GribFieldList>` object, which is built by consuming GRIB messages from the stream until the values of the metadata keys change. The generated :py:class:`FieldList <data.readers.grib.index.GribFieldList>` keeps GRIB messages in memory then gets deleted when going out of scope."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "574757de-cc05-4d73-b71c-cd49af36f655",
             "metadata": {
@@ -216,54 +216,46 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
-                        " GribField(msl,None,20230607,0,0,0)\n",
-                        " GribField(2t,None,20230607,0,0,0)\n",
-                        " GribField(2d,None,20230607,0,0,0)\n",
-                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
-                        " GribField(msl,None,20230607,1200,0,0)\n",
-                        " GribField(2t,None,20230607,1200,0,0)\n",
-                        " GribField(2d,None,20230607,1200,0,0)\n"
+                        "len=3 [('msl', 0), ('2t', 0), ('2d', 0)]\n",
+                        "len=3 [('msl', 0), ('2t', 0), ('2d', 0)]\n"
                     ]
                 }
             ],
             "source": [
-                "ds = earthkit.data.from_source(\"fdb\", request, group_by=\"time\")\n",
-                "for f in ds:\n",
-                "    print(type(f))\n",
-                "    for g in f:\n",
-                "        print(f\" {g}\")"
+                "ds = earthkit.data.from_source(\"fdb\", request)\n",
+                "for f in ds.group_by(\"time\"):\n",
+                "    print(f\"len={len(f)} {f.metadata(('param', 'level'))}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ethical-canyon",
             "metadata": {},
             "source": [
-                "#### Stream: using batch_size"
+                "#### Iteration with batched"
             ]
         },
         {
             "cell_type": "raw",
             "id": "731f4f11-d050-4754-8862-5ca5b2837934",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "We can read multiple fields into memory from the stream at a time by using :ref:`batch_size <data-sources-fdb>` in :ref:`from_source <data-sources-fdb>`, Please note that  :ref:`batch_size <data-sources-fdb>` cannot be used together with :ref:`group_by <data-sources-fdb>`."
+                "When we use the :py:meth:`batched <data.readers.grib.index.GribFieldList.batched>` method we can iterate throught the stream in batches of fixed size. In this example we create a stream and read 2 fields from it at a time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "precise-guyana",
             "metadata": {
@@ -274,55 +266,47 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
-                        " GribField(msl,None,20230607,0,0,0)\n",
-                        " GribField(2t,None,20230607,0,0,0)\n",
-                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
-                        " GribField(2d,None,20230607,0,0,0)\n",
-                        " GribField(msl,None,20230607,1200,0,0)\n",
-                        "<class 'earthkit.data.readers.grib.memory.FieldListInMemory'>\n",
-                        " GribField(2t,None,20230607,1200,0,0)\n",
-                        " GribField(2d,None,20230607,1200,0,0)\n"
+                        "len=2 [('msl', 0), ('2t', 0)]\n",
+                        "len=2 [('2d', 0), ('msl', 0)]\n",
+                        "len=2 [('2t', 0), ('2d', 0)]\n"
                     ]
                 }
             ],
             "source": [
-                "ds = earthkit.data.from_source(\"fdb\", request, batch_size=2)\n",
-                "for f in ds:\n",
-                "    print(type(f))\n",
-                "    for g in f:\n",
-                "        print(f\" {g}\")"
+                "ds = earthkit.data.from_source(\"fdb\", request)\n",
+                "for f in ds.batched(2):\n",
+                "    print(f\"len={len(f)} {f.metadata(('param', 'level'))}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "through-seven",
             "metadata": {},
             "source": [
-                "#### Stream: storing all the fields in memory"
+                "#### Storing all the fields in memory"
             ]
         },
         {
             "cell_type": "raw",
             "id": "1391881c-3484-405a-ab6f-4ee9d032bc35",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "When we use :ref:`batch_size <data-sources-fdb>`\\=0 all the fields are loaded into memory and the resulting object iswill behave like a FieldList:"
+                "We can load the whole stream into memory by using ``read_all=True`` in :ref:`from_source() <data-sources-fdb>`. The resulting object will be a FieldList."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "bizarre-basket",
             "metadata": {
@@ -330,93 +314,41 @@
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "ds = earthkit.data.from_source(\"fdb\", request, batch_size=0)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "concrete-filling",
-            "metadata": {},
-            "source": [
-                "Nothing is read at this moment:"
+                "ds = earthkit.data.from_source(\"fdb\", request, read_all=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "defensive-spell",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "stored fields count=0\n"
-                    ]
-                }
-            ],
-            "source": [
-                "print(f\"stored fields count={len(ds._reader._fields)}\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "blind-houston",
-            "metadata": {},
-            "source": [
-                "If we call any function on the fieldlist it reads the messages into memory"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 9,
             "id": "exciting-accused",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "6"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "len(ds)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "id": "efficient-submission",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "stored fields count=6\n"
-                    ]
-                }
-            ],
-            "source": [
-                "print(f\"stored fields count={len(ds._reader._fields)}\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 9,
             "id": "minus-horizon",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -452,120 +384,120 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>msl</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2d</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>msl</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2d</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
-                            "0   ecmf       msl     surface      0  20230607         0         0       an   \n",
-                            "1   ecmf        2t     surface      0  20230607         0         0       an   \n",
-                            "2   ecmf        2d     surface      0  20230607         0         0       an   \n",
-                            "3   ecmf       msl     surface      0  20230607      1200         0       an   \n",
-                            "4   ecmf        2t     surface      0  20230607      1200         0       an   \n",
-                            "5   ecmf        2d     surface      0  20230607      1200         0       an   \n",
+                            "0   ecmf       msl     surface      0  20240421         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20240421         0         0       an   \n",
+                            "2   ecmf        2d     surface      0  20240421         0         0       an   \n",
+                            "3   ecmf       msl     surface      0  20240421      1200         0       an   \n",
+                            "4   ecmf        2t     surface      0  20240421      1200         0       an   \n",
+                            "5   ecmf        2d     surface      0  20240421      1200         0       an   \n",
                             "\n",
                             "   number    gridType  \n",
                             "0       0  reduced_gg  \n",
                             "1       0  reduced_gg  \n",
                             "2       0  reduced_gg  \n",
                             "3       0  reduced_gg  \n",
                             "4       0  reduced_gg  \n",
                             "5       0  reduced_gg  "
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 10,
             "id": "tamil-tattoo",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -601,60 +533,60 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
-                            "0   ecmf        2t     surface      0  20230607         0         0       an   \n",
-                            "1   ecmf        2t     surface      0  20230607      1200         0       an   \n",
+                            "0   ecmf        2t     surface      0  20240421         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20240421      1200         0       an   \n",
                             "\n",
                             "   number    gridType  \n",
                             "0       0  reduced_gg  \n",
                             "1       0  reduced_gg  "
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.sel(param=\"2t\").ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 11,
             "id": "assumed-month",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
@@ -1020,17 +952,17 @@
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
                             "Dimensions:     (number: 1, time: 2, step: 1, surface: 1, values: 6599680)\n",
                             "Coordinates:\n",
                             "  * number      (number) int64 0\n",
-                            "  * time        (time) datetime64[ns] 2023-06-07 2023-06-07T12:00:00\n",
+                            "  * time        (time) datetime64[ns] 2024-04-21 2024-04-21T12:00:00\n",
                             "  * step        (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface     (surface) int64 0\n",
+                            "  * surface     (surface) float64 0.0\n",
                             "    latitude    (values) float64 ...\n",
                             "    longitude   (values) float64 ...\n",
                             "    valid_time  (time, step) datetime64[ns] ...\n",
                             "Dimensions without coordinates: values\n",
                             "Data variables:\n",
                             "    msl         (number, time, step, surface, values) float32 ...\n",
                             "    t2m         (number, time, step, surface, values) float32 ...\n",
@@ -1038,25 +970,25 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-06-08T11:49 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-dffa6f53-9be8-4f08-b96d-8904340a6bce' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-dffa6f53-9be8-4f08-b96d-8904340a6bce' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 2</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span>values</span>: 6599680</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-4aa2ffb9-169a-4df0-a8c7-7494a8bfde98' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4aa2ffb9-169a-4df0-a8c7-7494a8bfde98' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-1a9630df-a093-49b8-81fc-998188fc867f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1a9630df-a093-49b8-81fc-998188fc867f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-573b4489-a728-44fb-a034-64e092778b11' class='xr-var-data-in' type='checkbox'><label for='data-573b4489-a728-44fb-a034-64e092778b11' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2023-06-07 2023-06-07T12:00:00</div><input id='attrs-48835aef-88a4-4163-af88-998054832d94' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-48835aef-88a4-4163-af88-998054832d94' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e5ef026a-dde8-4b86-92fb-8c92dc2aa96d' class='xr-var-data-in' type='checkbox'><label for='data-e5ef026a-dde8-4b86-92fb-8c92dc2aa96d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2023-06-07T00:00:00.000000000&#x27;, &#x27;2023-06-07T12:00:00.000000000&#x27;],\n",
-                            "      dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-4c5c85af-316a-41ca-a195-cc7dafe614eb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-4c5c85af-316a-41ca-a195-cc7dafe614eb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f5e52f65-860b-4dfb-9461-e6165ec0e935' class='xr-var-data-in' type='checkbox'><label for='data-f5e52f65-860b-4dfb-9461-e6165ec0e935' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-53f01bfd-1aa2-4859-ab67-eb15ded06ae9' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-53f01bfd-1aa2-4859-ab67-eb15ded06ae9' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-93afaf42-acff-498e-ace0-3d2353ba22cc' class='xr-var-data-in' type='checkbox'><label for='data-93afaf42-acff-498e-ace0-3d2353ba22cc' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>latitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-58d3c743-4dbc-4bba-90cb-11de8f473751' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-58d3c743-4dbc-4bba-90cb-11de8f473751' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-64a97a47-7f81-4f8b-ad23-329f98f82e6f' class='xr-var-data-in' type='checkbox'><label for='data-64a97a47-7f81-4f8b-ad23-329f98f82e6f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>longitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-eef38fe3-2175-45d5-a024-198dbbd3c75f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-eef38fe3-2175-45d5-a024-198dbbd3c75f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-8339d5e0-48bf-4a0c-ac02-23c5cd78c511' class='xr-var-data-in' type='checkbox'><label for='data-8339d5e0-48bf-4a0c-ac02-23c5cd78c511' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-390e52c5-14ba-49c9-82d6-a054a9073006' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-390e52c5-14ba-49c9-82d6-a054a9073006' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e7fed87e-5f2b-4966-b395-25ccdc9c148c' class='xr-var-data-in' type='checkbox'><label for='data-e7fed87e-5f2b-4966-b395-25ccdc9c148c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[2 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-eadc2df8-fe5a-4fd8-bcc2-90ca3b6f069b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-eadc2df8-fe5a-4fd8-bcc2-90ca3b6f069b' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>msl</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-2b96ae7d-bcf0-4389-8e0e-8c7692f48f22' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-2b96ae7d-bcf0-4389-8e0e-8c7692f48f22' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1afea29b-c647-49b9-8df4-e63febac087d' class='xr-var-data-in' type='checkbox'><label for='data-1afea29b-c647-49b9-8df4-e63febac087d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>151</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>air_pressure_at_mean_sea_level</dd><dt><span>GRIB_cfVarName :</span></dt><dd>msl</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>msl</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>Pa</dd><dt><span>long_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>units :</span></dt><dd>Pa</dd><dt><span>standard_name :</span></dt><dd>air_pressure_at_mean_sea_level</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-8a90e69d-4b2b-4d07-90b6-8e058b2b054f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-8a90e69d-4b2b-4d07-90b6-8e058b2b054f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c8019ebc-d953-4385-88d0-4da64d674f83' class='xr-var-data-in' type='checkbox'><label for='data-c8019ebc-d953-4385-88d0-4da64d674f83' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>d2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-9594c5ef-de0f-4eaf-a673-1e659f0f881e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9594c5ef-de0f-4eaf-a673-1e659f0f881e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e1b705fe-931e-4b6b-8d5c-eefe712dbe9d' class='xr-var-data-in' type='checkbox'><label for='data-e1b705fe-931e-4b6b-8d5c-eefe712dbe9d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>168</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>d2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre dewpoint temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2d</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre dewpoint temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-38390609-7e8f-4a32-9f4c-05d9e9938f39' class='xr-section-summary-in' type='checkbox'  ><label for='section-38390609-7e8f-4a32-9f4c-05d9e9938f39' class='xr-section-summary' >Indexes: <span>(4)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-43f14fe3-5973-4c20-bdc0-ce88d73bfe0f' class='xr-index-data-in' type='checkbox'/><label for='index-43f14fe3-5973-4c20-bdc0-ce88d73bfe0f' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-332e6b04-16fa-4f1b-97d4-ad30202e90d9' class='xr-index-data-in' type='checkbox'/><label for='index-332e6b04-16fa-4f1b-97d4-ad30202e90d9' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2023-06-07 00:00:00&#x27;, &#x27;2023-06-07 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-3349020b-286d-445c-b847-d235c85e2753' class='xr-index-data-in' type='checkbox'/><label for='index-3349020b-286d-445c-b847-d235c85e2753' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e8cf740b-5f14-46cf-a62d-2f380bc34f3c' class='xr-index-data-in' type='checkbox'/><label for='index-e8cf740b-5f14-46cf-a62d-2f380bc34f3c' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;surface&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-64a95d2a-9d62-4c0a-a2b2-258e446ec68a' class='xr-section-summary-in' type='checkbox'  checked><label for='section-64a95d2a-9d62-4c0a-a2b2-258e446ec68a' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-06-08T11:49 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "    history:                 2024-04-22T11:01 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-b66993a0-0360-4f6e-b780-0ec6ed5bac3f' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-b66993a0-0360-4f6e-b780-0ec6ed5bac3f' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 2</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span>values</span>: 6599680</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-92ba425c-e1ba-417c-aaba-a5d56d3c835b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-92ba425c-e1ba-417c-aaba-a5d56d3c835b' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-1665b451-9232-4b63-b87e-2fecd6750121' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1665b451-9232-4b63-b87e-2fecd6750121' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-b23add1c-a672-46bf-a457-e26166adc43d' class='xr-var-data-in' type='checkbox'><label for='data-b23add1c-a672-46bf-a457-e26166adc43d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2024-04-21 2024-04-21T12:00:00</div><input id='attrs-cc5172c9-9654-461c-a349-5147c2d3408f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-cc5172c9-9654-461c-a349-5147c2d3408f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-28227e5d-f198-4d79-aa98-f5ea3c543d82' class='xr-var-data-in' type='checkbox'><label for='data-28227e5d-f198-4d79-aa98-f5ea3c543d82' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2024-04-21T00:00:00.000000000&#x27;, &#x27;2024-04-21T12:00:00.000000000&#x27;],\n",
+                            "      dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-a8b95478-6f8f-4b71-a767-4bc9e4c96a3f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a8b95478-6f8f-4b71-a767-4bc9e4c96a3f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-523274e6-e33a-4867-9272-362e69bb1e10' class='xr-var-data-in' type='checkbox'><label for='data-523274e6-e33a-4867-9272-362e69bb1e10' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-f1de763a-800e-4790-bf39-def49eb70bf7' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-f1de763a-800e-4790-bf39-def49eb70bf7' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c1418d54-5977-4fe3-8036-4c501cb0005e' class='xr-var-data-in' type='checkbox'><label for='data-c1418d54-5977-4fe3-8036-4c501cb0005e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>latitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-c8558bb5-22cf-4869-90c6-efa6a7631539' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-c8558bb5-22cf-4869-90c6-efa6a7631539' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-a62f0310-5666-41e5-8914-0fd0f5b469a1' class='xr-var-data-in' type='checkbox'><label for='data-a62f0310-5666-41e5-8914-0fd0f5b469a1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>longitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-037b35bb-ef15-4819-8fc1-b035faf76790' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-037b35bb-ef15-4819-8fc1-b035faf76790' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-b345dbc7-095c-475c-befb-0d14054a0a04' class='xr-var-data-in' type='checkbox'><label for='data-b345dbc7-095c-475c-befb-0d14054a0a04' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>[6599680 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-30f382b3-7be7-46cb-979e-0ecb4feddaeb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-30f382b3-7be7-46cb-979e-0ecb4feddaeb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e01b7e30-dc25-4bed-98d3-2d0390812358' class='xr-var-data-in' type='checkbox'><label for='data-e01b7e30-dc25-4bed-98d3-2d0390812358' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[2 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-4af160b6-521e-46fe-b24d-1adc392ac8bf' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4af160b6-521e-46fe-b24d-1adc392ac8bf' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>msl</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-e5261af4-896d-444d-962f-7c560df82dc8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e5261af4-896d-444d-962f-7c560df82dc8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-82974a5a-38bc-440e-9323-356e87878d2c' class='xr-var-data-in' type='checkbox'><label for='data-82974a5a-38bc-440e-9323-356e87878d2c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>151</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>air_pressure_at_mean_sea_level</dd><dt><span>GRIB_cfVarName :</span></dt><dd>msl</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>msl</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>Pa</dd><dt><span>long_name :</span></dt><dd>Mean sea level pressure</dd><dt><span>units :</span></dt><dd>Pa</dd><dt><span>standard_name :</span></dt><dd>air_pressure_at_mean_sea_level</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-7cd770c5-d0f6-485d-93f2-953a01f02065' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-7cd770c5-d0f6-485d-93f2-953a01f02065' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-594df006-9d85-47b1-840e-51ede18a5a45' class='xr-var-data-in' type='checkbox'><label for='data-594df006-9d85-47b1-840e-51ede18a5a45' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>d2m</span></div><div class='xr-var-dims'>(number, time, step, surface, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-1eedf1fd-a1b6-4d62-9870-2c7debd1d2ca' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1eedf1fd-a1b6-4d62-9870-2c7debd1d2ca' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-19912a4e-c579-4a5d-90cf-66ae7ea1aaf4' class='xr-var-data-in' type='checkbox'><label for='data-19912a4e-c579-4a5d-90cf-66ae7ea1aaf4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>168</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6599680</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_N :</span></dt><dd>1280</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>d2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Gaussian Latitude/Longitude Grid</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre dewpoint temperature</dd><dt><span>GRIB_pl :</span></dt><dd>[20 24 28 ... 28 24 20]</dd><dt><span>GRIB_shortName :</span></dt><dd>2d</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre dewpoint temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[13199360 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-23ac3cd2-47d9-4423-9748-313ad153b133' class='xr-section-summary-in' type='checkbox'  ><label for='section-23ac3cd2-47d9-4423-9748-313ad153b133' class='xr-section-summary' >Indexes: <span>(4)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-60aaff23-1083-4bde-9ec0-cff6e8351c2f' class='xr-index-data-in' type='checkbox'/><label for='index-60aaff23-1083-4bde-9ec0-cff6e8351c2f' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-414e097a-3b15-4df9-939d-d0d8eea9d389' class='xr-index-data-in' type='checkbox'/><label for='index-414e097a-3b15-4df9-939d-d0d8eea9d389' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2024-04-21 00:00:00&#x27;, &#x27;2024-04-21 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0dc4a42c-c595-4fe5-9a15-d6bf0dd35af0' class='xr-index-data-in' type='checkbox'/><label for='index-0dc4a42c-c595-4fe5-9a15-d6bf0dd35af0' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9e984db4-2b6f-4c11-b968-ae18e8df440d' class='xr-index-data-in' type='checkbox'/><label for='index-9e984db4-2b6f-4c11-b968-ae18e8df440d' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-ef832144-3fdc-4d09-b52a-ca99d14633d1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-ef832144-3fdc-4d09-b52a-ca99d14633d1' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2024-04-22T11:01 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.33.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:     (number: 1, time: 2, step: 1, surface: 1, values: 6599680)\n",
                             "Coordinates:\n",
                             "  * number      (number) int64 0\n",
-                            "  * time        (time) datetime64[ns] 2023-06-07 2023-06-07T12:00:00\n",
+                            "  * time        (time) datetime64[ns] 2024-04-21 2024-04-21T12:00:00\n",
                             "  * step        (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface     (surface) int64 0\n",
+                            "  * surface     (surface) float64 0.0\n",
                             "    latitude    (values) float64 ...\n",
                             "    longitude   (values) float64 ...\n",
                             "    valid_time  (time, step) datetime64[ns] ...\n",
                             "Dimensions without coordinates: values\n",
                             "Data variables:\n",
                             "    msl         (number, time, step, surface, values) float32 ...\n",
                             "    t2m         (number, time, step, surface, values) float32 ...\n",
@@ -1064,18 +996,18 @@
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-06-08T11:49 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2024-04-22T11:01 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.to_xarray()"
             ]
@@ -1101,15 +1033,15 @@
             },
             "source": [
                 "We can retrieve data from FDB into a file, which is located in the :ref:`cache <caching>`: "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 12,
             "id": "passing-georgia",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
@@ -1117,15 +1049,15 @@
             "outputs": [],
             "source": [
                 "ds = earthkit.data.from_source(\"fdb\", request, stream=False)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 13,
             "id": "foster-profile",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1161,109 +1093,109 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>msl</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2d</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>msl</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2t</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>2d</td>\n",
                             "      <td>surface</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>20230607</td>\n",
+                            "      <td>20240421</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>reduced_gg</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName typeOfLevel  level  dataDate  dataTime stepRange dataType  \\\n",
-                            "0   ecmf       msl     surface      0  20230607         0         0       an   \n",
-                            "1   ecmf        2t     surface      0  20230607         0         0       an   \n",
-                            "2   ecmf        2d     surface      0  20230607         0         0       an   \n",
-                            "3   ecmf       msl     surface      0  20230607      1200         0       an   \n",
-                            "4   ecmf        2t     surface      0  20230607      1200         0       an   \n",
-                            "5   ecmf        2d     surface      0  20230607      1200         0       an   \n",
+                            "0   ecmf       msl     surface      0  20240421         0         0       an   \n",
+                            "1   ecmf        2t     surface      0  20240421         0         0       an   \n",
+                            "2   ecmf        2d     surface      0  20240421         0         0       an   \n",
+                            "3   ecmf       msl     surface      0  20240421      1200         0       an   \n",
+                            "4   ecmf        2t     surface      0  20240421      1200         0       an   \n",
+                            "5   ecmf        2d     surface      0  20240421      1200         0       an   \n",
                             "\n",
                             "   number    gridType  \n",
                             "0       0  reduced_gg  \n",
                             "1       0  reduced_gg  \n",
                             "2       0  reduced_gg  \n",
                             "3       0  reduced_gg  \n",
                             "4       0  reduced_gg  \n",
                             "5       0  reduced_gg  "
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds.ls()"
             ]
@@ -1296,27 +1228,27 @@
             },
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "dev",
+            "display_name": "pyfdb",
             "language": "python",
-            "name": "dev"
+            "name": "pyfdb"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.8.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `earthkit_data-0.7.0/docs/examples/file_parts.ipynb` & `earthkit_data-0.8.1/docs/examples/file_parts.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/files.ipynb` & `earthkit_data-0.8.1/docs/examples/files.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/from_object.ipynb` & `earthkit_data-0.8.1/docs/examples/from_object.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/geojson_geopandas.ipynb` & `earthkit_data-0.8.1/docs/examples/geojson_geopandas.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_array_backends.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_array_backends.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_fdb_write.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_fdb_write.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_indexing.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_indexing.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_lat_lon_value.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_lat_lon_value.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_metadata.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_metadata.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_missing.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_missing.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_nearest_gridpoint.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_nearest_gridpoint.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_overview.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_overview.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_selection.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_selection.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_time_series.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_time_series.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/grib_to_netcdf.ipynb` & `earthkit_data-0.8.1/docs/examples/grib_to_netcdf.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/index.rst` & `earthkit_data-0.8.1/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/list_of_dict.ipynb` & `earthkit_data-0.8.1/docs/examples/list_of_dict.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/mars.ipynb` & `earthkit_data-0.8.1/docs/examples/mars.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/metadata.ipynb` & `earthkit_data-0.8.1/docs/examples/metadata.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/missing.grib` & `earthkit_data-0.8.1/docs/examples/missing.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/multi_files.ipynb` & `earthkit_data-0.8.1/docs/examples/multi_files.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/netcdf.ipynb` & `earthkit_data-0.8.1/docs/examples/netcdf.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/netcdf_fieldlist.ipynb` & `earthkit_data-0.8.1/docs/examples/netcdf_fieldlist.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/netcdf_opendap.ipynb` & `earthkit_data-0.8.1/docs/examples/netcdf_opendap.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/numpy_fieldlist.ipynb` & `earthkit_data-0.8.1/docs/examples/numpy_fieldlist.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/odb.ipynb` & `earthkit_data-0.8.1/docs/examples/odb.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/pandas.ipynb` & `earthkit_data-0.8.1/docs/examples/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/polytope.ipynb` & `earthkit_data-0.8.1/docs/examples/polytope.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/projection.ipynb` & `earthkit_data-0.8.1/docs/examples/projection.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/settings.ipynb` & `earthkit_data-0.8.1/docs/examples/settings.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/shapefile.ipynb` & `earthkit_data-0.8.1/docs/examples/shapefile.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982954545454545%*

 * *Differences: {"'cells'": "{1: {'metadata': {'vscode': OrderedDict([('languageId', 'raw')])}, 'source': ['The "*

 * *            'code below reads shapefile data as a :ref:`data-sources-file` source using '*

 * *            ':func:`from_source()`. Internally the data is represented as a geopandas dataframe. '*

 * *            "To make this example work geopandas **needs** to be installed.']}}"}*

```diff
@@ -13,18 +13,21 @@
             "id": "42cc4d64-7eba-40d0-ad71-423bb7b70793",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
-                "tags": []
+                "tags": [],
+                "vscode": {
+                    "languageId": "raw"
+                }
             },
             "source": [
-                "The code below reads shapefile data as a :ref:`source-data-file` source using :func:`from_source()`. Internally the data is represented as a geopandas dataframe. To make this example work geopandas **needs** to be installed."
+                "The code below reads shapefile data as a :ref:`data-sources-file` source using :func:`from_source()`. Internally the data is represented as a geopandas dataframe. To make this example work geopandas **needs** to be installed."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "4825665a-8fc1-4c24-b0fb-3c485bd462c5",
             "metadata": {
```

### Comparing `earthkit_data-0.7.0/docs/examples/synop_10.bufr` & `earthkit_data-0.8.1/docs/examples/synop_10.bufr`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/tar_files.ipynb` & `earthkit_data-0.8.1/docs/examples/tar_files.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/temp_10.bufr` & `earthkit_data-0.8.1/docs/examples/temp_10.bufr`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/test.grib` & `earthkit_data-0.8.1/docs/examples/test.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/test.nc` & `earthkit_data-0.8.1/docs/examples/test.nc`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/test.odb` & `earthkit_data-0.8.1/docs/examples/test.odb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/test4.grib` & `earthkit_data-0.8.1/docs/examples/test4.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/test6.grib` & `earthkit_data-0.8.1/docs/examples/test6.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/time_series.grib` & `earthkit_data-0.8.1/docs/examples/time_series.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/tuv_pl.grib` & `earthkit_data-0.8.1/docs/examples/tuv_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/tuv_pl.nc` & `earthkit_data-0.8.1/docs/examples/tuv_pl.nc`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/url.ipynb` & `earthkit_data-0.8.1/docs/examples/url.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/url_parts.ipynb` & `earthkit_data-0.8.1/docs/examples/url_parts.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/examples/wekeo.ipynb` & `earthkit_data-0.8.1/docs/examples/wekeo.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/guide/caching.rst` & `earthkit_data-0.8.1/docs/guide/caching.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/guide/data.rst` & `earthkit_data-0.8.1/docs/guide/data.rst`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 When we call :func:`from_source` it will return a **data object**. The actual object type depends on the source parameters and the :ref:`data format <data-format>`, but is supposed to implement a **common** set of methods/operators, some of which will only be available for certain :ref:`data types <data-format>`.
 
 The list of common methods/operators:
 
   - :ref:`conversion`
   - :ref:`concat`
   - :ref:`iter`
+  - :ref:`batched`
+  - :ref:`group_by`
   - :ref:`slice`
   - :ref:`sel`
   - :ref:`order_by`
   - :ref:`data_values`
   - :ref:`metadata`
   - :ref:`inspection`
 
@@ -73,14 +75,57 @@
     GribField(t,1000,20180801,1200,0,0)
     GribField(u,1000,20180801,1200,0,0)
     GribField(v,1000,20180801,1200,0,0)
     GribField(t,850,20180801,1200,0,0)
     GribField(u,850,20180801,1200,0,0)
     GribField(v,850,20180801,1200,0,0)
 
+.. _batched:
+
+Iteration with ``.batched()``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+When an earthkit-data data `source` or dataset provides a :class:`~data.core.fieldlist.FieldList` or message list, we can iterate through it in batches of fixed size using :meth:`~data.core.fieldlist.FieldList.batched`. This method also works for :ref:`streams <streams>`.
+
+In the the following example we read a GRIB file from disk and iterate through it in batches of 2. Each iteration step yields a :class:`~data.core.fieldlist.FieldList` of 2 fields.
+
+.. code-block:: python
+
+    >>> import earthkit.data
+    >>> ds = earthkit.data.from_source("file", "docs/examples/test6.grib")
+
+    >>> for f in ds.batched(2):
+    ...     print(f"len={len(f)} {f.metadata(('param', 'level'))}")
+    ...
+    len=2 [('t', 1000), ('u', 1000)]
+    len=2 [('v', 1000), ('t', 850)]
+    len=2 [('u', 850), ('v', 850)]
+
+
+.. _group_by:
+
+Iteration with ``.group_by()``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+When an earthkit-data data `source` or dataset provides a :class:`~data.core.fieldlist.FieldList` or message list, we can iterate through it in groups defined by metadata keys using :meth:`~data.core.fieldlist.FieldList.group_by`. This method also works for :ref:`streams <streams>`.
+
+In the the following example we read a GRIB file from disk and iterate through it in groups defined by the "level" metadata key. Each iteration step yields a :class:`~data.core.fieldlist.FieldList` containing fields with the same "level" value.
+
+.. code-block:: python
+
+    >>> import earthkit.data
+    >>> ds = earthkit.data.from_source("file", "docs/examples/test6.grib")
+
+    >>> for f in ds.group_by("level"):
+    ...     print(f"len={len(f)} {f.metadata(('param', 'level'))}")
+    ...
+    len=3 [('t', 1000), ('u', 1000), ('v', 1000)]
+    len=3 [('t', 850), ('u', 850), ('v', 850)]
+
+
 .. _slice:
 
 Selection with ``[...]``
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 When an earthkit-data data `source` or dataset provides a :class:`~data.core.fieldlist.FieldList` or message list, a subset of it can be created using the standard python list interface relying on brackets and slices. Slicing also works by providing a list or ndarray of indices.
```

### Comparing `earthkit_data-0.7.0/docs/guide/data_format/bufr.rst` & `earthkit_data-0.8.1/docs/guide/data_format/bufr.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/guide/data_format/grib.rst` & `earthkit_data-0.8.1/docs/guide/data_format/grib.rst`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,18 @@
      - API
    * - :ref:`conversion`
      - :meth:`~data.readers.grib.index.GribFieldList.to_xarray`
    * - :ref:`concat`
      -
    * - :ref:`iter`
      -
+   * - :ref:`batched`
+     - :meth:`~data.readers.grib.index.GribFieldList.batched`
+   * - :ref:`group_by`
+     - :meth:`~data.readers.grib.index.GribFieldList.group_by`
    * - :ref:`slice`
      -
    * - :ref:`sel`
      - :meth:`~data.readers.grib.index.GribFieldList.sel`
    * - :ref:`order_by`
      - :meth:`~data.readers.grib.index.GribFieldList.order_by`
    * - :ref:`data_values`
```

### Comparing `earthkit_data-0.7.0/docs/guide/include/settings-set.py` & `earthkit_data-0.8.1/docs/guide/include/settings-set.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/guide/misc/parts.rst` & `earthkit_data-0.8.1/docs/guide/misc/parts.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/guide/misc/split_on.rst` & `earthkit_data-0.8.1/docs/guide/misc/split_on.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/guide/settings.rst` & `earthkit_data-0.8.1/docs/guide/settings.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/guide/sources.rst` & `earthkit_data-0.8.1/docs/guide/sources.rst`

 * *Files 6% similar despite different names*

```diff
@@ -177,27 +177,26 @@
 
 
 .. _data-sources-url:
 
 url
 ---
 
-.. py:function:: from_source("url", url, unpack=True, parts=None, stream=False, batch_size=1, group_by=None)
+.. py:function:: from_source("url", url, unpack=True, parts=None, stream=False, read_all=False)
   :noindex:
 
   The ``url`` source will download the data from the address specified and store it in the :ref:`cache <caching>`. The supported data formats are the same as for the :ref:`file <data-sources-file>` data source above.
 
   :param url: the URL(s) to download. Each URL can contain the :ref:`parts <parts>` defining the byte ranges to read.
   :type url: str
   :param bool unpack: for archive formats such as ``.zip``, ``.tar``, ``.tar.gz``, etc, *earthkit-data* will attempt to open it and extract any usable file. To keep the downloaded file as is use ``unpack=False``
   :param parts: the :ref:`parts <parts>` to read from the resource(s) specified by ``url``. Cannot be used when ``url`` already defines the :ref:`parts <parts>`.
   :type parts: pair, list or tuple of pairs, None
-  :param bool stream: when it is ``True`` the data is read as a stream. Otherwise the data is retrieved into a file and stored in the :ref:`cache <caching>`. This option only works for GRIB data. No archive formats supported (``unpack`` is ignored). ``stream`` only works for ``http`` and ``https`` URLs.
-  :param int batch_size: used when ``stream=True`` and ``group_by`` is unset. It defines how many GRIB messages are consumed from the stream and kept in memory at a time. For details see :ref:`stream source <data-sources-stream>`.
-  :param group_by: used when ``stream=True`` and can specify one or more metadata keys to control how GRIB messages are read from the stream. For details see :ref:`stream source <data-sources-stream>`.
+  :param bool stream: when it is ``True`` the data is read as a :ref:`stream <streams>`. Otherwise the data is retrieved into a file and stored in the :ref:`cache <caching>`. This option only works for GRIB data. No archive formats supported (``unpack`` is ignored). ``stream`` only works for ``http`` and ``https`` URLs. See details about streams :ref:`here <streams>`.
+  :param bool read_all: when it is ``True`` all the data is read straight to memory from a :ref:`stream <streams>`. Used when ``stream=True``. *New in version 0.8.0*
   :type group_by: str, list of str
   :param dict **kwargs: other keyword arguments specifying the request
 
   .. code-block:: python
 
       >>> import earthkit.data
       >>> ds = earthkit.data.from_source(
@@ -223,14 +222,15 @@
         centre shortName    typeOfLevel  level  dataDate  dataTime stepRange dataType  number    gridType
       0   ecmf         t  isobaricInhPa    500  20070101      1200         0       an       0  regular_ll
       1   ecmf         t  isobaricInhPa    850  20070101      1200         0       an       0  regular_ll
 
   Further examples:
 
     - :ref:`/examples/url.ipynb`
+    - :ref:`/examples/url_parts.ipynb`
     - :ref:`/examples/url_stream.ipynb`
 
 
 .. _data-sources-url-pattern:
 
 
 url-pattern
@@ -298,27 +298,24 @@
 
 
 .. _data-sources-stream:
 
 stream
 --------------
 
-.. py:function:: from_source("stream", stream, batch_size=1, group_by=None)
+.. py:function:: from_source("stream", stream, read_all=False)
   :noindex:
 
-  The ``stream`` will read data from a stream, which can be an FDB stream, a standard Python IO stream or any object implementing the necessary stream methods. At the moment it only works for :ref:`grib` and CoverageJson data.
-
-  :param stream: the stream
-  :param int batch_size: used when ``group_by`` is unset. It defines how many GRIB messages are consumed from the stream and kept in memory at a time. ``batch_size=0`` means all the messages will be loaded and stored in memory.  When ``batch_size`` is not zero ``from_source`` gives us a stream iterator object. During the iteration temporary objects are created for each message then get deleted when going out of scope. Used when ``group_by`` is unset.
-  :param group_by: specify one or more metadata keys to control how GRIB messages are read from the stream. When it is set ``from_source`` gives us a stream iterator object. Each iteration step results in a Fieldlist object, which is built by consuming GRIB messages from the stream until the values of the ``group_by`` metadata keys change. The generated Fieldlist keeps GRIB messages in memory then gets deleted when going out of scope. When ``group_by`` is set ``batch_size`` is ignored.
-  :type group_by: str, list of str
-  :param dict **kwargs: other keyword arguments specifying the request
+  The ``stream`` source will read data from a stream (or streams), which can be an FDB stream, a standard Python IO stream or any object implementing the necessary stream methods. At the moment it only works for :ref:`grib` and CoverageJson data. For more details see :ref:`here <streams>`.
 
+  :param stream: the stream(s)
+  :type stream: stream, list, tuple
+  :param bool read_all: when it is ``True`` all the data is read into memory from a stream. Used when ``stream=True``. *New in version 0.8.0*
 
-  In the examples below, for simplicity, we create a file stream from a :ref:`grib` file and read it as a "stream". By default (``batch_size=1``) we will consume one message at a time:
+  In the examples below, for simplicity, we create a file stream from a :ref:`grib` file. By default :ref:`from_source() <data-sources-stream>` returns an object that can only be used as an iterator.
 
   .. code-block:: python
 
       >>> import earthkit.data
       >>> stream = open("docs/examples/test4.grib", "rb")
       >>> ds = earthkit.data.from_source("stream", stream)
 
@@ -327,62 +324,52 @@
       ...     print(f)
       ...
       GribField(t,500,20070101,1200,0,0)
       GribField(z,500,20070101,1200,0,0)
       GribField(t,850,20070101,1200,0,0)
       GribField(z,850,20070101,1200,0,0)
 
-
-  We can use ``group_by`` to read fields with a matching level. ``ds`` is still just an iterator, but ``f`` is now a :obj:`FieldList <data.readers.grib.index.FieldList>`:
+  We can also iterate through the stream in batches of fixed size using ``batched()``:
 
     .. code-block:: python
 
       >>> import earthkit.data
       >>> stream = open("docs/examples/test4.grib", "rb")
-      >>> ds = earthkit.data.from_source("stream", stream, group_by="level")
-      >>> for f in ds:
-      ...     print(len(f))
-      ...     for g in f:
-      ...         print(f" {g}")
+      >>> ds = earthkit.data.from_source("stream", stream, batch_size=2)
+
+       # f is a FieldList
+      >>> for f in ds.batched(2):
+      ...     print(f"len={len(f)} {f.metadata(('param', 'level'))}")
       ...
-      2
-       GribField(t,500,20070101,1200,0,0)
-       GribField(z,500,20070101,1200,0,0)
-      2
-       GribField(t,850,20070101,1200,0,0)
-       GribField(z,850,20070101,1200,0,0)
+      len=2 [('t', 500), ('z', 500)]
+      len=2 [('t', 850), ('z', 850)]
 
-  We can use ``batch_size=2`` to read 2 messages at a time:
+
+  When using ``group_by()`` we can iterate through the stream in groups defined by metadata keys. In this case each iteration step yields a :obj:`FieldList <data.readers.grib.index.FieldList>`.
 
     .. code-block:: python
 
       >>> import earthkit.data
       >>> stream = open("docs/examples/test4.grib", "rb")
-      >>> ds = earthkit.data.from_source("stream", stream, batch_size=2)
+      >>> ds = earthkit.data.from_source("stream", stream)
 
-      # f is a FieldList containing 2 GribFields
-      >>> for f in ds:
-      ...     print(len(f))
-      ...     for g in f:
-      ...         print(f" {g}")
+      # f is a FieldList
+      >>> for f in ds.group_by("level"):
+      ...     print(f"len={len(f)} {f.metadata(('param', 'level'))}")
       ...
-      2
-       GribField(t,500,20070101,1200,0,0)
-       GribField(z,500,20070101,1200,0,0)
-      2
-       GribField(t,850,20070101,1200,0,0)
-       GribField(z,850,20070101,1200,0,0)
+      len=2 [('t', 500), ('z', 500)]
+      len=2 [('t', 850), ('z', 850)]
 
-  With ``batch_size=0`` the whole stream will be consumed resulting in a FieldList object storing all the messages in memory. **Use this option carefully!**
+  We can consume the whole stream and load all the data into memory by using ``read_all=True`` in :ref:`from_source() <data-sources-stream>`. **Use this option carefully!**
 
     .. code-block:: python
 
       >>> import earthkit.data
       >>> stream = open("docs/examples/test4.grib", "rb")
-      >>> ds = earthkit.data.from_source("stream", stream, batch_size=0)
+      >>> ds = earthkit.data.from_source("stream", stream, read_all=True)
 
       # ds is empty at this point, but calling any method on it will
       # consume the whole stream
       >>> len(ds)
       4
 
       # now ds stores all the messages in memory
@@ -581,89 +568,91 @@
 
 
 .. _data-sources-fdb:
 
 fdb
 ---
 
-.. py:function:: from_source("fdb", *args, stream=True,  batch_size=1, group_by=None, **kwargs)
+.. py:function:: from_source("fdb", *args, stream=True, read_all=False, **kwargs)
   :noindex:
 
   The ``fdb`` source accesses the `FDB (Fields DataBase) <https://fields-database.readthedocs.io/en/latest/>`_, which is a domain-specific object store developed at ECMWF for storing, indexing and retrieving GRIB data. earthkit-data uses the `pyfdb <https://pyfdb.readthedocs.io/en/latest>`_ package to retrieve data from FDB.
 
   :param tuple *args: positional arguments specifying the request as a dict
-  :param bool stream: when it is ``True`` the data is read as a stream. Otherwise the data is retrieved into a file and stored in the :ref:`cache <caching>`. Stream-based access only works for :ref:`grib` data.
-  :param int batch_size: used when ``stream=True`` and ``group_by`` is unset. It defines how many GRIB messages are consumed from the stream and kept in memory at a time. ``batch_size=0`` means all the data is read straight to memory. For details see :ref:`stream source <data-sources-stream>`.
-  :param group_by: used when ``stream=True`` and can specify one or more metadata keys to control how GRIB messages are read from the stream. For details see :ref:`stream source <data-sources-stream>`.
-  :type group_by: str, list of str
+  :param bool stream: when it is ``True`` the data is read as a :ref:`stream <streams>`. Otherwise it is retrieved into a file and stored in the :ref:`cache <caching>`. Stream-based access only works for :ref:`grib` and CoverageJson data. See details about streams :ref:`here <streams>`.
+  :param bool read_all: when it is ``True`` all the data is read into memory from a :ref:`stream <streams>`. Used when ``stream=True``. *New in version 0.8.0*
   :param dict **kwargs: other keyword arguments specifying the request
 
   The following example retrieves analysis :ref:`grib` data for 3 surface parameters as stream.
   By default we will consume one message at a time and ``ds`` can only be used as an iterator:
 
   .. code-block:: python
 
       >>> import earthkit.data
       >>> request = {
       ...     "class": "od",
       ...     "expver": "0001",
       ...     "stream": "oper",
-      ...     "date": "20230607",
+      ...     "date": "20240421",
       ...     "time": [0, 12],
       ...     "domain": "g",
       ...     "type": "an",
       ...     "levtype": "sfc",
       ...     "step": 0,
       ...     "param": [151, 167, 168],
       ... }
       >>>
       >>> ds = earthkit.data.from_source("fdb", request)
       >>> for f in ds:
       ...     print(f)
       ...
-      GribField(msl,None,20230607,0,0,0)
-      GribField(2t,None,20230607,0,0,0)
-      GribField(msl,None,20230607,1200,0,0)
-      GribField(2t,None,20230607,1200,0,0)
+      GribField(msl,None,20240421,0,0,0)
+      GribField(2t,None,20240421,0,0,0)
+      GribField(2d,None,20240421,0,0,0)
+      GribField(msl,None,20240421,1200,0,0)
+      GribField(2t,None,20240421,1200,0,0)
+      GribField(2d,None,20240421,1200,0,0)
 
-  We can use ``group_by`` to read fields with a matching time. ``ds`` is still just an iterator, but ``f`` is now a :obj:`FieldList <data.readers.grib.index.FieldList>`:
+  We can also iterate through the stream in batches of fixed size using ``batched``:
 
-      >>> ds = earthkit.data.from_source("fdb", request, group_by="time")
-      >>> for f in ds:
-      ...     print(f)
-      ...     for g in f:
-      ...         print(f" {g}")
+  .. code-block:: python
+
+      >>> ds = earthkit.data.from_source("fdb", request)
+      >>> for f in ds.batched(2):
+      ...     print(f"len={len(f)} {f.metadata(('param', 'level'))}")
       ...
-      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
-       GribField(msl,None,20230607,0,0,0)
-       GribField(2t,None,20230607,0,0,0)
-       GribField(2d,None,20230607,0,0,0)
-      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
-       GribField(msl,None,20230607,1200,0,0)
-       GribField(2t,None,20230607,1200,0,0)
-       GribField(2d,None,20230607,1200,0,0)
+      len=2 [('msl', 0), ('2t', 0)]
+      len=2 [('2d', 0), ('msl', 0)]
+      len=2 [('2t', 0), ('2d', 0)]
 
-  We can use ``batch_size=2`` to read 2 fields at a time. ``ds`` is still just an iterator, but ``f`` is now a :obj:`FieldList <data.readers.grib.index.FieldList>` containing 2 fields:
 
-      >>> ds = earthkit.data.from_source("fdb", request, batch_size=2)
-      >>> for f in ds:
-      ...     print(f)
-      ...     for g in f:
-      ...         print(f" {g}")
+  When using ``group_by()`` we can iterate through the stream in groups defined by metadata keys. In this case each iteration step yields a :obj:`FieldList <data.readers.grib.index.FieldList>`.
+
+  .. code-block:: python
+
+      >>> ds = earthkit.data.from_source("fdb", request)
+      >>> for f in ds.group_by("time"):
+      ...     print(f"len={len(f)} {f.metadata(('param', 'level'))}")
       ...
-      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
-        GribField(msl,None,20230607,0,0,0)
-        GribField(2t,None,20230607,0,0,0)
-      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
-        GribField(2d,None,20230607,0,0,0)
-        GribField(msl,None,20230607,1200,0,0)
-      <class 'earthkit.data.readers.grib.memory.FieldListInMemory'>
-        GribField(2t,None,20230607,1200,0,0)
-        GribField(2d,None,20230607,1200,0,0)
+      len=3 [('msl', 0), ('2t', 0), ('2d', 0)]
+      len=3 [('msl', 0), ('2t', 0), ('2d', 0)]
 
+  We can consume the whole stream and load all the data into memory by using ``read_all=True`` in :ref:`from_source() <data-sources-stream>`. **Use this option carefully!**
+
+  .. code-block:: python
+
+      >>> import earthkit.data
+      >>> ds = earthkit.data.from_source("fdb", request, read_all=True)
+
+      # ds is empty at this point, but calling any method on it will
+      # consume the whole stream
+      >>> len(ds)
+      3
+
+      # now ds stores all the messages in memory
 
   Further examples:
 
       - :ref:`/examples/fdb.ipynb`
       - :ref:`/examples/grib_fdb_write.ipynb`
 
 
@@ -733,28 +722,26 @@
 
 
 .. _data-sources-polytope:
 
 polytope
 --------
 
-.. py:function:: from_source("polytope", collection, *args, address=None, user_email=None, user_key=None, stream=True, batch_size=1, group_by=None, **kwargs)
+.. py:function:: from_source("polytope", collection, *args, address=None, user_email=None, user_key=None, stream=True, read_all=False, **kwargs)
   :noindex:
 
   The ``polytope`` source accesses the `Polytope web services <https://polytope-client.readthedocs.io/en/latest/>`_ , using the polytope-client_ package.
 
   :param str collection: the name of the polytope collection
   :param tuple *args: specify the request as a dict
   :param str address: specify the address of the polytope service
-  :param str user_email: specify the user email credential. Must be used together with ``user_key``. This is an alternative to using the ``POLYTOPE_USER_EMAIL`` environment variable. *Added in version 0.7.0*
-  :param str user_key: specify the user key credential. Must be used together with ``user_email``. This is an alternative to using the ``POLYTOPE_USER_KEY`` environment variable. *Added in version 0.7.0*
-  :param bool stream: when it is ``True`` the data is read as a stream. Otherwise the data is retrieved into a file and stored in the :ref:`cache <caching>`. Stream-based access only works for :ref:`grib` and CoverageJson data.
-  :param int batch_size: used when ``stream=True`` and ``group_by`` is unset. It defines how many GRIB messages are consumed from the stream and kept in memory at a time. ``batch_size=0`` means all the data is read straight to memory. For details see :ref:`stream source <data-sources-stream>`.
-  :param group_by: used when ``stream=True`` and can specify one or more metadata keys to control how GRIB messages are read from the stream. For details see :ref:`stream source <data-sources-stream>`.
-  :type group_by: str, list of str
+  :param str user_email: specify the user email credential. Must be used together with ``user_key``. This is an alternative to using the ``POLYTOPE_USER_EMAIL`` environment variable. *New in version 0.7.0*
+  :param str user_key: specify the user key credential. Must be used together with ``user_email``. This is an alternative to using the ``POLYTOPE_USER_KEY`` environment variable. *New in version 0.7.0*
+  :param bool stream: when ``True`` the data is read as a :ref:`stream <streams>`. Otherwise it is retrieved into a file and stored in the :ref:`cache <caching>`. Stream-based access only works for :ref:`grib` and CoverageJson data. See details about streams :ref:`here <streams>`.
+  :param bool read_all: when ``True`` all the data is read into memory from a :ref:`stream <streams>`. Used when ``stream=True``. *New in version 0.8.0*
   :param dict **kwargs: other keyword arguments, these can include options passed to the polytope-client_
 
 
   The following example retrieves GRIB data from the "ecmwf-mars" polytope collection:
 
   .. code-block:: python
 
@@ -782,15 +769,14 @@
   To access data from polytope, you will need to register and retrieve an access token.
 
   Further examples:
 
       - :ref:`/examples/polytope.ipynb`
 
 
-
 .. _data-sources-wekeo:
 
 wekeo
 -----
 
 .. py:function:: from_source("wekeo", dataset, *args, prompt=True, **kwargs)
   :noindex:
```

### Comparing `earthkit_data-0.7.0/docs/howtos.rst` & `earthkit_data-0.8.1/docs/howtos.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/index.rst` & `earthkit_data-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/install.rst` & `earthkit_data-0.8.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/licence.rst` & `earthkit_data-0.8.1/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/make.bat` & `earthkit_data-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/plugins/index.rst` & `earthkit_data-0.8.1/docs/plugins/index.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/plugins/plugins.rst` & `earthkit_data-0.8.1/docs/plugins/plugins.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/plugins/sources_plugin.rst` & `earthkit_data-0.8.1/docs/plugins/sources_plugin.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/release_notes/version_0.2_updates.rst` & `earthkit_data-0.8.1/docs/release_notes/version_0.2_updates.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/release_notes/version_0.3_updates.rst` & `earthkit_data-0.8.1/docs/release_notes/version_0.3_updates.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/release_notes/version_0.4_updates.rst` & `earthkit_data-0.8.1/docs/release_notes/version_0.4_updates.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/release_notes/version_0.5_updates.rst` & `earthkit_data-0.8.1/docs/release_notes/version_0.5_updates.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/release_notes/version_0.7_updates.rst` & `earthkit_data-0.8.1/docs/release_notes/version_0.7_updates.rst`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/docs/skip_api_rules.py` & `earthkit_data-0.8.1/docs/skip_api_rules.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 
 try:
     # NOTE: the `version.py` file must not be present in the git repository
     #   as it is generated by setuptools at install time
-    from .version import __version__
+    from ._version import __version__
 except ImportError:  # pragma: no cover
     # Local copy or not installed with setuptools
     __version__ = "999"
 
 from earthkit.data.translators import transform
 from earthkit.data.wrappers import get_wrapper as from_object
```

### Comparing `earthkit_data-0.7.0/earthkit/data/arguments/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/arguments/args_kwargs.py` & `earthkit_data-0.8.1/src/earthkit/data/arguments/args_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/arguments/argument.py` & `earthkit_data-0.8.1/src/earthkit/data/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/arguments/earthkit_types.py` & `earthkit_data-0.8.1/src/earthkit/data/arguments/earthkit_types.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/arguments/input_manager.py` & `earthkit_data-0.8.1/src/earthkit/data/arguments/input_manager.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/arguments/transformers.py` & `earthkit_data-0.8.1/src/earthkit/data/arguments/transformers.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/conf/css/tab.css` & `earthkit_data-0.8.1/src/earthkit/data/conf/css/tab.css`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/conf/css/tree.css` & `earthkit_data-0.8.1/src/earthkit/data/conf/css/tree.css`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/conf/global_grids.json` & `earthkit_data-0.8.1/src/earthkit/data/conf/global_grids.json`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/conf/gridspec.yaml` & `earthkit_data-0.8.1/src/earthkit/data/conf/gridspec.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/conf/gridspec_schema.json` & `earthkit_data-0.8.1/src/earthkit/data/conf/gridspec_schema.json`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/core/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,44 +94,44 @@
         self._not_implemented()
 
     @abstractmethod
     def order_by(self, *args, **kwargs):
         """Reorder the elements of the object."""
         self._not_implemented()
 
-    def unique_values(self, *coords, remapping=None, progress_bar=True):
+    def unique_values(self, *coords, remapping=None, patches=None, progress_bar=True):
         """
         Given a list of metadata attributes, such as date, param, levels,
         returns the list of unique values for each attributes
         """
         from earthkit.data.core.order import build_remapping
         from earthkit.data.utils.progbar import progress_bar
 
         assert len(coords)
         assert all(isinstance(k, str) for k in coords), coords
 
-        remapping = build_remapping(remapping)
+        remapping = build_remapping(remapping, patches)
         iterable = self
 
         if progress_bar:
             iterable = progress_bar(
                 iterable=self,
                 desc=f"Finding coords in dataset for {coords}",
             )
 
-        dic = defaultdict(dict)
+        vals = defaultdict(dict)
         for f in iterable:
             metadata = remapping(f.metadata)
             for k in coords:
-                v = metadata(k)
-                dic[k][v] = True
+                v = metadata(k, default=None)
+                vals[k][v] = True
 
-        dic = {k: tuple(values.keys()) for k, values in dic.items()}
+        vals = {k: tuple(values.keys()) for k, values in vals.items()}
 
-        return dic
+        return vals
 
     # @abstractmethod
     # def to_points(self, *args, **kwargs):
     #     self._not_implemented()
 
     # @abstractmethod
     # def to_latlon(self, *args, **kwargs):
@@ -148,7 +148,15 @@
         module = self.__class__.__module__
         name = self.__class__.__name__
 
         extra = ""
         if hasattr(self, "path"):
             extra = f" on {self.path}"
         raise NotImplementedError(f"{module}.{name}.{func}(){extra}")
+
+    def batched(self, *args):
+        """Return iterator for batches of data"""
+        self._not_implemented()
+
+    def group_by(self, *args):
+        """Return iterator for batches of data grouped by metadata keys"""
+        self._not_implemented()
```

### Comparing `earthkit_data-0.7.0/earthkit/data/core/caching.py` & `earthkit_data-0.8.1/src/earthkit/data/core/caching.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/core/fieldlist.py` & `earthkit_data-0.8.1/src/earthkit/data/core/fieldlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 
 import math
 from abc import abstractmethod
 from collections import defaultdict
 
 from earthkit.data.core import Base
-from earthkit.data.core.index import Index
+from earthkit.data.core.index import Index, MaskIndex, MultiIndex
 from earthkit.data.decorators import cached_method, detect_out_filename
 from earthkit.data.utils.array import ensure_backend, numpy_backend
 from earthkit.data.utils.metadata import metadata_argument
 
 
 class Field(Base):
     r"""Represent a Field."""
@@ -337,14 +337,39 @@
         --------
         to_points
 
         """
         lon, lat = self.data(("lon", "lat"), flatten=flatten, dtype=dtype)
         return dict(lat=lat, lon=lon)
 
+    def grid_points(self):
+        r = self.to_latlon(flatten=True)
+        return r["lat"], r["lon"]
+
+    def grid_points_unrotated(self):
+        lat = self._metadata.geography.latitudes_unrotated()
+        lon = self._metadata.geography.longitudes_unrotated()
+        return lat, lon
+
+    @property
+    def rotation(self):
+        return self._metadata.geography.rotation
+
+    @property
+    def resolution(self):
+        return self._metadata.geography.resolution()
+
+    @property
+    def mars_grid(self):
+        return self._metadata.geography.mars_grid()
+
+    @property
+    def mars_area(self):
+        return self._metadata.geography.mars_area()
+
     @property
     def shape(self):
         r"""tuple: Get the shape of the field.
 
         For structured grids the shape is a tuple in the form of (Nj, Ni) where:
 
         - ni: the number of gridpoints in i direction (longitude for a regular latitude-longitude grid)
@@ -650,14 +675,18 @@
     def _init_from_mask(self, index):
         self._array_backend = index._index.array_backend
 
     def _init_from_multi(self, index):
         self._array_backend = index._indexes[0].array_backend
 
     @staticmethod
+    def from_fields(fields):
+        raise NotImplementedError
+
+    @staticmethod
     def from_numpy(array, metadata):
         from earthkit.data.sources.array_list import ArrayFieldList
 
         return ArrayFieldList(array, metadata, array_backend=numpy_backend())
 
     @staticmethod
     def from_array(array, metadata):
@@ -1412,7 +1441,31 @@
             array_backend = self._array_backend
         array_backend = ensure_backend(array_backend)
         return self._to_array_fieldlist(array_backend=array_backend, **kwargs)
 
     def _to_array_fieldlist(self, **kwargs):
         md = [f.metadata() for f in self]
         return self.from_array(self.to_array(**kwargs), md)
+
+    def cube(self, *args, **kwargs):
+        from earthkit.data.indexing.cube import FieldCube
+
+        return FieldCube(self, *args, **kwargs)
+
+    @classmethod
+    def new_mask_index(self, *args, **kwargs):
+        return MaskFieldList(*args, **kwargs)
+
+    @classmethod
+    def merge(cls, sources):
+        assert all(isinstance(_, FieldList) for _ in sources)
+        return MultiFieldList(sources)
+
+
+class MaskFieldList(FieldList, MaskIndex):
+    def __init__(self, *args, **kwargs):
+        MaskIndex.__init__(self, *args, **kwargs)
+
+
+class MultiFieldList(FieldList, MultiIndex):
+    def __init__(self, *args, **kwargs):
+        MultiIndex.__init__(self, *args, **kwargs)
```

### Comparing `earthkit_data-0.7.0/earthkit/data/core/geography.py` & `earthkit_data-0.8.1/src/earthkit/data/core/geography.py`

 * *Files 10% similar despite different names*

```diff
@@ -123,7 +123,19 @@
         r"""Return the grid specification.
 
         Returns
         -------
         :class:`~data.core.gridspec.GridSpec>`
         """
         pass
+
+    @abstractmethod
+    def resolution(self):
+        pass
+
+    @abstractmethod
+    def mars_grid(self):
+        pass
+
+    @abstractmethod
+    def mars_area(self):
+        pass
```

### Comparing `earthkit_data-0.7.0/earthkit/data/core/gridspec.py` & `earthkit_data-0.8.1/src/earthkit/data/core/gridspec.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/core/index.py` & `earthkit_data-0.8.1/src/earthkit/data/core/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         self.remapping = remapping
 
     @abstractmethod
     def build_actions(self, kwargs):
         raise NotImplementedError()
 
     def compare_elements(self, a, b):
+        assert callable(self.remapping), (type(self.remapping), self.remapping)
         a_metadata = self.remapping(a.metadata)
         b_metadata = self.remapping(b.metadata)
         for k, v in self.actions.items():
             n = v(a_metadata(k, default=None), b_metadata(k, default=None))
             if n != 0:
                 return n
         return 0
@@ -116,26 +117,26 @@
 class Order(OrderBase):
     def build_actions(self, kwargs):
         actions = {}
 
         def ascending(a, b):
             if a == b:
                 return 0
-            if a > b:
+            if b is None or a > b:
                 return 1
-            if a < b:
+            if a is None or a < b:
                 return -1
             raise ValueError(f"{a},{b}")
 
         def descending(a, b):
             if a == b:
                 return 0
-            if a > b:
+            if b is None or a > b:
                 return -1
-            if a < b:
+            if a is None or a < b:
                 return 1
             raise ValueError(f"{a},{b}")
 
         class Compare:
             def __init__(self, order):
                 self.order = order
 
@@ -165,14 +166,17 @@
             order = {}
             for i, key in enumerate(v):
                 order[str(key)] = i
                 try:
                     order[int(key)] = i
                 except ValueError:
                     pass
+                except TypeError:
+                    print('Cannot convert "%s" to int (%s)' % (key, type(key)))
+                    raise
                 try:
                     order[float(key)] = i
                 except ValueError:
                     pass
             actions[k] = Compare(order)
 
         return actions
@@ -269,21 +273,23 @@
         GribField(v,500,20180801,1200,0,0)
         GribField(u,400,20180801,1200,0,0)
         GribField(v,400,20180801, 1200,0,0)
 
         Using ``remapping`` to specify the selection by a key created from two other keys
         (we created key "param_level" from "param" and "levelist"):
 
-        >>> for f in ds.order_by(
+        >>> subset = ds.sel(
         ...     param_level=["t850", "u1000"],
         ...     remapping={"param_level": "{param}{levelist}"},
-        ... ):
+        ... )
+        >>> for f in subset:
         ...     print(f)
-        GribField(t,850,20180801,1200,0,0)
+        ...
         GribField(u,1000,20180801,1200,0,0)
+        GribField(t,850,20180801,1200,0,0)
         """
         kwargs = normalize_selection(*args, **kwargs)
         kwargs = self._normalize_kwargs_names(**kwargs)
         if not kwargs:
             return self
 
         selection = Selection(kwargs, remapping=remapping)
@@ -387,15 +393,15 @@
         kwargs = selection_from_index(self.index, kwargs)
 
         if not kwargs:
             return self.new_mask_index(self, [])
 
         return self.sel(**kwargs)
 
-    def order_by(self, *args, remapping=None, **kwargs):
+    def order_by(self, *args, remapping=None, patches=None, **kwargs):
         """Changes the order of the elements in a fieldlist-like object.
 
         Parameters
         ----------
         *args: tuple
             Positional arguments specifying the metadata keys to perform the ordering on.
             (See below for details)
@@ -484,15 +490,15 @@
         GribField(v,850,20180801,1200,0,0)
         GribField(v,1000,20180801,1200,0,0)
         GribField(u,850,20180801,1200,0,0)
         """
         kwargs = normalize_order_by(*args, **kwargs)
         kwargs = self._normalize_kwargs_names(**kwargs)
 
-        remapping = build_remapping(remapping)
+        remapping = build_remapping(remapping, patches)
 
         if not kwargs:
             return self
 
         order = Order(kwargs, remapping=remapping)
         # order = Order(*args, **kwargs)
         if order.is_empty:
@@ -503,43 +509,47 @@
 
         indices = list(range(len(self)))
         indices = sorted(indices, key=functools.cmp_to_key(cmp))
         return self.new_mask_index(self, indices)
 
     def __getitem__(self, n):
         if isinstance(n, slice):
-            return self.from_slice(n)
+            return self._from_slice(n)
         if isinstance(n, (tuple, list)):
-            return self.from_multi(n)
+            return self._from_sequence(n)
         if isinstance(n, dict):
-            return self.from_dict(n)
+            return self._from_dict(n)
         else:
             import numpy as np
 
             if isinstance(n, np.ndarray):
-                return self.from_multi(n)
+                return self._from_ndarray(n)
 
         return self._getitem(n)
 
-    def from_slice(self, s):
+    def _from_slice(self, s):
         indices = range(len(self))[s]
         return self.new_mask_index(self, indices)
 
-    def from_mask(self, lst):
+    def _from_mask(self, lst):
         indices = [i for i, x in enumerate(lst) if x]
         return self.new_mask_index(self, indices)
 
-    def from_multi(self, a):
-        import numpy as np
+    def _from_sequence(self, s):
+        return self.new_mask_index(self, s)
 
-        # will raise IndexError if an index is out of bounds
-        n = len(self)
-        indices = np.arange(0, n if n > 0 else 0)
-        indices = indices[a].tolist()
-        return self.new_mask_index(self, indices)
+    def _from_ndarray(self, a):
+        return self._from_sequence(a.tolist())
+        # import numpy as np
+
+        # # will raise IndexError if an index is out of bounds
+        # n = len(self)
+        # indices = np.arange(0, n if n > 0 else 0)
+        # indices = indices[a].tolist()
+        # return self.new_mask_index(self, indices)
 
     def from_dict(self, dic):
         return self.sel(dic)
 
     @classmethod
     def merge(cls, sources):
         assert all(isinstance(_, Index) for _ in sources)
@@ -549,14 +559,59 @@
         import numpy as np
 
         return np.array([f.to_numpy(*args, **kwargs) for f in self])
 
     def full(self, *coords):
         return FullIndex(self, *coords)
 
+    def batched(self, n):
+        """Iterate through the object in batches of ``n``.
+
+        Parameters
+        ----------
+        n: int
+            Batch size.
+
+        Returns
+        -------
+        object
+            Returns an iterator yielding batches of ``n`` elements. Each batch is a new object
+            containing a view to the data in the original object, so no data is copied. The last
+            batch may contain fewer than ``n`` elements.
+
+        """
+        from earthkit.data.utils.batch import batched
+
+        return batched(self, n, mode="indexed")
+
+    def group_by(self, *keys, sort=True):
+        """Iterate through the object in groups defined by metadata keys.
+
+        Parameters
+        ----------
+        *keys: tuple
+            Positional arguments specifying the metadata keys to group by.
+            Keys can be a single or multiple str, or a list or tuple of str.
+
+        sort: bool, optional
+            If ``True`` (default), the object is sorted by the metadata ``keys`` before grouping.
+            Sorting is only applied if the object is supporting the sorting operation.
+
+        Returns
+        -------
+        object
+            Returns an iterator yielding batches of elements grouped by the metadata ``keys``. Each
+            batch is a new object containing a view to the data in the original object, so no data
+            is copied. It generates a new group every time the value of the ``keys`` change.
+
+        """
+        from earthkit.data.utils.batch import group_by
+
+        return group_by(self, *keys, sort=sort, mode="indexed")
+
 
 class MaskIndex(Index):
     def __init__(self, index, indices):
         self._index = index
         self._indices = list(indices)
         # super().__init__(
         #     *self.index._init_args,
```

### Comparing `earthkit_data-0.7.0/earthkit/data/core/ipython.py` & `earthkit_data-0.8.1/src/earthkit/data/core/ipython.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/core/metadata.py` & `earthkit_data-0.8.1/src/earthkit/data/core/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     def _is_custom_key(self, key):
         return key in self.CUSTOM_KEYS and key not in self
 
     def _get_custom_key(self, key, default=None, raise_on_missing=True, **kwargs):
         if self._is_custom_key(key):
             try:
                 if key == DATETIME:
-                    return self._valid_datetime()
+                    return self._valid_datetime().isoformat()
                 elif key == GRIDSPEC:
                     return self.grid_spec
             except Exception as e:
                 if not raise_on_missing:
                     return default
                 else:
                     raise KeyError(f"{key}, reason={e}")
@@ -302,15 +302,15 @@
 
         If it is not available None is returned.
         """
         return None
 
     @property
     def gridspec(self):
-        r""":ref:`~data.core.gridspec.GridSpec`: Get grid description.
+        r""":class:`~data.core.gridspec.GridSpec`: Get grid description.
 
         If it is not available None is returned.
         """
         return None if self.geography is None else self.geography.gridspec()
 
     def ls_keys(self):
         r"""Return the keys to be used with the :meth:`ls` method."""
```

### Comparing `earthkit_data-0.7.0/earthkit/data/core/plugins.py` & `earthkit_data-0.8.1/src/earthkit/data/core/plugins.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/core/select.py` & `earthkit_data-0.8.1/src/earthkit/data/core/select.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/core/settings.py` & `earthkit_data-0.8.1/src/earthkit/data/core/settings.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/core/statistics.py` & `earthkit_data-0.8.1/src/earthkit/data/core/statistics.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/core/thread.py` & `earthkit_data-0.8.1/src/earthkit/data/core/thread.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/decorators.py` & `earthkit_data-0.8.1/src/earthkit/data/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             and hasattr(self, "path")
             and self.path is not None
             and os.path.isfile(self.path)
             and os.path.samefile(args[0], self.path)
         ):
             warnings.warn(
                 UserWarning(
-                    f"Earhtkit refusing to overwrite the file we are currently reading: {args[0]}"
+                    f"Earthkit refusing to overwrite the file we are currently reading: {args[0]}"
                 )
             )
             return
 
         return func(self, *args, **kwargs)
 
     return wrapped
```

### Comparing `earthkit_data-0.7.0/earthkit/data/indexing/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/indexing/database/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/indexing/database/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/indexing/database/json.py` & `earthkit_data-0.8.1/src/earthkit/data/indexing/database/json.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/indexing/database/sql.py` & `earthkit_data-0.8.1/src/earthkit/data/indexing/database/sql.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/indexing/database/stdout.py` & `earthkit_data-0.8.1/src/earthkit/data/indexing/database/stdout.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/mergers/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/mergers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/mergers/pandas.py` & `earthkit_data-0.8.1/src/earthkit/data/mergers/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/mergers/xarray.py` & `earthkit_data-0.8.1/src/earthkit/data/mergers/xarray.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/mirrors/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/mirrors/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/mirrors/directory_mirror.py` & `earthkit_data-0.8.1/src/earthkit/data/mirrors/directory_mirror.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/archive.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/archive.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/bufr/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/bufr/bufr.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/bufr/bufr.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/bufr/pandas.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/bufr/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/covjson.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/covjson.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,17 @@
             return d
 
 
 class CovjsonStreamReader(Reader):
     def __init__(self, stream):
         self.stream = stream
 
+    def __iter__(self):
+        return self
+
     def __next__(self):
         import json
 
         d = self.stream.read()
         if d:
             return CovjsonInMemory(json.loads(d))
         else:
```

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/csv.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/csv.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/directory.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/directory.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/geojson.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/geojson.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     return (magic is None or len(magic) == 0) and (
         content_type is None or len(content_type) == 0
     )
 
 
 def reader(source, path, *, magic=None, deeper_check=False, parts=None, **kwargs):
     if _match_magic(magic, deeper_check):
-        from .reader import GRIBReader
+        from .file import GRIBReader
 
         return GRIBReader(source, path, parts=parts)
 
 
 def memory_reader(source, buffer, *, magic=None, deeper_check=False, **kwargs):
     if _match_magic(magic, deeper_check):
         from .memory import GribFieldListInMemory, GribMessageMemoryReader
```

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/codes.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/codes.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/gridspec.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/gridspec.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/index/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/index/db.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/db.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/index/file.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/file.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/index/json.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/json.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/index/sql.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/index/sql.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/memory.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from earthkit.data.readers.grib.index import GribFieldList
 from earthkit.data.utils.array import ensure_backend
 
 LOG = logging.getLogger(__name__)
 
 
 class GribMemoryReader(Reader):
-    def __init__(self, array_backend=None):
+    def __init__(self, array_backend=None, **kwargs):
         self._peeked = None
         self._array_backend = ensure_backend(array_backend)
 
     def __iter__(self):
         return self
 
     def __next__(self):
@@ -32,65 +32,37 @@
             msg = self._peeked
             self._peeked = None
             return msg
         handle = self._next_handle()
         msg = self._message_from_handle(handle)
         if handle is not None:
             return msg
+        self.consumed_ = True
         raise StopIteration
 
     def _next_handle(self):
         raise NotImplementedError
 
     def _message_from_handle(self, handle):
         if handle is not None:
             return GribFieldInMemory(
                 GribCodesHandle(handle, None, None), self._array_backend
             )
 
-    def peek(self):
-        """Returns the next available message without consuming it"""
-        if self._peeked is None:
-            handle = self._next_handle()
-            self._peeked = self._message_from_handle(handle)
-        return self._peeked
-
-    def read_batch(self, n):
-        fields = []
-        for _ in range(n):
-            try:
-                fields.append(self.__next__())
-            except StopIteration:
-                break
-        if not fields:
-            raise StopIteration
+    def batched(self, n):
+        from earthkit.data.utils.batch import batched
 
-        return GribFieldListInMemory.from_fields(fields)
+        return batched(self, n, create=self.to_fieldlist)
 
-    def read_group(self, group):
-        assert isinstance(group, list)
+    def group_by(self, *args, **kwargs):
+        from earthkit.data.utils.batch import group_by
 
-        fields = []
-        current_group = {}
-        while True:
-            f = self.peek()
-            if f is not None:
-                group_md = f._attributes(group)
-                if not current_group:
-                    current_group = group_md
-                if current_group == group_md:
-                    fields.append(f)
-                    self.__next__()
-                else:
-                    break
-            elif fields:
-                break
-            else:
-                raise StopIteration
+        return group_by(self, *args, create=self.to_fieldlist, sort=False)
 
+    def to_fieldlist(self, fields):
         return GribFieldListInMemory.from_fields(fields)
 
 
 class GribFileMemoryReader(GribMemoryReader):
     def __init__(self, path, **kwargs):
         super().__init__(**kwargs)
         self.fp = open(path, "rb")
@@ -122,15 +94,15 @@
     """Wrapper around eccodes.Streamreader. The problem is that when iterating via
     the StreamReader it returns an eccodes.GRIBMessage that releases the handle when deleted.
     However, the handle has to be managed by earthkit-data so we access it directly
     using _next_handle
     """
 
     def __init__(self, stream, **kwargs):
-        super().__init__()
+        super().__init__(**kwargs)
         self._stream = stream
         self._reader = eccodes.StreamReader(stream)
 
     def __del__(self):
         self._stream.close()
 
     def _next_handle(self):
@@ -154,14 +126,18 @@
     def handle(self):
         return self._handle
 
     @GribField.handle.getter
     def offset(self):
         return None
 
+    @staticmethod
+    def to_fieldlist(fields):
+        return GribFieldListInMemory.from_fields(fields)
+
 
 class GribFieldListInMemory(GribFieldList, Reader):
     """Represent a GRIB field list in memory"""
 
     @staticmethod
     def from_fields(fields, array_backend=None):
         if array_backend is None and len(fields) > 0:
```

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/metadata.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import datetime
+import warnings
+from functools import cached_property
 
 from earthkit.data.core.geography import Geography
 from earthkit.data.core.metadata import Metadata
 from earthkit.data.decorators import cached_method
 from earthkit.data.indexing.database import GRIB_KEYS_NAMES
 from earthkit.data.readers.grib.gridspec import make_gridspec
 from earthkit.data.utils.bbox import BoundingBox
@@ -21,14 +23,15 @@
 def missing_is_none(x):
     return None if x == 2147483647 else x
 
 
 class GribFieldGeography(Geography):
     def __init__(self, metadata):
         self.metadata = metadata
+        self.check_rotated_support()
 
     def latitudes(self, dtype=None):
         r"""Return the latitudes of the field.
 
         Returns
         -------
         ndarray
@@ -134,24 +137,119 @@
             west=self.metadata.get("longitudeOfFirstGridPointInDegrees", None),
             east=self.metadata.get("longitudeOfLastGridPointInDegrees", None),
         )
 
     def gridspec(self):
         return make_gridspec(self.metadata)
 
+    def resolution(self):
+        grid_type = self.metadata.get("gridType")
+
+        if grid_type in ("reduced_gg", "reduced_rotated_gg"):
+            return self.metadata.get("gridName")
+
+        if grid_type == "regular_ll":
+            x = self.metadata.get("DxInDegrees")
+            y = self.metadata.get("DyInDegrees")
+            assert x == y, (x, y)
+            return x
+
+        if grid_type == "lambert":
+            x = self.metadata.get("DxInMetres")
+            y = self.metadata.get("DyInMetres")
+            assert x == y, (x, y)
+            return str(x / 1000).replace(".", "p") + "km"
+
+        raise ValueError(f"Unknown gridType={grid_type}")
+
+    def mars_grid(self):
+        if len(self.shape()) == 2:
+            return [
+                self.metadata.get("iDirectionIncrementInDegrees"),
+                self.metadata.get("jDirectionIncrementInDegrees"),
+            ]
+
+        return self.metadata.get("gridName")
+
+    def mars_area(self):
+        north = self.metadata.get("latitudeOfFirstGridPointInDegrees")
+        south = self.metadata.get("latitudeOfLastGridPointInDegrees")
+        west = self.metadata.get("longitudeOfFirstGridPointInDegrees")
+        east = self.metadata.get("longitudeOfLastGridPointInDegrees")
+        return [north, west, south, east]
+
+    @property
+    def rotation(self):
+        return (
+            self.metadata.get("latitudeOfSouthernPoleInDegrees"),
+            self.metadata.get("longitudeOfSouthernPoleInDegrees"),
+            self.metadata.get("angleOfRotationInDegrees"),
+        )
+
+    @cached_property
+    def rotated(self):
+        grid_type = self.metadata.get("gridType")
+        return "rotated" in grid_type
+
+    @cached_property
+    def rotated_iterator(self):
+        return self.metadata.get("iteratorDisableUnrotate") is not None
+
+    def check_rotated_support(self):
+        if self.rotated and self.metadata.get("gridType") == "reduced_rotated_gg":
+            from earthkit.data.utils.message import ECC_FEATURES
+
+            if not ECC_FEATURES.version >= (2, 35, 0):
+                raise RuntimeError(
+                    "gridType=rotated_reduced_gg requires ecCodes >= 2.35.0"
+                )
+
+    def latitudes_unrotated(self, **kwargs):
+        if not self.rotated:
+            return self.latitudes(**kwargs)
+
+        if not self.rotated_iterator:
+            from earthkit.geo.rotate import unrotate
+
+            grid_type = self.metadata.get("gridType")
+            warnings.warn(f"ecCodes does not support rotated iterator for {grid_type}")
+            lat, lon = self.latitudes(**kwargs), self.longitudes(**kwargs)
+            south_pole_lat, south_pole_lon, _ = self.rotation
+            lat, lon = unrotate(lat, lon, south_pole_lat, south_pole_lon)
+            return lat
+
+        with self.metadata._handle._set_tmp("iteratorDisableUnrotate", 1, 0):
+            return self.latitudes(**kwargs)
+
+    def longitudes_unrotated(self, **kwargs):
+        if not self.rotated:
+            return self.longitudes(**kwargs)
+
+        if not self.rotated_iterator:
+            from earthkit.geo.rotate import unrotate
+
+            grid_type = self.metadata.get("gridType")
+            warnings.warn(f"ecCodes does not support rotated iterator for {grid_type}")
+            lat, lon = self.latitudes(**kwargs), self.longitudes(**kwargs)
+            south_pole_lat, south_pole_lon, _ = self.rotation
+            lat, lon = unrotate(lat, lon, south_pole_lat, south_pole_lon)
+            return lon
+
+        with self.metadata._handle._set_tmp("iteratorDisableUnrotate", 1, 0):
+            return self.longitudes(**kwargs)
+
 
 class GribMetadata(Metadata):
     """Represent the metadata of a GRIB field.
 
     Parameters
     ----------
     handle: :obj:`GribCodesHandle`
         Object representing the ecCodes GRIB handle of the field.
 
-
     :obj:`GribMetadata` is created internally by a :obj:`GribField` and we can use
     the field's :meth:`metadata` method to access it.
 
     >>> ds = earthkit.data.from_source("file", "docs/examples/test4.grib")
     >>> md = ds[0].metadata()
     >>> md["shortName"]
     't'
```

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/output.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,17 +191,17 @@
             if "number" in metadata:
                 metadata["stream"] = "enfo"
                 metadata.setdefault("type", "pf")
 
         if "number" in metadata:
             compulsory += ("numberOfForecastsInEnsemble",)
             productDefinitionTemplateNumber = {"tp": 11}
-            metadata[
-                "productDefinitionTemplateNumber"
-            ] = productDefinitionTemplateNumber.get(handle.get("shortName"), 1)
+            metadata["productDefinitionTemplateNumber"] = (
+                productDefinitionTemplateNumber.get(handle.get("shortName"), 1)
+            )
 
         if metadata.get("type") in ("pf", "cf"):
             metadata.setdefault("typeOfGeneratingProcess", 4)
 
         if "levelist" in metadata:
             metadata.setdefault("levtype", "pl")
```

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/pandas.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/parsing.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/parsing.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/reader.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/file.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/grib/xarray.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/grib/xarray.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,20 +66,27 @@
         ----------
         **kwargs: dict, optional
             Other keyword arguments:
 
             xarray_open_dataset_kwargs: dict, optional
                 Keyword arguments passed to ``xarray.open_dataset()``. Default value is::
 
-                    {"backend_kwargs": {"errors": "raise"},
+                    {"backend_kwargs": {"errors": "raise", "ignore_keys": []},
                     "squeeze": False, "cache": True, "chunks": None,
                     "errors": "raise", "engine": "cfgrib"}
 
-                Please note that the settings ``errors="raise"`` and ``engine="cfgrib"`` are always
-                enforced and cannot be changed.
+                Please note that:
+
+                - ``backend_kwargs`` is passed to :xref:`cfgrib`, with the exception
+                  of ``ignore_keys``
+                - ``ignore_keys``  is not supported by :xref:`cfgrib`, but implemented in
+                  earthkit-data. It specifies the metadata keys that should be ignored when reading
+                  the GRIB messages in the backend.
+                - settings ``errors="raise"`` and ``engine="cfgrib"`` are always enforced and cannot
+                  be changed.
 
         Returns
         -------
         xarray DataSet
 
         Examples
         --------
@@ -117,25 +124,27 @@
                 user=user_xarray_open_dataset_kwargs.pop(key, {}),
                 default={"errors": "raise"},
                 forced={},
                 logging_owner="xarray_open_dataset_kwargs",
                 logging_main_key=key,
             )
 
-        default = dict(squeeze=False)  # TODO:Documenet me
+        default = dict(squeeze=False)  # TODO:Document me
         default.update(self.xarray_open_dataset_kwargs())
 
         xarray_open_dataset_kwargs.update(
             Kwargs(
                 user=user_xarray_open_dataset_kwargs,
                 default=default,
                 forced={
                     "errors": "raise",
                     "engine": "cfgrib",
                 },
+                logging_owner="xarray_open_dataset_kwargs",
+                warn_non_default=False,
             )
         )
 
         result = xr.open_dataset(
             IndexWrapperForCfGrib(self, ignore_keys=ignore_keys),
             **xarray_open_dataset_kwargs,
         )
```

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/netcdf/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/netcdf/coords.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/coords.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/netcdf/dataset.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/dataset.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/netcdf/field.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/field.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,31 +5,34 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 from datetime import timedelta
+from functools import cached_property
+
+import numpy as np
 
 from earthkit.data.core.fieldlist import Field
 from earthkit.data.core.geography import Geography
 from earthkit.data.core.metadata import RawMetadata
 from earthkit.data.utils.bbox import BoundingBox
 from earthkit.data.utils.dates import to_datetime
 from earthkit.data.utils.projections import Projection
 
 from .coords import LevelSlice, TimeSlice
 
 LOG = logging.getLogger(__name__)
 
 
 class XArrayFieldGeography(Geography):
-    def __init__(self, metadata, data_array, ds, variable):
+    def __init__(self, metadata, ds, variable):
         self.metadata = metadata
-        self.data_array = data_array
+        self.variable = variable
         self.ds = ds
         self.north, self.west, self.south, self.east = self.ds.bbox(variable)
 
     def latitudes(self, dtype=None):
         return self.ds._get_latlon(self.data_array, flatten=True, dtype=dtype)[0]
 
     def longitudes(self, dtype=None):
@@ -53,25 +56,44 @@
 
     def bounding_box(self):
         return BoundingBox(
             north=self.north, south=self.south, east=self.east, west=self.west
         )
 
     def _grid_mapping(self):
-        if "grid_mapping" in self.data_array.attrs:
-            grid_mapping = self.ds[self.data_array.attrs["grid_mapping"]]
+        da = self.data_array
+        if "grid_mapping" in da.attrs:
+            grid_mapping = self.ds[da.attrs["grid_mapping"]]
         else:
             raise AttributeError(
                 "no CF-compliant 'grid_mapping' detected in netCDF attributes"
             )
         return grid_mapping
 
     def gridspec(self):
         raise NotImplementedError("gridspec is not implemented for netcdf/xarray")
 
+    @property
+    def data_array(self):
+        return self.ds[self.variable]
+
+    def resolution(self):
+        # TODO: implement resolution
+        return None
+
+    @property
+    def mars_grid(self):
+        # TODO: implement mars_grid
+        return None
+
+    @property
+    def mars_area(self):
+        # TODO: code me
+        return [self.north, self.west, self.south, self.east]
+
 
 class XArrayMetadata(RawMetadata):
     LS_KEYS = ["variable", "level", "valid_datetime", "units"]
     NAMESPACES = [
         "default",
         "mars",
     ]
@@ -81,15 +103,16 @@
         if not isinstance(field, XArrayField):
             raise TypeError(
                 f"XArrayMetadata: expected field type XArrayField, got {type(field)}"
             )
         self._field = field
         self._geo = None
 
-        d = dict(self._field._da.attrs)
+        data_array = field._ds[field.variable]
+        d = dict(data_array.attrs)
 
         time = field.non_dim_coords.get("valid_time", field.non_dim_coords.get("time"))
         level = None
         level_type = "sfc"
 
         for s in field.slices:
             if isinstance(s, TimeSlice):
@@ -99,15 +122,15 @@
                 level = s.value
                 level_type = {"pressure": "pl"}.get(s.name, s.name)
 
         step = 0
         if time is not None:
             self.time = to_datetime(time)
             if "forecast_reference_time" in field._ds.data_vars:
-                forecast_reference_time = field.ds["forecast_reference_time"].data
+                forecast_reference_time = field._ds["forecast_reference_time"].data
                 assert forecast_reference_time.ndim == 0, forecast_reference_time
                 forecast_reference_time = forecast_reference_time.astype(
                     "datetime64[s]"
                 )
                 forecast_reference_time = forecast_reference_time.astype(object)
                 step = (time - forecast_reference_time).total_seconds()
                 assert step % 3600 == 0, step
@@ -130,15 +153,15 @@
     def override(self, *args, **kwargs):
         return None
 
     @property
     def geography(self):
         if self._geo is None:
             self._geo = XArrayFieldGeography(
-                self, self._field._da, self._field._ds, self._field.variable
+                self, self._field._ds, self._field.variable
             )
         return self._geo
 
     def as_namespace(self, namespace=None):
         if not isinstance(namespace, str) and namespace is not None:
             raise TypeError("namespace must be a str or None")
 
@@ -186,18 +209,14 @@
         return super()._get(_key_name(key), **kwargs)
 
 
 class XArrayField(Field):
     def __init__(self, ds, variable, slices, non_dim_coords, array_backend):
         super().__init__(array_backend)
         self._ds = ds
-        self._da = ds[variable]
-
-        # self.north, self.west, self.south, self.east = ds.bbox(variable)
-
         self.variable = variable
         self.slices = slices
         self.non_dim_coords = non_dim_coords
         self.name = self.variable
 
     def __repr__(self):
         return (
@@ -206,34 +225,60 @@
             + ")"
         )
 
     def _make_metadata(self):
         return XArrayMetadata(self)
 
     def to_xarray(self):
-        dims = self._da.dims
+        da = self._ds[self.variable]
+        dims = da.dims
         v = {}
         for s in self.slices:
             if s.is_dimension:
                 if s.name in dims:
                     v[s.name] = s.index
-        return self._da.isel(**v)
+        return da.isel(**v)
 
     def to_pandas(self):
         return self.to_xarray().to_pandas()
 
+    # def _to_numpy(self):
+    #     return self.to_xarray().to_numpy()
+
     def _to_numpy(self):
-        return self.to_xarray().to_numpy()
+        dimensions = dict((s.name, s.index) for s in self.slices)
+        # values = self.owner.xr_dataset[self.variable].isel(dimensions).values
+        values = self._ds[self.variable].isel(dimensions).values
+        return values
 
     def _values(self, dtype=None):
         if dtype is None:
             return self._to_numpy()
         else:
             return self._to_numpy().astype(dtype, copy=False)
 
+    @cached_property
+    def grid_mapping(self):
+        def tidy(x):
+            if isinstance(x, np.ndarray):
+                return x.tolist()
+            if isinstance(x, (tuple, list)):
+                return [tidy(y) for y in x]
+            if isinstance(x, dict):
+                return {k: tidy(v) for k, v in x.items()}
+            return x
+
+        # return tidy(
+        #     self.owner.xr_dataset[
+        #         self.owner.xr_dataset[self.variable].grid_mapping
+        #     ].attrs
+        # )
+
+        return tidy(self._ds[self._ds[self.variable].grid_mapping].attrs)
+
 
 class NetCDFMetadata(XArrayMetadata):
     pass
 
 
 class NetCDFField(XArrayField):
     def _make_metadata(self):
```

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/netcdf/fieldlist.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/netcdf/fieldlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
             fields.append(field_type(ds, name, slices, non_dim_coords, array_backend))
 
     # if not fields:
     #     raise Exception("NetCDFReader no 2D fields found in %s" % (self.path,))
 
     if check_only:
         return False
+
     return fields
 
 
 class XArrayFieldListCore(FieldList):
     FIELD_TYPE = None
 
     def __init__(self, *args, **kwargs):
@@ -167,15 +168,15 @@
             return get_fields_from_ds(
                 DataSet(self.xr_dataset),
                 self.array_backend,
                 field_type=self.FIELD_TYPE,
                 check_only=True,
             )
         else:
-            return len(self._fields)
+            return len(self._fields) > 0
 
     def _get_fields(self, ds):
         return get_fields_from_ds(ds, self.array_backend, field_type=self.FIELD_TYPE)
 
     def to_pandas(self, **kwargs):
         return self.to_xarray(**kwargs).to_pandas()
```

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/numpy.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/numpy.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/odb.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/odb.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/shapefile.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/shapefile.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/tar.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/tar.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/text.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/text.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/unknown.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/unknown.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/readers/zip.py` & `earthkit_data-0.8.1/src/earthkit/data/readers/zip.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/ads.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/ads.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/array_list.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/array_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         )
         self._array = array
 
     def _make_metadata(self):
         pass
 
     def _values(self, dtype=None):
-        """native array type"""
+        """Native array type"""
         if dtype is None:
             return self._array
         else:
             return self.array_backend.array_ns.astype(self._array, dtype, copy=False)
 
     def __repr__(self):
         return f"{self.__class__.__name__}()"
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/cds.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/cds.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/constants.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,17 +38,16 @@
         return None
 
     def _valid_datetime(self):
         return datetime.datetime.fromisoformat(self["valid_datetime"])
 
 
 class ConstantMaker:
-    def __init__(self, source_or_dataset):
-        self.source_or_dataset = source_or_dataset
-        self.field = source_or_dataset[0]
+    def __init__(self, field):
+        self.field = field
         self.shape = self.field.shape
 
     @cached_method
     def grid_points(self):
         d = self.field.to_latlon(flatten=True)
         return d["lat"], d["lon"]
 
@@ -180,49 +179,79 @@
         result = cos_solar_zenith_angle(
             date,
             self.latitude_(),
             self.longitude_(),
         )
         return result.flatten()
 
+    def __getattr__(self, name):
+        if "+" not in name and "-" not in name:
+            # If we are here, we are looking for a method that does not exist,
+            # it has to be a method with a time delta.
+            raise AttributeError(name)
+        if "+" in name:
+            fname, delta = name.split("+")
+            sign = 1
+        if "-" in name:
+            fname, delta = name.split("-")
+            sign = -1
+        method = getattr(self, fname)
+
+        if delta.endswith("h"):
+            factor = 60
+        elif delta.endswith("d"):
+            factor = 24 * 60
+        else:
+            raise ValueError(f"Invalid time delta {delta} in {name}")
+
+        delta = delta[:-1]
+        delta = int(delta)
+        delta = datetime.timedelta(minutes=delta) * factor * sign
+
+        def wrapper(date):
+            date = date + delta
+            value = method(date)
+            return value
+
+        return wrapper
+
 
 class ConstantField(Field):
-    def __init__(self, date, param, proc, shape, geometry, backend):
+    def __init__(self, maker, date, param, proc, number=None, array_backend=None):
+        self.maker = maker
         self.date = date
         self.param = param
         self.proc = proc
-        self._shape = shape
-        self._geometry = geometry
+        self.number = number
+        # self._shape = shape
+        # self._geometry = self.maker.field.metadata().geography
         d = dict(
             valid_datetime=date if isinstance(date, str) else date.isoformat(),
             param=param,
             level=None,
             levelist=None,
-            number=None,
+            number=number,
+            levtype=None,
+        )
+        super().__init__(
+            array_backend,
+            metadata=ConstantMetadata(d, self.maker.field.metadata().geography),
         )
-        super().__init__(backend, metadata=ConstantMetadata(d, geometry))
 
     def _make_metadata(self):
         pass
 
     def _values(self, dtype=None):
         values = self.proc(self.date)
         if dtype is not None:
             values = values.astype(dtype)
         return values
 
-    @property
-    def shape(self):
-        return self._shape
-
     def __repr__(self):
-        return "ConstantField(%s,%s)" % (
-            self.param,
-            self.date,
-        )
+        return "ConstantField(%s,%s,%s)" % (self.param, self.date, self.number)
 
 
 def make_datetime(date, time):
     if time is None:
         return date
     if date.hour or date.minute:
         raise ValueError(
@@ -254,42 +283,72 @@
     result = tuple(result)
 
     assert len(result) == len(shape)
     return result
 
 
 class ConstantsFieldListCore(FieldList):
-    def __init__(self, source_or_dataset, request={}, repeat=1, **kwargs):
+    def __init__(self, source_or_dataset, request={}, **kwargs):
         request = dict(**request)
         request.update(kwargs)
 
         self.request = self._request(**request)
 
-        if "date" in self.request:
-            self.dates = [
-                make_datetime(date, time)
-                for date, time in itertools.product(
-                    self.request["date"], self.request.get("time", [None])
-                )
-            ]
-            assert len(set(self.dates)) == len(
-                self.dates
-            ), "Duplicates dates in constants."
-        else:
-            self.dates = source_or_dataset.unique_values("valid_datetime")[
-                "valid_datetime"
-            ]
+        def find_numbers(source_or_dataset):
+            if "number" in self.request:
+                return self.request["number"]
+
+            assert hasattr(source_or_dataset, "unique_values"), (
+                f"{source_or_dataset} (type '{type(source_or_dataset).__name__}') is"
+                " not a proper source or dataset"
+            )
+
+            return source_or_dataset.unique_values(
+                "number", patches={"number": {None: 0}}
+            )["number"]
+
+        def find_dates(source_or_dataset):
+            if "date" not in self.request and "time" in self.request:
+                raise ValueError("Cannot specify time without date")
+
+            if "date" in self.request and "time" not in self.request:
+                return self.request["date"]
+
+            if "date" in self.request and "time" in self.request:
+                dates = [
+                    make_datetime(date, time)
+                    for date, time in itertools.product(
+                        self.request["date"], self.request["time"]
+                    )
+                ]
+                assert len(set(dates)) == len(dates), "Duplicates dates in constants."
+                return dates
+
+            assert "date" not in self.request and "time" not in self.request
+            assert hasattr(source_or_dataset, "unique_values"), (
+                f"{source_or_dataset} (type '{type(source_or_dataset).__name__}') is"
+                " not a proper source or dataset"
+            )
+
+            return source_or_dataset.unique_values("valid_datetime")["valid_datetime"]
+
+        self.dates = find_dates(source_or_dataset)
 
         self.params = self.request["param"]
-        if not isinstance(self.params, list):
+        if not isinstance(self.params, (tuple, list)):
             self.params = [self.params]
-        self.repeat = repeat  # For ensembles
-        self.maker = ConstantMaker(source_or_dataset)
+
+        # self.numbers = self.request.get("number", [None])
+        self.numbers = find_numbers(source_or_dataset)
+        if not isinstance(self.numbers, (tuple, list)):
+            self.numbers = [self.numbers]
+
+        self.maker = ConstantMaker(field=source_or_dataset[0])
         self.procs = {param: getattr(self.maker, param) for param in self.params}
-        self._len = len(self.dates) * len(self.params) * self.repeat
+        self._len = len(self.dates) * len(self.params) * len(self.numbers)
 
         super().__init__(**kwargs)
 
     @normalize("date", "date-list")
     @normalize("time", "int-list")
     @normalize("number", "int-list")
     def _request(self, **request):
@@ -308,31 +367,30 @@
         if isinstance(n, int):
             if n < 0:
                 n = self._len + n
 
             if n >= self._len or n < 0:
                 raise IndexError(n)
 
-            date, param, repeat = index_to_coords(
-                n, (len(self.dates), len(self.params), self.repeat)
+            date, param, number = index_to_coords(
+                n, (len(self.dates), len(self.params), len(self.numbers))
             )
 
-            assert repeat == 0, "Not implemented"
-
             date = self.dates[date]
             # assert isinstance(date, datetime.datetime), (date, type(date))
-
             param = self.params[param]
+            number = self.numbers[number]
+
             return ConstantField(
+                self.maker,
                 date,
                 param,
                 self.procs[param],
-                self.maker.shape,
-                self.maker.field.metadata().geography,
-                self.array_backend,
+                number=number,
+                array_backend=self.array_backend,
             )
 
 
 class ConstantsMaskFieldList(ConstantsFieldListCore, MaskIndex):
     def __init__(self, *args, **kwargs):
         MaskIndex.__init__(self, *args, **kwargs)
         FieldList._init_from_mask(self, self)
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/dummy_source.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/dummy_source.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/ecmwf_api.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/ecmwf_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             request,
         )
 
     @normalize("param", "variable-list(mars)")
     @normalize("date", "date-list(%Y-%m-%d)")
     @normalize("area", "bounding-box(list)")
     def requests(self, **kwargs):
+        kwargs.pop("accumulation_period", None)
         split_on = kwargs.pop("split_on", None)
         if split_on is None or not isinstance(kwargs.get(split_on), (list, tuple)):
             return [kwargs]
 
         result = []
 
         for v in kwargs[split_on]:
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/ecmwf_open_data.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/ecmwf_open_data.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/empty.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/empty.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-from . import Source
 
+from earthkit.data.core.fieldlist import FieldList
 
-class EmptySource(Source):
+
+class EmptySource(FieldList):
     def ignore(self):
         # Used by multi-source
         return True
 
     def __len__(self):
         return 0
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/fdb.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/fdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,23 @@
 LOG = logging.getLogger(__name__)
 
 
 class FDBSource(Source):
     def __init__(self, *args, stream=True, **kwargs):
         super().__init__()
 
-        self._stream_kwargs = dict()
         for k in ["group_by", "batch_size"]:
             if k in kwargs:
+                raise ValueError(
+                    f"Invalid argument '{k}' for FDBSource. Deprecated since 0.8.0."
+                )
+
+        self._stream_kwargs = dict()
+        for k in ["read_all"]:
+            if k in kwargs:
                 self._stream_kwargs[k] = kwargs.pop(k)
 
         self.stream = stream
 
         self.request = {}
         for a in args:
             self.request.update(a)
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/file.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,20 @@
     def path(self, v):
         self._path_and_parts.update(v)
 
     @property
     def parts(self):
         return self._path_and_parts.parts
 
+    def batched(self, *args):
+        return self._reader.batched(*args)
+
+    def group_by(self, *args):
+        return self._reader.group_by(*args)
+
 
 class IndexedFileSource(FileSource):
     def mutate(self):
         pass
 
 
 class File(FileSource):
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/file_indexed.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/file_indexed.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/file_pattern.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/file_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/indexed.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/indexed.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/list_of_dicts.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/list_of_dicts.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/mars.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/mars.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/memory.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,14 +80,20 @@
 
     def bounding_box(self):
         return self._reader.bounding_box()
 
     def statistics(self, **kwargs):
         return self._reader.statistics(**kwargs)
 
+    def batched(self, *args):
+        return self._reader.batched(*args)
+
+    def group_by(self, *args):
+        return self._reader.group_by(*args)
+
 
 class MemorySource(MemoryBaseSource):
     def __init__(self, buf, **kwargs):
         self._buf = buf
         self._reader_ = None
 
     def mutate(self):
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/multi.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/multi.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/multi_url.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/multi_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,13 +32,13 @@
                 "url",
                 url,
                 filter=filter,
                 merger=merger,
                 force=force,
                 # Load lazily so we can do parallel downloads
                 lazily=lazily,
-                **kwargs
+                **kwargs,
             )
             for url in urls
         ]
 
         super().__init__(sources, filter=filter, merger=merger)
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/numpy_list.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/numpy_list.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/opendap.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/opendap.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/polytope.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/polytope.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,17 +65,23 @@
         request,
         stream=True,
         **kwargs,
     ) -> None:
         super().__init__()
         assert isinstance(dataset, str)
 
-        self._stream_kwargs = dict()
         for k in ["group_by", "batch_size"]:
             if k in kwargs:
+                raise ValueError(
+                    f"Invalid argument '{k}' for Polytope. Deprecated since 0.8.0."
+                )
+
+        self._stream_kwargs = dict()
+        for k in ["read_all"]:
+            if k in kwargs:
                 self._stream_kwargs[k] = kwargs.pop(k)
 
         self.stream = stream
 
         self.request = dict(dataset=dataset, request=request)
 
         # all the kwargs are passed to the client!
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/prompt.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/prompt.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/sample.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/sample.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/url.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,17 +269,17 @@
                         range_method="auto",
                         http_headers=self.prepare_headers(url),
                         fake_headers=None,
                         auth=self.auth,
                     )
                 )
 
-            from .stream import _from_source
+            from .stream import make_stream_source_from_other
 
-            return _from_source(s, **self._kwargs)
+            return make_stream_source_from_other(s, **self._kwargs)
         else:
             return super().mutate()
 
     def out_of_date(self, url, path, cache_data):
         if SETTINGS.get("check-out-of-date-urls") is False:
             return False
 
@@ -431,17 +431,17 @@
         from urllib.parse import urlparse
 
         o = urlparse(self.url)
         if o.scheme not in ("http", "https"):
             raise NotImplementedError(f"Streams are not supported for {o.scheme} urls")
 
     def mutate(self):
-        from .stream import _from_source
+        from .stream import make_stream_source_from_other
 
-        return _from_source(self, **self._kwargs)
+        return make_stream_source_from_other(self, **self._kwargs)
 
     def to_stream(self):
         downloader = Downloader(
             self.url,
             chunk_size=self.chunk_size,
             parts=self.url_parts,
             timeout=SETTINGS.get("url-download-timeout"),
```

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/url_pattern.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/url_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/virtual.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/virtual.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/virtual_directory.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/virtual_directory.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/wekeo.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/wekeo.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sources/wekeocds.py` & `earthkit_data-0.8.1/src/earthkit/data/sources/wekeocds.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sphinxext/generate_settings_rst.py` & `earthkit_data-0.8.1/src/earthkit/data/sphinxext/generate_settings_rst.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sphinxext/module_output.py` & `earthkit_data-0.8.1/src/earthkit/data/sphinxext/module_output.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/sphinxext/xref.py` & `earthkit_data-0.8.1/src/earthkit/data/sphinxext/xref.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/testing.py` & `earthkit_data-0.8.1/src/earthkit/data/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,39 @@
     pass
 
 
 _NETWORK_PATCHER = patch("socket.socket", side_effect=OfflineError)
 
 _REMOTE_TEST_DATA_URL = "https://get.ecmwf.int/repository/test-data/earthkit-data/"
 
-_ROOT_DIR = top = os.path.dirname(os.path.dirname(os.path.dirname(__file__)))
+_ROOT_DIR = top = os.path.dirname(
+    os.path.dirname(os.path.dirname(os.path.dirname(__file__)))
+)
 if not os.path.exists(os.path.join(_ROOT_DIR, "tests", "data")):
     _ROOT_DIR = "./"
 
 
 @contextmanager
 def network_off():
     try:
         _NETWORK_PATCHER.start()
         yield None
     finally:
         _NETWORK_PATCHER.stop()
 
 
+@contextmanager
+def preserve_cwd():
+    current_dir = os.getcwd()
+    try:
+        yield None
+    finally:
+        os.chdir(current_dir)
+
+
 def earthkit_remote_test_data_file(*args):
     return os.path.join(_REMOTE_TEST_DATA_URL, *args)
 
 
 def earthkit_file(*args):
     return os.path.join(_ROOT_DIR, *args)
```

### Comparing `earthkit_data-0.7.0/earthkit/data/translators/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/translators/ndarray.py` & `earthkit_data-0.8.1/src/earthkit/data/translators/ndarray.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/translators/pandas.py` & `earthkit_data-0.8.1/src/earthkit/data/translators/pandas.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,28 +28,28 @@
 
 
 class PandasDataFrameTranslator(PandasSeriesTranslator):
     """Translator class for pandas `DataFrame`"""
 
     def __call__(self):
         """
-        DataFrame requested, if Series convert to DataFrame.
+        Return DataFrame, if Series convert to DataFrame.
         """
         if isinstance(self.data, pd.Series):
             return self.data.to_frame()
 
         return self.data
 
 
 class GeoPandasDataFrameTranslator(PandasSeriesTranslator):
     """Translator class for geopandas `DataFrame`"""
 
     def __call__(self):
         """
-        GeoDataFrame requested, if normal pandas convert to geopandas.
+        Return GeoDataFrame, if normal pandas convert to geopandas.
         """
         import geopandas as gpd
 
         if isinstance(self.data, pd.DataFrame):
             return gpd.GeoDataFrame(self.data)
 
         return self.data
```

### Comparing `earthkit_data-0.7.0/earthkit/data/translators/string.py` & `earthkit_data-0.8.1/src/earthkit/data/translators/string.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/translators/xarray.py` & `earthkit_data-0.8.1/src/earthkit/data/translators/xarray.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/array/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/array/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/array/cupy.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/array/cupy.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/array/numpy.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/array/numpy.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/array/pytorch.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/array/pytorch.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/availability.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/availability.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # does it submit to any jurisdiction.
 #
 
 import io
 import itertools
 import json
 import os
+import pickle
 
 import yaml
 
+from earthkit.data.utils import load_json_or_yaml
 from earthkit.data.utils.factorise import Tree, factorise
 
 from .humanize import dict_to_human, list_to_human
 
 
 def _tidy_dict(query):
     result = dict()
@@ -43,35 +45,64 @@
 
 
 def load_yaml(avail):
     with open(avail) as f:
         return yaml.load(f, Loader=yaml.SafeLoader)
 
 
-CONFIG_LOADERS = {
-    ".json": load_json,
-    ".yaml": load_yaml,
-}
-
-
 class Availability:
     def __init__(self, avail, intervals=None, parser=None):
+        CONFIG_LOADERS = {
+            "json": load_json,
+            "yaml": load_yaml,
+            # "marslist": Availability.from_mars_list,
+            "pickle": Availability.from_pickle,
+        }
         if not isinstance(avail, Tree):
             if isinstance(avail, str):
                 config_loader = load_json
                 if len(avail) > 5:
-                    config_loader = CONFIG_LOADERS.get(avail[-5:], load_str)
+                    ext = avail[-10:].split(".")[-1]
+                    config_loader = CONFIG_LOADERS.get(ext, load_str)
                     avail = config_loader(avail)
 
             if parser is not None:
                 avail = [parser(item) for item in avail]
 
-            avail = factorise(avail, intervals=intervals)
+            if isinstance(avail, Availability):
+                avail = avail._tree
+
+            if not isinstance(avail, Tree):
+                avail = factorise(avail, intervals=intervals)
         self._tree = avail
 
+    def as_mars_list(self, *args, **kwargs):
+        return self._tree.as_mars_list(*args, **kwargs)
+
+    def as_mars(self, *args, **kwargs):
+        return self._tree.as_mars(*args, **kwargs)
+
+    def to_pickle(self, filename):
+        with open(filename, "wb") as f:
+            pickle.dump(self._tree, f)
+
+    @classmethod
+    def from_pickle(cls, filename):
+        with open(filename, "rb") as f:
+            tree = pickle.load(f)
+            return cls(tree)
+
+    def to_yaml(self):
+        return yaml.dump(self._tree)
+
+    @classmethod
+    def from_yaml(cls, filename):
+        dic = load_json_or_yaml(filename)
+        return cls(dic)
+
     @classmethod
     def from_mars_list(cls, tree, intervals=None):
         if os.path.exists(tree):
             input = open(tree)
         else:
             input = io.StringIO(tree)
 
@@ -80,36 +111,42 @@
             for a in s.split(","):
                 p, v = a.split("=")
                 r[p] = v.split("/")
             return r
 
         requests = []
         stack = []
-        last = 0
+        last = -1
         for line in input:
             line = line.rstrip()
             cnt = 0
             while len(line) > 0 and line[0] == " ":
                 line = line[1:]
                 cnt += 1
-            if cnt <= last and stack:
+            if cnt <= last:
                 requests.append(as_dict(",".join(stack)))
-            while len(stack) <= cnt:
-                stack.append(None)
-            stack[cnt] = line
+            while len(stack) > cnt:
+                stack.pop()
+            stack.append(line)
             last = cnt
 
         if stack:
             requests.append(as_dict(",".join(stack)))
 
         return cls(requests, intervals)
 
     def _repr_html_(self):
         return "<hr><pre>{}</pre><hr>".format(self.tree())
 
+    def __str__(self):
+        return self.tree()
+
+    def __repr__(self):
+        return str(self.tree())
+
     def select(self, *args, **kwargs):
         return Availability(self._tree.select(*args, **kwargs))
 
     def missing(self, *args, **kwargs):
         # assert kwargs.keys() == self.unique_values().keys(), "kwargs must contain all dimensions"
         return Availability(self._tree.missing(*args, **kwargs))
```

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/bbox.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/bbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,52 +17,52 @@
     while lon >= minimum + 360:
         lon -= 360
 
     return lon
 
 
 class BoundingBox:
-    r"""Represents a geographic bounding box.
+    r"""Represent a geographic bounding box.
 
     Parameters
     ----------
     north: number
         Northern latitude (degrees)
     west: number
         Western longitude (degrees)
     south: number
         Southern latitude (degrees)
     east: number
         Eastern longitude (degrees)
     """
 
-    def __init__(self, *, north, west, south, east):
+    def __init__(self, *, north, west, south, east, check=True):
         # Convert to float as these values may come from Numpy
         self.north = min(float(north), 90.0)
         self.south = max(float(south), -90.0)
 
         self.is_periodic_west_east = (east - west) == 360
         self.west = _normalize(float(west), -180)  # Or 0?
 
         if self.is_periodic_west_east:
             self.east = self.west + 360
         else:
             self.east = _normalize(float(east), self.west)
 
-        if self.north < self.south:
+        if self.north < self.south and check:
             raise ValueError(
                 f"Invalid bounding box, north={self.north} < south={self.south}"
             )
 
-        if self.west > self.east:
+        if self.west > self.east and check:
             raise ValueError(
                 f"Invalid bounding box, west={self.west} > east={self.east}"
             )
 
-        if self.east > self.west + 360:
+        if self.east > self.west + 360 and check:
             raise ValueError(
                 f"Invalid bounding box, east={self.east} > west={self.west}+360"
             )
 
     def __repr__(self):
         return "BoundingBox(north=%g,west=%g,south=%g,east=%g)" % (
             self.north,
@@ -248,17 +248,23 @@
         try:
             bb = gdf.crs.area_of_use.bounds
             return BoundingBox(east=bb[0], south=bb[1], west=bb[2], north=bb[3])
         except AttributeError:
             return BoundingBox.make_invalid()
 
 
-def bounding_box(obj):
+def bounding_box(obj, check=True):
     if isinstance(obj, BoundingBox):
         return obj
 
     if isinstance(obj, (list, tuple)):
-        return BoundingBox(north=obj[0], west=obj[1], south=obj[2], east=obj[3])
+        return BoundingBox(
+            north=obj[0],
+            west=obj[1],
+            south=obj[2],
+            east=obj[3],
+            check=check,
+        )
 
     obj = get_wrapper(obj)
 
     return bounding_box(obj.bounding_box())
```

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/conventions.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/conventions.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/dates.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/dates.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/examples.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/examples.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/factorise.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/factorise.py`

 * *Files 4% similar despite different names*

```diff
@@ -393,14 +393,105 @@
         if not self._values and len(self._children) == 1:
             return self._children[0]
         return self
 
     def factorise(self):
         return _factorise(list(self._flatten_tree()), intervals=self._intervals)
 
+    def as_mars(self, verb="retrieve", extra=None):
+        result = []
+        for r in self.flatten():
+            req = [verb]
+            if extra is not None:
+                req.append(extra)
+            for k, v in r.items():
+                v = [str(_) for _ in v]
+                req.append(f"{k}={'/'.join(v)}")
+            result.append(",".join(req))
+        return "\n".join(result)
+
+    def as_mars_list(self):
+        text = []
+        indent = {}
+        order = {}
+
+        def V(request, depth):
+            if not request:
+                return
+
+            if depth not in indent:
+                indent[depth] = len(indent)
+
+            text.append(" " * indent[depth])
+
+            for k in sorted(request.keys()):
+                if k not in order:
+                    order[k] = len(order)
+
+            sep = ""
+            for k, v in sorted(request.items(), key=lambda x: order[x[0]]):
+                text.append(sep)
+                text.append(k)
+                text.append("=")
+
+                if isinstance(v[0], Interval):
+                    v = [str(x) for x in v]
+
+                if len(v) == 1:
+                    text.append(v[0])
+                else:
+                    start, end = self._to_date_interval(k, v)
+                    if start is not None:
+                        text.append(f"{start}/to/{end}")
+                    else:
+                        text.append("/".join([str(_) for _ in sorted(v)]))
+                sep = ","
+            text.append("\n")
+
+        self.visit(V)
+
+        return "".join(str(x) for x in text)
+
+    def _to_date_interval(self, k, v):
+        class ReturnNoneNone(Exception):
+            pass
+
+        def parse_date(d):
+            try:
+                return datetime.datetime.strptime(d, "%Y%m%d")
+            except:  # noqa: E722
+                raise ReturnNoneNone()
+
+        try:
+            if k != "date":
+                raise ReturnNoneNone()
+
+            if len(k) < 3:
+                raise ReturnNoneNone()
+
+            start = parse_date(str(v[0]))
+            step = parse_date(str(v[1])) - start
+
+            if step != datetime.timedelta(days=1):
+                raise ReturnNoneNone()
+
+            for i in range(2, len(v)):
+                current = parse_date(str(v[i]))
+                previous = parse_date(str(v[i - 1]))
+                if current - previous != step:
+                    print(int(v[i]))
+                    print(
+                        f"expecting {previous + step} after {previous}, found {current}"
+                    )
+                    raise ReturnNoneNone()
+            return str(v[0]), str(v[-1])
+
+        except ReturnNoneNone:
+            return None, None
+
     def tree(self):
         text = []
         indent = {}
         order = {}
 
         def V(request, depth):
             if not request:
@@ -423,17 +514,21 @@
 
                 if isinstance(v[0], Interval):
                     v = [str(x) for x in v]
 
                 if len(v) == 1:
                     text.append(v[0])
                 else:
-                    text.append("[")
-                    text.append(", ".join(sorted(str(x) for x in v)))
-                    text.append("]")
+                    start, end = self._to_date_interval(k, v)
+                    if start is not None:
+                        text.append(f"{start}/to/{end}")
+                    else:
+                        text.append("[")
+                        text.append(", ".join([str(_) for _ in sorted(v)]))
+                        text.append("]")
                 sep = ", "
             text.append("\n")
 
         self.visit(V)
 
         return "".join(str(x) for x in text)
 
@@ -548,27 +643,45 @@
         Sort the columns on the number of unique values (this column.diff).
         """
         for idx in self.colidx:
             self.cols[idx].compute_differences(self.rowidx)
 
         self.colidx.sort(key=lambda a: self.cols[a])
 
+    def compare_values(self, sa, sb):
+        if isinstance(sa, tuple) and isinstance(sb, tuple):
+            for a, b in zip(sa, sb):
+                n = self.compare_values(a, b)
+                if n != 0:
+                    return n
+            return 0
+
+        if type(sa) is type(sb):
+            if sa < sb:
+                return -1
+
+            if sa > sb:
+                return 1
+
+            return 0
+
+        return self.compare_values(str(type(sa)), str(type(sb)))
+
     def compare_rows(self, a, b):
         for idx in self.colidx:
             sa = self.cols[idx].value(a)
             sb = self.cols[idx].value(b)
 
             if sa is None and sb is None:
                 continue
 
-            if sa < sb:
-                return -1
+            n = self.compare_values(sa, sb)
 
-            if sa > sb:
-                return 1
+            if n != 0:
+                return n
 
         return 0
 
     def sort_rows(self):
         self.rowidx.sort(key=cmp_to_key(self.compare_rows))
 
     def pop_singles(self):
```

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/html.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/html.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/humanize.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/humanize.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,42 @@
 
 import datetime
 import re
 from collections import defaultdict
 
 
 def bytes(n):
-    u = ["", " KiB", " MiB", " GiB", " TiB", " PiB", "EiB", "ZiB", "YiB"]
+    """
+    >>> bytes(4096)
+    '4 KiB'
+    >>> bytes(4000)
+    '3.9 KiB'
+    """
+    if n < 0:
+        sign = "-"
+        n -= 0
+    else:
+        sign = ""
+
+    u = ["", " KiB", " MiB", " GiB", " TiB", " PiB", " EiB", " ZiB", " YiB"]
+    i = 0
+    while n >= 1024:
+        n /= 1024.0
+        i += 1
+    return "%s%g%s" % (sign, int(n * 10 + 0.5) / 10.0, u[i])
+
+
+def base2(n):
+    """
+    >>> base2(4096)
+    '4K'
+    >>> base2(4000)
+    '3.9K'
+    """
+    u = ["", "K", "M", "G", "T", " P", "E", "Z", "Y"]
     i = 0
     while n >= 1024:
         n /= 1024.0
         i += 1
     return "%g%s" % (int(n * 10 + 0.5) / 10.0, u[i])
 
 
@@ -250,22 +277,22 @@
 
 def dict_to_human(query):
     lst = [f"{k}={v}" for k, v in sorted(query.items())]
 
     return list_to_human(lst)
 
 
-def list_to_human(lst):
+def list_to_human(lst, conjunction="and"):
     if not lst:
         return "??"
 
     if len(lst) > 2:
         lst = [", ".join(lst[:-1]), lst[-1]]
 
-    return " and ".join(lst)
+    return f" {conjunction} ".join(lst)
 
 
 def as_number(value, name, units, none_ok):
     if value is None and none_ok:
         return None
 
     value = str(value)
```

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/interval.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/interval.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/kwargs.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/kwargs.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import copy
 import logging
+import warnings
 
 LOG = logging.getLogger(__name__)
 
 
 def deep_update(old, new):
     # deep update, merging dictionaries
     assert isinstance(new, dict), f"Expecting a dict, but received: {new}"
@@ -29,40 +30,42 @@
     def __init__(
         self,
         user,
         default=None,
         forced=None,
         logging_owner="",
         logging_main_key="",
+        warn_non_default=True,
     ):
         if default is None:
             default = {}
 
         if forced is None:
             forced = {}
 
         kwargs = copy.deepcopy(default)
 
         for k, v in user.items():
             if k in forced and v != forced[k]:
-                LOG.warning(
+                warnings.warn(
                     (
                         f"In {logging_owner} {logging_main_key},"
                         f"ignoring attempt to override {k}={forced[k]} with {k}={v}."
                     )
                 )
                 continue
 
-            if k in default and v != default[k]:
-                LOG.warning(
-                    (
-                        f"In {logging_owner} {logging_main_key}, overriding the default value "
-                        f"({k}={default[k]}) with {k}={v} is not recommended."
+            if warn_non_default:
+                if k in default and v != default[k]:
+                    warnings.warn(
+                        (
+                            f"In {logging_owner} {logging_main_key}, overriding the default value "
+                            f"({k}={default[k]}) with {k}={v} is not recommended."
+                        )
                     )
-                )
 
             kwargs[k] = v
 
         kwargs.update(forced)
 
         super().__init__(kwargs)
```

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/lazy.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/message.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import functools
 import json
 import logging
 import os
 import threading
 import time
+from contextlib import contextmanager
 
 import eccodes
 import numpy as np
 
 from earthkit.data.core.caching import CACHE, auxiliary_cache_file
 
 LOG = logging.getLogger(__name__)
@@ -55,14 +56,18 @@
             kwargs.pop("headers_only", None)
         return kwargs
 
     @property
     def versions(self):
         return f"ecCodes: {self._version} eccodes-python: {self._py_version}"
 
+    @property
+    def version(self):
+        return self._version
+
 
 ECC_FEATURES = EccodesFeatures()
 
 
 def check_clone_kwargs(func):
     @functools.wraps(func)
     def wrapped(*args, **kwargs):
@@ -265,14 +270,31 @@
 
             return eccodes.codes_set(self._handle, name, value)
         except Exception as e:
             LOG.error("Error setting %s=%s", name, value)
             LOG.exception(e)
             raise
 
+    @contextmanager
+    def _set_tmp(self, name, new_value, restore_value):
+        try:
+            if isinstance(new_value, list):
+                yield eccodes.codes_set_array(self._handle, name, new_value)
+            else:
+                yield eccodes.codes_set(self._handle, name, new_value)
+        except Exception as e:
+            LOG.error("Error setting %s=%s", name, new_value)
+            LOG.exception(e)
+            raise
+        finally:
+            if isinstance(restore_value, list):
+                eccodes.codes_set_array(self._handle, name, restore_value)
+            else:
+                eccodes.codes_set(self._handle, name, restore_value)
+
     def write(self, f):
         eccodes.codes_write(self._handle, f)
 
     def save(self, path):
         with open(path, "wb") as f:
             self.write_to(f)
             self.path = path
```

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/metadata.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/module_inputs_wrapper.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/module_inputs_wrapper.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/parts.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/parts.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/paths.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/paths.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/patterns.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/patterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,15 +82,22 @@
                 "Invalid value '{}' for parameter '{}', expected a string".format(
                     value, name
                 )
             )
         return self.format % value
 
 
-TYPES = {"": Any, "int": Int, "float": Float, "date": Datetime, "enum": Enum}
+TYPES = {
+    "": Any,
+    "int": Int,
+    "float": Float,
+    "date": Datetime,
+    "strftime": Datetime,
+    "enum": Enum,
+}
 
 
 class Constant:
     name = None
 
     def __init__(self, value):
         self.value = value
@@ -111,25 +118,45 @@
 
     def substitute(self, params):
         if self.name not in params:
             raise ValueError("Missing parameter '{}'".format(self.name))
         return self.kind.substitute(params[self.name], self.name)
 
 
+FUNCTIONS = dict(lower=lambda s: s.lower())
+
+
+class Function:
+    def __init__(self, value):
+        functions = value.split("|")
+        self.name = functions[0]
+        self.variable = Variable(functions[0])
+        self.functions = functions[1:]
+
+    def substitute(self, params):
+        value = self.variable.substitute(params)
+        for f in self.functions:
+            value = FUNCTIONS[f](value)
+        return value
+
+
 class Pattern:
     def __init__(self, pattern, ignore_missing_keys=False):
         self.ignore_missing_keys = ignore_missing_keys
 
         self.pattern = []
         self.variables = []
         for i, p in enumerate(RE1.split(pattern)):
             if i % 2 == 0:
                 self.pattern.append(Constant(p))
             else:
-                v = Variable(p)
+                if "|" in p:
+                    v = Function(p)
+                else:
+                    v = Variable(p)
                 self.variables.append(v)
                 self.pattern.append(v)
 
     @property
     def names(self):
         return sorted({v.name for v in self.variables})
```

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/progbar.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/projections/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/projections/cf.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/projections/cf.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/projections/proj.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/projections/proj.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/serialise.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/serialise.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/summary.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/summary.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/utils/url.py` & `earthkit_data-0.8.1/src/earthkit/data/utils/url.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/vocabularies/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/vocabularies/aliases.py` & `earthkit_data-0.8.1/src/earthkit/data/vocabularies/aliases.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/vocabularies/cf.py` & `earthkit_data-0.8.1/src/earthkit/data/vocabularies/cf.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/vocabularies/grib-paramid.csv` & `earthkit_data-0.8.1/src/earthkit/data/vocabularies/grib-paramid.csv`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/vocabularies/grib.py` & `earthkit_data-0.8.1/src/earthkit/data/vocabularies/grib.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/wrappers/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/wrappers/integer.py` & `earthkit_data-0.8.1/src/earthkit/data/wrappers/integer.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/wrappers/ndarray.py` & `earthkit_data-0.8.1/src/earthkit/data/wrappers/ndarray.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/wrappers/pandas.py` & `earthkit_data-0.8.1/src/earthkit/data/wrappers/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/wrappers/string.py` & `earthkit_data-0.8.1/src/earthkit/data/wrappers/string.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,18 +33,19 @@
     return parse(dt)
 
 
 class StrWrapper(Wrapper):
     def __init__(self, data):
         self.data = data
 
-    # DEPENDANCIES NOT YET INSTALLED
-    # def bounding_box(self):
-    #     from earthkit.data.utils.domains import domain_to_area
-    #     return domain_to_area(self.data)
+    def bounding_box(self):
+        if "/" in self.data:
+            return tuple(float(x) for x in self.data.split("/"))
+        else:
+            raise ValueError(f"Invalid bounding box '{self.data}'")
 
     def datetime(self):
         return parse_date(self.data)
 
     def to_datetime(self):
         return self.datetime()
```

### Comparing `earthkit_data-0.7.0/earthkit/data/wrappers/xarray.py` & `earthkit_data-0.8.1/src/earthkit/data/wrappers/xarray.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/writers/__init__.py` & `earthkit_data-0.8.1/src/earthkit/data/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit/data/writers/grib.py` & `earthkit_data-0.8.1/src/earthkit/data/writers/grib.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/earthkit_data.egg-info/PKG-INFO` & `earthkit_data-0.8.1/src/earthkit_data.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: earthkit-data
-Version: 0.7.0
+Version: 0.8.1
 Summary: A format-agnostic Python interface for geospatial data
-License: Apache License 2.0
+Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
+License: Apache License Version 2.0
+Project-URL: Documentation, https://earthkit-data.readthedocs.io/
+Project-URL: Homepage, https://github.com/ecmwf/earthkit-data/
+Project-URL: Issues, https://github.com/ecmwf/earthkit-data.issues
+Project-URL: Repository, https://github.com/ecmwf/earthkit-data/
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cfgrib>=0.9.10.1
 Requires-Dist: eccodes>=1.7.0
 Requires-Dist: dask
 Requires-Dist: entrypoints
 Requires-Dist: filelock
@@ -27,54 +33,55 @@
 Requires-Dist: multiurl
 Requires-Dist: netcdf4
 Requires-Dist: pandas
 Requires-Dist: pdbufr>=0.11.0
 Requires-Dist: pyyaml
 Requires-Dist: tqdm>=4.63.0
 Requires-Dist: xarray>=0.19.0
+Requires-Dist: earthkit-geo>=0.2.0
 Requires-Dist: earthkit-meteo>=0.0.1
-Provides-Extra: mars
-Requires-Dist: ecmwf-api-client>=1.6.1; extra == "mars"
-Provides-Extra: cds
-Requires-Dist: cdsapi; extra == "cds"
-Provides-Extra: fdb
-Requires-Dist: pyfdb; extra == "fdb"
-Provides-Extra: polytope
-Requires-Dist: polytope-client>=0.7.4; extra == "polytope"
-Provides-Extra: wekeo
-Requires-Dist: hda; extra == "wekeo"
-Provides-Extra: ecmwf-opendata
-Requires-Dist: ecmwf-opendata>=0.3.3; extra == "ecmwf-opendata"
-Provides-Extra: odb
-Requires-Dist: pyodc; extra == "odb"
-Provides-Extra: projection
-Requires-Dist: cartopy; extra == "projection"
-Provides-Extra: geopandas
-Requires-Dist: geopandas; extra == "geopandas"
-Provides-Extra: eccovjson
-Requires-Dist: eccovjson>=0.0.5; extra == "eccovjson"
 Provides-Extra: all
 Requires-Dist: earthkit-data[mars]; extra == "all"
 Requires-Dist: earthkit-data[cds]; extra == "all"
 Requires-Dist: earthkit-data[ecmwf-opendata]; extra == "all"
 Requires-Dist: earthkit-data[fdb]; extra == "all"
 Requires-Dist: earthkit-data[polytope]; extra == "all"
 Requires-Dist: earthkit-data[wekeo]; extra == "all"
 Requires-Dist: earthkit-data[odb]; extra == "all"
 Requires-Dist: earthkit-data[projection]; extra == "all"
 Requires-Dist: earthkit-data[geopandas]; extra == "all"
 Requires-Dist: earthkit-data[eccovjson]; extra == "all"
+Provides-Extra: cds
+Requires-Dist: cdsapi; extra == "cds"
+Provides-Extra: eccovjson
+Requires-Dist: eccovjson>=0.0.5; extra == "eccovjson"
+Provides-Extra: ecmwf-opendata
+Requires-Dist: ecmwf-opendata>=0.3.3; extra == "ecmwf-opendata"
+Provides-Extra: fdb
+Requires-Dist: pyfdb; extra == "fdb"
+Provides-Extra: geopandas
+Requires-Dist: geopandas; extra == "geopandas"
+Provides-Extra: mars
+Requires-Dist: ecmwf-api-client>=1.6.1; extra == "mars"
+Provides-Extra: odb
+Requires-Dist: pyodc; extra == "odb"
+Provides-Extra: polytope
+Requires-Dist: polytope-client>=0.7.4; extra == "polytope"
+Provides-Extra: projection
+Requires-Dist: cartopy; extra == "projection"
 Provides-Extra: test
 Requires-Dist: earthkit-data[all]; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-forked; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
 Requires-Dist: nbformat; extra == "test"
 Requires-Dist: nbconvert; extra == "test"
+Provides-Extra: wekeo
+Requires-Dist: hda; extra == "wekeo"
 
 # earthkit-data
 
 <img src="docs/_static/earthkit-data.png" width="120">
 
 [![PyPI version fury.io](https://badge.fury.io/py/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
```

### Comparing `earthkit_data-0.7.0/earthkit_data.egg-info/SOURCES.txt` & `earthkit_data-0.8.1/src/earthkit_data.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 README.md
 environment.yml
 pyproject.toml
 pytest.ini
 setup.cfg
 .github/ci-config.yml
 .github/ci-hpc-config.yml
+.github/workflows/cd-pypi.yml
 .github/workflows/ci.yml
-.github/workflows/ci_other.yml
 .github/workflows/label-public-pr.yml
+.github/workflows/legacy-ci.yml
 .github/workflows/notify-new-issue.yml
 .github/workflows/notify-new-pr.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/development.rst
 docs/howtos.rst
@@ -88,14 +89,15 @@
 docs/examples/url_stream.ipynb
 docs/examples/wekeo.ipynb
 docs/guide/caching.rst
 docs/guide/data.rst
 docs/guide/index.rst
 docs/guide/settings.rst
 docs/guide/sources.rst
+docs/guide/streams.rst
 docs/guide/data_format/bufr.rst
 docs/guide/data_format/csv.rst
 docs/guide/data_format/grib.rst
 docs/guide/data_format/index.rst
 docs/guide/data_format/netcdf.rst
 docs/guide/data_format/odb.rst
 docs/guide/include/settings-get.py
@@ -111,180 +113,184 @@
 docs/release_notes/index.rst
 docs/release_notes/version_0.2_updates.rst
 docs/release_notes/version_0.3_updates.rst
 docs/release_notes/version_0.4_updates.rst
 docs/release_notes/version_0.5_updates.rst
 docs/release_notes/version_0.6_updates.rst
 docs/release_notes/version_0.7_updates.rst
-earthkit/data/__init__.py
-earthkit/data/decorators.py
-earthkit/data/testing.py
-earthkit/data/version.py
-earthkit/data/arguments/__init__.py
-earthkit/data/arguments/args_kwargs.py
-earthkit/data/arguments/argument.py
-earthkit/data/arguments/earthkit_types.py
-earthkit/data/arguments/input_manager.py
-earthkit/data/arguments/transformers.py
-earthkit/data/conf/global_grids.json
-earthkit/data/conf/gridspec.yaml
-earthkit/data/conf/gridspec_schema.json
-earthkit/data/conf/css/tab.css
-earthkit/data/conf/css/table.css
-earthkit/data/conf/css/tree.css
-earthkit/data/core/__init__.py
-earthkit/data/core/caching.py
-earthkit/data/core/constants.py
-earthkit/data/core/fieldlist.py
-earthkit/data/core/geography.py
-earthkit/data/core/gridspec.py
-earthkit/data/core/index.py
-earthkit/data/core/ipython.py
-earthkit/data/core/metadata.py
-earthkit/data/core/order.py
-earthkit/data/core/plugins.py
-earthkit/data/core/select.py
-earthkit/data/core/settings.py
-earthkit/data/core/statistics.py
-earthkit/data/core/temporary.py
-earthkit/data/core/thread.py
-earthkit/data/indexing/__init__.py
-earthkit/data/indexing/database/__init__.py
-earthkit/data/indexing/database/json.py
-earthkit/data/indexing/database/sql.py
-earthkit/data/indexing/database/stdout.py
-earthkit/data/mergers/__init__.py
-earthkit/data/mergers/pandas.py
-earthkit/data/mergers/xarray.py
-earthkit/data/mirrors/__init__.py
-earthkit/data/mirrors/directory_mirror.py
-earthkit/data/readers/__init__.py
-earthkit/data/readers/archive.py
-earthkit/data/readers/covjson.py
-earthkit/data/readers/csv.py
-earthkit/data/readers/directory.py
-earthkit/data/readers/geojson.py
-earthkit/data/readers/numpy.py
-earthkit/data/readers/odb.py
-earthkit/data/readers/shapefile.py
-earthkit/data/readers/tar.py
-earthkit/data/readers/text.py
-earthkit/data/readers/unknown.py
-earthkit/data/readers/zip.py
-earthkit/data/readers/bufr/__init__.py
-earthkit/data/readers/bufr/bufr.py
-earthkit/data/readers/bufr/pandas.py
-earthkit/data/readers/grib/__init__.py
-earthkit/data/readers/grib/codes.py
-earthkit/data/readers/grib/gridspec.py
-earthkit/data/readers/grib/memory.py
-earthkit/data/readers/grib/metadata.py
-earthkit/data/readers/grib/output.py
-earthkit/data/readers/grib/pandas.py
-earthkit/data/readers/grib/parsing.py
-earthkit/data/readers/grib/reader.py
-earthkit/data/readers/grib/xarray.py
-earthkit/data/readers/grib/index/__init__.py
-earthkit/data/readers/grib/index/db.py
-earthkit/data/readers/grib/index/file.py
-earthkit/data/readers/grib/index/json.py
-earthkit/data/readers/grib/index/sql.py
-earthkit/data/readers/netcdf/__init__.py
-earthkit/data/readers/netcdf/coords.py
-earthkit/data/readers/netcdf/dataset.py
-earthkit/data/readers/netcdf/field.py
-earthkit/data/readers/netcdf/fieldlist.py
-earthkit/data/sources/__init__.py
-earthkit/data/sources/ads.py
-earthkit/data/sources/array_list.py
-earthkit/data/sources/cds.py
-earthkit/data/sources/constants.py
-earthkit/data/sources/dummy.grib
-earthkit/data/sources/dummy_source.py
-earthkit/data/sources/ecmwf_api.py
-earthkit/data/sources/ecmwf_open_data.py
-earthkit/data/sources/empty.py
-earthkit/data/sources/fdb.py
-earthkit/data/sources/file.py
-earthkit/data/sources/file_indexed.py
-earthkit/data/sources/file_pattern.py
-earthkit/data/sources/indexed.py
-earthkit/data/sources/list_of_dicts.py
-earthkit/data/sources/mars.py
-earthkit/data/sources/memory.py
-earthkit/data/sources/multi.py
-earthkit/data/sources/multi_url.py
-earthkit/data/sources/numpy_list.py
-earthkit/data/sources/opendap.py
-earthkit/data/sources/polytope.py
-earthkit/data/sources/prompt.py
-earthkit/data/sources/sample.py
-earthkit/data/sources/stream.py
-earthkit/data/sources/url.py
-earthkit/data/sources/url_pattern.py
-earthkit/data/sources/virtual.py
-earthkit/data/sources/virtual_directory.py
-earthkit/data/sources/wekeo.py
-earthkit/data/sources/wekeocds.py
-earthkit/data/sphinxext/__init__.py
-earthkit/data/sphinxext/generate_settings_rst.py
-earthkit/data/sphinxext/module_output.py
-earthkit/data/sphinxext/xref.py
-earthkit/data/translators/__init__.py
-earthkit/data/translators/ndarray.py
-earthkit/data/translators/pandas.py
-earthkit/data/translators/string.py
-earthkit/data/translators/xarray.py
-earthkit/data/utils/__init__.py
-earthkit/data/utils/availability.py
-earthkit/data/utils/bbox.py
-earthkit/data/utils/conventions.py
-earthkit/data/utils/dates.py
-earthkit/data/utils/examples.py
-earthkit/data/utils/factorise.py
-earthkit/data/utils/html.py
-earthkit/data/utils/humanize.py
-earthkit/data/utils/interval.py
-earthkit/data/utils/kwargs.py
-earthkit/data/utils/lazy.py
-earthkit/data/utils/message.py
-earthkit/data/utils/metadata.py
-earthkit/data/utils/module_inputs_wrapper.py
-earthkit/data/utils/parts.py
-earthkit/data/utils/paths.py
-earthkit/data/utils/patterns.py
-earthkit/data/utils/progbar.py
-earthkit/data/utils/serialise.py
-earthkit/data/utils/summary.py
-earthkit/data/utils/url.py
-earthkit/data/utils/array/__init__.py
-earthkit/data/utils/array/cupy.py
-earthkit/data/utils/array/numpy.py
-earthkit/data/utils/array/pytorch.py
-earthkit/data/utils/projections/__init__.py
-earthkit/data/utils/projections/cf.py
-earthkit/data/utils/projections/proj.py
-earthkit/data/vocabularies/__init__.py
-earthkit/data/vocabularies/aliases.py
-earthkit/data/vocabularies/cf.py
-earthkit/data/vocabularies/grib-paramid.csv
-earthkit/data/vocabularies/grib.py
-earthkit/data/wrappers/__init__.py
-earthkit/data/wrappers/integer.py
-earthkit/data/wrappers/ndarray.py
-earthkit/data/wrappers/pandas.py
-earthkit/data/wrappers/string.py
-earthkit/data/wrappers/xarray.py
-earthkit/data/writers/__init__.py
-earthkit/data/writers/grib.py
-earthkit_data.egg-info/PKG-INFO
-earthkit_data.egg-info/SOURCES.txt
-earthkit_data.egg-info/dependency_links.txt
-earthkit_data.egg-info/requires.txt
-earthkit_data.egg-info/top_level.txt
+docs/release_notes/version_0.8_updates.rst
+src/earthkit/data/__init__.py
+src/earthkit/data/_version.py
+src/earthkit/data/decorators.py
+src/earthkit/data/testing.py
+src/earthkit/data/arguments/__init__.py
+src/earthkit/data/arguments/args_kwargs.py
+src/earthkit/data/arguments/argument.py
+src/earthkit/data/arguments/earthkit_types.py
+src/earthkit/data/arguments/input_manager.py
+src/earthkit/data/arguments/transformers.py
+src/earthkit/data/conf/global_grids.json
+src/earthkit/data/conf/gridspec.yaml
+src/earthkit/data/conf/gridspec_schema.json
+src/earthkit/data/conf/css/tab.css
+src/earthkit/data/conf/css/table.css
+src/earthkit/data/conf/css/tree.css
+src/earthkit/data/core/__init__.py
+src/earthkit/data/core/caching.py
+src/earthkit/data/core/constants.py
+src/earthkit/data/core/fieldlist.py
+src/earthkit/data/core/geography.py
+src/earthkit/data/core/gridspec.py
+src/earthkit/data/core/index.py
+src/earthkit/data/core/ipython.py
+src/earthkit/data/core/metadata.py
+src/earthkit/data/core/order.py
+src/earthkit/data/core/plugins.py
+src/earthkit/data/core/select.py
+src/earthkit/data/core/settings.py
+src/earthkit/data/core/statistics.py
+src/earthkit/data/core/temporary.py
+src/earthkit/data/core/thread.py
+src/earthkit/data/indexing/__init__.py
+src/earthkit/data/indexing/cube.py
+src/earthkit/data/indexing/fieldlist.py
+src/earthkit/data/indexing/database/__init__.py
+src/earthkit/data/indexing/database/json.py
+src/earthkit/data/indexing/database/sql.py
+src/earthkit/data/indexing/database/stdout.py
+src/earthkit/data/mergers/__init__.py
+src/earthkit/data/mergers/pandas.py
+src/earthkit/data/mergers/xarray.py
+src/earthkit/data/mirrors/__init__.py
+src/earthkit/data/mirrors/directory_mirror.py
+src/earthkit/data/readers/__init__.py
+src/earthkit/data/readers/archive.py
+src/earthkit/data/readers/covjson.py
+src/earthkit/data/readers/csv.py
+src/earthkit/data/readers/directory.py
+src/earthkit/data/readers/geojson.py
+src/earthkit/data/readers/numpy.py
+src/earthkit/data/readers/odb.py
+src/earthkit/data/readers/shapefile.py
+src/earthkit/data/readers/tar.py
+src/earthkit/data/readers/text.py
+src/earthkit/data/readers/unknown.py
+src/earthkit/data/readers/zip.py
+src/earthkit/data/readers/bufr/__init__.py
+src/earthkit/data/readers/bufr/bufr.py
+src/earthkit/data/readers/bufr/pandas.py
+src/earthkit/data/readers/grib/__init__.py
+src/earthkit/data/readers/grib/codes.py
+src/earthkit/data/readers/grib/file.py
+src/earthkit/data/readers/grib/gridspec.py
+src/earthkit/data/readers/grib/memory.py
+src/earthkit/data/readers/grib/metadata.py
+src/earthkit/data/readers/grib/output.py
+src/earthkit/data/readers/grib/pandas.py
+src/earthkit/data/readers/grib/parsing.py
+src/earthkit/data/readers/grib/xarray.py
+src/earthkit/data/readers/grib/index/__init__.py
+src/earthkit/data/readers/grib/index/db.py
+src/earthkit/data/readers/grib/index/file.py
+src/earthkit/data/readers/grib/index/json.py
+src/earthkit/data/readers/grib/index/sql.py
+src/earthkit/data/readers/netcdf/__init__.py
+src/earthkit/data/readers/netcdf/coords.py
+src/earthkit/data/readers/netcdf/dataset.py
+src/earthkit/data/readers/netcdf/field.py
+src/earthkit/data/readers/netcdf/fieldlist.py
+src/earthkit/data/sources/__init__.py
+src/earthkit/data/sources/ads.py
+src/earthkit/data/sources/array_list.py
+src/earthkit/data/sources/cds.py
+src/earthkit/data/sources/constants.py
+src/earthkit/data/sources/dummy.grib
+src/earthkit/data/sources/dummy_source.py
+src/earthkit/data/sources/ecmwf_api.py
+src/earthkit/data/sources/ecmwf_open_data.py
+src/earthkit/data/sources/empty.py
+src/earthkit/data/sources/fdb.py
+src/earthkit/data/sources/file.py
+src/earthkit/data/sources/file_indexed.py
+src/earthkit/data/sources/file_pattern.py
+src/earthkit/data/sources/indexed.py
+src/earthkit/data/sources/list_of_dicts.py
+src/earthkit/data/sources/mars.py
+src/earthkit/data/sources/memory.py
+src/earthkit/data/sources/multi.py
+src/earthkit/data/sources/multi_url.py
+src/earthkit/data/sources/numpy_list.py
+src/earthkit/data/sources/opendap.py
+src/earthkit/data/sources/polytope.py
+src/earthkit/data/sources/prompt.py
+src/earthkit/data/sources/sample.py
+src/earthkit/data/sources/stream.py
+src/earthkit/data/sources/url.py
+src/earthkit/data/sources/url_pattern.py
+src/earthkit/data/sources/virtual.py
+src/earthkit/data/sources/virtual_directory.py
+src/earthkit/data/sources/wekeo.py
+src/earthkit/data/sources/wekeocds.py
+src/earthkit/data/sphinxext/__init__.py
+src/earthkit/data/sphinxext/generate_settings_rst.py
+src/earthkit/data/sphinxext/module_output.py
+src/earthkit/data/sphinxext/xref.py
+src/earthkit/data/translators/__init__.py
+src/earthkit/data/translators/ndarray.py
+src/earthkit/data/translators/pandas.py
+src/earthkit/data/translators/string.py
+src/earthkit/data/translators/xarray.py
+src/earthkit/data/utils/__init__.py
+src/earthkit/data/utils/availability.py
+src/earthkit/data/utils/batch.py
+src/earthkit/data/utils/bbox.py
+src/earthkit/data/utils/conventions.py
+src/earthkit/data/utils/dates.py
+src/earthkit/data/utils/examples.py
+src/earthkit/data/utils/factorise.py
+src/earthkit/data/utils/html.py
+src/earthkit/data/utils/humanize.py
+src/earthkit/data/utils/interval.py
+src/earthkit/data/utils/kwargs.py
+src/earthkit/data/utils/lazy.py
+src/earthkit/data/utils/message.py
+src/earthkit/data/utils/metadata.py
+src/earthkit/data/utils/module_inputs_wrapper.py
+src/earthkit/data/utils/parts.py
+src/earthkit/data/utils/paths.py
+src/earthkit/data/utils/patterns.py
+src/earthkit/data/utils/progbar.py
+src/earthkit/data/utils/serialise.py
+src/earthkit/data/utils/summary.py
+src/earthkit/data/utils/url.py
+src/earthkit/data/utils/array/__init__.py
+src/earthkit/data/utils/array/cupy.py
+src/earthkit/data/utils/array/numpy.py
+src/earthkit/data/utils/array/pytorch.py
+src/earthkit/data/utils/projections/__init__.py
+src/earthkit/data/utils/projections/cf.py
+src/earthkit/data/utils/projections/proj.py
+src/earthkit/data/vocabularies/__init__.py
+src/earthkit/data/vocabularies/aliases.py
+src/earthkit/data/vocabularies/cf.py
+src/earthkit/data/vocabularies/grib-paramid.csv
+src/earthkit/data/vocabularies/grib.py
+src/earthkit/data/wrappers/__init__.py
+src/earthkit/data/wrappers/integer.py
+src/earthkit/data/wrappers/ndarray.py
+src/earthkit/data/wrappers/pandas.py
+src/earthkit/data/wrappers/string.py
+src/earthkit/data/wrappers/xarray.py
+src/earthkit/data/writers/__init__.py
+src/earthkit/data/writers/grib.py
+src/earthkit_data.egg-info/PKG-INFO
+src/earthkit_data.egg-info/SOURCES.txt
+src/earthkit_data.egg-info/dependency_links.txt
+src/earthkit_data.egg-info/requires.txt
+src/earthkit_data.egg-info/top_level.txt
 tests/conftest.py
 tests/downstream-ci-requirements.txt
 tests/environment-unit-tests.yml
 tests/test_00_version.py
 tests/array_fieldlist/array_fl_fixtures.py
 tests/array_fieldlist/test_numpy_fl_write.py
 tests/array_fieldlist/test_numpy_fs.py
@@ -315,23 +321,28 @@
 tests/data/empty_file.grib
 tests/data/era5_2t_1.nc
 tests/data/era5_2t_2.nc
 tests/data/hovexp_vert_area.nc
 tests/data/mercator.grib
 tests/data/ml_data.grib
 tests/data/rgg_small_subarea_cellarea_ref.grib
+tests/data/rotated_N32_subarea.grib
+tests/data/rotated_wind_20x20.grib
 tests/data/t_pl.grib
 tests/data/t_time_series.grib
+tests/data/test4.nc
+tests/data/test6.nc
 tests/data/test_icon.grib
 tests/data/test_single.grib
 tests/data/test_single.nc
 tests/data/test_single_with_missing.grib
 tests/data/time_series.covjson
 tests/data/u_pl.grib
 tests/data/v_pl.grib
+tests/data/wind_20x20.grib
 tests/data/constants/proc.yaml
 tests/data/gridspec/healpix.yaml
 tests/data/gridspec/reduced_gg.yaml
 tests/data/gridspec/reduced_ll.yaml
 tests/data/gridspec/reduced_rotated_gg.yaml
 tests/data/gridspec/regular_gg.yaml
 tests/data/gridspec/regular_ll.yaml
@@ -341,18 +352,20 @@
 tests/data/gridspec/t_75_-60_10_40_5x5.grib1
 tests/documentation/test_examples.py
 tests/documentation/test_notebooks.py
 tests/grib/grib_fixtures.py
 tests/grib/test_grib_backend.py
 tests/grib/test_grib_concat.py
 tests/grib/test_grib_convert.py
+tests/grib/test_grib_cube.py
 tests/grib/test_grib_file_parts.py
 tests/grib/test_grib_geography.py
 tests/grib/test_grib_gridspec.py
 tests/grib/test_grib_inidces.py
+tests/grib/test_grib_iter.py
 tests/grib/test_grib_memory.py
 tests/grib/test_grib_metadata.py
 tests/grib/test_grib_order_by.py
 tests/grib/test_grib_output.py
 tests/grib/test_grib_sel.py
 tests/grib/test_grib_slice.py
 tests/grib/test_grib_stream.py
@@ -367,14 +380,15 @@
 tests/indexing/test_indexing_serialisation.py
 tests/indexing/test_order_kwargs.py
 tests/indexing/test_selection_kwargs.py
 tests/netcdf/test_netcdf_concat.py
 tests/netcdf/test_netcdf_convert.py
 tests/netcdf/test_netcdf_fieldlist.py
 tests/netcdf/test_netcdf_geography.py
+tests/netcdf/test_netcdf_iter.py
 tests/netcdf/test_netcdf_metadata.py
 tests/netcdf/test_netcdf_opendap.py
 tests/netcdf/test_netcdf_output.py
 tests/netcdf/test_netcdf_sel.py
 tests/netcdf/test_netcdf_slice.py
 tests/netcdf/test_netcdf_summary.py
 tests/netcdf/test_netcdf_values.py
```

### Comparing `earthkit_data-0.7.0/earthkit_data.egg-info/requires.txt` & `earthkit_data-0.8.1/src/earthkit_data.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 multiurl
 netcdf4
 pandas
 pdbufr>=0.11.0
 pyyaml
 tqdm>=4.63.0
 xarray>=0.19.0
+earthkit-geo>=0.2.0
 earthkit-meteo>=0.0.1
 
 [all]
 earthkit-data[mars]
 earthkit-data[cds]
 earthkit-data[ecmwf-opendata]
 earthkit-data[fdb]
```

### Comparing `earthkit_data-0.7.0/environment.yml` & `earthkit_data-0.8.1/environment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 - pip:
   - multiurl
   - git+https://github.com/ecmwf/pyfdb
   - ecmwf-opendata>=0.1.2
   - polytope-client>=0.7.4
   - earthkit-meteo>=0.0.1
   - eccovjson>=0.0.5
-  - earthkit-geo
+  - earthkit-geo>=0.2.0
 - tqdm>=4.63.0
 - markdown
 - make
 - mypy
 - myst-parser
 - pre-commit
 - pydata-sphinx-theme
```

### Comparing `earthkit_data-0.7.0/pytest.ini` & `earthkit_data-0.8.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/array_fieldlist/array_fl_fixtures.py` & `earthkit_data-0.8.1/tests/array_fieldlist/array_fl_fixtures.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fl_write.py` & `earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fl_write.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs.py` & `earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fs.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_concat.py` & `earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fs_concat.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_metadata.py` & `earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fs_metadata.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/array_fieldlist/test_numpy_fs_summary.py` & `earthkit_data-0.8.1/tests/array_fieldlist/test_numpy_fs_summary.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/bufr/test_bufr_concat.py` & `earthkit_data-0.8.1/tests/bufr/test_bufr_concat.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/bufr/test_bufr_contents.py` & `earthkit_data-0.8.1/tests/bufr/test_bufr_contents.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/bufr/test_bufr_convert.py` & `earthkit_data-0.8.1/tests/bufr/test_bufr_convert.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/bufr/test_bufr_file_parts.py` & `earthkit_data-0.8.1/tests/bufr/test_bufr_file_parts.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/bufr/test_bufr_order_by.py` & `earthkit_data-0.8.1/tests/bufr/test_bufr_order_by.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/bufr/test_bufr_sel.py` & `earthkit_data-0.8.1/tests/bufr/test_bufr_sel.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/bufr/test_bufr_summary.py` & `earthkit_data-0.8.1/tests/bufr/test_bufr_summary.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/conftest.py` & `earthkit_data-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/constants/constants_fixtures.py` & `earthkit_data-0.8.1/tests/constants/constants_fixtures.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/constants/test_constants_metadata.py` & `earthkit_data-0.8.1/tests/constants/test_constants_metadata.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/constants/test_constants_sel.py` & `earthkit_data-0.8.1/tests/constants/test_constants_sel.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/constants/test_constants_slice.py` & `earthkit_data-0.8.1/tests/constants/test_constants_slice.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,15 +69,19 @@
 
     # check the original fieldlist
     assert len(ds) == num
 
 
 @pytest.mark.parametrize(
     "indexes1,indexes2",
-    [(np.array([1, 16, 5, 9]), np.array([1, 3])), ([1, 16, 5, 9], [1, 3])],
+    [
+        (np.array([1, 16, 5, 9]), np.array([1, 3])),
+        ([1, 16, 5, 9], [1, 3]),
+        ((1, 16, 5, 9), (1, 3)),
+    ],
 )
 def test_constants_array_indexing(indexes1, indexes2):
     ds, md = load_constants_fs()
 
     # first subset
     r = ds[indexes1]
     ref_md = [md[i] for i in indexes1]
@@ -89,15 +93,23 @@
     r1 = r[indexes2]
     ref_md = [ref_md[i] for i in indexes2]
     ref_num = len(ref_md)
     assert len(r1) == ref_num
     assert r1.metadata(["valid_datetime", "param"]) == ref_md
 
 
-@pytest.mark.parametrize("indexes", [(np.array([1, 96, 5, 9])), ([1, 96, 5, 9])])
+@pytest.mark.skip(reason="Index range checking disabled")
+@pytest.mark.parametrize(
+    "indexes",
+    [
+        (np.array([1, 96, 5, 9])),
+        ([1, 16, 5, 9], [1, 3]),
+        ((1, 16, 5, 9), (1, 3)),
+    ],
+)
 def test_constants_array_indexing_bad(indexes):
     ds, _ = load_constants_fs()
     with pytest.raises(IndexError):
         ds[indexes]
 
 
 def test_constants_fieldlist_iterator():
```

### Comparing `earthkit_data-0.7.0/tests/constants/test_constants_source.py` & `earthkit_data-0.8.1/tests/constants/test_constants_source.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/constants/test_constants_values.py` & `earthkit_data-0.8.1/tests/constants/test_constants_values.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/constants/test_contants_proc.py` & `earthkit_data-0.8.1/tests/constants/test_contants_proc.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/core/test_cache.py` & `earthkit_data-0.8.1/tests/core/test_cache.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/core/test_gridspec.py` & `earthkit_data-0.8.1/tests/core/test_gridspec.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/core/test_metadata.py` & `earthkit_data-0.8.1/tests/core/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-import datetime
-
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.metadata import RawMetadata
 from earthkit.data.readers.grib.metadata import GribMetadata
 from earthkit.data.testing import earthkit_examples_file, earthkit_test_data_file
 
@@ -162,15 +160,15 @@
         md.get("centre", "shortName", "step")
 
 
 def test_grib_grib_metadata_valid_datetime():
     ds = from_source("file", earthkit_test_data_file("t_time_series.grib"))
     md = ds[4].metadata()
 
-    assert md["valid_datetime"] == datetime.datetime(2020, 12, 21, 18)
+    assert md["valid_datetime"] == "2020-12-21T18:00:00"
 
 
 def test_grib_metadata_override():
     ds = from_source("file", earthkit_examples_file("test.grib"))
     md = ds[0].metadata()
 
     md2 = md.override({"perturbationNumber": 5})
```

### Comparing `earthkit_data-0.7.0/tests/core/test_settings.py` & `earthkit_data-0.8.1/tests/core/test_settings.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/core/test_version.py` & `earthkit_data-0.8.1/tests/core/test_version.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/NUTS_RG_20M_2021_3035.geojson` & `earthkit_data-0.8.1/tests/data/NUTS_RG_20M_2021_3035.geojson`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/NUTS_RG_20M_2021_3035.shp.zip` & `earthkit_data-0.8.1/tests/data/NUTS_RG_20M_2021_3035.shp.zip`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/constants/proc.yaml` & `earthkit_data-0.8.1/tests/data/constants/proc.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/era5_2t_1.nc` & `earthkit_data-0.8.1/tests/data/era5_2t_1.nc`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/era5_2t_2.nc` & `earthkit_data-0.8.1/tests/data/era5_2t_2.nc`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/healpix.yaml` & `earthkit_data-0.8.1/tests/data/gridspec/healpix.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/reduced_gg.yaml` & `earthkit_data-0.8.1/tests/data/gridspec/reduced_gg.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/reduced_ll.yaml` & `earthkit_data-0.8.1/tests/data/gridspec/reduced_ll.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/reduced_rotated_gg.yaml` & `earthkit_data-0.8.1/tests/data/gridspec/reduced_rotated_gg.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/regular_gg.yaml` & `earthkit_data-0.8.1/tests/data/gridspec/regular_gg.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/regular_ll.yaml` & `earthkit_data-0.8.1/tests/data/gridspec/regular_ll.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/rotated_gg.yaml` & `earthkit_data-0.8.1/tests/data/gridspec/rotated_gg.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/rotated_ll.yaml` & `earthkit_data-0.8.1/tests/data/gridspec/rotated_ll.yaml`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/gridspec/t_75_-60_10_40_5x5.grib1` & `earthkit_data-0.8.1/tests/data/gridspec/t_75_-60_10_40_5x5.grib1`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/hovexp_vert_area.nc` & `earthkit_data-0.8.1/tests/data/hovexp_vert_area.nc`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/mercator.grib` & `earthkit_data-0.8.1/tests/data/mercator.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/ml_data.grib` & `earthkit_data-0.8.1/tests/data/ml_data.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/rgg_small_subarea_cellarea_ref.grib` & `earthkit_data-0.8.1/tests/data/rgg_small_subarea_cellarea_ref.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/t_pl.grib` & `earthkit_data-0.8.1/tests/data/t_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/t_time_series.grib` & `earthkit_data-0.8.1/tests/data/t_time_series.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/test_icon.grib` & `earthkit_data-0.8.1/tests/data/test_icon.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/test_single.nc` & `earthkit_data-0.8.1/tests/data/test_single.nc`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/time_series.covjson` & `earthkit_data-0.8.1/tests/data/time_series.covjson`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/u_pl.grib` & `earthkit_data-0.8.1/tests/data/u_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/data/v_pl.grib` & `earthkit_data-0.8.1/tests/data/v_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/documentation/test_examples.py` & `earthkit_data-0.8.1/tests/documentation/test_examples.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/documentation/test_notebooks.py` & `earthkit_data-0.8.1/tests/documentation/test_notebooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "ads.ipynb",
     "wekeo.ipynb",
     "polytope.ipynb",
     "grib_fdb_write.ipynb",
     "demo_source_plugin.ipynb",
     "ecmwf_open_data.ipynb",
     "shapefile.ipynb",
+    "netcdf_opendap.ipynb",
 ]
 
 if NO_PYTORCH:
     SKIP.append("grib_array_backends.ipynb")
 
 
 def notebooks_list():
```

### Comparing `earthkit_data-0.7.0/tests/environment-unit-tests.yml` & `earthkit_data-0.8.1/tests/environment-unit-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   - multiurl
   - git+https://github.com/ecmwf/pyfdb
   - ecmwf-opendata>=0.3.3
   - polytope-client>=0.7.4
   - earthkit-meteo>=0.0.1
   - git+https://github.com/ecmwf/earthkit-data-demo-source
   - eccovjson>=0.0.5
-  - earthkit-geo
+  - earthkit-geo>=0.2.0
 - tqdm>=4.63.0
 - markdown
 - make
 - mypy
 - myst-parser
 - pre-commit
 - pydata-sphinx-theme
```

### Comparing `earthkit_data-0.7.0/tests/grib/grib_fixtures.py` & `earthkit_data-0.8.1/tests/grib/grib_fixtures.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_backend.py` & `earthkit_data-0.8.1/tests/grib/test_grib_backend.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_concat.py` & `earthkit_data-0.8.1/tests/grib/test_grib_concat.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_convert.py` & `earthkit_data-0.8.1/tests/grib/test_grib_convert.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_file_parts.py` & `earthkit_data-0.8.1/tests/grib/test_grib_file_parts.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_gridspec.py` & `earthkit_data-0.8.1/tests/grib/test_grib_gridspec.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_inidces.py` & `earthkit_data-0.8.1/tests/grib/test_grib_inidces.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_memory.py` & `earthkit_data-0.8.1/tests/grib/test_grib_memory.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_metadata.py` & `earthkit_data-0.8.1/tests/grib/test_grib_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,15 @@
 
 @pytest.mark.parametrize("fl_type", FL_TYPES)
 @pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 def test_grib_valid_datetime(fl_type, array_backend):
     ds = load_grib_data("t_time_series.grib", fl_type, array_backend, folder="data")
     f = ds[4]
 
-    assert f.metadata("valid_datetime") == datetime.datetime(2020, 12, 21, 18)
+    assert f.metadata("valid_datetime") == "2020-12-21T18:00:00"
 
 
 @pytest.mark.parametrize("fl_type", ["file"])
 @pytest.mark.parametrize("array_backend", [None])
 def test_message(fl_type, array_backend):
     f = load_grib_data("test.grib", fl_type, array_backend)
     v = f[0].message()
```

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_order_by.py` & `earthkit_data-0.8.1/tests/grib/test_grib_order_by.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-import datetime
 import os
 import sys
 
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.testing import ARRAY_BACKENDS
@@ -182,20 +181,35 @@
 def test_grib_order_by_valid_datetime(fl_type, array_backend):
     f = load_grib_data("t_time_series.grib", fl_type, array_backend, folder="data")
 
     g = f.order_by(valid_datetime="descending")
     assert len(g) == 10
 
     ref = [
-        datetime.datetime(2020, 12, 23, 12, 0),
-        datetime.datetime(2020, 12, 23, 12, 0),
-        datetime.datetime(2020, 12, 21, 21, 0),
-        datetime.datetime(2020, 12, 21, 21, 0),
-        datetime.datetime(2020, 12, 21, 18, 0),
-        datetime.datetime(2020, 12, 21, 18, 0),
-        datetime.datetime(2020, 12, 21, 15, 0),
-        datetime.datetime(2020, 12, 21, 15, 0),
-        datetime.datetime(2020, 12, 21, 12, 0),
-        datetime.datetime(2020, 12, 21, 12, 0),
+        "2020-12-23T12:00:00",
+        "2020-12-23T12:00:00",
+        "2020-12-21T21:00:00",
+        "2020-12-21T21:00:00",
+        "2020-12-21T18:00:00",
+        "2020-12-21T18:00:00",
+        "2020-12-21T15:00:00",
+        "2020-12-21T15:00:00",
+        "2020-12-21T12:00:00",
+        "2020-12-21T12:00:00",
     ]
 
     assert g.metadata("valid_datetime") == ref
+
+
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_order_by_remapping(fl_type, array_backend):
+    ds = load_grib_data("test6.grib", fl_type, array_backend)
+
+    ordering = ["t850", "t1000", "u1000", "v850", "v1000", "u850"]
+    ref = [("t", 850), ("t", 1000), ("u", 1000), ("v", 850), ("v", 1000), ("u", 850)]
+
+    r = ds.order_by(
+        param_level=ordering, remapping={"param_level": "{param}{levelist}"}
+    )
+
+    assert r.metadata("param", "level") == ref
```

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_output.py` & `earthkit_data-0.8.1/tests/grib/test_grib_output.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_sel.py` & `earthkit_data-0.8.1/tests/grib/test_grib_sel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-import datetime
 import os
 import sys
 
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
@@ -194,15 +193,15 @@
 
 
 @pytest.mark.parametrize("fl_type", FL_TYPES)
 @pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 def test_grib_sel_valid_datetime(fl_type, array_backend):
     f = load_grib_data("t_time_series.grib", fl_type, array_backend, folder="data")
 
-    g = f.sel(valid_datetime=datetime.datetime(2020, 12, 21, 21))
+    g = f.sel(valid_datetime="2020-12-21T21:00:00")
     assert len(g) == 2
 
     ref_keys = ["shortName", "date", "time", "step"]
     ref = [
         ["t", 20201221, 1200, 9],
         ["z", 20201221, 1200, 9],
     ]
@@ -337,11 +336,31 @@
     assert len(g) == 2
     assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [
         ["t", 81, "hybrid"],
         ["t", 85, "hybrid"],
     ]
 
 
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_sel_remapping_1(fl_type, array_backend):
+    ds = load_grib_data("test6.grib", fl_type, array_backend)
+    ref = [("t", 850)]
+    r = ds.sel(param_level="t850", remapping={"param_level": "{param}{levelist}"})
+    assert r.metadata("param", "level") == ref
+
+
+@pytest.mark.parametrize("fl_type", FL_TYPES)
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_sel_remapping_2(fl_type, array_backend):
+    ds = load_grib_data("test6.grib", fl_type, array_backend)
+    ref = [("u", 1000), ("t", 850)]
+    r = ds.sel(
+        param_level=["t850", "u1000"], remapping={"param_level": "{param}{levelist}"}
+    )
+    assert r.metadata("param", "level") == ref
+
+
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main()
```

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_slice.py` & `earthkit_data-0.8.1/tests/grib/test_grib_slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,31 +104,43 @@
     assert f.metadata("shortName") == ["2t", "msl", "t", "z", "t", "z"]
 
 
 @pytest.mark.parametrize("fl_type", FL_TYPES)
 @pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
 @pytest.mark.parametrize(
     "indexes1,indexes2",
-    [(np.array([1, 16, 5, 9]), np.array([1, 3])), ([1, 16, 5, 9], [1, 3])],
+    [
+        (np.array([1, 16, 5, 9]), np.array([1, 3])),
+        ([1, 16, 5, 9], [1, 3]),
+        ((1, 16, 5, 9), (1, 3)),
+    ],
 )
 def test_grib_array_indexing(fl_type, array_backend, indexes1, indexes2):
     f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
 
     r = f[indexes1]
     assert len(r) == 4
     assert r.metadata("shortName") == ["u", "u", "v", "t"]
 
     r1 = r[indexes2]
     assert len(r1) == 2
     assert r1.metadata("shortName") == ["u", "t"]
 
 
+@pytest.mark.skip(reason="Index range checking disabled")
 @pytest.mark.parametrize("fl_type", FL_TYPES)
 @pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
-@pytest.mark.parametrize("indexes", [(np.array([1, 19, 5, 9])), ([1, 19, 5, 9])])
+@pytest.mark.parametrize(
+    "indexes",
+    [
+        (np.array([1, 19, 5, 9])),
+        ([1, 16, 5, 9], [1, 3]),
+        ((1, 16, 5, 9), (1, 3)),
+    ],
+)
 def test_grib_array_indexing_bad(fl_type, array_backend, indexes):
     f = load_grib_data("tuv_pl.grib", fl_type, array_backend)
     with pytest.raises(IndexError):
         f[indexes]
 
 
 @pytest.mark.parametrize("fl_type", FL_TYPES)
```

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_stream.py` & `earthkit_data-0.8.1/tests/grib/test_grib_stream.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,122 +10,44 @@
 #
 
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_file
+from earthkit.data.sources.stream import StreamFieldList
 from earthkit.data.testing import ARRAY_BACKENDS, earthkit_examples_file
 
 
 def repeat_list_items(items, count):
     return sum([[x] * count for x in items], [])
 
 
-@pytest.mark.parametrize(
-    "_kwargs,error",
-    [
-        # (dict(order_by="level"), TypeError),
-        (dict(group_by=1), TypeError),
-        (dict(group_by=["level", 1]), TypeError),
-        # (dict(group_by="level", batch_size=1), TypeError),
-        (dict(batch_size=-1), ValueError),
-    ],
-)
-def test_grib_from_stream_invalid_args(_kwargs, error):
-    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        with pytest.raises(error):
-            from_source("stream", stream, **_kwargs)
-
-
-@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
-@pytest.mark.parametrize(
-    "_kwargs",
-    [
-        {"group_by": "level"},
-        {"group_by": "level", "batch_size": 0},
-        {"group_by": "level", "batch_size": 1},
-        {"group_by": ["level", "gridType"]},
-    ],
-)
-def test_grib_from_stream_group_by(array_backend, _kwargs):
-    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        fs = from_source("stream", stream, **_kwargs, array_backend=array_backend)
-
-        # no methods are available
-        with pytest.raises(TypeError):
-            len(fs)
-
-        ref = [
-            [("t", 1000), ("u", 1000), ("v", 1000)],
-            [("t", 850), ("u", 850), ("v", 850)],
-        ]
-        for i, f in enumerate(fs):
-            assert len(f) == 3
-            assert f.metadata(("param", "level")) == ref[i]
-            afl = f.to_fieldlist(array_backend=array_backend)
-            assert afl is not f
-            assert len(afl) == 3
-
-        # stream consumed, no data is available
-        assert sum([1 for _ in fs]) == 0
+# @pytest.mark.parametrize(
+#     "_kwargs,error",
+#     [
+#         # (dict(order_by="level"), TypeError),
+#         (dict(group_by=1), TypeError),
+#         (dict(group_by=["level", 1]), TypeError),
+#         # (dict(group_by="level", batch_size=1), TypeError),
+#         (dict(batch_size=-1), ValueError),
+#     ],
+# )
+# def test_grib_from_stream_invalid_args(_kwargs, error):
+#     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+#         with pytest.raises(error):
+#             from_source("stream", stream, **_kwargs)
 
 
-@pytest.mark.parametrize(
-    "convert_kwargs,expected_shape",
-    [
-        ({}, (3, 7, 12)),
-        (None, (3, 7, 12)),
-        (None, (3, 7, 12)),
-        ({"flatten": False}, (3, 7, 12)),
-        ({"flatten": True}, (3, 84)),
-    ],
-)
-def test_grib_from_stream_group_by_convert_to_numpy(convert_kwargs, expected_shape):
-    group_by = "level"
+def test_grib_from_stream_iter():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        ds = from_source("stream", stream, group_by=group_by)
-
-        # no fieldlist methods are available on a StreamSource
-        with pytest.raises(TypeError):
-            len(ds)
-
-        ref = [
-            [("t", 1000), ("u", 1000), ("v", 1000)],
-            [("t", 850), ("u", 850), ("v", 850)],
-        ]
-
-        if convert_kwargs is None:
-            convert_kwargs = {}
-
-        for i, f in enumerate(ds):
-            df = f.to_fieldlist(array_backend="numpy", **convert_kwargs)
-            assert len(df) == 3
-            assert df.metadata(("param", "level")) == ref[i]
-            assert df._array.shape == expected_shape
-            assert df.to_numpy(**convert_kwargs).shape == expected_shape
-            assert df.to_fieldlist(array_backend="numpy", **convert_kwargs) is df
-
-        # stream consumed, no data is available
-        assert sum([1 for _ in ds]) == 0
-
-
-@pytest.mark.parametrize(
-    "_kwargs",
-    [
-        {},
-        {"batch_size": 1},
-    ],
-)
-def test_grib_from_stream_single_batch(_kwargs):
-    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        ds = from_source("stream", stream, **_kwargs)
+        ds = from_source("stream", stream)
 
         # no fieldlist methods are available
-        with pytest.raises(TypeError):
+        with pytest.raises((TypeError, NotImplementedError)):
             len(ds)
 
         ref = [
             ("t", 1000),
             ("u", 1000),
             ("v", 1000),
             ("t", 850),
@@ -136,30 +58,47 @@
         for i, f in enumerate(ds):
             assert f.metadata(("param", "level")) == ref[i], i
 
         # stream consumed, no data is available
         assert sum([1 for _ in ds]) == 0
 
 
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+def test_grib_from_stream_fieldlist_backend(array_backend):
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        ds = from_source("stream", stream, array_backend=array_backend)
+
+        assert isinstance(ds, StreamFieldList)
+
+        assert ds.array_backend.name == array_backend
+        assert ds.to_array().shape == (6, 7, 12)
+
+        assert sum([1 for _ in ds]) == 0
+
+        with pytest.raises((RuntimeError, ValueError)):
+            ds.to_array()
+
+
 @pytest.mark.parametrize(
     "_kwargs,expected_meta",
     [
-        ({"batch_size": 3}, [["t", "u", "v"], ["t", "u", "v"]]),
-        ({"batch_size": 4}, [["t", "u", "v", "t"], ["u", "v"]]),
+        ({"n": 1}, [["t"], ["u"], ["v"], ["t"], ["u"], ["v"]]),
+        ({"n": 3}, [["t", "u", "v"], ["t", "u", "v"]]),
+        ({"n": 4}, [["t", "u", "v", "t"], ["u", "v"]]),
     ],
 )
-def test_grib_from_stream_multi_batch(_kwargs, expected_meta):
+def test_grib_from_stream_batched(_kwargs, expected_meta):
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        ds = from_source("stream", stream, **_kwargs)
+        ds = from_source("stream", stream)
 
         # no methods are available
-        with pytest.raises(TypeError):
+        with pytest.raises((TypeError, NotImplementedError)):
             len(ds)
 
-        for i, f in enumerate(ds):
+        for i, f in enumerate(ds.batched(_kwargs["n"])):
             assert len(f) == len(expected_meta[i])
             f.metadata("param") == expected_meta[i]
 
         # stream consumed, no data is available
         assert sum([1 for _ in ds]) == 0
 
 
@@ -175,68 +114,127 @@
             (
                 2,
                 84,
             ),
         ),
     ],
 )
-def test_grib_from_stream_multi_batch_convert_to_numpy(convert_kwargs, expected_shape):
+def test_grib_from_stream_batched_convert_to_numpy(convert_kwargs, expected_shape):
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        ds = from_source("stream", stream, batch_size=2)
+        ds = from_source("stream", stream)
 
         ref = [
             [("t", 1000), ("u", 1000)],
             [("v", 1000), ("t", 850)],
             [("u", 850), ("v", 850)],
         ]
 
         if convert_kwargs is None:
             convert_kwargs = {}
 
-        for i, f in enumerate(ds):
+        for i, f in enumerate(ds.batched(2)):
             df = f.to_fieldlist(array_backend="numpy", **convert_kwargs)
             assert df.metadata(("param", "level")) == ref[i], i
             assert df._array.shape == expected_shape, i
             assert df.to_numpy(**convert_kwargs).shape == expected_shape, i
             assert df.to_fieldlist(array_backend="numpy", **convert_kwargs) is df, i
 
         # stream consumed, no data is available
         assert sum([1 for _ in ds]) == 0
 
 
+@pytest.mark.parametrize("array_backend", ARRAY_BACKENDS)
+@pytest.mark.parametrize("group", ["level", ["level", "gridType"]])
+def test_grib_from_stream_group_by(array_backend, group):
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        ds = from_source("stream", stream, array_backend=array_backend)
+
+        # no methods are available
+        with pytest.raises((TypeError, NotImplementedError)):
+            len(ds)
+
+        ref = [
+            [("t", 1000), ("u", 1000), ("v", 1000)],
+            [("t", 850), ("u", 850), ("v", 850)],
+        ]
+        for i, f in enumerate(ds.group_by(group)):
+            assert len(f) == 3
+            assert f.metadata(("param", "level")) == ref[i]
+            afl = f.to_fieldlist(array_backend=array_backend)
+            assert afl is not f
+            assert len(afl) == 3
+
+        # stream consumed, no data is available
+        assert sum([1 for _ in ds]) == 0
+
+
+@pytest.mark.parametrize(
+    "convert_kwargs,expected_shape",
+    [
+        ({}, (3, 7, 12)),
+        (None, (3, 7, 12)),
+        (None, (3, 7, 12)),
+        ({"flatten": False}, (3, 7, 12)),
+        ({"flatten": True}, (3, 84)),
+    ],
+)
+def test_grib_from_stream_group_by_convert_to_numpy(convert_kwargs, expected_shape):
+    group = "level"
+    with open(earthkit_examples_file("test6.grib"), "rb") as stream:
+        ds = from_source("stream", stream)
+
+        # no fieldlist methods are available on a StreamSource
+        with pytest.raises((TypeError, NotImplementedError)):
+            len(ds)
+
+        ref = [
+            [("t", 1000), ("u", 1000), ("v", 1000)],
+            [("t", 850), ("u", 850), ("v", 850)],
+        ]
+
+        if convert_kwargs is None:
+            convert_kwargs = {}
+
+        for i, f in enumerate(ds.group_by(group)):
+            df = f.to_fieldlist(array_backend="numpy", **convert_kwargs)
+            assert len(df) == 3
+            assert df.metadata(("param", "level")) == ref[i]
+            assert df._array.shape == expected_shape
+            assert df.to_numpy(**convert_kwargs).shape == expected_shape
+            assert df.to_fieldlist(array_backend="numpy", **convert_kwargs) is df
+
+        # stream consumed, no data is available
+        assert sum([1 for _ in ds]) == 0
+
+
 def test_grib_from_stream_in_memory():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
         ds = from_source(
             "stream",
             stream,
-            batch_size=0,
+            read_all=True,
         )
 
         assert len(ds) == 6
 
         expected_shape = (6, 7, 12)
         md_ref = [
             ("t", 1000),
             ("u", 1000),
             ("v", 1000),
             ("t", 850),
             ("u", 850),
             ("v", 850),
         ]
-        val = []
 
         # iteration
-        for f in ds:
-            v = f.metadata(("param", "level"))
-            val.append(v)
-
+        val = [f.metadata(("param", "level")) for f in ds]
         assert val == md_ref, "iteration"
 
         # metadata
-        val = []
         val = ds.metadata(("param", "level"))
         assert val == md_ref, "method"
 
         # data
         assert ds.to_numpy().shape == expected_shape
 
         ref = np.array(
@@ -279,36 +277,27 @@
         ({}, (6, 7, 12)),
         ({"flatten": False}, (6, 7, 12)),
         ({"flatten": True}, (6, 84)),
     ],
 )
 def test_grib_from_stream_in_memory_convert_to_numpy(convert_kwargs, expected_shape):
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        ds_s = from_source(
-            "stream",
-            stream,
-            batch_size=0,
-        )
+        ds_s = from_source("stream", stream, read_all=True)
 
         ds = ds_s.to_fieldlist(array_backend="numpy", **convert_kwargs)
 
         assert len(ds) == 6
 
         ref = ["t", "u", "v", "t", "u", "v"]
-        val = []
 
         # iteration
-        for f in ds:
-            v = f.metadata("param")
-            val.append(v)
-
+        val = [f.metadata("param") for f in ds]
         assert val == ref, "iteration"
 
         # metadata
-        val = []
         val = ds.metadata("param")
         assert val == ref, "method"
 
         # data
         assert ds.to_numpy(**convert_kwargs).shape == expected_shape
 
         ref = np.array(
@@ -330,19 +319,143 @@
         assert np.allclose(vals, ref)
         assert ds._array.shape == expected_shape
         assert ds.to_fieldlist(array_backend="numpy", **convert_kwargs) is ds
 
 
 def test_grib_save_when_loaded_from_stream():
     with open(earthkit_examples_file("test6.grib"), "rb") as stream:
-        fs = from_source("stream", stream, batch_size=0)
+        fs = from_source("stream", stream, read_all=True)
         assert len(fs) == 6
         with temp_file() as tmp:
             fs.save(tmp)
             fs_saved = from_source("file", tmp)
             assert len(fs) == len(fs_saved)
 
 
+def test_grib_multi_from_stream_iter():
+    stream1 = open(earthkit_examples_file("test.grib"), "rb")
+    stream2 = open(earthkit_examples_file("test4.grib"), "rb")
+    ds = from_source("stream", [stream1, stream2])
+
+    assert isinstance(ds, StreamFieldList)
+
+    # no fieldlist methods are available
+    with pytest.raises((TypeError, NotImplementedError)):
+        len(ds)
+
+    ref = [
+        ("2t", 0),
+        ("msl", 0),
+        ("t", 500),
+        ("z", 500),
+        ("t", 850),
+        ("z", 850),
+    ]
+
+    for i, f in enumerate(ds):
+        assert f.metadata(("param", "level")) == ref[i], i
+
+    # stream consumed, no data is available
+    assert sum([1 for _ in ds]) == 0
+
+
+@pytest.mark.parametrize(
+    "_kwargs,expected_meta",
+    [
+        ({"n": 1}, [["2t"], ["msl"], ["t"], ["z"], ["t"], ["z"]]),
+        ({"n": 2}, [["2t", "msl"], ["t", "z"], ["t", "z"]]),
+        ({"n": 3}, [["2t", "msl", "t"], ["z", "t", "z"]]),
+        ({"n": 4}, [["2t", "msl", "t", "z"], ["t", "z"]]),
+    ],
+)
+def test_grib_multi_grib_from_stream_batched(_kwargs, expected_meta):
+    stream1 = open(earthkit_examples_file("test.grib"), "rb")
+    stream2 = open(earthkit_examples_file("test4.grib"), "rb")
+    ds = from_source("stream", [stream1, stream2])
+
+    assert isinstance(ds, StreamFieldList)
+
+    # no methods are available
+    with pytest.raises((TypeError, NotImplementedError)):
+        len(ds)
+
+    cnt = 0
+    for i, f in enumerate(ds.batched(_kwargs["n"])):
+        assert len(f) == len(expected_meta[i])
+        f.metadata("param") == expected_meta[i]
+        cnt += 1
+
+    assert cnt == len(expected_meta)
+
+    # stream consumed, no data is available
+    assert sum([1 for _ in ds]) == 0
+
+
+def test_grib_multi_stream_memory():
+    stream1 = open(earthkit_examples_file("test.grib"), "rb")
+    stream2 = open(earthkit_examples_file("test4.grib"), "rb")
+    ds = from_source("stream", [stream1, stream2], read_all=True)
+
+    assert len(ds) == 6
+
+    md_ref = [
+        ("2t", 0),
+        ("msl", 0),
+        ("t", 500),
+        ("z", 500),
+        ("t", 850),
+        ("z", 850),
+    ]
+    # iteration
+    val = [f.metadata(("param", "level")) for f in ds]
+    assert val == md_ref, "iteration"
+
+    # metadata
+    val = ds.metadata(("param", "level"))
+    assert val == md_ref, "method"
+
+    # data
+    with pytest.raises(ValueError):
+        ds.to_numpy().shape
+
+    # first part
+    expected_shape = (2, 11, 19)
+    assert ds[0:2].to_numpy().shape == expected_shape
+
+    ref = np.array([262.78027344, 101947.8125])
+
+    vals = ds[0:2].to_numpy()[:, 0, 0]
+    assert np.allclose(vals, ref)
+
+    # second part
+    expected_shape = (4, 181, 360)
+    assert ds[2:].to_numpy().shape == expected_shape
+
+    ref = np.array([228.04600525, 48126.859375, 246.61032104, 11786.1132812])
+
+    vals = ds[2:].to_numpy()[:, 0, 0]
+    assert np.allclose(vals, ref)
+
+    # slicing
+    r = ds[0:3]
+    assert len(r) == 3
+    val = r.metadata(("param", "level"))
+    assert val == md_ref[0:3]
+
+    r = ds[-2:]
+    assert len(r) == 2
+    val = r.metadata(("param", "level"))
+    assert val == md_ref[-2:]
+
+    r = ds.sel(param="t")
+    assert len(r) == 2
+    val = r.metadata(("param", "level"))
+    assert val == [
+        ("t", 500),
+        ("t", 850),
+    ]
+
+
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main()
```

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_summary.py` & `earthkit_data-0.8.1/tests/grib/test_grib_summary.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_url.py` & `earthkit_data-0.8.1/tests/grib/test_grib_url.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_url_stream.py` & `earthkit_data-0.8.1/tests/grib/test_grib_url_stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,96 +10,69 @@
 #
 
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_file
+from earthkit.data.sources.stream import StreamFieldList
 from earthkit.data.testing import earthkit_remote_test_data_file
 
 
 def repeat_list_items(items, count):
     return sum([[x] * count for x in items], [])
 
 
-@pytest.mark.parametrize(
-    "_kwargs,error",
-    [
-        # (dict(order_by="level"), TypeError),
-        (dict(group_by=1), TypeError),
-        (dict(group_by=["level", 1]), TypeError),
-        # (dict(group_by="level", batch_size=1), TypeError),
-        (dict(batch_size=-1), ValueError),
-    ],
-)
-def test_grib_url_stream_invalid_args(_kwargs, error):
-    with pytest.raises(error):
-        from_source(
-            "url",
-            earthkit_remote_test_data_file("examples/test6.grib"),
-            stream=True,
-            **_kwargs,
-        )
-
-
-@pytest.mark.parametrize(
-    "_kwargs",
-    [
-        {"group_by": "level"},
-        {"group_by": "level", "batch_size": 0},
-        {"group_by": "level", "batch_size": 1},
-        {"group_by": ["level", "gridType"]},
-    ],
-)
-def test_grib_url_stream_group_by(_kwargs):
-    fs = from_source(
-        "url",
-        earthkit_remote_test_data_file("examples/test6.grib"),
-        stream=True,
-        **_kwargs,
-    )
-
-    # no methods are available
-    with pytest.raises(TypeError):
-        len(fs)
-
-    ref = [
-        [("t", 1000), ("u", 1000), ("v", 1000)],
-        [("t", 850), ("u", 850), ("v", 850)],
-    ]
-    cnt = 0
-    for i, f in enumerate(fs):
-        assert len(f) == 3
-        assert f.metadata(("param", "level")) == ref[i]
-        assert f.to_fieldlist(array_backend="numpy") is not f
-        cnt += 1
-
-    assert cnt == len(ref)
-
-    # stream consumed, no data is available
-    assert sum([1 for _ in fs]) == 0
-
-
-@pytest.mark.parametrize(
-    "_kwargs",
-    [
-        {},
-        {"batch_size": 1},
-    ],
-)
-def test_grib_url_stream_single_batch(_kwargs):
+# @pytest.mark.parametrize(
+#     "_kwargs,error",
+#     [
+#         # (dict(order_by="level"), TypeError),
+#         (dict(group_by=1), TypeError),
+#         (dict(group_by=["level", 1]), TypeError),
+#         # (dict(group_by="level", batch_size=1), TypeError),
+#         (dict(batch_size=-1), ValueError),
+#     ],
+# )
+# def test_grib_url_stream_invalid_args(_kwargs, error):
+#     with pytest.raises(error):
+#         from_source(
+#             "url",
+#             earthkit_remote_test_data_file("examples/test6.grib"),
+#             stream=True,
+#             **_kwargs,
+#         )
+
+
+# @pytest.mark.parametrize(
+#     "_kwargs",
+#     [
+#         {"group_by": "level"},
+#         {"group_by": "level", "batch_size": 0},
+#         {"group_by": "level", "batch_size": 1},
+#         {"group_by": ["level", "gridType"]},
+#     ],
+# )
+
+
+# @pytest.mark.parametrize(
+#     "_kwargs",
+#     [
+#         {},
+#         {"batch_size": 1},
+#     ],
+# )
+def test_grib_url_stream_iter():
     ds = from_source(
         "url",
         earthkit_remote_test_data_file("examples/test6.grib"),
         stream=True,
-        **_kwargs,
     )
 
     # no fieldlist methods are available
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, NotImplementedError)):
         len(ds)
 
     ref = [
         ("t", 1000),
         ("u", 1000),
         ("v", 1000),
         ("t", 850),
@@ -116,65 +89,87 @@
     # stream consumed, no data is available
     assert sum([1 for _ in ds]) == 0
 
 
 @pytest.mark.parametrize(
     "_kwargs,expected_meta",
     [
-        ({"batch_size": 3}, [["t", "u", "v"], ["t", "u", "v"]]),
-        ({"batch_size": 4}, [["t", "u", "v", "t"], ["u", "v"]]),
+        ({"n": 1}, [["t"], ["u"], ["v"], ["t"], ["u"], ["v"]]),
+        ({"n": 3}, [["t", "u", "v"], ["t", "u", "v"]]),
+        ({"n": 4}, [["t", "u", "v", "t"], ["u", "v"]]),
     ],
 )
-def test_grib_url_stream_multi_batch(_kwargs, expected_meta):
+def test_grib_from_stream_batched(_kwargs, expected_meta):
     ds = from_source(
         "url",
         earthkit_remote_test_data_file("examples/test6.grib"),
         stream=True,
-        **_kwargs,
     )
 
     # no methods are available
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, NotImplementedError)):
         len(ds)
 
     cnt = 0
-    for i, f in enumerate(ds):
+    for i, f in enumerate(ds.batched(_kwargs["n"])):
         assert len(f) == len(expected_meta[i])
         f.metadata("param") == expected_meta[i]
         cnt += 1
 
     assert cnt == len(expected_meta)
 
     # stream consumed, no data is available
     assert sum([1 for _ in ds]) == 0
 
 
+@pytest.mark.parametrize("group", ["level", ["level", "gridType"]])
+def test_grib_url_stream_group_by(group):
+    ds = from_source(
+        "url", earthkit_remote_test_data_file("examples/test6.grib"), stream=True
+    )
+
+    # no methods are available
+    with pytest.raises((TypeError, NotImplementedError)):
+        len(ds)
+
+    ref = [
+        [("t", 1000), ("u", 1000), ("v", 1000)],
+        [("t", 850), ("u", 850), ("v", 850)],
+    ]
+    cnt = 0
+    for i, f in enumerate(ds.group_by(group)):
+        assert len(f) == 3
+        assert f.metadata(("param", "level")) == ref[i]
+        assert f.to_fieldlist(array_backend="numpy") is not f
+        cnt += 1
+
+    assert cnt == len(ref)
+
+    # stream consumed, no data is available
+    assert sum([1 for _ in ds]) == 0
+
+
 def test_grib_url_stream_in_memory():
     ds = from_source(
         "url",
         earthkit_remote_test_data_file("examples/test6.grib"),
         stream=True,
-        batch_size=0,
+        read_all=True,
     )
 
     assert len(ds) == 6
 
     expected_shape = (6, 7, 12)
     ref = ["t", "u", "v", "t", "u", "v"]
-    val = []
 
     # iteration
-    for f in ds:
-        v = f.metadata("param")
-        val.append(v)
-
+    val = [f.metadata(("param")) for f in ds]
     assert val == ref, "iteration"
 
     # metadata
-    val = []
     val = ds.metadata("param")
     assert val == ref, "method"
 
     # data
     assert ds.to_numpy().shape == expected_shape
 
     ref = np.array(
@@ -193,43 +188,49 @@
 
 
 def test_grib_save_when_loaded_from_url_stream():
     ds = from_source(
         "url",
         earthkit_remote_test_data_file("examples/test6.grib"),
         stream=True,
-        batch_size=0,
+        read_all=True,
     )
     assert len(ds) == 6
     with temp_file() as tmp:
         ds.save(tmp)
         ds_saved = from_source("file", tmp)
         assert len(ds) == len(ds_saved)
 
 
-@pytest.mark.parametrize(
-    "_kwargs",
-    [
-        {},
-        {"batch_size": 1},
-    ],
-)
-def test_grib_multi_url_stream_single_batch(_kwargs):
+# @pytest.mark.parametrize(
+#     "_kwargs",
+#     [
+#         {},
+#         {"batch_size": 1},
+#     ],
+# )
+def test_grib_multi_url_stream_iter():
     ds = from_source(
         "url",
         [
             earthkit_remote_test_data_file("examples/test.grib"),
             earthkit_remote_test_data_file("examples/test4.grib"),
         ],
         stream=True,
-        **_kwargs,
     )
 
+    assert isinstance(ds, StreamFieldList)
+    assert len(ds._source.sources) == 2
+    assert ds._source._status() == [
+        {"reader": True, "stream": True},
+        {"reader": False, "stream": False},
+    ]
+
     # no fieldlist methods are available
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, NotImplementedError)):
         len(ds)
 
     ref = [
         ("2t", 0),
         ("msl", 0),
         ("t", 500),
         ("z", 500),
@@ -242,40 +243,45 @@
         cnt += 1
 
     assert cnt == len(ref)
 
     # stream consumed, no data is available
     assert sum([1 for _ in ds]) == 0
 
+    assert ds._source._status() == [
+        {"reader": True, "stream": True},
+        {"reader": True, "stream": True},
+    ]
+
 
 @pytest.mark.parametrize(
     "_kwargs,expected_meta",
     [
-        ({"batch_size": 2}, [["2t", "msl"], ["t", "z"], ["t", "z"]]),
-        ({"batch_size": 3}, [["2t", "msl", "t"], ["z", "t", "z"]]),
-        ({"batch_size": 4}, [["2t", "msl", "t", "z"], ["t", "z"]]),
+        ({"n": 1}, [["2t"], ["msl"], ["t"], ["z"], ["t"], ["z"]]),
+        ({"n": 2}, [["2t", "msl"], ["t", "z"], ["t", "z"]]),
+        ({"n": 3}, [["2t", "msl", "t"], ["z", "t", "z"]]),
+        ({"n": 4}, [["2t", "msl", "t", "z"], ["t", "z"]]),
     ],
 )
-def test_grib_multi_url_stream_batch(_kwargs, expected_meta):
+def test_grib_multi_url_stream_batched(_kwargs, expected_meta):
     ds = from_source(
         "url",
         [
             earthkit_remote_test_data_file("examples/test.grib"),
             earthkit_remote_test_data_file("examples/test4.grib"),
         ],
         stream=True,
-        **_kwargs,
     )
 
     # no methods are available
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, NotImplementedError)):
         len(ds)
 
     cnt = 0
-    for i, f in enumerate(ds):
+    for i, f in enumerate(ds.batched(_kwargs["n"])):
         assert len(f) == len(expected_meta[i])
         f.metadata("param") == expected_meta[i]
         cnt += 1
 
     assert cnt == len(expected_meta)
 
     # stream consumed, no data is available
@@ -286,39 +292,32 @@
     ds = from_source(
         "url",
         [
             earthkit_remote_test_data_file("examples/test.grib"),
             earthkit_remote_test_data_file("examples/test4.grib"),
         ],
         stream=True,
-        batch_size=0,
+        read_all=True,
     )
 
     assert len(ds) == 6
 
     md_ref = [
         ("2t", 0),
         ("msl", 0),
         ("t", 500),
         ("z", 500),
         ("t", 850),
         ("z", 850),
     ]
-
-    val = []
-
     # iteration
-    for f in ds:
-        v = f.metadata(("param", "level"))
-        val.append(v)
-
+    val = [f.metadata(("param", "level")) for f in ds]
     assert val == md_ref, "iteration"
 
     # metadata
-    val = []
     val = ds.metadata(("param", "level"))
     assert val == md_ref, "method"
 
     # data
     with pytest.raises(ValueError):
         ds.to_numpy().shape
 
@@ -381,15 +380,15 @@
         "url",
         earthkit_remote_test_data_file(path),
         parts=parts,
         stream=True,
     )
 
     # no fieldlist methods are available
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, NotImplementedError)):
         len(ds)
 
     cnt = 0
     for i, f in enumerate(ds):
         assert f.metadata(("param", "level")) == expected_meta[i], i
         cnt += 1
 
@@ -413,15 +412,15 @@
     ds = from_source(
         "url",
         [earthkit_remote_test_data_file("examples/test6.grib"), parts],
         stream=True,
     )
 
     # no fieldlist methods are available
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, NotImplementedError)):
         len(ds)
 
     cnt = 0
     for i, f in enumerate(ds):
         assert f.metadata(("param", "level")) == expected_meta[i], i
         cnt += 1
 
@@ -481,15 +480,15 @@
             [earthkit_remote_test_data_file("examples/test6.grib"), parts1],
             [earthkit_remote_test_data_file("examples/test.grib"), parts2],
         ],
         stream=True,
     )
 
     # no fieldlist methods are available
-    with pytest.raises(TypeError):
+    with pytest.raises((TypeError, NotImplementedError)):
         len(ds)
 
     cnt = 0
     for i, f in enumerate(ds):
         assert f.metadata(("param", "level")) == expected_meta[i], i
         cnt += 1
```

### Comparing `earthkit_data-0.7.0/tests/grib/test_grib_values.py` & `earthkit_data-0.8.1/tests/grib/test_grib_values.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/indexing/indexing_fixtures.py` & `earthkit_data-0.8.1/tests/indexing/indexing_fixtures.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/indexing/test_indexing_db.py` & `earthkit_data-0.8.1/tests/indexing/test_indexing_db.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/indexing/test_indexing_isel.py` & `earthkit_data-0.8.1/tests/indexing/test_indexing_isel.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/indexing/test_indexing_order_by.py` & `earthkit_data-0.8.1/tests/indexing/test_indexing_order_by.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/indexing/test_indexing_serialisation.py` & `earthkit_data-0.8.1/tests/indexing/test_indexing_serialisation.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/indexing/test_order_kwargs.py` & `earthkit_data-0.8.1/tests/indexing/test_order_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/indexing/test_selection_kwargs.py` & `earthkit_data-0.8.1/tests/indexing/test_selection_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_concat.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_concat.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_convert.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_convert.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_fieldlist.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_fieldlist.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_geography.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_geography.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_metadata.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,14 @@
     }
     assert ds.datetime() == ref
 
 
 @pytest.mark.parametrize("mode", ["nc", "xr"])
 def test_netcdf_valid_datetime(mode):
     ds = load_nc_or_xr_source(earthkit_examples_file("test.nc"), mode)
-    assert ds[0].metadata("valid_datetime") == datetime.datetime(2020, 5, 13, 12)
+    assert ds[0].metadata("valid_datetime") == "2020-05-13T12:00:00"
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main()
```

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_opendap.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_opendap.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_output.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_output.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_slice.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_slice.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,30 +92,42 @@
     assert len(f) == 2 + 18
     assert f.metadata("shortName") == ["2t", "msl", "t", "z", "t", "z"]
 
 
 @pytest.mark.parametrize("mode", ["nc", "xr"])
 @pytest.mark.parametrize(
     "indexes1,indexes2",
-    [(np.array([1, 16, 5, 9]), np.array([1, 3])), ([1, 16, 5, 9], [1, 3])],
+    [
+        (np.array([1, 16, 5, 9]), np.array([1, 3])),
+        ([1, 16, 5, 9], [1, 3]),
+        ((1, 16, 5, 9), (1, 3)),
+    ],
 )
 def test_netcdf_array_indexing(mode, indexes1, indexes2):
     f = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
 
     r = f[indexes1]
     assert len(r) == 4
     assert r.metadata("variable") == ["t", "v", "t", "u"]
 
     r1 = r[indexes2]
     assert len(r1) == 2
     assert r1.metadata("variable") == ["v", "u"]
 
 
+@pytest.mark.skip(reason="Index range checking disabled")
 @pytest.mark.parametrize("mode", ["nc", "xr"])
-@pytest.mark.parametrize("indexes", [(np.array([1, 19, 5, 9])), ([1, 19, 5, 9])])
+@pytest.mark.parametrize(
+    "indexes",
+    [
+        (np.array([1, 19, 5, 9])),
+        ([1, 16, 5, 9], [1, 3]),
+        ((1, 16, 5, 9), (1, 3)),
+    ],
+)
 def test_netcdf_array_indexing_bad(mode, indexes):
     f = load_nc_or_xr_source(earthkit_examples_file("tuv_pl.nc"), mode)
     with pytest.raises(IndexError):
         f[indexes]
 
 
 @pytest.mark.parametrize("mode", ["nc", "xr"])
```

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_summary.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_summary.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
-import datetime
-
 import pytest
 
 from earthkit.data.testing import earthkit_examples_file, load_nc_or_xr_source
 
 
 @pytest.mark.parametrize("mode", ["nc", "xr"])
 def test_netcdf_ls(mode):
@@ -23,34 +21,34 @@
     f1 = f[:4]
     df = f1.ls()
 
     ref = {
         "variable": {0: "t", 1: "t", 2: "t", 3: "t"},
         "level": {0: 1000, 1: 850, 2: 700, 3: 500},
         "valid_datetime": {
-            0: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
-            1: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
-            2: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
-            3: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
+            0: "2018-08-01T12:00:00",
+            1: "2018-08-01T12:00:00",
+            2: "2018-08-01T12:00:00",
+            3: "2018-08-01T12:00:00",
         },
         "units": {0: "K", 1: "K", 2: "K", 3: "K"},
     }
 
     assert ref == df.to_dict()
 
     # extra keys
     f1 = f[:2]
     df = f1.ls(extra_keys=["long_name"])
 
     ref = {
         "variable": {0: "t", 1: "t"},
         "level": {0: 1000, 1: 850},
         "valid_datetime": {
-            0: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
-            1: datetime.datetime.fromisoformat("2018-08-01 12:00:00"),
+            0: "2018-08-01T12:00:00",
+            1: "2018-08-01T12:00:00",
         },
         "units": {0: "K", 1: "K"},
         "long_name": {0: "Temperature", 1: "Temperature"},
     }
     assert ref == df.to_dict()
```

### Comparing `earthkit_data-0.7.0/tests/netcdf/test_netcdf_values.py` & `earthkit_data-0.8.1/tests/netcdf/test_netcdf_values.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_aliases.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_aliases.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_aliases_grib.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_aliases_grib.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_availability.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_availability.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_bbox.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_bbox.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_date.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_date.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_enum.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_enum.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_errors.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_errors.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_kwargs.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_normalize_parameter.py` & `earthkit_data-0.8.1/tests/normalize/test_normalize_parameter.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/normalize/test_transformers.py` & `earthkit_data-0.8.1/tests/normalize/test_transformers.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/plugins/test_sources_plugin.py` & `earthkit_data-0.8.1/tests/plugins/test_sources_plugin.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_covjson_reader.py` & `earthkit_data-0.8.1/tests/readers/test_covjson_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,27 +40,28 @@
 
 @pytest.mark.skipif(NO_ECCOVJSON, reason="no eccovjson available")
 def test_covjson_stream():
     stream = open(earthkit_test_data_file("time_series.covjson"), "rb")
 
     ds = from_source("stream", stream)
     assert ds
-    c = next(ds)
+    it = iter(ds)
+    c = next(it)
     a = c.to_xarray()
     assert len(a.data_vars) == 1
 
     with pytest.raises(StopIteration):
-        next(ds)
+        next(it)
 
 
 @pytest.mark.skipif(NO_ECCOVJSON, reason="no eccovjson available")
 def test_covjson_stream_memory():
     stream = open(earthkit_test_data_file("time_series.covjson"), "rb")
 
-    ds = from_source("stream", stream, batch_size=0)
+    ds = from_source("stream", stream, read_all=True)
     assert ds
     a = ds.to_xarray()
     assert len(a.data_vars) == 1
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
```

### Comparing `earthkit_data-0.7.0/tests/readers/test_csv_reader.py` & `earthkit_data-0.8.1/tests/readers/test_csv_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     df = s.to_pandas()
     assert len(df) == 3
     assert list(df.columns) == ["a", "b", "c"]
 
     ds = s.to_xarray()
     assert len(ds) == 3
-    assert list(ds.variables) == ["index", "a", "b", "c"]
+    assert set(ds.variables) == set(["index", "a", "b", "c"])
 
 
 def test_csv_2():
     s = from_source(
         "dummy-source",
         "csv",
         headers=["a", "b", "c"],
@@ -47,15 +47,15 @@
             [4, 5, 6],
             [7, 8, 9],
         ],
     )
 
     df = s.to_pandas()
     assert len(df) == 3
-    assert list(df.columns) == ["a", "b", "c"]
+    assert set(df.columns) == set(["a", "b", "c"])
 
 
 def test_csv_3():
     s = from_source(
         "dummy-source",
         "csv",
         headers=["a", "b", "c"],
@@ -64,15 +64,15 @@
             [4, "y", 6],
             [7, "z", 9],
         ],
     )
 
     df = s.to_pandas()
     assert len(df) == 3
-    assert list(df.columns) == ["a", "b", "c"]
+    assert set(df.columns) == set(["a", "b", "c"])
 
 
 def test_csv_4():
     s = from_source(
         "dummy-source",
         "csv",
         headers=["a", "b", "c"],
@@ -82,15 +82,15 @@
             [4, "y", 6],
             [7, "z", 9],
         ],
     )
 
     df = s.to_pandas()
     assert len(df) == 3
-    assert list(df.columns) == ["a", "b", "c"]
+    assert set(df.columns) == set(["a", "b", "c"])
 
 
 def test_csv_5():
     s = from_source(
         "dummy-source",
         "csv",
         headers=["a", "b", "c"],
@@ -137,15 +137,15 @@
             [7, "z", 9],
         ],
         extension=".txt",
     )
 
     df = s.to_pandas()
     assert len(df) == 3
-    assert list(df.columns) == ["a", "b", "c"]
+    assert set(df.columns) == set(["a", "b", "c"])
 
 
 def test_csv_with_comment():
     s = from_source(
         "dummy-source",
         "csv",
         headers=["a", "b", "c"],
@@ -156,19 +156,19 @@
             [7, "z", 9],
         ],
         comment_line="This is a comment",
     )
 
     df = s.to_pandas()
     assert len(df) == 3
-    assert list(df.columns) == ["a", "b", "c"]
+    assert set(df.columns) == set(["a", "b", "c"])
 
     ds = s.to_xarray()
     assert len(ds) == 3
-    assert list(ds.variables) == ["index", "a", "b", "c"]
+    assert set(ds.variables) == set(["index", "a", "b", "c"])
 
 
 def test_csv_mimetypes():
     assert mimetypes.guess_type("x.csv") == ("text/csv", None)
     assert mimetypes.guess_type("x.csv.gz") == ("text/csv", "gzip")
     assert mimetypes.guess_type("x.csv.bz2") == ("text/csv", "bzip2")
```

### Comparing `earthkit_data-0.7.0/tests/readers/test_empty_file.py` & `earthkit_data-0.8.1/tests/readers/test_empty_file.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_geojson_reader.py` & `earthkit_data-0.8.1/tests/readers/test_geojson_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_grib_reader.py` & `earthkit_data-0.8.1/tests/readers/test_grib_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_netcdf_reader.py` & `earthkit_data-0.8.1/tests/readers/test_netcdf_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_odb_reader.py` & `earthkit_data-0.8.1/tests/readers/test_odb_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_reader_padding_bytes.py` & `earthkit_data-0.8.1/tests/readers/test_reader_padding_bytes.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_shapefile_reader.py` & `earthkit_data-0.8.1/tests/readers/test_shapefile_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_tar_reader.py` & `earthkit_data-0.8.1/tests/readers/test_tar_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_unknown_reader.py` & `earthkit_data-0.8.1/tests/readers/test_unknown_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/readers/test_zip_reader.py` & `earthkit_data-0.8.1/tests/readers/test_zip_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_ads.py` & `earthkit_data-0.8.1/tests/sources/test_ads.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_cds.py` & `earthkit_data-0.8.1/tests/sources/test_cds.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import os
 
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_directory
-from earthkit.data.testing import NO_CDS
+from earthkit.data.testing import NO_CDS, preserve_cwd
 
 CDS_TIMEOUT = pytest.CDS_TIMEOUT
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
@@ -176,19 +176,18 @@
         product_type="reanalysis",
         area=[50, -50, 20, 50],
         date="2012-12-12",
         time="12:00",
     )
     with temp_directory() as tmpdir:
         # Check file can be saved in current dir with detected filename:
-        here = os.curdir
-        os.chdir(tmpdir)
-        s.save()
-        assert os.path.isfile(os.path.basename(s.source_filename))
-        os.chdir(here)
+        with preserve_cwd():
+            os.chdir(tmpdir)
+            s.save()
+            assert os.path.isfile(os.path.basename(s.source_filename))
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
 @pytest.mark.timeout(CDS_TIMEOUT)
 @pytest.mark.parametrize(
@@ -296,19 +295,18 @@
         date="2012-12-12",
         time="12:00",
         format="netcdf",
     )
 
     with temp_directory() as tmpdir:
         # Check file can be saved in current dir with detected filename:
-        here = os.curdir
-        os.chdir(tmpdir)
-        s.save()
-        assert os.path.isfile(os.path.basename(s.source_filename))
-        os.chdir(here)
+        with preserve_cwd():
+            os.chdir(tmpdir)
+            s.save()
+            assert os.path.isfile(os.path.basename(s.source_filename))
 
 
 @pytest.mark.long_test
 @pytest.mark.download
 @pytest.mark.skipif(NO_CDS, reason="No access to CDS")
 @pytest.mark.timeout(60)
 def test_cds_netcdf_selection_limited():
```

### Comparing `earthkit_data-0.7.0/tests/sources/test_ecmwf_open_data.py` & `earthkit_data-0.8.1/tests/sources/test_ecmwf_open_data.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_fdb.py` & `earthkit_data-0.8.1/tests/sources/test_fdb.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_file.py` & `earthkit_data-0.8.1/tests/sources/test_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,106 +5,108 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-
 import logging
 import os
 
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.core.temporary import temp_directory
-from earthkit.data.testing import earthkit_examples_file
+from earthkit.data.testing import earthkit_examples_file, preserve_cwd
 
 LOG = logging.getLogger(__name__)
 
 
 def test_file_source_grib():
+    from earthkit.data.readers.grib.file import GRIBReader
+
     s = from_source("file", earthkit_examples_file("test.grib"))
-    from earthkit.data.readers.grib.reader import GRIBReader
 
     assert isinstance(s, GRIBReader), s
     assert len(s) == 2
 
 
 def test_file_source_grib_save():
-    s = from_source("file", earthkit_examples_file("test.grib"))
+    ds = from_source("file", os.path.abspath(earthkit_examples_file("test.grib")))
     with temp_directory() as tmpdir:
         # Check file save to assigned filename
-        s.save(os.path.join(tmpdir, "test2.grib"))
-        assert os.path.isfile(os.path.join(tmpdir, "test2.grib"))
+        f_tmp = os.path.join(tmpdir, "test2.grib")
+        ds.save(f_tmp)
+        assert os.path.isfile(f_tmp)
         # Check file can be saved in current dir with detected filename:
-        here = os.curdir
-        os.chdir(tmpdir)
-        s.save()
-        assert os.path.isfile("test.grib")
-        os.chdir(here)
+        with preserve_cwd():
+            os.chdir(tmpdir)
+            ds.save()
+            assert os.path.isfile("test.grib")
 
 
 def test_file_source_grib_no_overwrite():
-    _s = from_source("file", earthkit_examples_file("test.grib"))
+    ds = from_source("file", os.path.abspath(earthkit_examples_file("test.grib")))
     with temp_directory() as tmpdir:
-        os.chdir(tmpdir)
-        # Save the file locally
-        _s.save("test.grib")
-        # Open the local file
-        s = from_source("file", "test.grib")
-        with pytest.warns(
-            UserWarning,
-            match="Earhtkit refusing to overwrite the file we are currently reading",
-        ):
-            s.save("test.grib")
-        with pytest.warns(
-            UserWarning,
-            match="Earhtkit refusing to overwrite the file we are currently reading",
-        ):
-            s.save()
+        with preserve_cwd():
+            os.chdir(tmpdir)
+            # Save the file locally
+            ds.save("test.grib")
+            # Open the local file
+            ds1 = from_source("file", "test.grib")
+            with pytest.warns(
+                UserWarning,
+                match="Earthkit refusing to overwrite the file we are currently reading",
+            ):
+                ds1.save("test.grib")
+            with pytest.warns(
+                UserWarning,
+                match="Earthkit refusing to overwrite the file we are currently reading",
+            ):
+                ds1.save()
 
 
 def test_file_source_netcdf():
     s = from_source("file", earthkit_examples_file("test.nc"))
     assert len(s) == 2
 
 
 def test_file_source_netcdf_save():
-    s = from_source("file", earthkit_examples_file("test.nc"))
+    ds = from_source("file", os.path.abspath(earthkit_examples_file("test.nc")))
     with temp_directory() as tmpdir:
         # Check file save to assigned filename
-        s.save(os.path.join(tmpdir, "test2.nc"))
-        assert os.path.isfile(os.path.join(tmpdir, "test2.nc"))
+        f_tmp = os.path.join(tmpdir, "test2.nc")
+        ds.save(f_tmp)
+        assert os.path.isfile(f_tmp)
         # Check file can be saved in current dir with detected filename:
-        here = os.curdir
-        os.chdir(tmpdir)
-        s.save()
-        assert os.path.isfile("test.nc")
-        os.chdir(here)
+        with preserve_cwd():
+            os.chdir(tmpdir)
+            ds.save()
+            assert os.path.isfile("test.nc")
 
 
 def test_file_source_netcdf_no_overwrite():
-    _s = from_source("file", earthkit_examples_file("test.nc"))
+    ds = from_source("file", os.path.abspath(earthkit_examples_file("test.nc")))
     with temp_directory() as tmpdir:
-        os.chdir(tmpdir)
-        # Save the file locally
-        _s.save("test.nc")
-        # Open the local file
-        s = from_source("file", "test.nc")
-        with pytest.warns(
-            UserWarning,
-            match="Earhtkit refusing to overwrite the file we are currently reading",
-        ):
-            s.save("test.nc")
-        with pytest.warns(
-            UserWarning,
-            match="Earhtkit refusing to overwrite the file we are currently reading",
-        ):
-            s.save()
+        with preserve_cwd():
+            os.chdir(tmpdir)
+            # Save the file locally
+            ds.save("test.nc")
+            # Open the local file
+            ds1 = from_source("file", "test.nc")
+            with pytest.warns(
+                UserWarning,
+                match="Earthkit refusing to overwrite the file we are currently reading",
+            ):
+                ds1.save("test.nc")
+            with pytest.warns(
+                UserWarning,
+                match="Earthkit refusing to overwrite the file we are currently reading",
+            ):
+                ds1.save()
 
 
 def test_file_source_odb():
     s = from_source("file", earthkit_examples_file("test.odb"))
     assert s.path == earthkit_examples_file("test.odb")
```

### Comparing `earthkit_data-0.7.0/tests/sources/test_list_of_dicts.py` & `earthkit_data-0.8.1/tests/sources/test_list_of_dicts.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_mars.py` & `earthkit_data-0.8.1/tests/sources/test_mars.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_multi.py` & `earthkit_data-0.8.1/tests/sources/test_multi.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_polytope.py` & `earthkit_data-0.8.1/tests/sources/test_polytope.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_samples.py` & `earthkit_data-0.8.1/tests/sources/test_samples.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_url.py` & `earthkit_data-0.8.1/tests/sources/test_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 import sys
 
 import pytest
 
 from earthkit.data import from_source, settings
 from earthkit.data.core.temporary import temp_directory, temp_file
 from earthkit.data.testing import (
-    earthkit_file,
+    earthkit_examples_file,
     earthkit_remote_test_data_file,
     network_off,
 )
 
 
 @pytest.mark.skipif(  # TODO: fix
     sys.platform == "win32",
     reason="file:// not working on Windows yet",
 )
 def test_url_file_source():
-    filename = os.path.abspath(earthkit_file("docs/examples/test.nc"))
+    filename = os.path.abspath(earthkit_examples_file("test.nc"))
     s = from_source("url", f"file://{filename}")
     assert len(s) == 2
 
 
 def test_url_source_1():
     from_source(
         "url",
@@ -168,15 +168,15 @@
 
 
 @pytest.mark.skipif(  # TODO: fix
     sys.platform == "win32",
     reason="file:// not working on Windows yet",
 )
 def test_url_part_file_source():
-    filename = os.path.abspath(earthkit_file("docs/examples/test.grib"))
+    filename = os.path.abspath(earthkit_examples_file("test.grib"))
     ds = from_source(
         "url",
         f"file://{filename}",
         parts=[
             (0, 4),
             (522, 4),
             (526, 4),
```

### Comparing `earthkit_data-0.7.0/tests/sources/test_url_pattern.py` & `earthkit_data-0.8.1/tests/sources/test_url_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_wekeo.py` & `earthkit_data-0.8.1/tests/sources/test_wekeo.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/sources/test_wekeocds.py` & `earthkit_data-0.8.1/tests/sources/test_wekeocds.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/translators/test_translators.py` & `earthkit_data-0.8.1/tests/translators/test_translators.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/utils/test_array.py` & `earthkit_data-0.8.1/tests/utils/test_array.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/utils/test_bbox.py` & `earthkit_data-0.8.1/tests/utils/test_bbox.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/utils/test_dates.py` & `earthkit_data-0.8.1/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/utils/test_download_examples.py` & `earthkit_data-0.8.1/tests/utils/test_download_examples.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/utils/test_interval.py` & `earthkit_data-0.8.1/tests/utils/test_interval.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/utils/test_module_inputs_wrapper.py` & `earthkit_data-0.8.1/tests/utils/test_module_inputs_wrapper.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/utils/test_parts.py` & `earthkit_data-0.8.1/tests/utils/test_parts.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/utils/test_projections.py` & `earthkit_data-0.8.1/tests/utils/test_projections.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/wrappers/test_ndarray.py` & `earthkit_data-0.8.1/tests/wrappers/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/wrappers/test_pandas.py` & `earthkit_data-0.8.1/tests/wrappers/test_pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/wrappers/test_string.py` & `earthkit_data-0.8.1/tests/wrappers/test_string.py`

 * *Files identical despite different names*

### Comparing `earthkit_data-0.7.0/tests/wrappers/test_xarray.py` & `earthkit_data-0.8.1/tests/wrappers/test_xarray.py`

 * *Files identical despite different names*

