# Comparing `tmp/grafana_foundation_sdk-1716894257!11.0.0.tar.gz` & `tmp/grafana_foundation_sdk-1716894270!10.4.0.tar.gz`

## Comparing `grafana_foundation_sdk-1716894257!11.0.0.tar` & `grafana_foundation_sdk-1716894270!10.4.0.tar`

### file list

```diff
@@ -1,103 +1,105 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/accesspolicy.py
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/alerting.py
--rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/annotationslist.py
--rw-r--r--   0        0        0    27561 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/azuremonitor.py
--rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/barchart.py
--rw-r--r--   0        0        0    22315 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/bargauge.py
--rw-r--r--   0        0        0    50009 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/candlestick.py
--rw-r--r--   0        0        0    20481 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/canvas.py
--rw-r--r--   0        0        0    29243 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/cloudwatch.py
--rw-r--r--   0        0        0    49538 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/common.py
--rw-r--r--   0        0        0    72631 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/dashboard.py
--rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/dashboardlist.py
--rw-r--r--   0        0        0    18861 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/datagrid.py
--rw-r--r--   0        0        0    19038 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/debug.py
--rw-r--r--   0        0        0    63305 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/elasticsearch.py
--rw-r--r--   0        0        0    50546 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/expr.py
--rw-r--r--   0        0        0    21279 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/gauge.py
--rw-r--r--   0        0        0    20204 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/geomap.py
--rw-r--r--   0        0        0    19800 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/grafanapyroscope.py
--rw-r--r--   0        0        0    30297 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/heatmap.py
--rw-r--r--   0        0        0    34584 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/histogram.py
--rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/librarypanel.py
--rw-r--r--   0        0        0    21476 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/logs.py
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/loki.py
--rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/news.py
--rw-r--r--   0        0        0    19063 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/nodegraph.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/parca.py
--rw-r--r--   0        0        0    21960 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/piechart.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/preferences.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/prometheus.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/publicdashboard.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/role.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/rolebinding.py
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/stat.py
--rw-r--r--   0        0        0    24178 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/statetimeline.py
--rw-r--r--   0        0        0    23895 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/statushistory.py
--rw-r--r--   0        0        0    28817 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/table.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/team.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/tempo.py
--rw-r--r--   0        0        0    18787 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/testdata.py
--rw-r--r--   0        0        0    19310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/text.py
--rw-r--r--   0        0        0    48021 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/timeseries.py
--rw-r--r--   0        0        0    47390 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/trend.py
--rw-r--r--   0        0        0    37141 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/xychart.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/cog/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/cog/builder.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/cog/encoder.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/cog/plugins.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/cog/runtime.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/cog/variants.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/__init__.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/accesspolicy.py
--rw-r--r--   0        0        0    26784 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/alerting.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/annotationslist.py
--rw-r--r--   0        0        0    40649 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/azuremonitor.py
--rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/barchart.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/bargauge.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/candlestick.py
--rw-r--r--   0        0        0    15808 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/canvas.py
--rw-r--r--   0        0        0    39640 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/cloudwatch.py
--rw-r--r--   0        0        0    87730 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/common.py
--rw-r--r--   0        0        0    86957 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/dashboard.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/dashboardlist.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/datagrid.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/debug.py
--rw-r--r--   0        0        0    91710 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/elasticsearch.py
--rw-r--r--   0        0        0    66523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/expr.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/gauge.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/geomap.py
--rw-r--r--   0        0        0    27529 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/grafanapyroscope.py
--rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/heatmap.py
--rw-r--r--   0        0        0     8475 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/histogram.py
--rw-r--r--   0        0        0    16344 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/librarypanel.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/logs.py
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/loki.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/news.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/nodegraph.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/parca.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/piechart.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/preferences.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/prometheus.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/publicdashboard.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/role.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/rolebinding.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/stat.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/statetimeline.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/statushistory.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/table.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/team.py
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/tempo.py
--rw-r--r--   0        0        0    28219 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/testdata.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/text.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/timeseries.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/trend.py
--rw-r--r--   0        0        0    18310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/xychart.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/LICENSE.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/README.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/pyproject.toml
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894257!11.0.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/accesspolicy.py
+-rw-r--r--   0        0        0    19667 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/alertgroups.py
+-rw-r--r--   0        0        0    19721 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/alerting.py
+-rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/annotationslist.py
+-rw-r--r--   0        0        0    27683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/azuremonitor.py
+-rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/barchart.py
+-rw-r--r--   0        0        0    22315 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/bargauge.py
+-rw-r--r--   0        0        0    50009 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/candlestick.py
+-rw-r--r--   0        0        0    20481 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/canvas.py
+-rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/cloudwatch.py
+-rw-r--r--   0        0        0    49508 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/common.py
+-rw-r--r--   0        0        0    72631 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/dashboard.py
+-rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/dashboardlist.py
+-rw-r--r--   0        0        0    18861 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/datagrid.py
+-rw-r--r--   0        0        0    19038 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/debug.py
+-rw-r--r--   0        0        0    63427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/elasticsearch.py
+-rw-r--r--   0        0        0    50546 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/expr.py
+-rw-r--r--   0        0        0    21279 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/gauge.py
+-rw-r--r--   0        0        0    20204 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/geomap.py
+-rw-r--r--   0        0        0    19922 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/grafanapyroscope.py
+-rw-r--r--   0        0        0    30297 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/heatmap.py
+-rw-r--r--   0        0        0    33665 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/histogram.py
+-rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/librarypanel.py
+-rw-r--r--   0        0        0    21476 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/logs.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/loki.py
+-rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/news.py
+-rw-r--r--   0        0        0    19063 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/nodegraph.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/parca.py
+-rw-r--r--   0        0        0    21960 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/piechart.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/preferences.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/prometheus.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/publicdashboard.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/role.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/rolebinding.py
+-rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/stat.py
+-rw-r--r--   0        0        0    24178 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/statetimeline.py
+-rw-r--r--   0        0        0    23895 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/statushistory.py
+-rw-r--r--   0        0        0    28817 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/table.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/team.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/tempo.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/testdata.py
+-rw-r--r--   0        0        0    19310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/text.py
+-rw-r--r--   0        0        0    47677 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/timeseries.py
+-rw-r--r--   0        0        0    47390 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/trend.py
+-rw-r--r--   0        0        0    37141 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/xychart.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/cog/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/cog/builder.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/cog/encoder.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/cog/plugins.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/cog/runtime.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/cog/variants.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/accesspolicy.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/alertgroups.py
+-rw-r--r--   0        0        0    27052 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/alerting.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/annotationslist.py
+-rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/azuremonitor.py
+-rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/barchart.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/bargauge.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/candlestick.py
+-rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/canvas.py
+-rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/cloudwatch.py
+-rw-r--r--   0        0        0    87540 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/common.py
+-rw-r--r--   0        0        0    86957 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/dashboard.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/dashboardlist.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/datagrid.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/debug.py
+-rw-r--r--   0        0        0    91828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/elasticsearch.py
+-rw-r--r--   0        0        0    66523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/expr.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/gauge.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/geomap.py
+-rw-r--r--   0        0        0    27647 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/grafanapyroscope.py
+-rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/heatmap.py
+-rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/histogram.py
+-rw-r--r--   0        0        0    16344 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/librarypanel.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/logs.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/loki.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/news.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/nodegraph.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/parca.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/piechart.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/preferences.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/prometheus.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/publicdashboard.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/role.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/rolebinding.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/stat.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/statetimeline.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/statushistory.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/table.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/team.py
+-rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/tempo.py
+-rw-r--r--   0        0        0    21562 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/testdata.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/text.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/timeseries.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/trend.py
+-rw-r--r--   0        0        0    18310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/xychart.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/LICENSE.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716894270!10.4.0/PKG-INFO
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/accesspolicy.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/alerting.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/alerting.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,30 +53,117 @@
     def template(self, template: str) -> typing.Self:        
         self._internal.template = template
     
         return self
     
 
 class TimeInterval(cogbuilder.Builder[alerting.TimeInterval]):    
+    """
+    TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    within the interval.
+    """
+    
     _internal: alerting.TimeInterval
 
     def __init__(self):
         self._internal = alerting.TimeInterval()
 
     def build(self) -> alerting.TimeInterval:
         return self._internal    
     
-    def name(self, name: str) -> typing.Self:        
-        self._internal.name = name
+    def days_of_month(self, days_of_month: list[str]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.days_of_month = days_of_month
+    
+        return self
+    
+    def location(self, location: str) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.location = location
+    
+        return self
+    
+    def months(self, months: list[str]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.months = months
     
         return self
     
-    def time_intervals(self, time_intervals: list[cogbuilder.Builder[alerting.TimeInterval]]) -> typing.Self:        
-        time_intervals_resources = [r1.build() for r1 in time_intervals]
-        self._internal.time_intervals = time_intervals_resources
+    def times(self, times: list[cogbuilder.Builder[alerting.TimeRange]]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        times_resources = [r1.build() for r1 in times]
+        self._internal.times = times_resources
+    
+        return self
+    
+    def weekdays(self, weekdays: list[str]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.weekdays = weekdays
+    
+        return self
+    
+    def years(self, years: list[str]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.years = years
+    
+        return self
+    
+
+class TimeRange(cogbuilder.Builder[alerting.TimeRange]):    
+    """
+    Redefining this to avoid an import cycle
+    """
+    
+    _internal: alerting.TimeRange
+
+    def __init__(self):
+        self._internal = alerting.TimeRange()
+
+    def build(self) -> alerting.TimeRange:
+        return self._internal    
+    
+    def from_val(self, from_val: str) -> typing.Self:    
+        """
+        Redefining this to avoid an import cycle
+        """
+            
+        self._internal.from_val = from_val
+    
+        return self
+    
+    def to(self, to: str) -> typing.Self:    
+        """
+        Redefining this to avoid an import cycle
+        """
+            
+        self._internal.to = to
     
         return self
     
 
 class RuleGroup(cogbuilder.Builder[alerting.RuleGroup]):    
     _internal: alerting.RuleGroup
 
@@ -198,20 +285,14 @@
         return self
     
     def no_data_state(self, no_data_state: typing.Literal["Alerting", "NoData", "OK"]) -> typing.Self:        
         self._internal.no_data_state = no_data_state
     
         return self
     
-    def notification_settings(self, notification_settings: cogbuilder.Builder[alerting.NotificationSettings]) -> typing.Self:        
-        notification_settings_resource = notification_settings.build()
-        self._internal.notification_settings = notification_settings_resource
-    
-        return self
-    
     def org_id(self, org_id: int) -> typing.Self:        
         self._internal.org_id = org_id
     
         return self
     
     def provenance(self, provenance: alerting.Provenance) -> typing.Self:        
         self._internal.provenance = provenance
@@ -247,54 +328,14 @@
     
     def updated(self, updated: str) -> typing.Self:        
         self._internal.updated = updated
     
         return self
     
 
-class NotificationSettings(cogbuilder.Builder[alerting.NotificationSettings]):    
-    _internal: alerting.NotificationSettings
-
-    def __init__(self):
-        self._internal = alerting.NotificationSettings()
-
-    def build(self) -> alerting.NotificationSettings:
-        return self._internal    
-    
-    def group_by(self, group_by: list[str]) -> typing.Self:        
-        self._internal.group_by = group_by
-    
-        return self
-    
-    def group_interval(self, group_interval: str) -> typing.Self:        
-        self._internal.group_interval = group_interval
-    
-        return self
-    
-    def group_wait(self, group_wait: str) -> typing.Self:        
-        self._internal.group_wait = group_wait
-    
-        return self
-    
-    def mute_time_intervals(self, mute_time_intervals: list[str]) -> typing.Self:        
-        self._internal.mute_time_intervals = mute_time_intervals
-    
-        return self
-    
-    def receiver(self, receiver: str) -> typing.Self:        
-        self._internal.receiver = receiver
-    
-        return self
-    
-    def repeat_interval(self, repeat_interval: str) -> typing.Self:        
-        self._internal.repeat_interval = repeat_interval
-    
-        return self
-    
-
 class Query(cogbuilder.Builder[alerting.Query]):    
     _internal: alerting.Query
 
     def __init__(self, ref_id: typing.Optional[str]):
         self._internal = alerting.Query()        
         self._internal.ref_id = ref_id
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/annotationslist.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/azuremonitor.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/azuremonitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/barchart.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/barchart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/bargauge.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/bargauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/candlestick.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/candlestick.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/canvas.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/canvas.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/cloudwatch.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/cloudwatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,15 +191,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -630,15 +632,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -774,15 +778,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/common.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -1509,19 +1511,14 @@
         return self._internal    
     
     def mode(self, mode: common.TableCellBackgroundDisplayMode) -> typing.Self:        
         self._internal.mode = mode
     
         return self
     
-    def apply_to_row(self, apply_to_row: bool) -> typing.Self:        
-        self._internal.apply_to_row = apply_to_row
-    
-        return self
-    
 
 class DataSourceRef(cogbuilder.Builder[common.DataSourceRef]):    
     _internal: common.DataSourceRef
 
     def __init__(self):
         self._internal = common.DataSourceRef()
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/dashboard.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/dashboardlist.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/dashboardlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/datagrid.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/debug.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/elasticsearch.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/elasticsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1437,15 +1437,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/expr.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/expr.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/gauge.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/gauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/geomap.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/grafanapyroscope.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/grafanapyroscope.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,15 +68,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/heatmap.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/heatmap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/histogram.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -704,29 +704,14 @@
             self._internal.field_config.defaults.custom = histogram.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
         hide_from_resource = hide_from.build()
         self._internal.field_config.defaults.custom.hide_from = hide_from_resource
     
         return self
     
-    def stacking(self, stacking: cogbuilder.Builder[common.StackingConfig]) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = histogram.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
-        stacking_resource = stacking.build()
-        self._internal.field_config.defaults.custom.stacking = stacking_resource
-    
-        return self
-    
     def gradient_mode(self, gradient_mode: common.GraphGradientMode) -> typing.Self:    
         """
         Set the mode of the gradient fill. Fill gradient is based on the line color. To change the color, use the standard color scheme field option.
         Gradient appearance is influenced by the Fill opacity setting.
         """
             
         if self._internal.field_config is None:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/librarypanel.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/librarypanel.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/logs.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/logs.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/loki.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/loki.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,15 +91,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/news.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/nodegraph.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/parca.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/parca.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/piechart.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/preferences.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/prometheus.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/prometheus.py`

 * *Files 16% similar despite different names*

```diff
@@ -83,28 +83,36 @@
         See https://github.com/grafana/grafana/issues/48081
         """
             
         self._internal.interval_factor = interval_factor
     
         return self
     
+    def scope(self, scope: cogbuilder.Builder[prometheus.PrometheusDataqueryScope]) -> typing.Self:        
+        scope_resource = scope.build()
+        self._internal.scope = scope_resource
+    
+        return self
+    
     def ref_id(self, ref_id: str) -> typing.Self:    
         """
         A unique identifier for the query within the list of targets.
         In server side expressions, the refId is used as a variable name to identify results.
         By default, the UI will assign A->Z; however setting meaningful names may be useful.
         """
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -134,8 +142,23 @@
         An additional lower limit for the step parameter of the Prometheus query and for the
         `$__interval` and `$__rate_interval` variables.
         """
             
         self._internal.interval = interval
     
         return self
+    
+
+class PrometheusDataqueryScope(cogbuilder.Builder[prometheus.PrometheusDataqueryScope]):    
+    _internal: prometheus.PrometheusDataqueryScope
+
+    def __init__(self):
+        self._internal = prometheus.PrometheusDataqueryScope()
+
+    def build(self) -> prometheus.PrometheusDataqueryScope:
+        return self._internal    
+    
+    def matchers(self, matchers: str) -> typing.Self:        
+        self._internal.matchers = matchers
+    
+        return self
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/publicdashboard.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/role.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/rolebinding.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/stat.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/stat.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/statetimeline.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/statushistory.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/table.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/table.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/team.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/tempo.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/tempo.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/text.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/timeseries.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,22 +480,14 @@
             self._internal.options = timeseries.Options()
         assert isinstance(self._internal.options, timeseries.Options)
         tooltip_resource = tooltip.build()
         self._internal.options.tooltip = tooltip_resource
     
         return self
     
-    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = timeseries.Options()
-        assert isinstance(self._internal.options, timeseries.Options)
-        self._internal.options.orientation = orientation
-    
-        return self
-    
     def draw_style(self, draw_style: common.GraphDrawStyle) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/trend.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/trend.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/builders/xychart.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/builders/xychart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/cog/plugins.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/cog/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..models import statetimeline
-from ..models import xychart
-from ..models import expr
-from ..models import barchart
-from ..models import bargauge
-from ..models import stat
+from ..models import debug
 from ..models import table
-from ..models import timeseries
+from ..models import testdata
+from ..models import bargauge
+from ..models import datagrid
 from ..models import piechart
-from ..models import canvas
-from ..models import gauge
+from ..models import timeseries
+from ..models import xychart
+from ..models import dashboardlist
+from ..models import heatmap
 from ..models import histogram
-from ..models import text
-from ..models import annotationslist
+from ..models import logs
+from ..models import tempo
+from ..models import grafanapyroscope
 from ..models import elasticsearch
-from ..models import geomap
+from ..models import googlecloudmonitoring
 from ..models import loki
-from ..models import azuremonitor
-from ..models import dashboardlist
-from ..models import debug
-from ..models import heatmap
-from ..models import parca
+from ..models import news
 from ..models import nodegraph
-from ..models import statushistory
+from ..models import alertgroups
+from ..models import cloudwatch
+from ..models import text
 from ..models import trend
+from ..models import statushistory
+from ..models import gauge
+from ..models import parca
 from ..models import candlestick
-from ..models import cloudwatch
-from ..models import googlecloudmonitoring
+from ..models import canvas
 from ..models import prometheus
-from ..models import tempo
-from ..models import datagrid
-from ..models import grafanapyroscope
-from ..models import logs
-from ..models import news
+from ..models import stat
+from ..models import statetimeline
+from ..models import barchart
+from ..models import expr
+from ..models import azuremonitor
+from ..models import geomap
+from ..models import annotationslist
 from . import runtime as cogruntime
 
 
 def register_default_plugins():
     # Panelcfg variants
+    cogruntime.register_panelcfg_variant(alertgroups.variant_config())
     cogruntime.register_panelcfg_variant(annotationslist.variant_config())
     cogruntime.register_panelcfg_variant(barchart.variant_config())
     cogruntime.register_panelcfg_variant(bargauge.variant_config())
     cogruntime.register_panelcfg_variant(candlestick.variant_config())
     cogruntime.register_panelcfg_variant(canvas.variant_config())
     cogruntime.register_panelcfg_variant(dashboardlist.variant_config())
     cogruntime.register_panelcfg_variant(datagrid.variant_config())
@@ -71,7 +74,8 @@
     cogruntime.register_dataquery_variant(expr.variant_config())
     cogruntime.register_dataquery_variant(googlecloudmonitoring.variant_config())
     cogruntime.register_dataquery_variant(grafanapyroscope.variant_config())
     cogruntime.register_dataquery_variant(loki.variant_config())
     cogruntime.register_dataquery_variant(parca.variant_config())
     cogruntime.register_dataquery_variant(prometheus.variant_config())
     cogruntime.register_dataquery_variant(tempo.variant_config())
+    cogruntime.register_dataquery_variant(testdata.variant_config())
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/cog/runtime.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/cog/runtime.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/accesspolicy.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/alerting.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/alerting.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,38 +138,114 @@
         if "to" in data:
             args["to"] = data["to"]        
 
         return cls(**args)
 
 
 class TimeInterval:
-    name: typing.Optional[str]
-    time_intervals: typing.Optional[list['TimeInterval']]
+    """
+    TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    within the interval.
+    """
+
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    days_of_month: typing.Optional[list[str]]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    location: typing.Optional[str]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    months: typing.Optional[list[str]]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    times: typing.Optional[list['TimeRange']]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    weekdays: typing.Optional[list[str]]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    years: typing.Optional[list[str]]
+
+    def __init__(self, days_of_month: typing.Optional[list[str]] = None, location: typing.Optional[str] = None, months: typing.Optional[list[str]] = None, times: typing.Optional[list['TimeRange']] = None, weekdays: typing.Optional[list[str]] = None, years: typing.Optional[list[str]] = None):
+        self.days_of_month = days_of_month
+        self.location = location
+        self.months = months
+        self.times = times
+        self.weekdays = weekdays
+        self.years = years
 
-    def __init__(self, name: typing.Optional[str] = None, time_intervals: typing.Optional[list['TimeInterval']] = None):
-        self.name = name
-        self.time_intervals = time_intervals
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+        }
+        if self.days_of_month is not None:
+            payload["days_of_month"] = self.days_of_month
+        if self.location is not None:
+            payload["location"] = self.location
+        if self.months is not None:
+            payload["months"] = self.months
+        if self.times is not None:
+            payload["times"] = self.times
+        if self.weekdays is not None:
+            payload["weekdays"] = self.weekdays
+        if self.years is not None:
+            payload["years"] = self.years
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "days_of_month" in data:
+            args["days_of_month"] = data["days_of_month"]
+        if "location" in data:
+            args["location"] = data["location"]
+        if "months" in data:
+            args["months"] = data["months"]
+        if "times" in data:
+            args["times"] = data["times"]
+        if "weekdays" in data:
+            args["weekdays"] = data["weekdays"]
+        if "years" in data:
+            args["years"] = data["years"]        
+
+        return cls(**args)
+
+
+class TimeRange:
+    """
+    Redefining this to avoid an import cycle
+    """
+
+    # Redefining this to avoid an import cycle
+    from_val: typing.Optional[str]
+    # Redefining this to avoid an import cycle
+    to: typing.Optional[str]
+
+    def __init__(self, from_val: typing.Optional[str] = None, to: typing.Optional[str] = None):
+        self.from_val = from_val
+        self.to = to
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
-        if self.name is not None:
-            payload["name"] = self.name
-        if self.time_intervals is not None:
-            payload["time_intervals"] = self.time_intervals
+        if self.from_val is not None:
+            payload["from"] = self.from_val
+        if self.to is not None:
+            payload["to"] = self.to
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "name" in data:
-            args["name"] = data["name"]
-        if "time_intervals" in data:
-            args["time_intervals"] = data["time_intervals"]        
+        if "from" in data:
+            args["from_val"] = data["from"]
+        if "to" in data:
+            args["to"] = data["to"]        
 
         return cls(**args)
 
 
 class RuleGroup:
     folder_uid: typing.Optional[str]
     # The interval, in seconds, at which all rules in the group are evaluated.
@@ -222,34 +298,32 @@
     # The amount of time, in seconds, for which the rule must be breached for the rule to be considered to be Firing.
     # Before this time has elapsed, the rule is only considered to be Pending.
     for_val: str
     id_val: typing.Optional[int]
     is_paused: typing.Optional[bool]
     labels: typing.Optional[dict[str, str]]
     no_data_state: typing.Literal["Alerting", "NoData", "OK"]
-    notification_settings: typing.Optional['NotificationSettings']
     org_id: int
     provenance: typing.Optional['Provenance']
     rule_group: str
     title: str
     uid: typing.Optional[str]
     updated: typing.Optional[str]
 
-    def __init__(self, annotations: typing.Optional[dict[str, str]] = None, condition: str = "", data: typing.Optional[list['Query']] = None, exec_err_state: typing.Optional[typing.Literal["OK", "Alerting", "Error"]] = None, folder_uid: str = "", for_val: str = "", id_val: typing.Optional[int] = None, is_paused: typing.Optional[bool] = None, labels: typing.Optional[dict[str, str]] = None, no_data_state: typing.Optional[typing.Literal["Alerting", "NoData", "OK"]] = None, notification_settings: typing.Optional['NotificationSettings'] = None, org_id: int = 0, provenance: typing.Optional['Provenance'] = None, rule_group: str = "", title: str = "", uid: typing.Optional[str] = None, updated: typing.Optional[str] = None):
+    def __init__(self, annotations: typing.Optional[dict[str, str]] = None, condition: str = "", data: typing.Optional[list['Query']] = None, exec_err_state: typing.Optional[typing.Literal["OK", "Alerting", "Error"]] = None, folder_uid: str = "", for_val: str = "", id_val: typing.Optional[int] = None, is_paused: typing.Optional[bool] = None, labels: typing.Optional[dict[str, str]] = None, no_data_state: typing.Optional[typing.Literal["Alerting", "NoData", "OK"]] = None, org_id: int = 0, provenance: typing.Optional['Provenance'] = None, rule_group: str = "", title: str = "", uid: typing.Optional[str] = None, updated: typing.Optional[str] = None):
         self.annotations = annotations
         self.condition = condition
         self.data = data if data is not None else []
         self.exec_err_state = exec_err_state if exec_err_state is not None else "OK"
         self.folder_uid = folder_uid
         self.for_val = for_val
         self.id_val = id_val
         self.is_paused = is_paused
         self.labels = labels
         self.no_data_state = no_data_state if no_data_state is not None else "Alerting"
-        self.notification_settings = notification_settings
         self.org_id = org_id
         self.provenance = provenance
         self.rule_group = rule_group
         self.title = title
         self.uid = uid
         self.updated = updated
 
@@ -269,16 +343,14 @@
             payload["annotations"] = self.annotations
         if self.id_val is not None:
             payload["id"] = self.id_val
         if self.is_paused is not None:
             payload["isPaused"] = self.is_paused
         if self.labels is not None:
             payload["labels"] = self.labels
-        if self.notification_settings is not None:
-            payload["notification_settings"] = self.notification_settings
         if self.provenance is not None:
             payload["provenance"] = self.provenance
         if self.uid is not None:
             payload["uid"] = self.uid
         if self.updated is not None:
             payload["updated"] = self.updated
         return payload
@@ -303,16 +375,14 @@
             args["id_val"] = data["id"]
         if "isPaused" in data:
             args["is_paused"] = data["isPaused"]
         if "labels" in data:
             args["labels"] = data["labels"]
         if "noDataState" in data:
             args["no_data_state"] = data["noDataState"]
-        if "notification_settings" in data:
-            args["notification_settings"] = NotificationSettings.from_json(data["notification_settings"])
         if "orgID" in data:
             args["org_id"] = data["orgID"]
         if "provenance" in data:
             args["provenance"] = data["provenance"]
         if "ruleGroup" in data:
             args["rule_group"] = data["ruleGroup"]
         if "title" in data:
@@ -321,66 +391,14 @@
             args["uid"] = data["uid"]
         if "updated" in data:
             args["updated"] = data["updated"]        
 
         return cls(**args)
 
 
-class NotificationSettings:
-    group_by: typing.Optional[list[str]]
-    group_interval: typing.Optional[str]
-    group_wait: typing.Optional[str]
-    mute_time_intervals: typing.Optional[list[str]]
-    receiver: str
-    repeat_interval: typing.Optional[str]
-
-    def __init__(self, group_by: typing.Optional[list[str]] = None, group_interval: typing.Optional[str] = None, group_wait: typing.Optional[str] = None, mute_time_intervals: typing.Optional[list[str]] = None, receiver: str = "", repeat_interval: typing.Optional[str] = None):
-        self.group_by = group_by if group_by is not None else ["alertname", "grafana_folder"]
-        self.group_interval = group_interval
-        self.group_wait = group_wait
-        self.mute_time_intervals = mute_time_intervals
-        self.receiver = receiver
-        self.repeat_interval = repeat_interval
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "receiver": self.receiver,
-        }
-        if self.group_by is not None:
-            payload["group_by"] = self.group_by
-        if self.group_interval is not None:
-            payload["group_interval"] = self.group_interval
-        if self.group_wait is not None:
-            payload["group_wait"] = self.group_wait
-        if self.mute_time_intervals is not None:
-            payload["mute_time_intervals"] = self.mute_time_intervals
-        if self.repeat_interval is not None:
-            payload["repeat_interval"] = self.repeat_interval
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "group_by" in data:
-            args["group_by"] = data["group_by"]
-        if "group_interval" in data:
-            args["group_interval"] = data["group_interval"]
-        if "group_wait" in data:
-            args["group_wait"] = data["group_wait"]
-        if "mute_time_intervals" in data:
-            args["mute_time_intervals"] = data["mute_time_intervals"]
-        if "receiver" in data:
-            args["receiver"] = data["receiver"]
-        if "repeat_interval" in data:
-            args["repeat_interval"] = data["repeat_interval"]        
-
-        return cls(**args)
-
-
 class Query:
     datasource_uid: typing.Optional[str]
     model: typing.Optional[cogvariants.Dataquery]
     query_type: typing.Optional[str]
     ref_id: typing.Optional[str]
     relative_time_range: typing.Optional['RelativeTimeRange']
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/annotationslist.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/azuremonitor.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/azuremonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class AzureMonitorQuery(cogvariants.Dataquery):
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # Azure subscription containing the resource(s) to be queried.
     subscription: typing.Optional[str]
     # Subscriptions to be queried via Azure Resource Graph.
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/barchart.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/barchart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/bargauge.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/bargauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/candlestick.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/candlestick.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/canvas.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,24 +54,22 @@
 class Placement:
     top: typing.Optional[float]
     left: typing.Optional[float]
     right: typing.Optional[float]
     bottom: typing.Optional[float]
     width: typing.Optional[float]
     height: typing.Optional[float]
-    rotation: typing.Optional[float]
 
-    def __init__(self, top: typing.Optional[float] = None, left: typing.Optional[float] = None, right: typing.Optional[float] = None, bottom: typing.Optional[float] = None, width: typing.Optional[float] = None, height: typing.Optional[float] = None, rotation: typing.Optional[float] = None):
+    def __init__(self, top: typing.Optional[float] = None, left: typing.Optional[float] = None, right: typing.Optional[float] = None, bottom: typing.Optional[float] = None, width: typing.Optional[float] = None, height: typing.Optional[float] = None):
         self.top = top
         self.left = left
         self.right = right
         self.bottom = bottom
         self.width = width
         self.height = height
-        self.rotation = rotation
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.top is not None:
             payload["top"] = self.top
         if self.left is not None:
@@ -80,16 +78,14 @@
             payload["right"] = self.right
         if self.bottom is not None:
             payload["bottom"] = self.bottom
         if self.width is not None:
             payload["width"] = self.width
         if self.height is not None:
             payload["height"] = self.height
-        if self.rotation is not None:
-            payload["rotation"] = self.rotation
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "top" in data:
@@ -99,17 +95,15 @@
         if "right" in data:
             args["right"] = data["right"]
         if "bottom" in data:
             args["bottom"] = data["bottom"]
         if "width" in data:
             args["width"] = data["width"]
         if "height" in data:
-            args["height"] = data["height"]
-        if "rotation" in data:
-            args["rotation"] = data["rotation"]        
+            args["height"] = data["height"]        
 
         return cls(**args)
 
 
 class BackgroundImageSize(enum.StrEnum):
     ORIGINAL = "original"
     CONTAIN = "contain"
@@ -152,42 +146,36 @@
 
         return cls(**args)
 
 
 class LineConfig:
     color: typing.Optional[common.ColorDimensionConfig]
     width: typing.Optional[float]
-    radius: typing.Optional[float]
 
-    def __init__(self, color: typing.Optional[common.ColorDimensionConfig] = None, width: typing.Optional[float] = None, radius: typing.Optional[float] = None):
+    def __init__(self, color: typing.Optional[common.ColorDimensionConfig] = None, width: typing.Optional[float] = None):
         self.color = color
         self.width = width
-        self.radius = radius
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.color is not None:
             payload["color"] = self.color
         if self.width is not None:
             payload["width"] = self.width
-        if self.radius is not None:
-            payload["radius"] = self.radius
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "color" in data:
             args["color"] = common.ColorDimensionConfig.from_json(data["color"])
         if "width" in data:
-            args["width"] = data["width"]
-        if "radius" in data:
-            args["radius"] = data["radius"]        
+            args["width"] = data["width"]        
 
         return cls(**args)
 
 
 class HttpRequestMethod(enum.StrEnum):
     GET = "GET"
     POST = "POST"
@@ -228,47 +216,35 @@
 class CanvasConnection:
     source: 'ConnectionCoordinates'
     target: 'ConnectionCoordinates'
     target_name: typing.Optional[str]
     path: 'ConnectionPath'
     color: typing.Optional[common.ColorDimensionConfig]
     size: typing.Optional[common.ScaleDimensionConfig]
-    vertices: typing.Optional[list['ConnectionCoordinates']]
-    source_original: typing.Optional['ConnectionCoordinates']
-    target_original: typing.Optional['ConnectionCoordinates']
 
-    def __init__(self, source: typing.Optional['ConnectionCoordinates'] = None, target: typing.Optional['ConnectionCoordinates'] = None, target_name: typing.Optional[str] = None, path: typing.Optional['ConnectionPath'] = None, color: typing.Optional[common.ColorDimensionConfig] = None, size: typing.Optional[common.ScaleDimensionConfig] = None, vertices: typing.Optional[list['ConnectionCoordinates']] = None, source_original: typing.Optional['ConnectionCoordinates'] = None, target_original: typing.Optional['ConnectionCoordinates'] = None):
+    def __init__(self, source: typing.Optional['ConnectionCoordinates'] = None, target: typing.Optional['ConnectionCoordinates'] = None, target_name: typing.Optional[str] = None, path: typing.Optional['ConnectionPath'] = None, color: typing.Optional[common.ColorDimensionConfig] = None, size: typing.Optional[common.ScaleDimensionConfig] = None):
         self.source = source if source is not None else ConnectionCoordinates()
         self.target = target if target is not None else ConnectionCoordinates()
         self.target_name = target_name
         self.path = path if path is not None else ConnectionPath.STRAIGHT
         self.color = color
         self.size = size
-        self.vertices = vertices
-        self.source_original = source_original
-        self.target_original = target_original
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "source": self.source,
             "target": self.target,
             "path": self.path,
         }
         if self.target_name is not None:
             payload["targetName"] = self.target_name
         if self.color is not None:
             payload["color"] = self.color
         if self.size is not None:
             payload["size"] = self.size
-        if self.vertices is not None:
-            payload["vertices"] = self.vertices
-        if self.source_original is not None:
-            payload["sourceOriginal"] = self.source_original
-        if self.target_original is not None:
-            payload["targetOriginal"] = self.target_original
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "source" in data:
@@ -278,21 +254,15 @@
         if "targetName" in data:
             args["target_name"] = data["targetName"]
         if "path" in data:
             args["path"] = data["path"]
         if "color" in data:
             args["color"] = common.ColorDimensionConfig.from_json(data["color"])
         if "size" in data:
-            args["size"] = common.ScaleDimensionConfig.from_json(data["size"])
-        if "vertices" in data:
-            args["vertices"] = data["vertices"]
-        if "sourceOriginal" in data:
-            args["source_original"] = ConnectionCoordinates.from_json(data["sourceOriginal"])
-        if "targetOriginal" in data:
-            args["target_original"] = ConnectionCoordinates.from_json(data["targetOriginal"])        
+            args["size"] = common.ScaleDimensionConfig.from_json(data["size"])        
 
         return cls(**args)
 
 
 class CanvasElementOptions:
     name: str
     type_val: str
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/cloudwatch.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/cloudwatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,17 @@
     expression: typing.Optional[str]
     # When the metric query type is `metricQueryType` is set to `Query`, this field is used to specify the query string.
     sql_expression: typing.Optional[str]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # AWS region to query for the metric
     region: str
     # A namespace is a container for CloudWatch metrics. Metrics in different namespaces are isolated from each other, so that metrics from different applications are not mistakenly aggregated into the same statistics. For example, Amazon EC2 uses the AWS/EC2 namespace.
@@ -614,15 +616,17 @@
     stats_groups: typing.Optional[list[str]]
     # Log groups to query
     log_groups: typing.Optional[list['LogGroup']]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # @deprecated use logGroups
     log_group_names: typing.Optional[list[str]]
     # For mixed data sources the selected datasource is on the query level.
@@ -757,15 +761,17 @@
     # e.g. `arn:aws:sns:us-east-1:123456789012:my-app-` would match `arn:aws:sns:us-east-1:123456789012:my-app-action`
     # but not match `arn:aws:sns:us-east-1:123456789012:your-app-action`
     action_prefix: typing.Optional[str]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # AWS region to query for the metric
     region: str
     # A namespace is a container for CloudWatch metrics. Metrics in different namespaces are isolated from each other, so that metrics from different applications are not mistakenly aggregated into the same statistics. For example, Amazon EC2 uses the AWS/EC2 namespace.
@@ -890,15 +896,15 @@
         return cls(**args)
 
 
 CloudWatchQuery: typing.TypeAlias = typing.Union['CloudWatchMetricsQuery', 'CloudWatchLogsQuery', 'CloudWatchAnnotationQuery']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
-    decoding_map: dict[str, typing.Union[typing.Type[CloudWatchMetricsQuery], typing.Type[CloudWatchLogsQuery], typing.Type[CloudWatchAnnotationQuery]]] = {"Metrics": CloudWatchMetricsQuery, "Logs": CloudWatchLogsQuery, "Annotations": CloudWatchAnnotationQuery}
+    decoding_map: dict[str, typing.Union[typing.Type[CloudWatchAnnotationQuery], typing.Type[CloudWatchMetricsQuery], typing.Type[CloudWatchLogsQuery]]] = {"Annotations": CloudWatchAnnotationQuery, "Metrics": CloudWatchMetricsQuery, "Logs": CloudWatchLogsQuery}
     return cogruntime.DataqueryConfig(
         identifier="cloudwatch",
         from_json_hook=lambda data: decoding_map[data["queryMode"]].from_json(data),
     )
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/common.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,17 @@
     properties for the given context.
     """
 
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
@@ -2269,39 +2271,33 @@
 class TableColoredBackgroundCellOptions:
     """
     Colored background cell options
     """
 
     type_val: typing.Literal["color-background"]
     mode: typing.Optional['TableCellBackgroundDisplayMode']
-    apply_to_row: typing.Optional[bool]
 
-    def __init__(self, mode: typing.Optional['TableCellBackgroundDisplayMode'] = None, apply_to_row: typing.Optional[bool] = None):
+    def __init__(self, mode: typing.Optional['TableCellBackgroundDisplayMode'] = None):
         self.type_val = "color-background"
         self.mode = mode
-        self.apply_to_row = apply_to_row
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
         }
         if self.mode is not None:
             payload["mode"] = self.mode
-        if self.apply_to_row is not None:
-            payload["applyToRow"] = self.apply_to_row
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "mode" in data:
-            args["mode"] = data["mode"]
-        if "applyToRow" in data:
-            args["apply_to_row"] = data["applyToRow"]        
+            args["mode"] = data["mode"]        
 
         return cls(**args)
 
 
 class TableCellHeight(enum.StrEnum):
     """
     Height of a table cell
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/dashboard.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/dashboardlist.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/dashboardlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/datagrid.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/debug.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/elasticsearch.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/elasticsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1910,15 +1910,17 @@
     bucket_aggs: typing.Optional[list['BucketAggregation']]
     # List of metric aggregations
     metrics: typing.Optional[list['MetricAggregation']]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/expr.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..cog import variants as cogvariants
 
 
 Expr: typing.TypeAlias = typing.Union['TypeMath', 'TypeReduce', 'TypeResample', 'TypeClassicConditions', 'TypeThreshold', 'TypeSql']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
-    decoding_map: dict[str, typing.Union[typing.Type[TypeResample], typing.Type[TypeClassicConditions], typing.Type[TypeThreshold], typing.Type[TypeSql], typing.Type[TypeMath], typing.Type[TypeReduce]]] = {"resample": TypeResample, "classic_conditions": TypeClassicConditions, "threshold": TypeThreshold, "sql": TypeSql, "math": TypeMath, "reduce": TypeReduce}
+    decoding_map: dict[str, typing.Union[typing.Type[TypeReduce], typing.Type[TypeResample], typing.Type[TypeClassicConditions], typing.Type[TypeThreshold], typing.Type[TypeSql], typing.Type[TypeMath]]] = {"reduce": TypeReduce, "resample": TypeResample, "classic_conditions": TypeClassicConditions, "threshold": TypeThreshold, "sql": TypeSql, "math": TypeMath}
     return cogruntime.DataqueryConfig(
         identifier="__expr__",
         from_json_hook=lambda data: decoding_map[data["type"]].from_json(data),
     )
 
 
 class TypeMath(cogvariants.Dataquery):
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/gauge.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/gauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/geomap.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/googlecloudmonitoring.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/googlecloudmonitoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class CloudMonitoringQuery(cogvariants.Dataquery):
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # Aliases can be set to modify the legend labels. e.g. {{metric.label.xxx}}. See docs for more detail.
     alias_by: typing.Optional[str]
     # GCM query type.
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/grafanapyroscope.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/grafanapyroscope.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     group_by: typing.Optional[list[str]]
     # Sets the maximum number of nodes in the flamegraph.
     max_nodes: typing.Optional[int]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/heatmap.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/heatmap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/histogram.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,34 +71,32 @@
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
     axis_centered_zero: typing.Optional[bool]
     hide_from: typing.Optional[common.HideSeriesConfig]
-    stacking: typing.Optional[common.StackingConfig]
     # Set the mode of the gradient fill. Fill gradient is based on the line color. To change the color, use the standard color scheme field option.
     # Gradient appearance is influenced by the Fill opacity setting.
     gradient_mode: typing.Optional[common.GraphGradientMode]
     axis_border_show: typing.Optional[bool]
 
-    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, stacking: typing.Optional[common.StackingConfig] = None, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_border_show: typing.Optional[bool] = None):
+    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_border_show: typing.Optional[bool] = None):
         self.line_width = line_width
         self.fill_opacity = fill_opacity
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
         self.axis_centered_zero = axis_centered_zero
         self.hide_from = hide_from
-        self.stacking = stacking
         self.gradient_mode = gradient_mode if gradient_mode is not None else common.GraphGradientMode.NONE
         self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.line_width is not None:
@@ -121,16 +119,14 @@
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
         if self.axis_centered_zero is not None:
             payload["axisCenteredZero"] = self.axis_centered_zero
         if self.hide_from is not None:
             payload["hideFrom"] = self.hide_from
-        if self.stacking is not None:
-            payload["stacking"] = self.stacking
         if self.gradient_mode is not None:
             payload["gradientMode"] = self.gradient_mode
         if self.axis_border_show is not None:
             payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
@@ -157,16 +153,14 @@
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
         if "axisCenteredZero" in data:
             args["axis_centered_zero"] = data["axisCenteredZero"]
         if "hideFrom" in data:
             args["hide_from"] = common.HideSeriesConfig.from_json(data["hideFrom"])
-        if "stacking" in data:
-            args["stacking"] = common.StackingConfig.from_json(data["stacking"])
         if "gradientMode" in data:
             args["gradient_mode"] = data["gradientMode"]
         if "axisBorderShow" in data:
             args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/librarypanel.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/librarypanel.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/logs.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/logs.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/loki.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/loki.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,15 +45,17 @@
     instant: typing.Optional[bool]
     # Used to set step value for range queries.
     step: typing.Optional[str]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/news.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/nodegraph.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/parca.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/parca.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     label_selector: typing.Optional[str]
     # Specifies the type of profile to query.
     profile_type_id: typing.Optional[str]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/piechart.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/preferences.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/prometheus.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/prometheus.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,41 +31,45 @@
     # Query format to determine how to display data points in panel. It can be "time_series", "table", "heatmap"
     format_val: typing.Optional['PromQueryFormat']
     # Series name override or template. Ex. {{hostname}} will be replaced with label value for hostname
     legend_format: typing.Optional[str]
     # @deprecated Used to specify how many times to divide max data points by. We use max data points under query options
     # See https://github.com/grafana/grafana/issues/48081
     interval_factor: typing.Optional[float]
+    scope: typing.Optional['PrometheusDataqueryScope']
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
     # An additional lower limit for the step parameter of the Prometheus query and for the
     # `$__interval` and `$__rate_interval` variables.
     interval: typing.Optional[str]
 
-    def __init__(self, expr: typing.Optional[str] = None, instant: typing.Optional[bool] = None, range_val: typing.Optional[bool] = None, exemplar: typing.Optional[bool] = None, editor_mode: typing.Optional['QueryEditorMode'] = None, format_val: typing.Optional['PromQueryFormat'] = None, legend_format: typing.Optional[str] = None, interval_factor: typing.Optional[float] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None, interval: typing.Optional[str] = None):
+    def __init__(self, expr: typing.Optional[str] = None, instant: typing.Optional[bool] = None, range_val: typing.Optional[bool] = None, exemplar: typing.Optional[bool] = None, editor_mode: typing.Optional['QueryEditorMode'] = None, format_val: typing.Optional['PromQueryFormat'] = None, legend_format: typing.Optional[str] = None, interval_factor: typing.Optional[float] = None, scope: typing.Optional['PrometheusDataqueryScope'] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None, interval: typing.Optional[str] = None):
         self.expr = expr
         self.instant = instant
         self.range_val = range_val
         self.exemplar = exemplar
         self.editor_mode = editor_mode
         self.format_val = format_val
         self.legend_format = legend_format
         self.interval_factor = interval_factor
+        self.scope = scope
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.datasource = datasource
         self.interval = interval
 
     def to_json(self) -> dict[str, object]:
@@ -83,14 +87,16 @@
             payload["editorMode"] = self.editor_mode
         if self.format_val is not None:
             payload["format"] = self.format_val
         if self.legend_format is not None:
             payload["legendFormat"] = self.legend_format
         if self.interval_factor is not None:
             payload["intervalFactor"] = self.interval_factor
+        if self.scope is not None:
+            payload["scope"] = self.scope
         if self.ref_id is not None:
             payload["refId"] = self.ref_id
         if self.hide is not None:
             payload["hide"] = self.hide
         if self.query_type is not None:
             payload["queryType"] = self.query_type
         if self.datasource is not None:
@@ -115,14 +121,16 @@
             args["editor_mode"] = data["editorMode"]
         if "format" in data:
             args["format_val"] = data["format"]
         if "legendFormat" in data:
             args["legend_format"] = data["legendFormat"]
         if "intervalFactor" in data:
             args["interval_factor"] = data["intervalFactor"]
+        if "scope" in data:
+            args["scope"] = PrometheusDataqueryScope.from_json(data["scope"])
         if "refId" in data:
             args["ref_id"] = data["refId"]
         if "hide" in data:
             args["hide"] = data["hide"]
         if "queryType" in data:
             args["query_type"] = data["queryType"]
         if "datasource" in data:
@@ -136,8 +144,30 @@
 def variant_config() -> cogruntime.DataqueryConfig:
     return cogruntime.DataqueryConfig(
         identifier="prometheus",
         from_json_hook=Dataquery.from_json,
     )
 
 
+class PrometheusDataqueryScope:
+    matchers: str
+
+    def __init__(self, matchers: str = ""):
+        self.matchers = matchers
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "matchers": self.matchers,
+        }
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "matchers" in data:
+            args["matchers"] = data["matchers"]        
+
+        return cls(**args)
+
+
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/publicdashboard.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/role.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/rolebinding.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/stat.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/stat.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/statetimeline.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/statushistory.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/table.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/table.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/team.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/tempo.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/tempo.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class TempoQuery(cogvariants.Dataquery):
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # TraceQL query or trace ID
     query: typing.Optional[str]
     # @deprecated Logfmt query to filter traces by their tags. Example: http.status_code=200 error=true
@@ -149,16 +151,21 @@
     return cogruntime.DataqueryConfig(
         identifier="tempo",
         from_json_hook=TempoQuery.from_json,
     )
 
 
 class TempoQueryType(enum.StrEnum):
+    """
+    search = Loki search, nativeSearch = Tempo search for backwards compatibility
+    """
+
     TRACEQL = "traceql"
     TRACEQL_SEARCH = "traceqlSearch"
+    SEARCH = "search"
     SERVICE_MAP = "serviceMap"
     UPLOAD = "upload"
     NATIVE_SEARCH = "nativeSearch"
     TRACE_ID = "traceId"
     CLEAR = "clear"
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/testdata.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/testdata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,708 +1,568 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..cog import variants as cogvariants
+import enum
 import typing
+from ..cog import variants as cogvariants
 from ..cog import runtime as cogruntime
 
 
-class Dataquery(cogvariants.Dataquery):
-    alias: typing.Optional[str]
-    # Used for live query
-    channel: typing.Optional[str]
-    csv_content: typing.Optional[str]
-    csv_file_name: typing.Optional[str]
-    csv_wave: typing.Optional[list['CSVWave']]
-    # The datasource
-    datasource: typing.Optional['Datasource']
-    # Drop percentage (the chance we will lose a point 0-100)
-    drop_percent: typing.Optional[float]
-    # Possible enum values:
-    #  - `"frontend_exception"` 
-    #  - `"frontend_observable"` 
-    #  - `"server_panic"` 
-    error_type: typing.Optional[typing.Literal["frontend_exception", "frontend_observable", "server_panic"]]
-    flamegraph_diff: typing.Optional[bool]
-    # true if query is disabled (ie should not be returned to the dashboard)
-    # NOTE: this does not always imply that the query should not be executed since
-    # the results from a hidden query may be used as the input to other queries (SSE etc)
-    hide: typing.Optional[bool]
-    # Interval is the suggested duration between time points in a time series query.
-    # NOTE: the values for intervalMs is not saved in the query model.  It is typically calculated
-    # from the interval required to fill a pixels in the visualization
-    interval_ms: typing.Optional[float]
-    labels: typing.Optional[str]
-    level_column: typing.Optional[bool]
-    lines: typing.Optional[int]
-    max_val: typing.Optional[float]
-    # MaxDataPoints is the maximum number of data points that should be returned from a time series query.
-    # NOTE: the values for maxDataPoints is not saved in the query model.  It is typically calculated
-    # from the number of pixels visible in a visualization
-    max_data_points: typing.Optional[int]
-    min_val: typing.Optional[float]
-    nodes: typing.Optional['NodesQuery']
-    noise: typing.Optional[float]
-    points: typing.Optional[list[list[object]]]
-    pulse_wave: typing.Optional['PulseWaveQuery']
-    # QueryType is an optional identifier for the type of query.
-    # It can be used to distinguish different types of queries.
-    query_type: typing.Optional[str]
-    raw_frame_content: typing.Optional[str]
-    # RefID is the unique identifier of the query, set by the frontend call.
-    ref_id: typing.Optional[str]
-    # Optionally define expected query result behavior
-    result_assertions: typing.Optional['ResultAssertions']
-    # Possible enum values:
-    #  - `"annotations"` 
-    #  - `"arrow"` 
-    #  - `"csv_content"` 
-    #  - `"csv_file"` 
-    #  - `"csv_metric_values"` 
-    #  - `"datapoints_outside_range"` 
-    #  - `"exponential_heatmap_bucket_data"` 
-    #  - `"flame_graph"` 
-    #  - `"grafana_api"` 
-    #  - `"linear_heatmap_bucket_data"` 
-    #  - `"live"` 
-    #  - `"logs"` 
-    #  - `"manual_entry"` 
-    #  - `"no_data_points"` 
-    #  - `"node_graph"` 
-    #  - `"predictable_csv_wave"` 
-    #  - `"predictable_pulse"` 
-    #  - `"random_walk"` 
-    #  - `"random_walk_table"` 
-    #  - `"random_walk_with_error"` 
-    #  - `"raw_frame"` 
-    #  - `"server_error_500"` 
-    #  - `"simulation"` 
-    #  - `"slow_query"` 
-    #  - `"streaming_client"` 
-    #  - `"table_static"` 
-    #  - `"trace"` 
-    #  - `"usa"` 
-    #  - `"variables-query"` 
-    scenario_id: typing.Optional[typing.Literal["annotations", "arrow", "csv_content", "csv_file", "csv_metric_values", "datapoints_outside_range", "exponential_heatmap_bucket_data", "flame_graph", "grafana_api", "linear_heatmap_bucket_data", "live", "logs", "manual_entry", "no_data_points", "node_graph", "predictable_csv_wave", "predictable_pulse", "random_walk", "random_walk_table", "random_walk_with_error", "raw_frame", "server_error_500", "simulation", "slow_query", "streaming_client", "table_static", "trace", "usa", "variables-query"]]
-    series_count: typing.Optional[int]
-    sim: typing.Optional['SimulationQuery']
-    span_count: typing.Optional[int]
-    spread: typing.Optional[float]
-    start_value: typing.Optional[float]
-    stream: typing.Optional['StreamingQuery']
-    # common parameter used by many query types
-    string_input: typing.Optional[str]
-    # TimeRange represents the query range
-    # NOTE: unlike generic /ds/query, we can now send explicit time values in each query
-    # NOTE: the values for timeRange are not saved in a dashboard, they are constructed on the fly
-    time_range: typing.Optional['TimeRange']
-    usa: typing.Optional['USAQuery']
-    with_nil: typing.Optional[bool]
+class TestDataQueryType(enum.StrEnum):
+    RANDOM_WALK = "random_walk"
+    SLOW_QUERY = "slow_query"
+    RANDOM_WALK_WITH_ERROR = "random_walk_with_error"
+    RANDOM_WALK_TABLE = "random_walk_table"
+    EXPONENTIAL_HEATMAP_BUCKET_DATA = "exponential_heatmap_bucket_data"
+    LINEAR_HEATMAP_BUCKET_DATA = "linear_heatmap_bucket_data"
+    NO_DATA_POINTS = "no_data_points"
+    DATA_POINTS_OUTSIDE_RANGE = "datapoints_outside_range"
+    CSV_METRIC_VALUES = "csv_metric_values"
+    PREDICTABLE_PULSE = "predictable_pulse"
+    PREDICTABLE_CSV_WAVE = "predictable_csv_wave"
+    STREAMING_CLIENT = "streaming_client"
+    SIMULATION = "simulation"
+    USA = "usa"
+    LIVE = "live"
+    GRAFANA_API = "grafana_api"
+    ARROW = "arrow"
+    ANNOTATIONS = "annotations"
+    TABLE_STATIC = "table_static"
+    SERVER_ERROR500 = "server_error_500"
+    LOGS = "logs"
+    NODE_GRAPH = "node_graph"
+    FLAME_GRAPH = "flame_graph"
+    RAW_FRAME = "raw_frame"
+    CSV_FILE = "csv_file"
+    CSV_CONTENT = "csv_content"
+    TRACE = "trace"
+    MANUAL_ENTRY = "manual_entry"
+    VARIABLES_QUERY = "variables-query"
 
-    def __init__(self, alias: typing.Optional[str] = None, channel: typing.Optional[str] = None, csv_content: typing.Optional[str] = None, csv_file_name: typing.Optional[str] = None, csv_wave: typing.Optional[list['CSVWave']] = None, datasource: typing.Optional['Datasource'] = None, drop_percent: typing.Optional[float] = None, error_type: typing.Optional[typing.Literal["frontend_exception", "frontend_observable", "server_panic"]] = None, flamegraph_diff: typing.Optional[bool] = None, hide: typing.Optional[bool] = None, interval_ms: typing.Optional[float] = None, labels: typing.Optional[str] = None, level_column: typing.Optional[bool] = None, lines: typing.Optional[int] = None, max_val: typing.Optional[float] = None, max_data_points: typing.Optional[int] = None, min_val: typing.Optional[float] = None, nodes: typing.Optional['NodesQuery'] = None, noise: typing.Optional[float] = None, points: typing.Optional[list[list[object]]] = None, pulse_wave: typing.Optional['PulseWaveQuery'] = None, query_type: typing.Optional[str] = None, raw_frame_content: typing.Optional[str] = None, ref_id: typing.Optional[str] = None, result_assertions: typing.Optional['ResultAssertions'] = None, scenario_id: typing.Optional[typing.Literal["annotations", "arrow", "csv_content", "csv_file", "csv_metric_values", "datapoints_outside_range", "exponential_heatmap_bucket_data", "flame_graph", "grafana_api", "linear_heatmap_bucket_data", "live", "logs", "manual_entry", "no_data_points", "node_graph", "predictable_csv_wave", "predictable_pulse", "random_walk", "random_walk_table", "random_walk_with_error", "raw_frame", "server_error_500", "simulation", "slow_query", "streaming_client", "table_static", "trace", "usa", "variables-query"]] = None, series_count: typing.Optional[int] = None, sim: typing.Optional['SimulationQuery'] = None, span_count: typing.Optional[int] = None, spread: typing.Optional[float] = None, start_value: typing.Optional[float] = None, stream: typing.Optional['StreamingQuery'] = None, string_input: typing.Optional[str] = None, time_range: typing.Optional['TimeRange'] = None, usa: typing.Optional['USAQuery'] = None, with_nil: typing.Optional[bool] = None):
-        self.alias = alias
-        self.channel = channel
-        self.csv_content = csv_content
-        self.csv_file_name = csv_file_name
-        self.csv_wave = csv_wave
-        self.datasource = datasource
-        self.drop_percent = drop_percent
-        self.error_type = error_type
-        self.flamegraph_diff = flamegraph_diff
-        self.hide = hide
-        self.interval_ms = interval_ms
-        self.labels = labels
-        self.level_column = level_column
-        self.lines = lines
-        self.max_val = max_val
-        self.max_data_points = max_data_points
-        self.min_val = min_val
-        self.nodes = nodes
-        self.noise = noise
-        self.points = points
-        self.pulse_wave = pulse_wave
-        self.query_type = query_type
-        self.raw_frame_content = raw_frame_content
-        self.ref_id = ref_id
-        self.result_assertions = result_assertions
-        self.scenario_id = scenario_id
-        self.series_count = series_count
-        self.sim = sim
-        self.span_count = span_count
+
+class StreamingQuery:
+    type_val: typing.Literal["signal", "logs", "fetch", "traces"]
+    speed: int
+    spread: int
+    noise: int
+    bands: typing.Optional[int]
+    url: typing.Optional[str]
+
+    def __init__(self, type_val: typing.Optional[typing.Literal["signal", "logs", "fetch", "traces"]] = None, speed: int = 0, spread: int = 0, noise: int = 0, bands: typing.Optional[int] = None, url: typing.Optional[str] = None):
+        self.type_val = type_val if type_val is not None else "signal"
+        self.speed = speed
         self.spread = spread
-        self.start_value = start_value
-        self.stream = stream
-        self.string_input = string_input
-        self.time_range = time_range
-        self.usa = usa
-        self.with_nil = with_nil
+        self.noise = noise
+        self.bands = bands
+        self.url = url
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
+            "type": self.type_val,
+            "speed": self.speed,
+            "spread": self.spread,
+            "noise": self.noise,
         }
-        if self.alias is not None:
-            payload["alias"] = self.alias
-        if self.channel is not None:
-            payload["channel"] = self.channel
-        if self.csv_content is not None:
-            payload["csvContent"] = self.csv_content
-        if self.csv_file_name is not None:
-            payload["csvFileName"] = self.csv_file_name
-        if self.csv_wave is not None:
-            payload["csvWave"] = self.csv_wave
-        if self.datasource is not None:
-            payload["datasource"] = self.datasource
-        if self.drop_percent is not None:
-            payload["dropPercent"] = self.drop_percent
-        if self.error_type is not None:
-            payload["errorType"] = self.error_type
-        if self.flamegraph_diff is not None:
-            payload["flamegraphDiff"] = self.flamegraph_diff
-        if self.hide is not None:
-            payload["hide"] = self.hide
-        if self.interval_ms is not None:
-            payload["intervalMs"] = self.interval_ms
-        if self.labels is not None:
-            payload["labels"] = self.labels
-        if self.level_column is not None:
-            payload["levelColumn"] = self.level_column
-        if self.lines is not None:
-            payload["lines"] = self.lines
-        if self.max_val is not None:
-            payload["max"] = self.max_val
-        if self.max_data_points is not None:
-            payload["maxDataPoints"] = self.max_data_points
-        if self.min_val is not None:
-            payload["min"] = self.min_val
-        if self.nodes is not None:
-            payload["nodes"] = self.nodes
-        if self.noise is not None:
-            payload["noise"] = self.noise
-        if self.points is not None:
-            payload["points"] = self.points
-        if self.pulse_wave is not None:
-            payload["pulseWave"] = self.pulse_wave
-        if self.query_type is not None:
-            payload["queryType"] = self.query_type
-        if self.raw_frame_content is not None:
-            payload["rawFrameContent"] = self.raw_frame_content
-        if self.ref_id is not None:
-            payload["refId"] = self.ref_id
-        if self.result_assertions is not None:
-            payload["resultAssertions"] = self.result_assertions
-        if self.scenario_id is not None:
-            payload["scenarioId"] = self.scenario_id
-        if self.series_count is not None:
-            payload["seriesCount"] = self.series_count
-        if self.sim is not None:
-            payload["sim"] = self.sim
-        if self.span_count is not None:
-            payload["spanCount"] = self.span_count
-        if self.spread is not None:
-            payload["spread"] = self.spread
-        if self.start_value is not None:
-            payload["startValue"] = self.start_value
-        if self.stream is not None:
-            payload["stream"] = self.stream
-        if self.string_input is not None:
-            payload["stringInput"] = self.string_input
-        if self.time_range is not None:
-            payload["timeRange"] = self.time_range
-        if self.usa is not None:
-            payload["usa"] = self.usa
-        if self.with_nil is not None:
-            payload["withNil"] = self.with_nil
+        if self.bands is not None:
+            payload["bands"] = self.bands
+        if self.url is not None:
+            payload["url"] = self.url
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "alias" in data:
-            args["alias"] = data["alias"]
-        if "channel" in data:
-            args["channel"] = data["channel"]
-        if "csvContent" in data:
-            args["csv_content"] = data["csvContent"]
-        if "csvFileName" in data:
-            args["csv_file_name"] = data["csvFileName"]
-        if "csvWave" in data:
-            args["csv_wave"] = data["csvWave"]
-        if "datasource" in data:
-            args["datasource"] = Datasource.from_json(data["datasource"])
-        if "dropPercent" in data:
-            args["drop_percent"] = data["dropPercent"]
-        if "errorType" in data:
-            args["error_type"] = data["errorType"]
-        if "flamegraphDiff" in data:
-            args["flamegraph_diff"] = data["flamegraphDiff"]
-        if "hide" in data:
-            args["hide"] = data["hide"]
-        if "intervalMs" in data:
-            args["interval_ms"] = data["intervalMs"]
-        if "labels" in data:
-            args["labels"] = data["labels"]
-        if "levelColumn" in data:
-            args["level_column"] = data["levelColumn"]
-        if "lines" in data:
-            args["lines"] = data["lines"]
-        if "max" in data:
-            args["max_val"] = data["max"]
-        if "maxDataPoints" in data:
-            args["max_data_points"] = data["maxDataPoints"]
-        if "min" in data:
-            args["min_val"] = data["min"]
-        if "nodes" in data:
-            args["nodes"] = NodesQuery.from_json(data["nodes"])
-        if "noise" in data:
-            args["noise"] = data["noise"]
-        if "points" in data:
-            args["points"] = data["points"]
-        if "pulseWave" in data:
-            args["pulse_wave"] = PulseWaveQuery.from_json(data["pulseWave"])
-        if "queryType" in data:
-            args["query_type"] = data["queryType"]
-        if "rawFrameContent" in data:
-            args["raw_frame_content"] = data["rawFrameContent"]
-        if "refId" in data:
-            args["ref_id"] = data["refId"]
-        if "resultAssertions" in data:
-            args["result_assertions"] = ResultAssertions.from_json(data["resultAssertions"])
-        if "scenarioId" in data:
-            args["scenario_id"] = data["scenarioId"]
-        if "seriesCount" in data:
-            args["series_count"] = data["seriesCount"]
-        if "sim" in data:
-            args["sim"] = SimulationQuery.from_json(data["sim"])
-        if "spanCount" in data:
-            args["span_count"] = data["spanCount"]
+        if "type" in data:
+            args["type_val"] = data["type"]
+        if "speed" in data:
+            args["speed"] = data["speed"]
         if "spread" in data:
             args["spread"] = data["spread"]
-        if "startValue" in data:
-            args["start_value"] = data["startValue"]
-        if "stream" in data:
-            args["stream"] = StreamingQuery.from_json(data["stream"])
-        if "stringInput" in data:
-            args["string_input"] = data["stringInput"]
-        if "timeRange" in data:
-            args["time_range"] = TimeRange.from_json(data["timeRange"])
-        if "usa" in data:
-            args["usa"] = USAQuery.from_json(data["usa"])
-        if "withNil" in data:
-            args["with_nil"] = data["withNil"]        
+        if "noise" in data:
+            args["noise"] = data["noise"]
+        if "bands" in data:
+            args["bands"] = data["bands"]
+        if "url" in data:
+            args["url"] = data["url"]        
 
         return cls(**args)
 
 
-def variant_config() -> cogruntime.DataqueryConfig:
-    return cogruntime.DataqueryConfig(
-        identifier="",
-        from_json_hook=Dataquery.from_json,
-    )
-
-
-class CSVWave:
-    labels: typing.Optional[str]
-    name: typing.Optional[str]
+class PulseWaveQuery:
     time_step: typing.Optional[int]
-    values_csv: typing.Optional[str]
+    on_count: typing.Optional[int]
+    off_count: typing.Optional[int]
+    on_value: typing.Optional[float]
+    off_value: typing.Optional[float]
 
-    def __init__(self, labels: typing.Optional[str] = None, name: typing.Optional[str] = None, time_step: typing.Optional[int] = None, values_csv: typing.Optional[str] = None):
-        self.labels = labels
-        self.name = name
+    def __init__(self, time_step: typing.Optional[int] = None, on_count: typing.Optional[int] = None, off_count: typing.Optional[int] = None, on_value: typing.Optional[float] = None, off_value: typing.Optional[float] = None):
         self.time_step = time_step
-        self.values_csv = values_csv
+        self.on_count = on_count
+        self.off_count = off_count
+        self.on_value = on_value
+        self.off_value = off_value
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
-        if self.labels is not None:
-            payload["labels"] = self.labels
-        if self.name is not None:
-            payload["name"] = self.name
         if self.time_step is not None:
             payload["timeStep"] = self.time_step
-        if self.values_csv is not None:
-            payload["valuesCSV"] = self.values_csv
+        if self.on_count is not None:
+            payload["onCount"] = self.on_count
+        if self.off_count is not None:
+            payload["offCount"] = self.off_count
+        if self.on_value is not None:
+            payload["onValue"] = self.on_value
+        if self.off_value is not None:
+            payload["offValue"] = self.off_value
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "labels" in data:
-            args["labels"] = data["labels"]
-        if "name" in data:
-            args["name"] = data["name"]
         if "timeStep" in data:
             args["time_step"] = data["timeStep"]
-        if "valuesCSV" in data:
-            args["values_csv"] = data["valuesCSV"]        
+        if "onCount" in data:
+            args["on_count"] = data["onCount"]
+        if "offCount" in data:
+            args["off_count"] = data["offCount"]
+        if "onValue" in data:
+            args["on_value"] = data["onValue"]
+        if "offValue" in data:
+            args["off_value"] = data["offValue"]        
 
         return cls(**args)
 
 
-class Datasource:
-    # The datasource plugin type
-    type_val: str
-    # Datasource UID
-    uid: typing.Optional[str]
+class SimulationQuery:
+    key: 'Key'
+    config: typing.Optional[object]
+    stream: typing.Optional[bool]
+    last: typing.Optional[bool]
 
-    def __init__(self, type_val: str = "", uid: typing.Optional[str] = None):
-        self.type_val = type_val
-        self.uid = uid
+    def __init__(self, key: typing.Optional['Key'] = None, config: typing.Optional[object] = None, stream: typing.Optional[bool] = None, last: typing.Optional[bool] = None):
+        self.key = key if key is not None else Key()
+        self.config = config
+        self.stream = stream
+        self.last = last
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "type": self.type_val,
+            "key": self.key,
         }
-        if self.uid is not None:
-            payload["uid"] = self.uid
+        if self.config is not None:
+            payload["config"] = self.config
+        if self.stream is not None:
+            payload["stream"] = self.stream
+        if self.last is not None:
+            payload["last"] = self.last
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "type" in data:
-            args["type_val"] = data["type"]
-        if "uid" in data:
-            args["uid"] = data["uid"]        
+        if "key" in data:
+            args["key"] = Key.from_json(data["key"])
+        if "config" in data:
+            args["config"] = data["config"]
+        if "stream" in data:
+            args["stream"] = data["stream"]
+        if "last" in data:
+            args["last"] = data["last"]        
 
         return cls(**args)
 
 
 class NodesQuery:
+    type_val: typing.Optional[typing.Literal["random", "response_small", "response_medium", "random edges"]]
     count: typing.Optional[int]
     seed: typing.Optional[int]
-    # Possible enum values:
-    #  - `"random"` 
-    #  - `"random edges"` 
-    #  - `"response_medium"` 
-    #  - `"response_small"` 
-    #  - `"feature_showcase"` 
-    type_val: typing.Optional[typing.Literal["random", "random edges", "response_medium", "response_small", "feature_showcase"]]
 
-    def __init__(self, count: typing.Optional[int] = None, seed: typing.Optional[int] = None, type_val: typing.Optional[typing.Literal["random", "random edges", "response_medium", "response_small", "feature_showcase"]] = None):
+    def __init__(self, type_val: typing.Optional[typing.Literal["random", "response_small", "response_medium", "random edges"]] = None, count: typing.Optional[int] = None, seed: typing.Optional[int] = None):
+        self.type_val = type_val
         self.count = count
         self.seed = seed
-        self.type_val = type_val
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
+        if self.type_val is not None:
+            payload["type"] = self.type_val
         if self.count is not None:
             payload["count"] = self.count
         if self.seed is not None:
             payload["seed"] = self.seed
-        if self.type_val is not None:
-            payload["type"] = self.type_val
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
+        if "type" in data:
+            args["type_val"] = data["type"]
         if "count" in data:
             args["count"] = data["count"]
         if "seed" in data:
-            args["seed"] = data["seed"]
-        if "type" in data:
-            args["type_val"] = data["type"]        
+            args["seed"] = data["seed"]        
 
         return cls(**args)
 
 
-class PulseWaveQuery:
-    off_count: typing.Optional[int]
-    off_value: typing.Optional[float]
-    on_count: typing.Optional[int]
-    on_value: typing.Optional[float]
-    time_step: typing.Optional[int]
+class USAQuery:
+    mode: typing.Optional[str]
+    period: typing.Optional[str]
+    fields: typing.Optional[list[str]]
+    states: typing.Optional[list[str]]
 
-    def __init__(self, off_count: typing.Optional[int] = None, off_value: typing.Optional[float] = None, on_count: typing.Optional[int] = None, on_value: typing.Optional[float] = None, time_step: typing.Optional[int] = None):
-        self.off_count = off_count
-        self.off_value = off_value
-        self.on_count = on_count
-        self.on_value = on_value
-        self.time_step = time_step
+    def __init__(self, mode: typing.Optional[str] = None, period: typing.Optional[str] = None, fields: typing.Optional[list[str]] = None, states: typing.Optional[list[str]] = None):
+        self.mode = mode
+        self.period = period
+        self.fields = fields
+        self.states = states
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
-        if self.off_count is not None:
-            payload["offCount"] = self.off_count
-        if self.off_value is not None:
-            payload["offValue"] = self.off_value
-        if self.on_count is not None:
-            payload["onCount"] = self.on_count
-        if self.on_value is not None:
-            payload["onValue"] = self.on_value
-        if self.time_step is not None:
-            payload["timeStep"] = self.time_step
+        if self.mode is not None:
+            payload["mode"] = self.mode
+        if self.period is not None:
+            payload["period"] = self.period
+        if self.fields is not None:
+            payload["fields"] = self.fields
+        if self.states is not None:
+            payload["states"] = self.states
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "offCount" in data:
-            args["off_count"] = data["offCount"]
-        if "offValue" in data:
-            args["off_value"] = data["offValue"]
-        if "onCount" in data:
-            args["on_count"] = data["onCount"]
-        if "onValue" in data:
-            args["on_value"] = data["onValue"]
-        if "timeStep" in data:
-            args["time_step"] = data["timeStep"]        
+        if "mode" in data:
+            args["mode"] = data["mode"]
+        if "period" in data:
+            args["period"] = data["period"]
+        if "fields" in data:
+            args["fields"] = data["fields"]
+        if "states" in data:
+            args["states"] = data["states"]        
 
         return cls(**args)
 
 
-class ResultAssertions:
-    # Maximum frame count
-    max_frames: typing.Optional[int]
-    # Type asserts that the frame matches a known type structure.
-    # Possible enum values:
-    #  - `""` 
-    #  - `"timeseries-wide"` 
-    #  - `"timeseries-long"` 
-    #  - `"timeseries-many"` 
-    #  - `"timeseries-multi"` 
-    #  - `"directory-listing"` 
-    #  - `"table"` 
-    #  - `"numeric-wide"` 
-    #  - `"numeric-multi"` 
-    #  - `"numeric-long"` 
-    #  - `"log-lines"` 
-    type_val: typing.Optional[typing.Literal["", "timeseries-wide", "timeseries-long", "timeseries-many", "timeseries-multi", "directory-listing", "table", "numeric-wide", "numeric-multi", "numeric-long", "log-lines"]]
-    # TypeVersion is the version of the Type property. Versions greater than 0.0 correspond to the dataplane
-    # contract documentation https://grafana.github.io/dataplane/contract/.
-    type_version: list[int]
+class CSVWave:
+    time_step: typing.Optional[int]
+    name: typing.Optional[str]
+    values_csv: typing.Optional[str]
+    labels: typing.Optional[str]
 
-    def __init__(self, max_frames: typing.Optional[int] = None, type_val: typing.Optional[typing.Literal["", "timeseries-wide", "timeseries-long", "timeseries-many", "timeseries-multi", "directory-listing", "table", "numeric-wide", "numeric-multi", "numeric-long", "log-lines"]] = None, type_version: typing.Optional[list[int]] = None):
-        self.max_frames = max_frames
-        self.type_val = type_val
-        self.type_version = type_version if type_version is not None else []
+    def __init__(self, time_step: typing.Optional[int] = None, name: typing.Optional[str] = None, values_csv: typing.Optional[str] = None, labels: typing.Optional[str] = None):
+        self.time_step = time_step
+        self.name = name
+        self.values_csv = values_csv
+        self.labels = labels
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "typeVersion": self.type_version,
         }
-        if self.max_frames is not None:
-            payload["maxFrames"] = self.max_frames
-        if self.type_val is not None:
-            payload["type"] = self.type_val
+        if self.time_step is not None:
+            payload["timeStep"] = self.time_step
+        if self.name is not None:
+            payload["name"] = self.name
+        if self.values_csv is not None:
+            payload["valuesCSV"] = self.values_csv
+        if self.labels is not None:
+            payload["labels"] = self.labels
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "maxFrames" in data:
-            args["max_frames"] = data["maxFrames"]
-        if "type" in data:
-            args["type_val"] = data["type"]
-        if "typeVersion" in data:
-            args["type_version"] = data["typeVersion"]        
+        if "timeStep" in data:
+            args["time_step"] = data["timeStep"]
+        if "name" in data:
+            args["name"] = data["name"]
+        if "valuesCSV" in data:
+            args["values_csv"] = data["valuesCSV"]
+        if "labels" in data:
+            args["labels"] = data["labels"]        
 
         return cls(**args)
 
 
-class Key:
-    tick: float
-    type_val: str
-    uid: typing.Optional[str]
+class Scenario:
+    """
+    TODO: Should this live here given it's not used in the dataquery?
+    """
 
-    def __init__(self, tick: float = 0, type_val: str = "", uid: typing.Optional[str] = None):
-        self.tick = tick
-        self.type_val = type_val
-        self.uid = uid
+    id_val: str
+    name: str
+    string_input: str
+    description: typing.Optional[str]
+    hide_alias_field: typing.Optional[bool]
+
+    def __init__(self, id_val: str = "", name: str = "", string_input: str = "", description: typing.Optional[str] = None, hide_alias_field: typing.Optional[bool] = None):
+        self.id_val = id_val
+        self.name = name
+        self.string_input = string_input
+        self.description = description
+        self.hide_alias_field = hide_alias_field
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "tick": self.tick,
-            "type": self.type_val,
+            "id": self.id_val,
+            "name": self.name,
+            "stringInput": self.string_input,
         }
-        if self.uid is not None:
-            payload["uid"] = self.uid
+        if self.description is not None:
+            payload["description"] = self.description
+        if self.hide_alias_field is not None:
+            payload["hideAliasField"] = self.hide_alias_field
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "tick" in data:
-            args["tick"] = data["tick"]
-        if "type" in data:
-            args["type_val"] = data["type"]
-        if "uid" in data:
-            args["uid"] = data["uid"]        
+        if "id" in data:
+            args["id_val"] = data["id"]
+        if "name" in data:
+            args["name"] = data["name"]
+        if "stringInput" in data:
+            args["string_input"] = data["stringInput"]
+        if "description" in data:
+            args["description"] = data["description"]
+        if "hideAliasField" in data:
+            args["hide_alias_field"] = data["hideAliasField"]        
 
         return cls(**args)
 
 
-class SimulationQuery:
-    config: typing.Optional[object]
-    key: 'Key'
-    last: typing.Optional[bool]
-    stream: typing.Optional[bool]
+class Dataquery(cogvariants.Dataquery):
+    alias: typing.Optional[str]
+    scenario_id: typing.Optional['TestDataQueryType']
+    string_input: typing.Optional[str]
+    stream: typing.Optional['StreamingQuery']
+    pulse_wave: typing.Optional['PulseWaveQuery']
+    sim: typing.Optional['SimulationQuery']
+    csv_wave: typing.Optional[list['CSVWave']]
+    labels: typing.Optional[str]
+    lines: typing.Optional[int]
+    level_column: typing.Optional[bool]
+    channel: typing.Optional[str]
+    nodes: typing.Optional['NodesQuery']
+    csv_file_name: typing.Optional[str]
+    csv_content: typing.Optional[str]
+    raw_frame_content: typing.Optional[str]
+    series_count: typing.Optional[int]
+    usa: typing.Optional['USAQuery']
+    error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]]
+    span_count: typing.Optional[int]
+    points: typing.Optional[list[list[typing.Union[str, int]]]]
+    # Drop percentage (the chance we will lose a point 0-100)
+    drop_percent: typing.Optional[float]
+    flamegraph_diff: typing.Optional[bool]
+    # A unique identifier for the query within the list of targets.
+    # In server side expressions, the refId is used as a variable name to identify results.
+    # By default, the UI will assign A->Z; however setting meaningful names may be useful.
+    ref_id: typing.Optional[str]
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
+    hide: typing.Optional[bool]
+    # Specify the query flavor
+    # TODO make this required and give it a default
+    query_type: typing.Optional[str]
+    # For mixed data sources the selected datasource is on the query level.
+    # For non mixed scenarios this is undefined.
+    # TODO find a better way to do this ^ that's friendly to schema
+    # TODO this shouldn't be unknown but DataSourceRef | null
+    datasource: typing.Optional[object]
 
-    def __init__(self, config: typing.Optional[object] = None, key: typing.Optional['Key'] = None, last: typing.Optional[bool] = None, stream: typing.Optional[bool] = None):
-        self.config = config
-        self.key = key if key is not None else Key()
-        self.last = last
+    def __init__(self, alias: typing.Optional[str] = None, scenario_id: typing.Optional['TestDataQueryType'] = None, string_input: typing.Optional[str] = None, stream: typing.Optional['StreamingQuery'] = None, pulse_wave: typing.Optional['PulseWaveQuery'] = None, sim: typing.Optional['SimulationQuery'] = None, csv_wave: typing.Optional[list['CSVWave']] = None, labels: typing.Optional[str] = None, lines: typing.Optional[int] = None, level_column: typing.Optional[bool] = None, channel: typing.Optional[str] = None, nodes: typing.Optional['NodesQuery'] = None, csv_file_name: typing.Optional[str] = None, csv_content: typing.Optional[str] = None, raw_frame_content: typing.Optional[str] = None, series_count: typing.Optional[int] = None, usa: typing.Optional['USAQuery'] = None, error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]] = None, span_count: typing.Optional[int] = None, points: typing.Optional[list[list[typing.Union[str, int]]]] = None, drop_percent: typing.Optional[float] = None, flamegraph_diff: typing.Optional[bool] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
+        self.alias = alias
+        self.scenario_id = scenario_id if scenario_id is not None else TestDataQueryType.RANDOM_WALK
+        self.string_input = string_input
         self.stream = stream
+        self.pulse_wave = pulse_wave
+        self.sim = sim
+        self.csv_wave = csv_wave
+        self.labels = labels
+        self.lines = lines
+        self.level_column = level_column
+        self.channel = channel
+        self.nodes = nodes
+        self.csv_file_name = csv_file_name
+        self.csv_content = csv_content
+        self.raw_frame_content = raw_frame_content
+        self.series_count = series_count
+        self.usa = usa
+        self.error_type = error_type
+        self.span_count = span_count
+        self.points = points
+        self.drop_percent = drop_percent
+        self.flamegraph_diff = flamegraph_diff
+        self.ref_id = ref_id
+        self.hide = hide
+        self.query_type = query_type
+        self.datasource = datasource
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "key": self.key,
         }
-        if self.config is not None:
-            payload["config"] = self.config
-        if self.last is not None:
-            payload["last"] = self.last
+        if self.alias is not None:
+            payload["alias"] = self.alias
+        if self.scenario_id is not None:
+            payload["scenarioId"] = self.scenario_id
+        if self.string_input is not None:
+            payload["stringInput"] = self.string_input
         if self.stream is not None:
             payload["stream"] = self.stream
+        if self.pulse_wave is not None:
+            payload["pulseWave"] = self.pulse_wave
+        if self.sim is not None:
+            payload["sim"] = self.sim
+        if self.csv_wave is not None:
+            payload["csvWave"] = self.csv_wave
+        if self.labels is not None:
+            payload["labels"] = self.labels
+        if self.lines is not None:
+            payload["lines"] = self.lines
+        if self.level_column is not None:
+            payload["levelColumn"] = self.level_column
+        if self.channel is not None:
+            payload["channel"] = self.channel
+        if self.nodes is not None:
+            payload["nodes"] = self.nodes
+        if self.csv_file_name is not None:
+            payload["csvFileName"] = self.csv_file_name
+        if self.csv_content is not None:
+            payload["csvContent"] = self.csv_content
+        if self.raw_frame_content is not None:
+            payload["rawFrameContent"] = self.raw_frame_content
+        if self.series_count is not None:
+            payload["seriesCount"] = self.series_count
+        if self.usa is not None:
+            payload["usa"] = self.usa
+        if self.error_type is not None:
+            payload["errorType"] = self.error_type
+        if self.span_count is not None:
+            payload["spanCount"] = self.span_count
+        if self.points is not None:
+            payload["points"] = self.points
+        if self.drop_percent is not None:
+            payload["dropPercent"] = self.drop_percent
+        if self.flamegraph_diff is not None:
+            payload["flamegraphDiff"] = self.flamegraph_diff
+        if self.ref_id is not None:
+            payload["refId"] = self.ref_id
+        if self.hide is not None:
+            payload["hide"] = self.hide
+        if self.query_type is not None:
+            payload["queryType"] = self.query_type
+        if self.datasource is not None:
+            payload["datasource"] = self.datasource
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "config" in data:
-            args["config"] = data["config"]
-        if "key" in data:
-            args["key"] = Key.from_json(data["key"])
-        if "last" in data:
-            args["last"] = data["last"]
+        if "alias" in data:
+            args["alias"] = data["alias"]
+        if "scenarioId" in data:
+            args["scenario_id"] = data["scenarioId"]
+        if "stringInput" in data:
+            args["string_input"] = data["stringInput"]
         if "stream" in data:
-            args["stream"] = data["stream"]        
+            args["stream"] = StreamingQuery.from_json(data["stream"])
+        if "pulseWave" in data:
+            args["pulse_wave"] = PulseWaveQuery.from_json(data["pulseWave"])
+        if "sim" in data:
+            args["sim"] = SimulationQuery.from_json(data["sim"])
+        if "csvWave" in data:
+            args["csv_wave"] = data["csvWave"]
+        if "labels" in data:
+            args["labels"] = data["labels"]
+        if "lines" in data:
+            args["lines"] = data["lines"]
+        if "levelColumn" in data:
+            args["level_column"] = data["levelColumn"]
+        if "channel" in data:
+            args["channel"] = data["channel"]
+        if "nodes" in data:
+            args["nodes"] = NodesQuery.from_json(data["nodes"])
+        if "csvFileName" in data:
+            args["csv_file_name"] = data["csvFileName"]
+        if "csvContent" in data:
+            args["csv_content"] = data["csvContent"]
+        if "rawFrameContent" in data:
+            args["raw_frame_content"] = data["rawFrameContent"]
+        if "seriesCount" in data:
+            args["series_count"] = data["seriesCount"]
+        if "usa" in data:
+            args["usa"] = USAQuery.from_json(data["usa"])
+        if "errorType" in data:
+            args["error_type"] = data["errorType"]
+        if "spanCount" in data:
+            args["span_count"] = data["spanCount"]
+        if "points" in data:
+            args["points"] = data["points"]
+        if "dropPercent" in data:
+            args["drop_percent"] = data["dropPercent"]
+        if "flamegraphDiff" in data:
+            args["flamegraph_diff"] = data["flamegraphDiff"]
+        if "refId" in data:
+            args["ref_id"] = data["refId"]
+        if "hide" in data:
+            args["hide"] = data["hide"]
+        if "queryType" in data:
+            args["query_type"] = data["queryType"]
+        if "datasource" in data:
+            args["datasource"] = data["datasource"]        
 
         return cls(**args)
 
 
-class StreamingQuery:
-    bands: typing.Optional[int]
-    noise: float
-    speed: float
-    spread: float
-    # Possible enum values:
-    #  - `"fetch"` 
-    #  - `"logs"` 
-    #  - `"signal"` 
-    #  - `"traces"` 
-    type_val: typing.Literal["fetch", "logs", "signal", "traces"]
-    url: typing.Optional[str]
+def variant_config() -> cogruntime.DataqueryConfig:
+    return cogruntime.DataqueryConfig(
+        identifier="testdata",
+        from_json_hook=Dataquery.from_json,
+    )
 
-    def __init__(self, bands: typing.Optional[int] = None, noise: float = 0, speed: float = 0, spread: float = 0, type_val: typing.Optional[typing.Literal["fetch", "logs", "signal", "traces"]] = None, url: typing.Optional[str] = None):
-        self.bands = bands
-        self.noise = noise
-        self.speed = speed
-        self.spread = spread
-        self.type_val = type_val if type_val is not None else "fetch"
-        self.url = url
+
+class Key:
+    type_val: str
+    tick: float
+    uid: typing.Optional[str]
+
+    def __init__(self, type_val: str = "", tick: float = 0, uid: typing.Optional[str] = None):
+        self.type_val = type_val
+        self.tick = tick
+        self.uid = uid
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "noise": self.noise,
-            "speed": self.speed,
-            "spread": self.spread,
             "type": self.type_val,
+            "tick": self.tick,
         }
-        if self.bands is not None:
-            payload["bands"] = self.bands
-        if self.url is not None:
-            payload["url"] = self.url
+        if self.uid is not None:
+            payload["uid"] = self.uid
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "bands" in data:
-            args["bands"] = data["bands"]
-        if "noise" in data:
-            args["noise"] = data["noise"]
-        if "speed" in data:
-            args["speed"] = data["speed"]
-        if "spread" in data:
-            args["spread"] = data["spread"]
         if "type" in data:
             args["type_val"] = data["type"]
-        if "url" in data:
-            args["url"] = data["url"]        
-
-        return cls(**args)
-
-
-class TimeRange:
-    # From is the start time of the query.
-    from_val: str
-    # To is the end time of the query.
-    to: str
-
-    def __init__(self, from_val: str = "now-6h", to: str = "now"):
-        self.from_val = from_val
-        self.to = to
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "from": self.from_val,
-            "to": self.to,
-        }
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "from" in data:
-            args["from_val"] = data["from"]
-        if "to" in data:
-            args["to"] = data["to"]        
-
-        return cls(**args)
-
-
-class USAQuery:
-    fields: typing.Optional[list[str]]
-    mode: typing.Optional[str]
-    period: typing.Optional[str]
-    states: typing.Optional[list[str]]
-
-    def __init__(self, fields: typing.Optional[list[str]] = None, mode: typing.Optional[str] = None, period: typing.Optional[str] = None, states: typing.Optional[list[str]] = None):
-        self.fields = fields
-        self.mode = mode
-        self.period = period
-        self.states = states
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-        }
-        if self.fields is not None:
-            payload["fields"] = self.fields
-        if self.mode is not None:
-            payload["mode"] = self.mode
-        if self.period is not None:
-            payload["period"] = self.period
-        if self.states is not None:
-            payload["states"] = self.states
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "fields" in data:
-            args["fields"] = data["fields"]
-        if "mode" in data:
-            args["mode"] = data["mode"]
-        if "period" in data:
-            args["period"] = data["period"]
-        if "states" in data:
-            args["states"] = data["states"]        
+        if "tick" in data:
+            args["tick"] = data["tick"]
+        if "uid" in data:
+            args["uid"] = data["uid"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/text.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/timeseries.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/timeseries.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,45 +5,39 @@
 from ..cog import runtime as cogruntime
 
 
 class Options:
     timezone: typing.Optional[list[common.TimeZone]]
     legend: common.VizLegendOptions
     tooltip: common.VizTooltipOptions
-    orientation: typing.Optional[common.VizOrientation]
 
-    def __init__(self, timezone: typing.Optional[list[common.TimeZone]] = None, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, orientation: typing.Optional[common.VizOrientation] = None):
+    def __init__(self, timezone: typing.Optional[list[common.TimeZone]] = None, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None):
         self.timezone = timezone
         self.legend = legend if legend is not None else common.VizLegendOptions(calcs=[], display_mode=common.LegendDisplayMode.LIST, placement=common.LegendPlacement.BOTTOM)
         self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
-        self.orientation = orientation
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "legend": self.legend,
             "tooltip": self.tooltip,
         }
         if self.timezone is not None:
             payload["timezone"] = self.timezone
-        if self.orientation is not None:
-            payload["orientation"] = self.orientation
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "timezone" in data:
             args["timezone"] = data["timezone"]
         if "legend" in data:
             args["legend"] = common.VizLegendOptions.from_json(data["legend"])
         if "tooltip" in data:
-            args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])
-        if "orientation" in data:
-            args["orientation"] = data["orientation"]        
+            args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])        
 
         return cls(**args)
 
 
 FieldConfig: typing.TypeAlias = common.GraphFieldConfig
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/trend.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/trend.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/grafana_foundation_sdk/models/xychart.py` & `grafana_foundation_sdk-1716894270!10.4.0/grafana_foundation_sdk/models/xychart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/LICENSE.md` & `grafana_foundation_sdk-1716894270!10.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/README.md` & `grafana_foundation_sdk-1716894270!10.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v11.0.x.**
+> This branch contains **types and builders generated for Grafana v10.4.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1716894257!11.0.0'
+python3 -m pip install 'grafana_foundation_sdk==1716894270!10.4.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/pyproject.toml` & `grafana_foundation_sdk-1716894270!10.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "observability",
     "sdk",
     "grafana",
     "logs",
     "traces",
     "metrics"
 ]
-version = "1716894257!11.0.0"
+version = "1716894270!10.4.0"
 dependencies = []
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `grafana_foundation_sdk-1716894257!11.0.0/PKG-INFO` & `grafana_foundation_sdk-1716894270!10.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grafana_foundation_sdk
-Version: 1716894257!11.0.0
+Version: 1716894270!10.4.0
 Summary: A set of tools, types and libraries for building and manipulating Grafana objects.
 Project-URL: Homepage, https://github.com/grafana/grafana-foundation-sdk
 Project-URL: Repository, https://github.com/grafana/grafana-foundation-sdk.git
 Project-URL: Issues, https://github.com/grafana/grafana-foundation-sdk/issues
 Author: Grafana Labs
 License-File: LICENSE.md
 Keywords: grafana,logs,metrics,observability,sdk,traces
@@ -21,21 +21,21 @@
 Description-Content-Type: text/markdown
 
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v11.0.x.**
+> This branch contains **types and builders generated for Grafana v10.4.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1716894257!11.0.0'
+python3 -m pip install 'grafana_foundation_sdk==1716894270!10.4.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

