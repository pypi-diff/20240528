# Comparing `tmp/lunchable-1.3.2.tar.gz` & `tmp/lunchable-1.3.3.tar.gz`

## Comparing `lunchable-1.3.2.tar` & `lunchable-1.3.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 lunchable-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 lunchable-1.3.2/.releaserc.json
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 lunchable-1.3.2/Dockerfile
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lunchable-1.3.2/docker-compose.yaml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 lunchable-1.3.2/mkdocs.yaml
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/dependabot.yaml
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/labels.yaml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/release-drafter.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/docker.yaml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/labeler.yaml
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 lunchable-1.3.2/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 lunchable-1.3.2/docs/cli.md
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 lunchable-1.3.2/docs/contributing.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 lunchable-1.3.2/docs/gen_pages.py
--rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 lunchable-1.3.2/docs/interacting.md
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 lunchable-1.3.2/docs/plugins.md
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 lunchable-1.3.2/docs/usage.md
--rw-r--r--   0        0        0   124987 2020-02-02 00:00:00.000000 lunchable-1.3.2/docs/static/lunchable.png
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/__main__.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/_cli.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/_version.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/_config/__init__.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/_config/api_config.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/_config/file_config.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/_config/logging_config.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/__init__.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/_base.py
--rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/_core.py
--rw-r--r--   0        0        0    20073 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/_descriptions.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/_lunchmoney.py
--rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/assets.py
--rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/budgets.py
--rw-r--r--   0        0        0    16339 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/categories.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/crypto.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/plaid_accounts.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/recurring_expenses.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/tags.py
--rw-r--r--   0        0        0    34403 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/transactions.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/models/user.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/plugins/__init__.py
--rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 lunchable-1.3.2/lunchable/plugins/app.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements/requirements-all.py3.10.txt
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements/requirements-all.py3.11.txt
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements/requirements-all.py3.12.txt
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements/requirements-all.py3.8.txt
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements/requirements-all.py3.9.txt
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements/requirements-lint.txt
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 lunchable-1.3.2/requirements/requirements-test.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/__init__.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/conftest.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/test_cli.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_assets.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_budgets.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_categories.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_crypto.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_plaid_accounts.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_recurring_expenses.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_tags.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_transactions.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/test_user.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_204_response.yaml
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_add_to_category_group.yaml
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_create_and_delete_transaction_group.yaml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_create_asset.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_create_category.yaml
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_create_category_group.yaml
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_delete_budget.yaml
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_delete_category.yaml
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_delete_category_force.yaml
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_assets.yaml
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_budgets.yaml
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_categories.yaml
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_categories_flattened.yaml
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_categories_nested.yaml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_category.yaml
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_crypto.yaml
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_plaid_accounts.yaml
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_recurring_expenses.yaml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_tags.yaml
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_transaction.yaml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_transaction_group.yaml
--rw-r--r--   0        0        0    23722 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_transactions.yaml
--rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_transactions_no_paginate.yaml
--rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_uncleared_transactions.yaml
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_get_user.yaml
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_insert_transactions.yaml
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_split_transaction.yaml
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_trigger_fetch_from_plaid.yaml
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_unsplit_transaction.yaml
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_update_asset.yaml
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_update_category.yaml
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_update_crypto.yaml
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_update_transaction.yaml
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 lunchable-1.3.2/tests/models/cassettes/test_upsert_budget.yaml
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 lunchable-1.3.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 lunchable-1.3.2/LICENSE
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 lunchable-1.3.2/README.md
--rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 lunchable-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 lunchable-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 lunchable-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 lunchable-1.3.3/.releaserc.json
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 lunchable-1.3.3/Dockerfile
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lunchable-1.3.3/docker-compose.yaml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 lunchable-1.3.3/mkdocs.yaml
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/labels.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/release-drafter.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/docker.yaml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/labeler.yaml
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 lunchable-1.3.3/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 lunchable-1.3.3/docs/cli.md
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 lunchable-1.3.3/docs/contributing.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 lunchable-1.3.3/docs/gen_pages.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 lunchable-1.3.3/docs/interacting.md
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 lunchable-1.3.3/docs/plugins.md
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 lunchable-1.3.3/docs/usage.md
+-rw-r--r--   0        0        0   124987 2020-02-02 00:00:00.000000 lunchable-1.3.3/docs/static/lunchable.png
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/__main__.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/_cli.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/_version.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/_config/__init__.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/_config/api_config.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/_config/file_config.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/_config/logging_config.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/__init__.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/_base.py
+-rw-r--r--   0        0        0    11532 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/_core.py
+-rw-r--r--   0        0        0    20073 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/_descriptions.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/_lunchmoney.py
+-rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/assets.py
+-rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/budgets.py
+-rw-r--r--   0        0        0    16339 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/categories.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/crypto.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/plaid_accounts.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/recurring_expenses.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/tags.py
+-rw-r--r--   0        0        0    34403 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/transactions.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/models/user.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/plugins/__init__.py
+-rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 lunchable-1.3.3/lunchable/plugins/app.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements/requirements-all.py3.10.txt
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements/requirements-all.py3.11.txt
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements/requirements-all.py3.12.txt
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements/requirements-all.py3.8.txt
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements/requirements-all.py3.9.txt
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements/requirements-lint.txt
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 lunchable-1.3.3/requirements/requirements-test.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/__init__.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/conftest.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/test_cli.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_assets.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_budgets.py
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_categories.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_crypto.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_plaid_accounts.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_recurring_expenses.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_tags.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_transactions.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/test_user.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_204_response.yaml
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_add_to_category_group.yaml
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_create_and_delete_transaction_group.yaml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_create_asset.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_create_category.yaml
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_create_category_group.yaml
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_delete_budget.yaml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_delete_category.yaml
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_delete_category_force.yaml
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_assets.yaml
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_budgets.yaml
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_categories.yaml
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_categories_flattened.yaml
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_categories_nested.yaml
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_category.yaml
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_crypto.yaml
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_plaid_accounts.yaml
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_recurring_expenses.yaml
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_tags.yaml
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_transaction.yaml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_transaction_group.yaml
+-rw-r--r--   0        0        0    23722 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_transactions.yaml
+-rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_transactions_no_paginate.yaml
+-rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_uncleared_transactions.yaml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_get_user.yaml
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_insert_transactions.yaml
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_split_transaction.yaml
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_trigger_fetch_from_plaid.yaml
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_unsplit_transaction.yaml
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_update_asset.yaml
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_update_category.yaml
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_update_crypto.yaml
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_update_transaction.yaml
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 lunchable-1.3.3/tests/models/cassettes/test_upsert_budget.yaml
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 lunchable-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 lunchable-1.3.3/LICENSE
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 lunchable-1.3.3/README.md
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 lunchable-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 lunchable-1.3.3/PKG-INFO
```

### Comparing `lunchable-1.3.2/.pre-commit-config.yaml` & `lunchable-1.3.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 default_stages: [commit]
 fail_fast: false
 
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-ast
     -   id: check-docstring-first
     -   id: check-merge-conflict
     -   id: mixed-line-ending
 
 -   repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-    rev: v2.8.0
+    rev: v2.13.0
     hooks:
     -   id: pretty-format-toml
         args: [--autofix]
     -   id: pretty-format-yaml
         args: [--autofix, --indent, '4']
 
 -   repo: https://github.com/pre-commit/mirrors-prettier
```

### Comparing `lunchable-1.3.2/.releaserc.json` & `lunchable-1.3.3/.releaserc.json`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/Dockerfile` & `lunchable-1.3.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/docker-compose.yaml` & `lunchable-1.3.3/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/mkdocs.yaml` & `lunchable-1.3.3/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/requirements.txt` & `lunchable-1.3.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/dependabot.yaml` & `lunchable-1.3.3/.github/dependabot.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/labels.yaml` & `lunchable-1.3.3/.github/labels.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/release-drafter.yaml` & `lunchable-1.3.3/.github/release-drafter.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/semantic_release/package-lock.json` & `lunchable-1.3.3/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/semantic_release/release_notes.hbs` & `lunchable-1.3.3/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/workflows/docker.yaml` & `lunchable-1.3.3/.github/workflows/docker.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/workflows/labeler.yaml` & `lunchable-1.3.3/.github/workflows/labeler.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/workflows/lint.yaml` & `lunchable-1.3.3/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/workflows/publish.yaml` & `lunchable-1.3.3/.github/workflows/publish.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 name: Publishing
 
 on:
     release:
         types:
         -   published
+    workflow_dispatch:
 
 jobs:
     pypi-publish:
         name: PyPI
         if: github.repository_owner == 'juftin'
         runs-on: ubuntu-latest
+        environment:
+            name: pypi
+            url: https://pypi.org/p/lunchable
+        permissions:
+            id-token: write
         steps:
         -   name: Check out the repository
             uses: actions/checkout@v4
             with:
                 fetch-depth: 2
         -   name: Set up Python
             uses: actions/setup-python@v5
@@ -24,18 +30,15 @@
                 python -m pip install --upgrade pip
                 python -m pip install -q hatch pre-commit
                 hatch --version
         -   name: Build package
             run: |
                 hatch build
         -   name: Publish package on PyPI
-            uses: pypa/gh-action-pypi-publish@v1.8.11
-            with:
-                user: __token__
-                password: ${{ secrets.PYPI_TOKEN }}
+            uses: pypa/gh-action-pypi-publish@release/v1
 
     docker-hub-publish:
         name: docker-hub
         if: github.repository_owner == 'juftin'
         runs-on: ubuntu-latest
         steps:
         -   name: Check out the repository
```

### Comparing `lunchable-1.3.2/.github/workflows/release.yaml` & `lunchable-1.3.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.github/workflows/tests.yaml` & `lunchable-1.3.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/docs/contributing.md` & `lunchable-1.3.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/docs/gen_pages.py` & `lunchable-1.3.3/docs/gen_pages.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/docs/interacting.md` & `lunchable-1.3.3/docs/interacting.md`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/docs/plugins.md` & `lunchable-1.3.3/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/docs/usage.md` & `lunchable-1.3.3/docs/usage.md`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/docs/static/lunchable.png` & `lunchable-1.3.3/docs/static/lunchable.png`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/__init__.py` & `lunchable-1.3.3/lunchable/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/_cli.py` & `lunchable-1.3.3/lunchable/_cli.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/_config/api_config.py` & `lunchable-1.3.3/lunchable/_config/api_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/_config/logging_config.py` & `lunchable-1.3.3/lunchable/_config/logging_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/__init__.py` & `lunchable-1.3.3/lunchable/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/_core.py` & `lunchable-1.3.3/lunchable/models/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Lunchmoney SDK Core
 """
 
 from __future__ import annotations
 
-import logging
 from functools import cached_property
 from typing import (
     Any,
     AsyncIterable,
     Iterable,
     Mapping,
     Optional,
@@ -18,16 +17,14 @@
 import httpx
 import pydantic_core
 from httpx import Client
 
 from lunchable._config import APIConfig
 from lunchable.exceptions import LunchMoneyHTTPError
 
-logger = logging.getLogger(__name__)
-
 
 class LunchMoneyClient(Client):
     """
     API HTTP Client
     """
 
     def __init__(self, access_token: str | None = None) -> None:
@@ -264,29 +261,26 @@
         ----------
         response: httpx.Response
             An HTTPX Response Object
         """
         try:
             response.raise_for_status()
         except httpx.HTTPError as he:
-            logger.exception(he)
-            logger.error(response.text)
             raise LunchMoneyHTTPError(response.text) from he
         if response.content:
             returned_data = response.json()
         else:
             returned_data = None
         if isinstance(returned_data, dict) and any(
             ["error" in returned_data.keys(), "errors" in returned_data.keys()]
         ):
             try:
                 errors = returned_data["error"]
             except KeyError:
                 errors = returned_data["errors"]
-            logger.exception(errors)
             raise LunchMoneyHTTPError(errors)
         return returned_data
 
     def make_request(
         self,
         method: str,
         url_path: Union[list[Union[str, int]], str, int],
```

### Comparing `lunchable-1.3.2/lunchable/models/_descriptions.py` & `lunchable-1.3.3/lunchable/models/_descriptions.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/_lunchmoney.py` & `lunchable-1.3.3/lunchable/models/_lunchmoney.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/assets.py` & `lunchable-1.3.3/lunchable/models/assets.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/budgets.py` & `lunchable-1.3.3/lunchable/models/budgets.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/categories.py` & `lunchable-1.3.3/lunchable/models/categories.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/crypto.py` & `lunchable-1.3.3/lunchable/models/crypto.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/plaid_accounts.py` & `lunchable-1.3.3/lunchable/models/plaid_accounts.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/recurring_expenses.py` & `lunchable-1.3.3/lunchable/models/recurring_expenses.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/tags.py` & `lunchable-1.3.3/lunchable/models/tags.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/transactions.py` & `lunchable-1.3.3/lunchable/models/transactions.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/models/user.py` & `lunchable-1.3.3/lunchable/models/user.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/lunchable/plugins/app.py` & `lunchable-1.3.3/lunchable/plugins/app.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/requirements/requirements-all.py3.10.txt` & `lunchable-1.3.3/requirements/requirements-all.py3.10.txt`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/requirements/requirements-all.py3.11.txt` & `lunchable-1.3.3/requirements/requirements-all.py3.11.txt`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/requirements/requirements-all.py3.12.txt` & `lunchable-1.3.3/requirements/requirements-all.py3.12.txt`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/requirements/requirements-all.py3.8.txt` & `lunchable-1.3.3/requirements/requirements-all.py3.8.txt`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/requirements/requirements-all.py3.9.txt` & `lunchable-1.3.3/requirements/requirements-all.py3.9.txt`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/requirements/requirements-docs.txt` & `lunchable-1.3.3/requirements/requirements-docs.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     # via
     #   griffe
     #   mkdocs-material
 fieldz==0.0.2
     # via griffe-fieldz
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.39.1
+griffe==0.40.0
     # via
     #   griffe-fieldz
     #   mkdocstrings-python
 griffe-fieldz==0.1.2
     # via hatch.envs.docs
 h11==0.14.0
     # via
@@ -103,19 +103,14 @@
     #   hatch.envs.docs
     #   lunchable
 jinja2==3.1.3
     # via
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
-lunchable==1.2.2
-    # via
-    #   lunchable-primelunch
-    #   lunchable-pushlunch
-    #   lunchable-splitlunch
 lunchable-primelunch==1.0.1
     # via
     #   -c requirements.txt
     #   hatch.envs.docs
 lunchable-pushlunch==1.0.1
     # via
     #   -c requirements.txt
@@ -137,15 +132,15 @@
     # via hatch.envs.docs
 markdown-exec==1.8.0
     # via hatch.envs.docs
 markdown-it-py==3.0.0
     # via
     #   -c requirements.txt
     #   rich
-markupsafe==2.1.4
+markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocstrings
 mdurl==0.1.2
     # via
     #   -c requirements.txt
@@ -167,15 +162,15 @@
     #   mkdocstrings
 mkdocs-click==0.8.1
     # via hatch.envs.docs
 mkdocs-gen-files==0.5.0
     # via hatch.envs.docs
 mkdocs-literate-nav==0.6.1
     # via hatch.envs.docs
-mkdocs-material==9.5.6
+mkdocs-material==9.5.8
     # via hatch.envs.docs
 mkdocs-material-extensions==1.3.1
     # via mkdocs-material
 mkdocs-section-index==0.3.8
     # via hatch.envs.docs
 mkdocstrings==0.24.0
     # via
@@ -197,15 +192,15 @@
     # via mkdocs-material
 pandas==2.2.0
     # via
     #   -c requirements.txt
     #   lunchable-primelunch
 pathspec==0.12.1
     # via mkdocs
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via
     #   mkdocs
     #   mkdocstrings
 pydantic==2.6.0
     # via
     #   -c requirements.txt
     #   hatch.envs.docs
@@ -284,13 +279,16 @@
     # via
     #   -c requirements.txt
     #   pandas
 urllib3==2.1.0
     # via
     #   -c requirements.txt
     #   requests
-watchdog==3.0.0
+watchdog==4.0.0
     # via mkdocs
 zipp==3.17.0
     # via
     #   -c requirements.txt
     #   importlib-metadata
+
+# The following packages are considered to be unsafe in a requirements file:
+# lunchable
```

### Comparing `lunchable-1.3.2/requirements/requirements-lint.txt` & `lunchable-1.3.3/requirements/requirements-lint.txt`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/requirements/requirements-test.txt` & `lunchable-1.3.3/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/conftest.py` & `lunchable-1.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/test_cli.py` & `lunchable-1.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/test_assets.py` & `lunchable-1.3.3/tests/models/test_assets.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/test_budgets.py` & `lunchable-1.3.3/tests/models/test_budgets.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/test_categories.py` & `lunchable-1.3.3/tests/models/test_categories.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/test_crypto.py` & `lunchable-1.3.3/tests/models/test_crypto.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/test_plaid_accounts.py` & `lunchable-1.3.3/tests/models/test_plaid_accounts.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/test_recurring_expenses.py` & `lunchable-1.3.3/tests/models/test_recurring_expenses.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/test_tags.py` & `lunchable-1.3.3/tests/models/test_tags.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/test_transactions.py` & `lunchable-1.3.3/tests/models/test_transactions.py`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_204_response.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_204_response.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_add_to_category_group.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_add_to_category_group.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_create_and_delete_transaction_group.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_create_and_delete_transaction_group.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_create_asset.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_create_asset.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_create_category.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_create_category.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_create_category_group.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_create_category_group.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_delete_budget.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_delete_budget.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_delete_category.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_delete_category.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_delete_category_force.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_delete_category_force.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_assets.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_assets.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_budgets.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_budgets.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_categories.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_categories.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_categories_flattened.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_categories_flattened.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_categories_nested.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_categories_nested.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_category.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_category.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_crypto.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_crypto.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_plaid_accounts.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_plaid_accounts.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_recurring_expenses.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_recurring_expenses.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_tags.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_tags.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_transaction.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_transaction_group.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_transaction_group.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_transactions.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_transactions.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_transactions_no_paginate.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_transactions_no_paginate.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_uncleared_transactions.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_uncleared_transactions.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_get_user.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_get_user.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_insert_transactions.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_insert_transactions.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_split_transaction.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_split_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_trigger_fetch_from_plaid.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_trigger_fetch_from_plaid.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_unsplit_transaction.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_unsplit_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_update_asset.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_update_asset.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_update_category.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_update_category.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_update_crypto.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_update_crypto.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_update_transaction.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_update_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/tests/models/cassettes/test_upsert_budget.yaml` & `lunchable-1.3.3/tests/models/cassettes/test_upsert_budget.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/.gitignore` & `lunchable-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/LICENSE` & `lunchable-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lunchable-1.3.2/README.md` & `lunchable-1.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     width="400" alt="lunchable">  </a>
 </div>
 
 <p align="center">
   <a href="https://github.com/juftin/lunchable"><img src="https://img.shields.io/pypi/v/lunchable?color=blue&label=lunchable" alt="PyPI"></a>
   <a href="https://pypi.python.org/pypi/lunchable/"><img src="https://img.shields.io/pypi/pyversions/lunchable" alt="PyPI - Python Version"></a>
   <a href="https://hub.docker.com/r/juftin/lunchable"><img src="https://img.shields.io/docker/v/juftin/lunchable?color=blue&label=docker&logo=docker" alt="Docker Image Version"></a>
+  <a href="https://github.com/conda-forge/lunchable-feedstock"><img src="https://img.shields.io/conda/v/conda-forge/lunchable?label=conda-forge" alt="Conda Version"></a>
   <a href="https://github.com/juftin/lunchable/blob/main/LICENSE"><img src="https://img.shields.io/github/license/juftin/lunchable?color=blue&label=License" alt="GitHub License"></a>
   <a href="https://github.com/juftin/lunchable/actions/workflows/tests.yaml?query=branch%3Amain"><img src="https://github.com/juftin/lunchable/actions/workflows/tests.yaml/badge.svg?branch=main" alt="Testing Status"></a>
   <a href="https://codecov.io/gh/juftin/lunchable"><img src="https://codecov.io/gh/juftin/lunchable/graph/badge.svg?token=2IGD9E5L8K"/></a>
   <a href="https://github.com/pypa/hatch"><img src="https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg" alt="Hatch project"></a>
   <a href="https://github.com/astral-sh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="Ruff"></a>
   <a href="https://github.com/pre-commit/pre-commit"><img src="https://img.shields.io/badge/pre--commit-enabled-lightgreen?logo=pre-commit" alt="pre-commit"></a>
   <a href="https://github.com/semantic-release/semantic-release"><img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="semantic-release"></a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                             ************ lluunncchhaabbllee ************
                                   _[_l_u_n_c_h_a_b_l_e_]
-  _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_D_o_c_k_e_r_ _I_m_a_g_e_ _V_e_r_s_i_o_n_]_[_G_i_t_H_u_b_ _L_i_c_e_n_s_e_]_[_T_e_s_t_i_n_g
-             _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_j_u_f_t_i_n_/_l_u_n_c_h_a_b_l_e_/_g_r_a_p_h_/
+   _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_D_o_c_k_e_r_ _I_m_a_g_e_ _V_e_r_s_i_o_n_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_G_i_t_H_u_b
+    _L_i_c_e_n_s_e_]_[_T_e_s_t_i_n_g_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_j_u_f_t_i_n_/_l_u_n_c_h_a_b_l_e_/_g_r_a_p_h_/
 _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_2_I_G_D_9_E_5_L_8_K_]_[_H_a_t_c_h_ _p_r_o_j_e_c_t_]_[_R_u_f_f_]_[_p_r_e_-_c_o_m_m_i_t_]_[_s_e_m_a_n_t_i_c_-_r_e_l_e_a_s_e_]
                                    _[_G_i_t_m_o_j_i_]
 **lunchable** is a Python Client for the [Lunch Money Developer API](https://
 lunchmoney.dev). It's built on top of [pydantic](https://github.com/pydantic/
 pydantic) and [httpx](https://github.com/encode/httpx/), it offers an
 _intuitive_ API, a _simple_ CLI, complete coverage of all endpoints, and a
 _plugin_ framework for extending the functionality of the library. ###
```

### Comparing `lunchable-1.3.2/pyproject.toml` & `lunchable-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,18 @@
 
 [tool.hatch.envs.docs]
 detached = false
 extra-dependencies = [
   "griffe-fieldz"
 ]
 features = ["all"]
+pip-compile-args = [
+  "--unsafe-package",
+  "lunchable"
+]
 pip-compile-constraint = "default"
 template = "docs"
 type = "pip-compile"
 
 [tool.hatch.envs.gen]
 detached = true
```

### Comparing `lunchable-1.3.2/PKG-INFO` & `lunchable-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lunchable
-Version: 1.3.2
+Version: 1.3.3
 Summary: A simple Python SDK around the Lunch Money Developer API
 Project-URL: Changelog, https://github.com/juftin/lunchable/releases
 Project-URL: Discussions, https://github.com/juftin/lunchable/discussions
 Project-URL: Docker, https://hub.docker.com/r/juftin/lunchable
 Project-URL: Documentation, https://github.com/juftin/lunchable#readme
 Project-URL: Issues, https://github.com/juftin/lunchable/issues
 Project-URL: Source, https://github.com/juftin/lunchable
@@ -54,14 +54,15 @@
     width="400" alt="lunchable">  </a>
 </div>
 
 <p align="center">
   <a href="https://github.com/juftin/lunchable"><img src="https://img.shields.io/pypi/v/lunchable?color=blue&label=lunchable" alt="PyPI"></a>
   <a href="https://pypi.python.org/pypi/lunchable/"><img src="https://img.shields.io/pypi/pyversions/lunchable" alt="PyPI - Python Version"></a>
   <a href="https://hub.docker.com/r/juftin/lunchable"><img src="https://img.shields.io/docker/v/juftin/lunchable?color=blue&label=docker&logo=docker" alt="Docker Image Version"></a>
+  <a href="https://github.com/conda-forge/lunchable-feedstock"><img src="https://img.shields.io/conda/v/conda-forge/lunchable?label=conda-forge" alt="Conda Version"></a>
   <a href="https://github.com/juftin/lunchable/blob/main/LICENSE"><img src="https://img.shields.io/github/license/juftin/lunchable?color=blue&label=License" alt="GitHub License"></a>
   <a href="https://github.com/juftin/lunchable/actions/workflows/tests.yaml?query=branch%3Amain"><img src="https://github.com/juftin/lunchable/actions/workflows/tests.yaml/badge.svg?branch=main" alt="Testing Status"></a>
   <a href="https://codecov.io/gh/juftin/lunchable"><img src="https://codecov.io/gh/juftin/lunchable/graph/badge.svg?token=2IGD9E5L8K"/></a>
   <a href="https://github.com/pypa/hatch"><img src="https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg" alt="Hatch project"></a>
   <a href="https://github.com/astral-sh/ruff"><img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="Ruff"></a>
   <a href="https://github.com/pre-commit/pre-commit"><img src="https://img.shields.io/badge/pre--commit-enabled-lightgreen?logo=pre-commit" alt="pre-commit"></a>
   <a href="https://github.com/semantic-release/semantic-release"><img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="semantic-release"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lunchable Version: 1.3.2 Summary: A simple Python
+Metadata-Version: 2.3 Name: lunchable Version: 1.3.3 Summary: A simple Python
 SDK around the Lunch Money Developer API Project-URL: Changelog, https://
 github.com/juftin/lunchable/releases Project-URL: Discussions, https://
 github.com/juftin/lunchable/discussions Project-URL: Docker, https://
 hub.docker.com/r/juftin/lunchable Project-URL: Documentation, https://
 github.com/juftin/lunchable#readme Project-URL: Issues, https://github.com/
 juftin/lunchable/issues Project-URL: Source, https://github.com/juftin/
 lunchable Author-email: Justin Flannery
@@ -25,16 +25,16 @@
 extra == 'plugins' Requires-Dist: lunchable-splitlunch; extra == 'plugins'
 Provides-Extra: primelunch Requires-Dist: lunchable-primelunch; extra ==
 'primelunch' Provides-Extra: pushlunch Requires-Dist: lunchable-pushlunch;
 extra == 'pushlunch' Provides-Extra: splitlunch Requires-Dist: lunchable-
 splitlunch; extra == 'splitlunch' Description-Content-Type: text/markdown
                             ************ lluunncchhaabbllee ************
                                   _[_l_u_n_c_h_a_b_l_e_]
-  _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_D_o_c_k_e_r_ _I_m_a_g_e_ _V_e_r_s_i_o_n_]_[_G_i_t_H_u_b_ _L_i_c_e_n_s_e_]_[_T_e_s_t_i_n_g
-             _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_j_u_f_t_i_n_/_l_u_n_c_h_a_b_l_e_/_g_r_a_p_h_/
+   _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_D_o_c_k_e_r_ _I_m_a_g_e_ _V_e_r_s_i_o_n_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_G_i_t_H_u_b
+    _L_i_c_e_n_s_e_]_[_T_e_s_t_i_n_g_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_j_u_f_t_i_n_/_l_u_n_c_h_a_b_l_e_/_g_r_a_p_h_/
 _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_2_I_G_D_9_E_5_L_8_K_]_[_H_a_t_c_h_ _p_r_o_j_e_c_t_]_[_R_u_f_f_]_[_p_r_e_-_c_o_m_m_i_t_]_[_s_e_m_a_n_t_i_c_-_r_e_l_e_a_s_e_]
                                    _[_G_i_t_m_o_j_i_]
 **lunchable** is a Python Client for the [Lunch Money Developer API](https://
 lunchmoney.dev). It's built on top of [pydantic](https://github.com/pydantic/
 pydantic) and [httpx](https://github.com/encode/httpx/), it offers an
 _intuitive_ API, a _simple_ CLI, complete coverage of all endpoints, and a
 _plugin_ framework for extending the functionality of the library. ###
```

