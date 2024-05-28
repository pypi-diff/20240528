# Comparing `tmp/tiled-0.1.0b1.tar.gz` & `tmp/tiled-0.1.0b2.tar.gz`

## Comparing `tiled-0.1.0b1.tar` & `tiled-0.1.0b2.tar`

### file list

```diff
@@ -1,443 +1,445 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.codecov.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.coveragerc
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.git_archival.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.gitattributes
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.isort.cfg
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.mypy.ini
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 tiled-0.1.0b1/CHANGELOG.md
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 tiled-0.1.0b1/Dockerfile
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 tiled-0.1.0b1/asv.conf.json
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 tiled-0.1.0b1/canary-validator.yml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docker-compose.yml
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_log_config.yml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tiled-0.1.0b1/pytest.ini
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.github/pull_request_template.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.github/workflows/build-and-validate-image.yml
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.github/workflows/publish-image.yml
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/benchmarks/__init__.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 tiled-0.1.0b1/benchmarks/benchmarks.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 tiled-0.1.0b1/continuous_integration/docker-configs/ldap-docker-compose.yml
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 tiled-0.1.0b1/continuous_integration/scripts/download_sqlite_data.sh
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 tiled-0.1.0b1/continuous_integration/scripts/install.sh
--rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 tiled-0.1.0b1/continuous_integration/scripts/start_LDAP.sh
--rwxr-xr-x   0        0        0      447 2020-02-02 00:00:00.000000 tiled-0.1.0b1/continuous_integration/scripts/start_postgres.sh
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/Makefile
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/make.bat
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/conf.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/_static/.placeholder
--rw-r--r--   0        0        0   521536 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/_static/grafana-screenshot.png
--rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/_static/orcid-authorize.png
--rw-r--r--   0        0        0    39311 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/_static/orcid-login.png
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/access-control.md
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/architecture.md
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/caching.md
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/catalog.md
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/compression.md
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/faq.md
--rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/lineage.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/metadata.md
--rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/security.md
--rw-r--r--   0        0        0     8830 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/specialized-formats.md
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/standards.md
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/explanations/structures.md
--rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/api-keys.md
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/client-logger.md
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/configuration.md
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/custom-clients.md
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/custom-export-formats.md
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/direct-client.md
--rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/docker.md
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/metrics.md
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/profiles.md
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/read-custom-formats.md
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/register.md
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/how-to/tiled-authn-database.md
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/authentication.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/client-profiles-header.txt
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/commandline.md
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/http-api-overview.md
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/min-versions.rst
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/python-client.md
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/queries.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/release-history.rst
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/scopes.md
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/service-configuration-header.txt
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/reference/service.md
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/export.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/installation.rst
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/login.md
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/navigation.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/plotly-integration.md
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/search.md
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/serving-files.md
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/slicing.md
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 tiled-0.1.0b1/docs/source/tutorials/writing.md
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/google_auth.yml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/multiple_providers.yml
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/orcid_auth.yml
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/saml.yml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/single_catalog_single_user.yml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/small_single_user_demo.yml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/toy_authentication.yml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/custom_export_formats/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/custom_export_formats/custom_exporters.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/external_service/README.md
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/external_service/custom.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/simple_oidc/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/simple_oidc/oidc_provider_config.json
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tiled-0.1.0b1/example_configs/simple_oidc/users.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 tiled-0.1.0b1/monitoring_example/README.md
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 tiled-0.1.0b1/monitoring_example/grafana/main.yml
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 tiled-0.1.0b1/monitoring_example/grafana/dashboards/dashboard.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tiled-0.1.0b1/monitoring_example/grafana/provisioning/datasources/prometheus.yml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 tiled-0.1.0b1/monitoring_example/prometheus/prometheus.yml
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 tiled-0.1.0b1/scripts/json_indexes.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/.identifying_file_72628d5f953b4229b58c9f1f8f6a9a09
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/static/default_ui_settings.yml
--rw-r--r--   0        0        0    16958 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/static/favicon.ico
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/templates/device_code_failure.html
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/templates/device_code_form.html
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/templates/device_code_success.html
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/templates/index.html
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/templates/page.html
--rw-r--r--   0        0        0    16958 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/favicon.ico
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/index.html
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/manifest.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/robots.txt
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/Checkbox.841ff07f.js
--rw-r--r--   0        0        0   306714 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/DataGrid.b013c811.js
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/FormControlLabel.93f22896.js
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/FormGroup.25250c88.js
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/FormLabel.a3eda031.js
--rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/Input.ed778d26.js
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/ListItemIcon.fcfd88bf.js
--rw-r--r--   0        0        0    93768 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/TextField.8d6efd58.js
--rw-r--r--   0        0        0   382818 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/array-1d.0797372d.js
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/array-nd.16ddeaf4.js
--rw-r--r--   0        0        0    50971 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/browse.0916686d.js
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/choose-partition.93f44af2.js
--rw-r--r--   0        0        0  1027938 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/default-highlight.19f6d178.js
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/download-array.e7fdb5ff.js
--rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/download-core.1ace673a.js
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/download-node.acad50b8.js
--rw-r--r--   0        0        0    18381 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/download-table.e6c78057.js
--rw-r--r--   0        0        0   256242 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/index.72e24882.js
--rw-r--r--   0        0        0    16361 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/index.d49bee11.css
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/index.esm.31c0e330.js
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/json-viewer.c5226ec8.js
--rw-r--r--   0        0        0    40299 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/metadata-view.3cdbfa99.js
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/overview-array.ec18d178.js
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/overview-generic-node.553dc45c.js
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/overview-table.75ff538b.js
--rw-r--r--   0        0        0    65164 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-all-300-normal.6d79427c.woff
--rw-r--r--   0        0        0    65456 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-all-400-normal.e41533d5.woff
--rw-r--r--   0        0        0    65756 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-all-500-normal.8f838c80.woff
--rw-r--r--   0        0        0    65556 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-all-700-normal.b5883883.woff
--rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-300-normal.47aa3bfa.woff2
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-400-normal.495d38d4.woff2
--rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-500-normal.3728fbdd.woff2
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-700-normal.6a84eeee.woff2
--rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-ext-300-normal.435e4b7f.woff2
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-ext-400-normal.b7ef2cd1.woff2
--rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-ext-500-normal.aeed0e51.woff2
--rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-ext-700-normal.3c505383.woff2
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-greek-300-normal.455c2c1a.woff2
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-greek-400-normal.daf51ab5.woff2
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-greek-500-normal.713780d8.woff2
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-greek-700-normal.1c9cc76f.woff2
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-300-normal.f7591131.woff2
--rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-400-normal.f6734f81.woff2
--rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-500-normal.b0195382.woff2
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-700-normal.f5aebdfe.woff2
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-ext-300-normal.b076e863.woff2
--rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-ext-400-normal.3c23eb02.woff2
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-ext-500-normal.7f1c829b.woff2
--rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-ext-700-normal.fc66f942.woff2
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-vietnamese-300-normal.51f3f418.woff2
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-vietnamese-400-normal.77b24796.woff2
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-vietnamese-500-normal.0948409a.woff2
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/roboto-vietnamese-700-normal.4ec57f2a.woff2
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 tiled-0.1.0b1/share/tiled/ui/assets/toPropertyKey.012fc217.js
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/__main__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_version.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/access_policies.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/alembic_utils.py
--rw-r--r--   0        0        0    33555 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authenticators.py
--rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/config.py
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/iterviews.py
--rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/media_type_registration.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/mimetypes.py
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/profiles.py
--rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/queries.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/query_registration.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/scopes.py
--rw-r--r--   0        0        0    21974 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/utils.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/validation_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/__init__.py
--rw-r--r--   0        0        0     7750 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/conftest.py
--rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_access_control.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_allow_origins.py
--rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_array.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_asset_access.py
--rw-r--r--   0        0        0    26064 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_authentication.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_authenticators.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_awkward.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_caches.py
--rw-r--r--   0        0        0    17936 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_catalog.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_cli.py
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_client.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_client_cache.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_client_smoke.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_compression.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_config.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_container_fields.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_container_files.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_custom_format.py
--rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_dataframe.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_decoders.py
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_directory_walker.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_distinct.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_export.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_hdf5.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_history.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_import_object.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_indexers.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_inlined_contents.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_json.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_metrics.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_no_heavy_imports.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_openapi.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_pickle.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_profiles.py
--rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_protocols.py
--rw-r--r--   0        0        0    11221 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_queries.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_register.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_resource_cache.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_routes.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_scaled_config_option.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_search.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_select_metadata.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_sentinel.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_size_limit.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_sort.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_sparse.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_specs.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_structured_array.py
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_sync.py
--rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_tiff.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_tokenize.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_validation.py
--rw-r--r--   0        0        0    19202 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_writing.py
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_xarray.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/sql/__init__.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/sql/before_creating_fts5_virtual_table.sql
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_configs/config_missing_api_key.yml
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_configs/config_missing_secret_keys.yml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_configs/config_missing_secret_keys_public.yml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_configs/config_public_no_authenticator.yml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_configs/config_with_api_key.yml
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/_tests/test_configs/config_with_secret_keys.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/__init__.py
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/array.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/awkward.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/awkward_buffers.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/awkward_directory_container.py
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/csv.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/dataframe.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/excel.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/files.py
--rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/hdf5.py
--rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/mapping.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/netcdf.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/parquet.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/protocols.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/resource_cache.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/sparse.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/sparse_blocks_parquet.py
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/table.py
--rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/tiff.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/type_alliases.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/utils.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/xarray.py
--rw-r--r--   0        0        0     8743 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/adapters/zarr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/__init__.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/__main__.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/alembic.ini.template
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/alembic_constants.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/base.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/connection_pool.py
--rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/core.py
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/orm.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/README
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/script.py.mako
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/versions/13024b8a6b74_add_register_scope_to_default_roles.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/versions/481830dd6c11_initialize.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/versions/4a9dfaba4a98_add_pendingsession.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/versions/769180ce732e_add_write_principals_scope_to_admin.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/authn_database/migrations/versions/c7bd2573716d_add_session_state_column.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/__init__.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/__main__.py
--rw-r--r--   0        0        0    54868 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/adapter.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/alembic.ini.template
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/alembic_constants.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/base.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/core.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/explain.py
--rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/orm.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/utils.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/README
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/script.py.mako
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/0b033e7fbe30_add_awkward_to_structurefamily_enum.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/1cd99c02d0c7_create_index_for_fulltext_search.py
--rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/2ca16566d692_separate_structure_table.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/3db11ff95b6c_changing_top_level_metadata_to_btree_gin.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/6825c778aa3c_initialize.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/83889e049ddc_add_table_to_structurefamily_enum.py
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/a66028395cab_enrich_datasource_asset_association.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/e756b9381c14_add_structure_family_to_data_sources.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/catalog/migrations/versions/ed3a4223a600_create_sqlite_table_for_fulltext_search.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/CACHEY_LICENSE.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/__init__.py
--rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/array.py
--rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/auth.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/awkward.py
--rw-r--r--   0        0        0    15285 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/base.py
--rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/cache.py
--rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/cache_control.py
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/constructors.py
--rw-r--r--   0        0        0    38030 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/container.py
--rw-r--r--   0        0        0    32235 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/context.py
--rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/dataframe.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/decoders.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/download.py
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/logger.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/node.py
--rw-r--r--   0        0        0    18859 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/register.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/smoke.py
--rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/sparse.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/sync.py
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/transport.py
--rw-r--r--   0        0        0    10618 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/utils.py
--rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/client/xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/__init__.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/_admin.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/_api_key.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/_catalog.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/_profile.py
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/_register.py
--rw-r--r--   0        0        0    21272 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/_serve.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/_utils.py
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/commandline/main.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/config_schemas/client_profiles.yml
--rw-r--r--   0        0        0    16258 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/config_schemas/service_configuration.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/examples/__init__.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/examples/generate_files.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/examples/generated.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/examples/generated_minimal.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/examples/nexus.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/examples/numpy_structured_dtypes.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/examples/toy_authentication.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/examples/xdi.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/__init__.py
--rw-r--r--   0        0        0    88253 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/_zipfile_py39.py
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/array.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/awkward.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/container.py
--rw-r--r--   0        0        0    12933 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/image_serializer_helpers.py
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/scikit-image-LICENSE.txt
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/sparse.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/table.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/serialization/xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/__init__.py
--rw-r--r--   0        0        0    38276 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/app.py
--rw-r--r--   0        0        0    42177 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/authentication.py
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/compression.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/core.py
--rw-r--r--   0        0        0     6642 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/dependencies.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/etag.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/links.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/metrics.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/protocols.py
--rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/pydantic_array.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/pydantic_awkward.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/pydantic_sparse.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/pydantic_table.py
--rw-r--r--   0        0        0    56890 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/router.py
--rw-r--r--   0        0        0    13961 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/schemas.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/settings.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/server/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/structures/__init__.py
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/structures/array.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/structures/awkward.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/structures/core.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/structures/data_source.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/structures/sparse.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 tiled-0.1.0b1/tiled/structures/table.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/.eslintrc.json
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/.prettierignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/.prettierrc.json
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/README.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/import-sorter.json
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/index.html
--rw-r--r--   0        0        0   618647 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/package-lock.json
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/package.json
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/tsconfig.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/vite.config.js
--rw-r--r--   0        0        0    16958 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/public/favicon.ico
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/public/manifest.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/public/robots.txt
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/App.css
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/App.test.tsx
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/App.tsx
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/client.ts
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/clipboard-copy.d.ts
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/index.tsx
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/openapi_schemas.ts
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/settings.ts
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/setupTests.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/theme.ts
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/array-1d.tsx
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/array-nd.tsx
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/choose-partition.tsx
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/column-list.tsx
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/contents.tsx
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/cut-slider.tsx
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/download-array.tsx
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/download-core.tsx
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/download-node.tsx
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/download-table.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/error-boundary.tsx
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/json-viewer.tsx
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/line.tsx
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/metadata-view.tsx
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/node-breadcrumbs.tsx
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/node-contents.tsx
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/node-lazy-contents.tsx
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/overview-array.tsx
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/overview-generic-node.tsx
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/overview-table.tsx
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/range-slider.tsx
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/components/tiled-app-bar.tsx
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/context/settings.tsx
--rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 tiled-0.1.0b1/web-frontend/src/routes/browse.tsx
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tiled-0.1.0b1/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 tiled-0.1.0b1/LICENSE
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 tiled-0.1.0b1/README.md
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 tiled-0.1.0b1/hatch_build.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 tiled-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0    16858 2020-02-02 00:00:00.000000 tiled-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.codecov.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.coveragerc
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.flake8
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.git_archival.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.gitattributes
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.isort.cfg
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.mypy.ini
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 tiled-0.1.0b2/CHANGELOG.md
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 tiled-0.1.0b2/Dockerfile
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 tiled-0.1.0b2/asv.conf.json
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 tiled-0.1.0b2/canary-validator.yml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docker-compose.yml
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_log_config.yml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tiled-0.1.0b2/pytest.ini
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.github/pull_request_template.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.github/workflows/build-and-validate-image.yml
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.github/workflows/publish-image.yml
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/benchmarks/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 tiled-0.1.0b2/benchmarks/benchmarks.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 tiled-0.1.0b2/continuous_integration/docker-configs/ldap-docker-compose.yml
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 tiled-0.1.0b2/continuous_integration/scripts/download_sqlite_data.sh
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 tiled-0.1.0b2/continuous_integration/scripts/install.sh
+-rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 tiled-0.1.0b2/continuous_integration/scripts/start_LDAP.sh
+-rwxr-xr-x   0        0        0      447 2020-02-02 00:00:00.000000 tiled-0.1.0b2/continuous_integration/scripts/start_postgres.sh
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/Makefile
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/make.bat
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/conf.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0   521536 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/_static/grafana-screenshot.png
+-rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/_static/orcid-authorize.png
+-rw-r--r--   0        0        0    39311 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/_static/orcid-login.png
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/access-control.md
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/architecture.md
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/caching.md
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/catalog.md
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/compression.md
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/faq.md
+-rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/lineage.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/metadata.md
+-rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/security.md
+-rw-r--r--   0        0        0     8830 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/specialized-formats.md
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/standards.md
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/explanations/structures.md
+-rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/api-keys.md
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/client-logger.md
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/configuration.md
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/custom-clients.md
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/custom-export-formats.md
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/direct-client.md
+-rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/docker.md
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/metrics.md
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/profiles.md
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/read-custom-formats.md
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/register.md
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/how-to/tiled-authn-database.md
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/authentication.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/client-profiles-header.txt
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/commandline.md
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/http-api-overview.md
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/min-versions.rst
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/python-client.md
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/queries.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/release-history.rst
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/scopes.md
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/service-configuration-header.txt
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/reference/service.md
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/export.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/installation.rst
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/login.md
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/navigation.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/plotly-integration.md
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/search.md
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/serving-files.md
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/slicing.md
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 tiled-0.1.0b2/docs/source/tutorials/writing.md
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/google_auth.yml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/multiple_providers.yml
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/orcid_auth.yml
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/saml.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/single_catalog_single_user.yml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/small_single_user_demo.yml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/toy_authentication.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/custom_export_formats/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/custom_export_formats/custom_exporters.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/external_service/README.md
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/external_service/custom.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/simple_oidc/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/simple_oidc/oidc_provider_config.json
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tiled-0.1.0b2/example_configs/simple_oidc/users.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 tiled-0.1.0b2/monitoring_example/README.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 tiled-0.1.0b2/monitoring_example/grafana/main.yml
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 tiled-0.1.0b2/monitoring_example/grafana/dashboards/dashboard.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tiled-0.1.0b2/monitoring_example/grafana/provisioning/datasources/prometheus.yml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 tiled-0.1.0b2/monitoring_example/prometheus/prometheus.yml
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 tiled-0.1.0b2/scripts/json_indexes.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/.identifying_file_72628d5f953b4229b58c9f1f8f6a9a09
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/static/default_ui_settings.yml
+-rw-r--r--   0        0        0    16958 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/static/favicon.ico
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/templates/device_code_failure.html
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/templates/device_code_form.html
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/templates/device_code_success.html
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/templates/index.html
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/templates/page.html
+-rw-r--r--   0        0        0    16958 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/favicon.ico
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/index.html
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/manifest.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/robots.txt
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/Checkbox.841ff07f.js
+-rw-r--r--   0        0        0   306714 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/DataGrid.b013c811.js
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/FormControlLabel.93f22896.js
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/FormGroup.25250c88.js
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/FormLabel.a3eda031.js
+-rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/Input.ed778d26.js
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/ListItemIcon.fcfd88bf.js
+-rw-r--r--   0        0        0    93768 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/TextField.8d6efd58.js
+-rw-r--r--   0        0        0   382818 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/array-1d.0797372d.js
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/array-nd.16ddeaf4.js
+-rw-r--r--   0        0        0    50971 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/browse.0916686d.js
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/choose-partition.93f44af2.js
+-rw-r--r--   0        0        0  1027938 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/default-highlight.19f6d178.js
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/download-array.e7fdb5ff.js
+-rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/download-core.1ace673a.js
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/download-node.acad50b8.js
+-rw-r--r--   0        0        0    18381 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/download-table.e6c78057.js
+-rw-r--r--   0        0        0   256242 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/index.72e24882.js
+-rw-r--r--   0        0        0    16361 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/index.d49bee11.css
+-rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/index.esm.31c0e330.js
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/json-viewer.c5226ec8.js
+-rw-r--r--   0        0        0    40299 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/metadata-view.3cdbfa99.js
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/overview-array.ec18d178.js
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/overview-generic-node.553dc45c.js
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/overview-table.75ff538b.js
+-rw-r--r--   0        0        0    65164 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-all-300-normal.6d79427c.woff
+-rw-r--r--   0        0        0    65456 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-all-400-normal.e41533d5.woff
+-rw-r--r--   0        0        0    65756 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-all-500-normal.8f838c80.woff
+-rw-r--r--   0        0        0    65556 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-all-700-normal.b5883883.woff
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-300-normal.47aa3bfa.woff2
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-400-normal.495d38d4.woff2
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-500-normal.3728fbdd.woff2
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-700-normal.6a84eeee.woff2
+-rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-ext-300-normal.435e4b7f.woff2
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-ext-400-normal.b7ef2cd1.woff2
+-rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-ext-500-normal.aeed0e51.woff2
+-rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-ext-700-normal.3c505383.woff2
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-greek-300-normal.455c2c1a.woff2
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-greek-400-normal.daf51ab5.woff2
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-greek-500-normal.713780d8.woff2
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-greek-700-normal.1c9cc76f.woff2
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-300-normal.f7591131.woff2
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-400-normal.f6734f81.woff2
+-rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-500-normal.b0195382.woff2
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-700-normal.f5aebdfe.woff2
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-ext-300-normal.b076e863.woff2
+-rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-ext-400-normal.3c23eb02.woff2
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-ext-500-normal.7f1c829b.woff2
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-ext-700-normal.fc66f942.woff2
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-vietnamese-300-normal.51f3f418.woff2
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-vietnamese-400-normal.77b24796.woff2
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-vietnamese-500-normal.0948409a.woff2
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/roboto-vietnamese-700-normal.4ec57f2a.woff2
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 tiled-0.1.0b2/share/tiled/ui/assets/toPropertyKey.012fc217.js
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/__main__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_version.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/access_policies.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/alembic_utils.py
+-rw-r--r--   0        0        0    33555 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authenticators.py
+-rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/config.py
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/iterviews.py
+-rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/media_type_registration.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/mimetypes.py
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/profiles.py
+-rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/queries.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/query_registration.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/scopes.py
+-rw-r--r--   0        0        0    21974 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/utils.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/validation_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/__init__.py
+-rw-r--r--   0        0        0     7750 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/conftest.py
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_access_control.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_allow_origins.py
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_array.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_asset_access.py
+-rw-r--r--   0        0        0    26064 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_authentication.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_authenticators.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_awkward.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_caches.py
+-rw-r--r--   0        0        0    17936 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_catalog.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_cli.py
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_client.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_client_cache.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_client_smoke.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_compression.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_config.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_container_fields.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_container_files.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_custom_format.py
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_dataframe.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_decoders.py
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_directory_walker.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_distinct.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_export.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_hdf5.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_history.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_import_object.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_indexers.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_inlined_contents.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_json.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_metrics.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_no_heavy_imports.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_openapi.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_pickle.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_profiles.py
+-rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_protocols.py
+-rw-r--r--   0        0        0    11221 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_queries.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_register.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_resource_cache.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_routes.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_scaled_config_option.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_search.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_select_metadata.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_sentinel.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_size_limit.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_sort.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_sparse.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_specs.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_structured_array.py
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_sync.py
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_tiff.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_tokenize.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_validation.py
+-rw-r--r--   0        0        0    19202 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_writing.py
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_xarray.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/sql/__init__.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/sql/before_creating_fts5_virtual_table.sql
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_configs/config_missing_api_key.yml
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_configs/config_missing_secret_keys.yml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_configs/config_missing_secret_keys_public.yml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_configs/config_public_no_authenticator.yml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_configs/config_with_api_key.yml
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/_tests/test_configs/config_with_secret_keys.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/__init__.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/array.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/awkward.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/awkward_buffers.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/awkward_directory_container.py
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/csv.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/dataframe.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/excel.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/files.py
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/hdf5.py
+-rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/mapping.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/netcdf.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/parquet.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/protocols.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/resource_cache.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/sparse.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/sparse_blocks_parquet.py
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/table.py
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/tiff.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/type_alliases.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/utils.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/xarray.py
+-rw-r--r--   0        0        0     8743 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/adapters/zarr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/__init__.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/__main__.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/alembic.ini.template
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/alembic_constants.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/base.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/connection_pool.py
+-rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/core.py
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/orm.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/README
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/script.py.mako
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/versions/13024b8a6b74_add_register_scope_to_default_roles.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/versions/481830dd6c11_initialize.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/versions/4a9dfaba4a98_add_pendingsession.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/versions/769180ce732e_add_write_principals_scope_to_admin.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/authn_database/migrations/versions/c7bd2573716d_add_session_state_column.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/__init__.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/__main__.py
+-rw-r--r--   0        0        0    54868 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/adapter.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/alembic.ini.template
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/alembic_constants.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/base.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/core.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/explain.py
+-rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/orm.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/utils.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/README
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/script.py.mako
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/0b033e7fbe30_add_awkward_to_structurefamily_enum.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/1cd99c02d0c7_create_index_for_fulltext_search.py
+-rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/2ca16566d692_separate_structure_table.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/3db11ff95b6c_changing_top_level_metadata_to_btree_gin.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/6825c778aa3c_initialize.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/83889e049ddc_add_table_to_structurefamily_enum.py
+-rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/a66028395cab_enrich_datasource_asset_association.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/e756b9381c14_add_structure_family_to_data_sources.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/catalog/migrations/versions/ed3a4223a600_create_sqlite_table_for_fulltext_search.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/CACHEY_LICENSE.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/__init__.py
+-rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/array.py
+-rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/auth.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/awkward.py
+-rw-r--r--   0        0        0    15285 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/base.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/cache.py
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/cache_control.py
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/constructors.py
+-rw-r--r--   0        0        0    38030 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/container.py
+-rw-r--r--   0        0        0    32235 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/context.py
+-rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/dataframe.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/decoders.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/download.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/logger.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/node.py
+-rw-r--r--   0        0        0    18859 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/register.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/smoke.py
+-rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/sparse.py
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/sync.py
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/transport.py
+-rw-r--r--   0        0        0    10618 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/utils.py
+-rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/client/xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/__init__.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/_admin.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/_api_key.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/_catalog.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/_profile.py
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/_register.py
+-rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/_serve.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/_utils.py
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/commandline/main.py
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/config_schemas/client_profiles.yml
+-rw-r--r--   0        0        0    16258 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/config_schemas/service_configuration.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/examples/__init__.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/examples/generate_files.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/examples/generated.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/examples/generated_minimal.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/examples/nexus.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/examples/numpy_structured_dtypes.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/examples/toy_authentication.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/examples/xdi.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/__init__.py
+-rw-r--r--   0        0        0    88253 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/_zipfile_py39.py
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/array.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/awkward.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/container.py
+-rw-r--r--   0        0        0    12933 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/image_serializer_helpers.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/scikit-image-LICENSE.txt
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/sparse.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/table.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/serialization/xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/__init__.py
+-rw-r--r--   0        0        0    38813 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/app.py
+-rw-r--r--   0        0        0    42299 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/authentication.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/compression.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/core.py
+-rw-r--r--   0        0        0     6642 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/dependencies.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/etag.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/links.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/logging_config.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/metrics.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/principal_log_filter.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/protocols.py
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/pydantic_array.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/pydantic_awkward.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/pydantic_sparse.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/pydantic_table.py
+-rw-r--r--   0        0        0    56890 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/router.py
+-rw-r--r--   0        0        0    13961 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/schemas.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/settings.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/server/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/structures/__init__.py
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/structures/array.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/structures/awkward.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/structures/core.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/structures/data_source.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/structures/sparse.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 tiled-0.1.0b2/tiled/structures/table.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/.eslintrc.json
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/.prettierignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/.prettierrc.json
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/README.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/import-sorter.json
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/index.html
+-rw-r--r--   0        0        0   618647 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/package-lock.json
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/package.json
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/tsconfig.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/vite.config.js
+-rw-r--r--   0        0        0    16958 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/public/favicon.ico
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/public/manifest.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/public/robots.txt
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/App.css
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/App.test.tsx
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/App.tsx
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/client.ts
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/clipboard-copy.d.ts
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/index.tsx
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/openapi_schemas.ts
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/settings.ts
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/setupTests.ts
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/theme.ts
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/array-1d.tsx
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/array-nd.tsx
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/choose-partition.tsx
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/column-list.tsx
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/contents.tsx
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/cut-slider.tsx
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/download-array.tsx
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/download-core.tsx
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/download-node.tsx
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/download-table.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/error-boundary.tsx
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/json-viewer.tsx
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/line.tsx
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/metadata-view.tsx
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/node-breadcrumbs.tsx
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/node-contents.tsx
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/node-lazy-contents.tsx
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/overview-array.tsx
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/overview-generic-node.tsx
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/overview-table.tsx
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/range-slider.tsx
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/components/tiled-app-bar.tsx
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/context/settings.tsx
+-rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 tiled-0.1.0b2/web-frontend/src/routes/browse.tsx
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tiled-0.1.0b2/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 tiled-0.1.0b2/LICENSE
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 tiled-0.1.0b2/README.md
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 tiled-0.1.0b2/hatch_build.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 tiled-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0    16858 2020-02-02 00:00:00.000000 tiled-0.1.0b2/PKG-INFO
```

### Comparing `tiled-0.1.0b1/.mypy.ini` & `tiled-0.1.0b2/.mypy.ini`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/.pre-commit-config.yaml` & `tiled-0.1.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/CHANGELOG.md` & `tiled-0.1.0b2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 <!-- Add the recent changes in the code under the relevant category.
 Write the date in place of the "Unreleased" in the case a new version is released. -->
 
 # Changelog
 
+## v0.1.0b2 (2024-05-28)
+
+## Changed
+
+- Customized default logging configuration to include correlation ID and username
+  of authenticated user.
+- Added `--log-timestamps` CLI flag to `tiled serve ...` to opt in to including
+  timestamp prefix in log messages.
+
 ## v0.1.0b1 (2024-05-25)
 
 ### Added
 
 - Support for `FullText` search on SQLite-backed catalogs
 
 ### Fixed
```

### Comparing `tiled-0.1.0b1/Dockerfile` & `tiled-0.1.0b2/Dockerfile`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/asv.conf.json` & `tiled-0.1.0b2/asv.conf.json`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/canary-validator.yml` & `tiled-0.1.0b2/canary-validator.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docker-compose.yml` & `tiled-0.1.0b2/docker-compose.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 version: "3.2"
 services:
   tiled:
-    image: ghcr.io/bluesky/tiled:v0.1.0b1
+    image: ghcr.io/bluesky/tiled:v0.1.0b2
     environment:
       - TILED_SINGLE_USER_API_KEY=${TILED_SINGLE_USER_API_KEY}
     ports:
       - 8000:8000
     restart: unless-stopped
 
   # Below we additionally configure monitoring with Prometheus and Grafana.
```

### Comparing `tiled-0.1.0b1/example_log_config.yml` & `tiled-0.1.0b2/example_log_config.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/.github/workflows/build-and-validate-image.yml` & `tiled-0.1.0b2/.github/workflows/build-and-validate-image.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/.github/workflows/ci.yml` & `tiled-0.1.0b2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/.github/workflows/docs.yml` & `tiled-0.1.0b2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/.github/workflows/publish-docs.yml` & `tiled-0.1.0b2/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/.github/workflows/publish-image.yml` & `tiled-0.1.0b2/.github/workflows/publish-image.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/.github/workflows/publish-pypi.yml` & `tiled-0.1.0b2/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/benchmarks/benchmarks.py` & `tiled-0.1.0b2/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/Makefile` & `tiled-0.1.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/make.bat` & `tiled-0.1.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/conf.py` & `tiled-0.1.0b2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/index.md` & `tiled-0.1.0b2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/_static/grafana-screenshot.png` & `tiled-0.1.0b2/docs/source/_static/grafana-screenshot.png`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/_static/orcid-authorize.png` & `tiled-0.1.0b2/docs/source/_static/orcid-authorize.png`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/_static/orcid-login.png` & `tiled-0.1.0b2/docs/source/_static/orcid-login.png`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/access-control.md` & `tiled-0.1.0b2/docs/source/explanations/access-control.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/architecture.md` & `tiled-0.1.0b2/docs/source/explanations/architecture.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/caching.md` & `tiled-0.1.0b2/docs/source/explanations/caching.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/catalog.md` & `tiled-0.1.0b2/docs/source/explanations/catalog.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/compression.md` & `tiled-0.1.0b2/docs/source/explanations/compression.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/faq.md` & `tiled-0.1.0b2/docs/source/explanations/faq.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/lineage.md` & `tiled-0.1.0b2/docs/source/explanations/lineage.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/metadata.md` & `tiled-0.1.0b2/docs/source/explanations/metadata.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/security.md` & `tiled-0.1.0b2/docs/source/explanations/security.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/specialized-formats.md` & `tiled-0.1.0b2/docs/source/explanations/specialized-formats.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/standards.md` & `tiled-0.1.0b2/docs/source/explanations/standards.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/explanations/structures.md` & `tiled-0.1.0b2/docs/source/explanations/structures.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/api-keys.md` & `tiled-0.1.0b2/docs/source/how-to/api-keys.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/client-logger.md` & `tiled-0.1.0b2/docs/source/how-to/client-logger.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/configuration.md` & `tiled-0.1.0b2/docs/source/how-to/configuration.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/custom-clients.md` & `tiled-0.1.0b2/docs/source/how-to/custom-clients.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/custom-export-formats.md` & `tiled-0.1.0b2/docs/source/how-to/custom-export-formats.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/direct-client.md` & `tiled-0.1.0b2/docs/source/how-to/direct-client.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/docker.md` & `tiled-0.1.0b2/docs/source/how-to/docker.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/metrics.md` & `tiled-0.1.0b2/docs/source/how-to/metrics.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/profiles.md` & `tiled-0.1.0b2/docs/source/how-to/profiles.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/read-custom-formats.md` & `tiled-0.1.0b2/docs/source/how-to/read-custom-formats.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/register.md` & `tiled-0.1.0b2/docs/source/how-to/register.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/how-to/tiled-authn-database.md` & `tiled-0.1.0b2/docs/source/how-to/tiled-authn-database.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/authentication.md` & `tiled-0.1.0b2/docs/source/reference/authentication.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/client-profiles-header.txt` & `tiled-0.1.0b2/docs/source/reference/client-profiles-header.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/http-api-overview.md` & `tiled-0.1.0b2/docs/source/reference/http-api-overview.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/min-versions.rst` & `tiled-0.1.0b2/docs/source/reference/min-versions.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/python-client.md` & `tiled-0.1.0b2/docs/source/reference/python-client.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/queries.md` & `tiled-0.1.0b2/docs/source/reference/queries.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/scopes.md` & `tiled-0.1.0b2/docs/source/reference/scopes.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/service-configuration-header.txt` & `tiled-0.1.0b2/docs/source/reference/service-configuration-header.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/reference/service.md` & `tiled-0.1.0b2/docs/source/reference/service.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/export.md` & `tiled-0.1.0b2/docs/source/tutorials/export.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/installation.rst` & `tiled-0.1.0b2/docs/source/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/login.md` & `tiled-0.1.0b2/docs/source/tutorials/login.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/navigation.md` & `tiled-0.1.0b2/docs/source/tutorials/navigation.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/plotly-integration.md` & `tiled-0.1.0b2/docs/source/tutorials/plotly-integration.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/search.md` & `tiled-0.1.0b2/docs/source/tutorials/search.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/serving-files.md` & `tiled-0.1.0b2/docs/source/tutorials/serving-files.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/slicing.md` & `tiled-0.1.0b2/docs/source/tutorials/slicing.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/docs/source/tutorials/writing.md` & `tiled-0.1.0b2/docs/source/tutorials/writing.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/google_auth.yml` & `tiled-0.1.0b2/example_configs/google_auth.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/multiple_providers.yml` & `tiled-0.1.0b2/example_configs/multiple_providers.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/orcid_auth.yml` & `tiled-0.1.0b2/example_configs/orcid_auth.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/saml.yml` & `tiled-0.1.0b2/example_configs/saml.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/single_catalog_single_user.yml` & `tiled-0.1.0b2/example_configs/single_catalog_single_user.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/toy_authentication.yml` & `tiled-0.1.0b2/example_configs/toy_authentication.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/custom_export_formats/custom_exporters.py` & `tiled-0.1.0b2/example_configs/custom_export_formats/custom_exporters.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/external_service/custom.py` & `tiled-0.1.0b2/example_configs/external_service/custom.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/simple_oidc/README.md` & `tiled-0.1.0b2/example_configs/simple_oidc/README.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/example_configs/simple_oidc/oidc_provider_config.json` & `tiled-0.1.0b2/example_configs/simple_oidc/oidc_provider_config.json`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/monitoring_example/README.md` & `tiled-0.1.0b2/monitoring_example/README.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/monitoring_example/grafana/dashboards/dashboard.json` & `tiled-0.1.0b2/monitoring_example/grafana/dashboards/dashboard.json`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/scripts/json_indexes.py` & `tiled-0.1.0b2/scripts/json_indexes.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/static/default_ui_settings.yml` & `tiled-0.1.0b2/share/tiled/static/default_ui_settings.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/static/favicon.ico` & `tiled-0.1.0b2/share/tiled/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/templates/device_code_form.html` & `tiled-0.1.0b2/share/tiled/templates/device_code_form.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/templates/index.html` & `tiled-0.1.0b2/share/tiled/templates/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/favicon.ico` & `tiled-0.1.0b2/share/tiled/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/index.html` & `tiled-0.1.0b2/share/tiled/ui/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/Checkbox.841ff07f.js` & `tiled-0.1.0b2/share/tiled/ui/assets/Checkbox.841ff07f.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/DataGrid.b013c811.js` & `tiled-0.1.0b2/share/tiled/ui/assets/DataGrid.b013c811.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/FormControlLabel.93f22896.js` & `tiled-0.1.0b2/share/tiled/ui/assets/FormControlLabel.93f22896.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/FormGroup.25250c88.js` & `tiled-0.1.0b2/share/tiled/ui/assets/FormGroup.25250c88.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/FormLabel.a3eda031.js` & `tiled-0.1.0b2/share/tiled/ui/assets/FormLabel.a3eda031.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/Input.ed778d26.js` & `tiled-0.1.0b2/share/tiled/ui/assets/Input.ed778d26.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/ListItemIcon.fcfd88bf.js` & `tiled-0.1.0b2/share/tiled/ui/assets/ListItemIcon.fcfd88bf.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/TextField.8d6efd58.js` & `tiled-0.1.0b2/share/tiled/ui/assets/TextField.8d6efd58.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/array-1d.0797372d.js` & `tiled-0.1.0b2/share/tiled/ui/assets/array-1d.0797372d.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/array-nd.16ddeaf4.js` & `tiled-0.1.0b2/share/tiled/ui/assets/array-nd.16ddeaf4.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/browse.0916686d.js` & `tiled-0.1.0b2/share/tiled/ui/assets/browse.0916686d.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/choose-partition.93f44af2.js` & `tiled-0.1.0b2/share/tiled/ui/assets/choose-partition.93f44af2.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/default-highlight.19f6d178.js` & `tiled-0.1.0b2/share/tiled/ui/assets/default-highlight.19f6d178.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/download-array.e7fdb5ff.js` & `tiled-0.1.0b2/share/tiled/ui/assets/download-array.e7fdb5ff.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/download-core.1ace673a.js` & `tiled-0.1.0b2/share/tiled/ui/assets/download-core.1ace673a.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/download-table.e6c78057.js` & `tiled-0.1.0b2/share/tiled/ui/assets/download-table.e6c78057.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/index.72e24882.js` & `tiled-0.1.0b2/share/tiled/ui/assets/index.72e24882.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/index.d49bee11.css` & `tiled-0.1.0b2/share/tiled/ui/assets/index.d49bee11.css`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/index.esm.31c0e330.js` & `tiled-0.1.0b2/share/tiled/ui/assets/index.esm.31c0e330.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/json-viewer.c5226ec8.js` & `tiled-0.1.0b2/share/tiled/ui/assets/json-viewer.c5226ec8.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/metadata-view.3cdbfa99.js` & `tiled-0.1.0b2/share/tiled/ui/assets/metadata-view.3cdbfa99.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/overview-array.ec18d178.js` & `tiled-0.1.0b2/share/tiled/ui/assets/overview-array.ec18d178.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/overview-generic-node.553dc45c.js` & `tiled-0.1.0b2/share/tiled/ui/assets/overview-generic-node.553dc45c.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/overview-table.75ff538b.js` & `tiled-0.1.0b2/share/tiled/ui/assets/overview-table.75ff538b.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-all-300-normal.6d79427c.woff` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-all-300-normal.6d79427c.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-all-400-normal.e41533d5.woff` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-all-400-normal.e41533d5.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-all-500-normal.8f838c80.woff` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-all-500-normal.8f838c80.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-all-700-normal.b5883883.woff` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-all-700-normal.b5883883.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-300-normal.47aa3bfa.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-300-normal.47aa3bfa.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-400-normal.495d38d4.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-400-normal.495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-500-normal.3728fbdd.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-500-normal.3728fbdd.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-700-normal.6a84eeee.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-700-normal.6a84eeee.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-ext-300-normal.435e4b7f.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-ext-300-normal.435e4b7f.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-ext-400-normal.b7ef2cd1.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-ext-400-normal.b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-ext-500-normal.aeed0e51.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-ext-500-normal.aeed0e51.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-cyrillic-ext-700-normal.3c505383.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-cyrillic-ext-700-normal.3c505383.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-greek-300-normal.455c2c1a.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-greek-300-normal.455c2c1a.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-greek-400-normal.daf51ab5.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-greek-400-normal.daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-greek-500-normal.713780d8.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-greek-500-normal.713780d8.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-greek-700-normal.1c9cc76f.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-greek-700-normal.1c9cc76f.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-300-normal.f7591131.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-300-normal.f7591131.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-400-normal.f6734f81.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-400-normal.f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-500-normal.b0195382.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-500-normal.b0195382.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-700-normal.f5aebdfe.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-700-normal.f5aebdfe.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-ext-300-normal.b076e863.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-ext-300-normal.b076e863.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-ext-400-normal.3c23eb02.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-ext-400-normal.3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-ext-500-normal.7f1c829b.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-ext-500-normal.7f1c829b.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-latin-ext-700-normal.fc66f942.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-latin-ext-700-normal.fc66f942.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-vietnamese-300-normal.51f3f418.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-vietnamese-300-normal.51f3f418.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-vietnamese-400-normal.77b24796.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-vietnamese-400-normal.77b24796.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-vietnamese-500-normal.0948409a.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-vietnamese-500-normal.0948409a.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/roboto-vietnamese-700-normal.4ec57f2a.woff2` & `tiled-0.1.0b2/share/tiled/ui/assets/roboto-vietnamese-700-normal.4ec57f2a.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/share/tiled/ui/assets/toPropertyKey.012fc217.js` & `tiled-0.1.0b2/share/tiled/ui/assets/toPropertyKey.012fc217.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/access_policies.py` & `tiled-0.1.0b2/tiled/access_policies.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/alembic_utils.py` & `tiled-0.1.0b2/tiled/alembic_utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authenticators.py` & `tiled-0.1.0b2/tiled/authenticators.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/config.py` & `tiled-0.1.0b2/tiled/config.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/iterviews.py` & `tiled-0.1.0b2/tiled/iterviews.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/media_type_registration.py` & `tiled-0.1.0b2/tiled/media_type_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/mimetypes.py` & `tiled-0.1.0b2/tiled/mimetypes.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/profiles.py` & `tiled-0.1.0b2/tiled/profiles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/queries.py` & `tiled-0.1.0b2/tiled/queries.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/query_registration.py` & `tiled-0.1.0b2/tiled/query_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/scopes.py` & `tiled-0.1.0b2/tiled/scopes.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/utils.py` & `tiled-0.1.0b2/tiled/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/validation_registration.py` & `tiled-0.1.0b2/tiled/validation_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/conftest.py` & `tiled-0.1.0b2/tiled/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_access_control.py` & `tiled-0.1.0b2/tiled/_tests/test_access_control.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_allow_origins.py` & `tiled-0.1.0b2/tiled/_tests/test_allow_origins.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_array.py` & `tiled-0.1.0b2/tiled/_tests/test_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_asset_access.py` & `tiled-0.1.0b2/tiled/_tests/test_asset_access.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_authentication.py` & `tiled-0.1.0b2/tiled/_tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_authenticators.py` & `tiled-0.1.0b2/tiled/_tests/test_authenticators.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_awkward.py` & `tiled-0.1.0b2/tiled/_tests/test_awkward.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_caches.py` & `tiled-0.1.0b2/tiled/_tests/test_caches.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_catalog.py` & `tiled-0.1.0b2/tiled/_tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_cli.py` & `tiled-0.1.0b2/tiled/_tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,19 +21,25 @@
     process.terminate()
 
 
 def scrape_server_url_from_logs(process):
     "Scrape from server logs 'Uvicorn running on https://...'"
 
     def target(queue):
-        pattern = re.compile(r"Uvicorn running on (\S*)")
+        pattern = re.compile(r"Uvicorn running on .*(http:\/\/\S+:\d+).*")
+        lines = []
         while not process.poll():
             line = process.stderr.readline()
+            lines.append(line.decode())
             if match := pattern.search(line.decode()):
                 break
+        else:
+            raise RuntimeError(
+                "Did not find server URL in log output:\n" + "\n".join(lines)
+            )
         url = match.group(1)
         queue.put(url)
 
     queue = Queue()
     thread = threading.Thread(target=target, args=(queue,))
     thread.start()
     url = queue.get(timeout=10)
@@ -55,24 +61,53 @@
     "args",
     [
         "",
         "--verbose",
         "--api-key secret",
     ],
 )
-def test_serve_directory(args, tmpdir):
+def test_serve_directory(args, tmp_path):
     "Test 'tiled serve directory ... with a variety of arguments."
-    with run_cli(f"tiled serve directory {tmpdir!s} --port 0 " + args) as process:
+    with run_cli(f"tiled serve directory {tmp_path!s} --port 0 " + args) as process:
         check_server_readiness(process)
 
 
 @pytest.mark.parametrize(
     "args",
     [
         "",
         "--api-key secret",
     ],
 )
-def test_serve_catalog_temp(args, tmpdir):
+def test_serve_catalog_temp(args, tmp_path):
     "Test 'tiled serve catalog --temp ... with a variety of arguments."
-    with run_cli(f"tiled serve directory {tmpdir!s} --port 0 " + args) as process:
+    with run_cli(f"tiled serve directory {tmp_path!s} --port 0 " + args) as process:
+        check_server_readiness(process)
+
+
+@pytest.mark.parametrize(
+    "args",
+    [
+        "",
+    ],
+)
+def test_serve_config(args, tmp_path):
+    "Test 'tiled serve config' with a tmp config file."
+    (tmp_path / "data").mkdir()
+    (tmp_path / "config").mkdir()
+    config_filepath = tmp_path / "config" / "config.yml"
+    with open(config_filepath, "w") as file:
+        file.write(
+            f"""
+authentication:
+  allow_anonymous_access: false
+trees:
+  - path: /
+    tree: catalog
+    args:
+      uri: sqlite+aiosqlite:///{tmp_path / 'catalog.db'}
+      writable_storage: {tmp_path / 'data'}
+      init_if_not_exists: true
+"""
+        )
+    with run_cli(f"tiled serve config {config_filepath} --port 0 " + args) as process:
         check_server_readiness(process)
```

### Comparing `tiled-0.1.0b1/tiled/_tests/test_client.py` & `tiled-0.1.0b2/tiled/_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_client_cache.py` & `tiled-0.1.0b2/tiled/_tests/test_client_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_client_smoke.py` & `tiled-0.1.0b2/tiled/_tests/test_client_smoke.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_compression.py` & `tiled-0.1.0b2/tiled/_tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_config.py` & `tiled-0.1.0b2/tiled/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_container_fields.py` & `tiled-0.1.0b2/tiled/_tests/test_container_fields.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_container_files.py` & `tiled-0.1.0b2/tiled/_tests/test_container_files.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_custom_format.py` & `tiled-0.1.0b2/tiled/_tests/test_custom_format.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_dataframe.py` & `tiled-0.1.0b2/tiled/_tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_decoders.py` & `tiled-0.1.0b2/tiled/_tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_directory_walker.py` & `tiled-0.1.0b2/tiled/_tests/test_directory_walker.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_distinct.py` & `tiled-0.1.0b2/tiled/_tests/test_distinct.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_export.py` & `tiled-0.1.0b2/tiled/_tests/test_export.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_hdf5.py` & `tiled-0.1.0b2/tiled/_tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_history.py` & `tiled-0.1.0b2/tiled/_tests/test_history.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_import_object.py` & `tiled-0.1.0b2/tiled/_tests/test_import_object.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_indexers.py` & `tiled-0.1.0b2/tiled/_tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_inlined_contents.py` & `tiled-0.1.0b2/tiled/_tests/test_inlined_contents.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_json.py` & `tiled-0.1.0b2/tiled/_tests/test_json.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_metrics.py` & `tiled-0.1.0b2/tiled/_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_openapi.py` & `tiled-0.1.0b2/tiled/_tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_pickle.py` & `tiled-0.1.0b2/tiled/_tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_profiles.py` & `tiled-0.1.0b2/tiled/_tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_protocols.py` & `tiled-0.1.0b2/tiled/_tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_queries.py` & `tiled-0.1.0b2/tiled/_tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_resource_cache.py` & `tiled-0.1.0b2/tiled/_tests/test_resource_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_scaled_config_option.py` & `tiled-0.1.0b2/tiled/_tests/test_scaled_config_option.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_search.py` & `tiled-0.1.0b2/tiled/_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_select_metadata.py` & `tiled-0.1.0b2/tiled/_tests/test_select_metadata.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_size_limit.py` & `tiled-0.1.0b2/tiled/_tests/test_size_limit.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_sort.py` & `tiled-0.1.0b2/tiled/_tests/test_sort.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_sparse.py` & `tiled-0.1.0b2/tiled/_tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_specs.py` & `tiled-0.1.0b2/tiled/_tests/test_specs.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_structured_array.py` & `tiled-0.1.0b2/tiled/_tests/test_structured_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_sync.py` & `tiled-0.1.0b2/tiled/_tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_tiff.py` & `tiled-0.1.0b2/tiled/_tests/test_tiff.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_validation.py` & `tiled-0.1.0b2/tiled/_tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_writing.py` & `tiled-0.1.0b2/tiled/_tests/test_writing.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/test_xarray.py` & `tiled-0.1.0b2/tiled/_tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/utils.py` & `tiled-0.1.0b2/tiled/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/_tests/sql/before_creating_fts5_virtual_table.sql` & `tiled-0.1.0b2/tiled/_tests/sql/before_creating_fts5_virtual_table.sql`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/array.py` & `tiled-0.1.0b2/tiled/adapters/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/awkward.py` & `tiled-0.1.0b2/tiled/adapters/awkward.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/awkward_buffers.py` & `tiled-0.1.0b2/tiled/adapters/awkward_buffers.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/awkward_directory_container.py` & `tiled-0.1.0b2/tiled/adapters/awkward_directory_container.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/csv.py` & `tiled-0.1.0b2/tiled/adapters/csv.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/excel.py` & `tiled-0.1.0b2/tiled/adapters/excel.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/hdf5.py` & `tiled-0.1.0b2/tiled/adapters/hdf5.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/mapping.py` & `tiled-0.1.0b2/tiled/adapters/mapping.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/parquet.py` & `tiled-0.1.0b2/tiled/adapters/parquet.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/protocols.py` & `tiled-0.1.0b2/tiled/adapters/protocols.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/resource_cache.py` & `tiled-0.1.0b2/tiled/adapters/resource_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/sparse.py` & `tiled-0.1.0b2/tiled/adapters/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/sparse_blocks_parquet.py` & `tiled-0.1.0b2/tiled/adapters/sparse_blocks_parquet.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/table.py` & `tiled-0.1.0b2/tiled/adapters/table.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/tiff.py` & `tiled-0.1.0b2/tiled/adapters/tiff.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/utils.py` & `tiled-0.1.0b2/tiled/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/xarray.py` & `tiled-0.1.0b2/tiled/adapters/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/adapters/zarr.py` & `tiled-0.1.0b2/tiled/adapters/zarr.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/__main__.py` & `tiled-0.1.0b2/tiled/authn_database/__main__.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/alembic.ini.template` & `tiled-0.1.0b2/tiled/authn_database/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/connection_pool.py` & `tiled-0.1.0b2/tiled/authn_database/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/core.py` & `tiled-0.1.0b2/tiled/authn_database/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/orm.py` & `tiled-0.1.0b2/tiled/authn_database/orm.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/migrations/env.py` & `tiled-0.1.0b2/tiled/authn_database/migrations/env.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/migrations/versions/13024b8a6b74_add_register_scope_to_default_roles.py` & `tiled-0.1.0b2/tiled/authn_database/migrations/versions/13024b8a6b74_add_register_scope_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/migrations/versions/481830dd6c11_initialize.py` & `tiled-0.1.0b2/tiled/authn_database/migrations/versions/481830dd6c11_initialize.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/migrations/versions/4a9dfaba4a98_add_pendingsession.py` & `tiled-0.1.0b2/tiled/authn_database/migrations/versions/4a9dfaba4a98_add_pendingsession.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py` & `tiled-0.1.0b2/tiled/authn_database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py` & `tiled-0.1.0b2/tiled/authn_database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/migrations/versions/769180ce732e_add_write_principals_scope_to_admin.py` & `tiled-0.1.0b2/tiled/authn_database/migrations/versions/769180ce732e_add_write_principals_scope_to_admin.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/authn_database/migrations/versions/c7bd2573716d_add_session_state_column.py` & `tiled-0.1.0b2/tiled/authn_database/migrations/versions/c7bd2573716d_add_session_state_column.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/__main__.py` & `tiled-0.1.0b2/tiled/catalog/__main__.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/adapter.py` & `tiled-0.1.0b2/tiled/catalog/adapter.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/alembic.ini.template` & `tiled-0.1.0b2/tiled/catalog/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/core.py` & `tiled-0.1.0b2/tiled/catalog/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/explain.py` & `tiled-0.1.0b2/tiled/catalog/explain.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/orm.py` & `tiled-0.1.0b2/tiled/catalog/orm.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/env.py` & `tiled-0.1.0b2/tiled/catalog/migrations/env.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/versions/0b033e7fbe30_add_awkward_to_structurefamily_enum.py` & `tiled-0.1.0b2/tiled/catalog/migrations/versions/0b033e7fbe30_add_awkward_to_structurefamily_enum.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/versions/1cd99c02d0c7_create_index_for_fulltext_search.py` & `tiled-0.1.0b2/tiled/catalog/migrations/versions/1cd99c02d0c7_create_index_for_fulltext_search.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/versions/2ca16566d692_separate_structure_table.py` & `tiled-0.1.0b2/tiled/catalog/migrations/versions/2ca16566d692_separate_structure_table.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/versions/3db11ff95b6c_changing_top_level_metadata_to_btree_gin.py` & `tiled-0.1.0b2/tiled/catalog/migrations/versions/3db11ff95b6c_changing_top_level_metadata_to_btree_gin.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/versions/83889e049ddc_add_table_to_structurefamily_enum.py` & `tiled-0.1.0b2/tiled/catalog/migrations/versions/83889e049ddc_add_table_to_structurefamily_enum.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/versions/a66028395cab_enrich_datasource_asset_association.py` & `tiled-0.1.0b2/tiled/catalog/migrations/versions/a66028395cab_enrich_datasource_asset_association.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/versions/e756b9381c14_add_structure_family_to_data_sources.py` & `tiled-0.1.0b2/tiled/catalog/migrations/versions/e756b9381c14_add_structure_family_to_data_sources.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/catalog/migrations/versions/ed3a4223a600_create_sqlite_table_for_fulltext_search.py` & `tiled-0.1.0b2/tiled/catalog/migrations/versions/ed3a4223a600_create_sqlite_table_for_fulltext_search.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/CACHEY_LICENSE.txt` & `tiled-0.1.0b2/tiled/client/CACHEY_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/array.py` & `tiled-0.1.0b2/tiled/client/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/auth.py` & `tiled-0.1.0b2/tiled/client/auth.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/awkward.py` & `tiled-0.1.0b2/tiled/client/awkward.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/base.py` & `tiled-0.1.0b2/tiled/client/base.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/cache.py` & `tiled-0.1.0b2/tiled/client/cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/cache_control.py` & `tiled-0.1.0b2/tiled/client/cache_control.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/constructors.py` & `tiled-0.1.0b2/tiled/client/constructors.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/container.py` & `tiled-0.1.0b2/tiled/client/container.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/context.py` & `tiled-0.1.0b2/tiled/client/context.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/dataframe.py` & `tiled-0.1.0b2/tiled/client/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/decoders.py` & `tiled-0.1.0b2/tiled/client/decoders.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/download.py` & `tiled-0.1.0b2/tiled/client/download.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/logger.py` & `tiled-0.1.0b2/tiled/client/logger.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/register.py` & `tiled-0.1.0b2/tiled/client/register.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/smoke.py` & `tiled-0.1.0b2/tiled/client/smoke.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/sparse.py` & `tiled-0.1.0b2/tiled/client/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/sync.py` & `tiled-0.1.0b2/tiled/client/sync.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/transport.py` & `tiled-0.1.0b2/tiled/client/transport.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/utils.py` & `tiled-0.1.0b2/tiled/client/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/client/xarray.py` & `tiled-0.1.0b2/tiled/client/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/commandline/_admin.py` & `tiled-0.1.0b2/tiled/commandline/_admin.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/commandline/_api_key.py` & `tiled-0.1.0b2/tiled/commandline/_api_key.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/commandline/_catalog.py` & `tiled-0.1.0b2/tiled/commandline/_catalog.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/commandline/_profile.py` & `tiled-0.1.0b2/tiled/commandline/_profile.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/commandline/_register.py` & `tiled-0.1.0b2/tiled/commandline/_register.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/commandline/_serve.py` & `tiled-0.1.0b2/tiled/commandline/_serve.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,17 @@
             "example: --host `'::'`."
         ),
     ),
     port: int = typer.Option(8000, help="Bind to a socket with this port."),
     log_config: Optional[str] = typer.Option(
         None, help="Custom uvicorn logging configuration file"
     ),
+    log_timestamps: bool = typer.Option(
+        False, help="Include timestamps in log output."
+    ),
 ):
     "Serve a Tree instance from a directory of files."
     import tempfile
 
     temp_directory = Path(tempfile.TemporaryDirectory().name)
     temp_directory.mkdir()
     typer.echo(
@@ -195,20 +198,19 @@
         },
         server_settings,
     )
     import functools
 
     import anyio
     import uvicorn
-    from uvicorn.config import LOGGING_CONFIG
 
     from ..client import from_uri as client_from_uri
 
     print_admin_api_key_if_generated(web_app, host=host, port=port, force=generated)
-    log_config = log_config or LOGGING_CONFIG  # fall back to uvicorn default
+    log_config = _setup_log_config(log_config, log_timestamps)
     config = uvicorn.Config(web_app, host=host, port=port, log_config=log_config)
     server = uvicorn.Server(config)
 
     async def run_server():
         await server.serve()
 
     async def wait_for_server():
@@ -335,14 +337,17 @@
         help=(
             "This verifies that the configuration is compatible with scaled (multi-process) deployments."
         ),
     ),
     log_config: Optional[str] = typer.Option(
         None, help="Custom uvicorn logging configuration file"
     ),
+    log_timestamps: bool = typer.Option(
+        False, help="Include timestamps in log output."
+    ),
 ):
     "Serve a catalog."
     import urllib.parse
 
     from ..catalog import from_uri
     from ..server.app import build_app, print_admin_api_key_if_generated
 
@@ -433,17 +438,16 @@
         },
         server_settings,
         scalable=scalable,
     )
     print_admin_api_key_if_generated(web_app, host=host, port=port)
 
     import uvicorn
-    from uvicorn.config import LOGGING_CONFIG
 
-    log_config = log_config or LOGGING_CONFIG  # fall back to uvicorn default
+    log_config = _setup_log_config(log_config, log_timestamps)
     uvicorn.run(web_app, host=host, port=port, log_config=log_config)
 
 
 serve_app.command("catalog")(serve_catalog)
 
 
 @serve_app.command("pyobject")
@@ -483,14 +487,17 @@
         help=(
             "This verifies that the configuration is compatible with scaled (multi-process) deployments."
         ),
     ),
     log_config: Optional[str] = typer.Option(
         None, help="Custom uvicorn logging configuration file"
     ),
+    log_timestamps: bool = typer.Option(
+        False, help="Include timestamps in log output."
+    ),
 ):
     "Serve a Tree instance from a Python module."
     from ..server.app import build_app, print_admin_api_key_if_generated
     from ..utils import import_object
 
     tree = import_object(object_path)
     server_settings = {}
@@ -502,17 +509,16 @@
         },
         server_settings,
         scalable=scalable,
     )
     print_admin_api_key_if_generated(web_app, host=host, port=port)
 
     import uvicorn
-    from uvicorn.config import LOGGING_CONFIG
 
-    log_config = log_config or LOGGING_CONFIG  # fall back to uvicorn default
+    log_config = _setup_log_config(log_config, log_timestamps)
     uvicorn.run(web_app, host=host, port=port, log_config=log_config)
 
 
 @serve_app.command("demo")
 def serve_demo(
     host: str = typer.Option(
         "127.0.0.1",
@@ -582,14 +588,17 @@
         help=(
             "This verifies that the configuration is compatible with scaled (multi-process) deployments."
         ),
     ),
     log_config: Optional[str] = typer.Option(
         None, help="Custom uvicorn logging configuration file"
     ),
+    log_timestamps: bool = typer.Option(
+        False, help="Include timestamps in log output."
+    ),
 ):
     "Serve a Tree as specified in configuration file(s)."
     import os
 
     from ..config import parse_configs
 
     config_path = config_path or os.getenv("TILED_CONFIG", "config.yml")
@@ -619,15 +628,18 @@
     )
 
     # Extract config for uvicorn.
     uvicorn_kwargs = parsed_config.pop("uvicorn", {})
     # If --host is given, it overrides host in config. Same for --port and --log-config.
     uvicorn_kwargs["host"] = host or uvicorn_kwargs.get("host", "127.0.0.1")
     uvicorn_kwargs["port"] = port or uvicorn_kwargs.get("port", 8000)
-    uvicorn_kwargs["log_config"] = log_config or uvicorn_kwargs.get("log_config")
+    uvicorn_kwargs["log_config"] = _setup_log_config(
+        log_config or uvicorn_kwargs.get("log_config"),
+        log_timestamps,
+    )
 
     # This config was already validated when it was parsed. Do not re-validate.
     logger.info(f"Using configuration from {Path(config_path).absolute()}")
 
     if root_path := uvicorn_kwargs.get("root_path", ""):
         parsed_config["root_path"] = root_path
 
@@ -639,7 +651,36 @@
     )
 
     # Likewise, delay this import.
 
     import uvicorn
 
     uvicorn.run(web_app, **uvicorn_kwargs)
+
+
+def _setup_log_config(log_config, log_timestamps):
+    if log_config is None:
+        from ..server.logging_config import LOGGING_CONFIG
+
+        log_config = LOGGING_CONFIG
+
+    if log_timestamps:
+        import copy
+
+        log_config = copy.deepcopy(log_config)
+        try:
+            log_config["formatters"]["access"]["format"] = (
+                "[%(asctime)s.%(msecs)03dZ] "
+                + log_config["formatters"]["access"]["format"]
+            )
+            log_config["formatters"]["default"]["format"] = (
+                "[%(asctime)s.%(msecs)03dZ] "
+                + log_config["formatters"]["default"]["format"]
+            )
+        except KeyError:
+            typer.echo(
+                "The --log-timestamps option is only applicable with a logging "
+                "configuration that, like the default logging configuration, has "
+                "formatters 'access' and 'default'."
+            )
+            raise typer.Abort()
+    return log_config
```

### Comparing `tiled-0.1.0b1/tiled/commandline/_utils.py` & `tiled-0.1.0b2/tiled/commandline/_utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/commandline/main.py` & `tiled-0.1.0b2/tiled/commandline/main.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/config_schemas/client_profiles.yml` & `tiled-0.1.0b2/tiled/config_schemas/client_profiles.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/config_schemas/service_configuration.yml` & `tiled-0.1.0b2/tiled/config_schemas/service_configuration.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/examples/generate_files.py` & `tiled-0.1.0b2/tiled/examples/generate_files.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/examples/generated.py` & `tiled-0.1.0b2/tiled/examples/generated.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/examples/generated_minimal.py` & `tiled-0.1.0b2/tiled/examples/generated_minimal.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/examples/nexus.py` & `tiled-0.1.0b2/tiled/examples/nexus.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/examples/toy_authentication.py` & `tiled-0.1.0b2/tiled/examples/toy_authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/examples/xdi.py` & `tiled-0.1.0b2/tiled/examples/xdi.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/__init__.py` & `tiled-0.1.0b2/tiled/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/_zipfile_py39.py` & `tiled-0.1.0b2/tiled/serialization/_zipfile_py39.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/array.py` & `tiled-0.1.0b2/tiled/serialization/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/awkward.py` & `tiled-0.1.0b2/tiled/serialization/awkward.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/container.py` & `tiled-0.1.0b2/tiled/serialization/container.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/image_serializer_helpers.py` & `tiled-0.1.0b2/tiled/serialization/image_serializer_helpers.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/scikit-image-LICENSE.txt` & `tiled-0.1.0b2/tiled/serialization/scikit-image-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/sparse.py` & `tiled-0.1.0b2/tiled/serialization/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/table.py` & `tiled-0.1.0b2/tiled/serialization/table.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/serialization/xarray.py` & `tiled-0.1.0b2/tiled/serialization/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/app.py` & `tiled-0.1.0b2/tiled/server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import collections
+import contextvars
 import logging
 import os
 import secrets
 import sys
 import urllib.parse
 import warnings
 from contextlib import asynccontextmanager
@@ -34,15 +35,15 @@
 )
 
 from ..authenticators import Mode
 from ..config import construct_build_app_kwargs
 from ..media_type_registration import (
     compression_registry as default_compression_registry,
 )
-from ..utils import SHARE_TILED_PATH, Conflicts, UnsupportedQueryType
+from ..utils import SHARE_TILED_PATH, Conflicts, SpecialUsers, UnsupportedQueryType
 from ..validation_registration import validation_registry as default_validation_registry
 from . import schemas
 from .authentication import get_current_principal
 from .compression import CompressionMiddleware
 from .core import PatchedStreamingResponse
 from .dependencies import (
     get_query_registry,
@@ -73,14 +74,18 @@
 logger.setLevel("INFO")
 handler = logging.StreamHandler()
 handler.setLevel("DEBUG")
 handler.setFormatter(logging.Formatter("%(message)s"))
 logger.addHandler(handler)
 
 
+# This is used to pass the currently-authenticated principal into the logger.
+current_principal = contextvars.ContextVar("current_principal")
+
+
 def custom_openapi(app):
     """
     The app's openapi method will be monkey-patched with this.
 
     This is the approach the documentation recommends.
 
     https://fastapi.tiangolo.com/advanced/extending-openapi/
@@ -861,14 +866,22 @@
                 response.__class__ = PatchedStreamingResponse  # tolerate memoryview
                 metrics.capture_request_metrics(request, response)
 
             # This is a *real* response (i.e., not the 'only_for_metrics' response).
             # An exception above would have triggered an early exit.
             return response
 
+    @app.middleware("http")
+    async def current_principal_logging_filter(request: Request, call_next):
+        request.state.principal = SpecialUsers.public
+        response = await call_next(request)
+        response.__class__ = PatchedStreamingResponse  # tolerate memoryview
+        current_principal.set(request.state.principal)
+        return response
+
     app.add_middleware(
         CorrelationIdMiddleware,
         header_name="X-Tiled-Request-ID",
         generator=lambda: secrets.token_hex(8),
     )
 
     return app
```

### Comparing `tiled-0.1.0b1/tiled/server/authentication.py` & `tiled-0.1.0b2/tiled/server/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,14 +369,16 @@
             detail=(
                 "Not enough permissions. "
                 f"Requires scopes {security_scopes.scopes}. "
                 f"Request had scopes {list(scopes)}"
             ),
             headers=headers_for_401(request, security_scopes),
         )
+    # This is used to pass the currently-authenticated principal into the logger.
+    request.state.principal = principal
     return principal
 
 
 async def create_pending_session(db):
     device_code = secrets.token_bytes(32)
     hashed_device_code = hashlib.sha256(device_code).digest()
     for _ in range(3):
```

### Comparing `tiled-0.1.0b1/tiled/server/compression.py` & `tiled-0.1.0b2/tiled/server/compression.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/core.py` & `tiled-0.1.0b2/tiled/server/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/dependencies.py` & `tiled-0.1.0b2/tiled/server/dependencies.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/etag.py` & `tiled-0.1.0b2/tiled/server/etag.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/links.py` & `tiled-0.1.0b2/tiled/server/links.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/metrics.py` & `tiled-0.1.0b2/tiled/server/metrics.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/pydantic_array.py` & `tiled-0.1.0b2/tiled/server/pydantic_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/pydantic_sparse.py` & `tiled-0.1.0b2/tiled/server/pydantic_sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/pydantic_table.py` & `tiled-0.1.0b2/tiled/server/pydantic_table.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/router.py` & `tiled-0.1.0b2/tiled/server/router.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/schemas.py` & `tiled-0.1.0b2/tiled/server/schemas.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/settings.py` & `tiled-0.1.0b2/tiled/server/settings.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/server/utils.py` & `tiled-0.1.0b2/tiled/server/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/structures/array.py` & `tiled-0.1.0b2/tiled/structures/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/structures/awkward.py` & `tiled-0.1.0b2/tiled/structures/awkward.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/structures/core.py` & `tiled-0.1.0b2/tiled/structures/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/structures/data_source.py` & `tiled-0.1.0b2/tiled/structures/data_source.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/structures/sparse.py` & `tiled-0.1.0b2/tiled/structures/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/tiled/structures/table.py` & `tiled-0.1.0b2/tiled/structures/table.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/README.md` & `tiled-0.1.0b2/web-frontend/README.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/index.html` & `tiled-0.1.0b2/web-frontend/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/package-lock.json` & `tiled-0.1.0b2/web-frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/package.json` & `tiled-0.1.0b2/web-frontend/package.json`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/vite.config.js` & `tiled-0.1.0b2/web-frontend/vite.config.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/public/favicon.ico` & `tiled-0.1.0b2/web-frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/App.css` & `tiled-0.1.0b2/web-frontend/src/App.css`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/App.tsx` & `tiled-0.1.0b2/web-frontend/src/App.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/client.ts` & `tiled-0.1.0b2/web-frontend/src/client.ts`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/index.tsx` & `tiled-0.1.0b2/web-frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/openapi_schemas.ts` & `tiled-0.1.0b2/web-frontend/src/openapi_schemas.ts`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/settings.ts` & `tiled-0.1.0b2/web-frontend/src/settings.ts`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/array-1d.tsx` & `tiled-0.1.0b2/web-frontend/src/components/array-1d.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/array-nd.tsx` & `tiled-0.1.0b2/web-frontend/src/components/array-nd.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/choose-partition.tsx` & `tiled-0.1.0b2/web-frontend/src/components/choose-partition.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/column-list.tsx` & `tiled-0.1.0b2/web-frontend/src/components/column-list.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/contents.tsx` & `tiled-0.1.0b2/web-frontend/src/components/contents.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/cut-slider.tsx` & `tiled-0.1.0b2/web-frontend/src/components/cut-slider.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/download-array.tsx` & `tiled-0.1.0b2/web-frontend/src/components/download-array.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/download-core.tsx` & `tiled-0.1.0b2/web-frontend/src/components/download-core.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/download-node.tsx` & `tiled-0.1.0b2/web-frontend/src/components/download-node.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/download-table.tsx` & `tiled-0.1.0b2/web-frontend/src/components/download-table.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/error-boundary.tsx` & `tiled-0.1.0b2/web-frontend/src/components/error-boundary.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/json-viewer.tsx` & `tiled-0.1.0b2/web-frontend/src/components/json-viewer.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/line.tsx` & `tiled-0.1.0b2/web-frontend/src/components/line.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/metadata-view.tsx` & `tiled-0.1.0b2/web-frontend/src/components/metadata-view.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/node-breadcrumbs.tsx` & `tiled-0.1.0b2/web-frontend/src/components/node-breadcrumbs.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/node-contents.tsx` & `tiled-0.1.0b2/web-frontend/src/components/node-contents.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/node-lazy-contents.tsx` & `tiled-0.1.0b2/web-frontend/src/components/node-lazy-contents.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/overview-array.tsx` & `tiled-0.1.0b2/web-frontend/src/components/overview-array.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/overview-generic-node.tsx` & `tiled-0.1.0b2/web-frontend/src/components/overview-generic-node.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/overview-table.tsx` & `tiled-0.1.0b2/web-frontend/src/components/overview-table.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/range-slider.tsx` & `tiled-0.1.0b2/web-frontend/src/components/range-slider.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/components/tiled-app-bar.tsx` & `tiled-0.1.0b2/web-frontend/src/components/tiled-app-bar.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/web-frontend/src/routes/browse.tsx` & `tiled-0.1.0b2/web-frontend/src/routes/browse.tsx`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/.gitignore` & `tiled-0.1.0b2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -58,7 +58,8 @@
 prometheus_data
 grafana_data
 data
 
 tiled/_version.py
 
 .env
+.asv/
```

### Comparing `tiled-0.1.0b1/LICENSE` & `tiled-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/README.md` & `tiled-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/hatch_build.py` & `tiled-0.1.0b2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/pyproject.toml` & `tiled-0.1.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0b1/PKG-INFO` & `tiled-0.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tiled
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Structured Scientific Data Access Service
 Project-URL: Homepage, https://github.com/bluesky/tiled
 Project-URL: Documentation, https://blueskyproject.io/tiled
 Project-URL: Bug Tracker, https://github.com/bluesky/tiled/issues
 Author-email: Bluesky Project Contributors <dallan@bnl.gov>
 Maintainer-email: Brookhaven National Laboratory <dallan@bnl.gov>
 License-File: LICENSE
```

