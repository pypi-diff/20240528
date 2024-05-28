# Comparing `tmp/python_gitlab-4.5.0.tar.gz` & `tmp/python_gitlab-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_gitlab-4.5.0.tar", last modified: Mon May 13 22:19:49 2024, max compression
+gzip compressed data, was "python_gitlab-4.6.0.tar", last modified: Tue May 28 00:46:07 2024, max compression
```

## Comparing `python_gitlab-4.5.0.tar` & `python_gitlab-4.6.0.tar`

### file list

```diff
@@ -1,359 +1,360 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.682675 python_gitlab-4.5.0/
--rw-r--r--   0 root         (0) root         (0)      526 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)   704321 2024-05-13 22:19:43.000000 python_gitlab-4.5.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     7651 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/COPYING
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8223 2024-05-13 22:19:49.682675 python_gitlab-4.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6472 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.618675 python_gitlab-4.5.0/docs/
--rw-r--r--   0 root         (0) root         (0)     6790 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.606675 python_gitlab-4.5.0/docs/_static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.618675 python_gitlab-4.5.0/docs/_static/js/
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/_static/js/gitter.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.618675 python_gitlab-4.5.0/docs/api/
--rw-r--r--   0 root         (0) root         (0)     1362 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api/gitlab.rst
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api/gitlab.v4.rst
--rw-r--r--   0 root         (0) root         (0)     4280 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api-levels.rst
--rw-r--r--   0 root         (0) root         (0)     1702 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api-objects.rst
--rw-r--r--   0 root         (0) root         (0)     6622 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api-usage-advanced.rst
--rw-r--r--   0 root         (0) root         (0)    15176 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api-usage.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/changelog.md
--rw-r--r--   0 root         (0) root         (0)     7780 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/cli-examples.rst
--rw-r--r--   0 root         (0) root         (0)      643 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/cli-objects.rst
--rw-r--r--   0 root         (0) root         (0)    11215 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/cli-usage.rst
--rw-r--r--   0 root         (0) root         (0)     9858 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.618675 python_gitlab-4.5.0/docs/ext/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/ext/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/ext/docstrings.py
--rw-r--r--   0 root         (0) root         (0)     1246 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/ext/manager_tmpl.j2
--rw-r--r--   0 root         (0) root         (0)     3828 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/faq.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.630675 python_gitlab-4.5.0/docs/gl_objects/
--rw-r--r--   0 root         (0) root         (0)     1487 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/access_requests.rst
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/appearance.rst
--rw-r--r--   0 root         (0) root         (0)      619 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/applications.rst
--rw-r--r--   0 root         (0) root         (0)     1088 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/badges.rst
--rw-r--r--   0 root         (0) root         (0)     2409 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/boards.rst
--rw-r--r--   0 root         (0) root         (0)      848 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/branches.rst
--rw-r--r--   0 root         (0) root         (0)     2142 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/bulk_imports.rst
--rw-r--r--   0 root         (0) root         (0)     1865 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/ci_lint.rst
--rw-r--r--   0 root         (0) root         (0)     1930 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/clusters.rst
--rw-r--r--   0 root         (0) root         (0)     3354 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/commits.rst
--rw-r--r--   0 root         (0) root         (0)     1247 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/deploy_keys.rst
--rw-r--r--   0 root         (0) root         (0)     4093 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/deploy_tokens.rst
--rw-r--r--   0 root         (0) root         (0)     1803 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/deployments.rst
--rw-r--r--   0 root         (0) root         (0)     3431 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/discussions.rst
--rw-r--r--   0 root         (0) root         (0)     1461 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/draft_notes.rst
--rw-r--r--   0 root         (0) root         (0)     1196 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/emojis.rst
--rw-r--r--   0 root         (0) root         (0)      984 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/environments.rst
--rw-r--r--   0 root         (0) root         (0)     1302 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/epics.rst
--rw-r--r--   0 root         (0) root         (0)     2206 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/events.rst
--rw-r--r--   0 root         (0) root         (0)      625 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/features.rst
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/geo_nodes.rst
--rw-r--r--   0 root         (0) root         (0)     1128 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/group_access_tokens.rst
--rw-r--r--   0 root         (0) root         (0)    10727 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/groups.rst
--rw-r--r--   0 root         (0) root         (0)     2057 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/invitations.rst
--rw-r--r--   0 root         (0) root         (0)     7003 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/issues.rst
--rw-r--r--   0 root         (0) root         (0)      694 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/iterations.rst
--rw-r--r--   0 root         (0) root         (0)     2960 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/job_token_scope.rst
--rw-r--r--   0 root         (0) root         (0)      490 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/keys.rst
--rw-r--r--   0 root         (0) root         (0)     2292 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/labels.rst
--rw-r--r--   0 root         (0) root         (0)     2923 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/merge_request_approvals.rst
--rw-r--r--   0 root         (0) root         (0)     5625 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/merge_requests.rst
--rw-r--r--   0 root         (0) root         (0)      625 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/merge_trains.rst
--rw-r--r--   0 root         (0) root         (0)      988 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/messages.rst
--rw-r--r--   0 root         (0) root         (0)     2671 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/milestones.rst
--rw-r--r--   0 root         (0) root         (0)      697 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/namespaces.rst
--rw-r--r--   0 root         (0) root         (0)     1675 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/notes.rst
--rw-r--r--   0 root         (0) root         (0)     1877 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/notifications.rst
--rw-r--r--   0 root         (0) root         (0)     3520 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/packages.rst
--rw-r--r--   0 root         (0) root         (0)     1240 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/pagesdomains.rst
--rw-r--r--   0 root         (0) root         (0)     2093 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/personal_access_tokens.rst
--rw-r--r--   0 root         (0) root         (0)     9572 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/pipelines_and_jobs.rst
--rw-r--r--   0 root         (0) root         (0)     1162 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/project_access_tokens.rst
--rw-r--r--   0 root         (0) root         (0)    22202 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/projects.rst
--rw-r--r--   0 root         (0) root         (0)     1456 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/protected_branches.rst
--rw-r--r--   0 root         (0) root         (0)     1061 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/protected_environments.rst
--rw-r--r--   0 root         (0) root         (0)     2038 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/releases.rst
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/remote_mirrors.rst
--rw-r--r--   0 root         (0) root         (0)      760 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/repositories.rst
--rw-r--r--   0 root         (0) root         (0)     1128 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/repository_tags.rst
--rw-r--r--   0 root         (0) root         (0)      970 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/resource_groups.rst
--rw-r--r--   0 root         (0) root         (0)     3906 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/runners.rst
--rw-r--r--   0 root         (0) root         (0)     2351 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/search.rst
--rw-r--r--   0 root         (0) root         (0)     1036 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/secure_files.rst
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/settings.rst
--rw-r--r--   0 root         (0) root         (0)      393 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/sidekiq.rst
--rw-r--r--   0 root         (0) root         (0)     1585 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/snippets.rst
--rw-r--r--   0 root         (0) root         (0)      357 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/statistics.rst
--rw-r--r--   0 root         (0) root         (0)      596 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/system_hooks.rst
--rw-r--r--   0 root         (0) root         (0)     2062 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/templates.rst
--rw-r--r--   0 root         (0) root         (0)      840 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/todos.rst
--rw-r--r--   0 root         (0) root         (0)      969 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/topics.rst
--rw-r--r--   0 root         (0) root         (0)    11029 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/users.rst
--rw-r--r--   0 root         (0) root         (0)     2513 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/variables.rst
--rw-r--r--   0 root         (0) root         (0)     2393 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/wikis.rst
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6715 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     8182 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/release-notes.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.634675 python_gitlab-4.5.0/gitlab/
--rw-r--r--   0 root         (0) root         (0)     1382 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)       68 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.634675 python_gitlab-4.5.0/gitlab/_backends/
--rw-r--r--   0 root         (0) root         (0)      392 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/_backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)      842 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/_backends/protocol.py
--rw-r--r--   0 root         (0) root         (0)     5534 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/_backends/requests_backend.py
--rw-r--r--   0 root         (0) root         (0)      249 2024-05-13 22:19:43.000000 python_gitlab-4.5.0/gitlab/_version.py
--rw-r--r--   0 root         (0) root         (0)    13780 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/base.py
--rw-r--r--   0 root         (0) root         (0)    12870 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/cli.py
--rw-r--r--   0 root         (0) root         (0)    48755 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/client.py
--rw-r--r--   0 root         (0) root         (0)     9088 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/config.py
--rw-r--r--   0 root         (0) root         (0)     5352 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/const.py
--rw-r--r--   0 root         (0) root         (0)     8303 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    36350 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/mixins.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/py.typed
--rw-r--r--   0 root         (0) root         (0)     3312 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/types.py
--rw-r--r--   0 root         (0) root         (0)     6396 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.634675 python_gitlab-4.5.0/gitlab/v4/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21455 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.650675 python_gitlab-4.5.0/gitlab/v4/objects/
--rw-r--r--   0 root         (0) root         (0)     1958 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/access_requests.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/appearance.py
--rw-r--r--   0 root         (0) root         (0)      591 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/applications.py
--rw-r--r--   0 root         (0) root         (0)     5025 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1910 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/audit_events.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/award_emojis.py
--rw-r--r--   0 root         (0) root         (0)     1464 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/badges.py
--rw-r--r--   0 root         (0) root         (0)     2680 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/boards.py
--rw-r--r--   0 root         (0) root         (0)     1814 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/branches.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/broadcast_messages.py
--rw-r--r--   0 root         (0) root         (0)     1573 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/bulk_imports.py
--rw-r--r--   0 root         (0) root         (0)     2270 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/ci_lint.py
--rw-r--r--   0 root         (0) root         (0)     3750 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/clusters.py
--rw-r--r--   0 root         (0) root         (0)     8214 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/commits.py
--rw-r--r--   0 root         (0) root         (0)     3341 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     1875 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/custom_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1826 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/deploy_keys.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/deploy_tokens.py
--rw-r--r--   0 root         (0) root         (0)     2880 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/deployments.py
--rw-r--r--   0 root         (0) root         (0)     3457 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/discussions.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/draft_notes.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/environments.py
--rw-r--r--   0 root         (0) root         (0)     4150 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/epics.py
--rw-r--r--   0 root         (0) root         (0)     7067 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/events.py
--rw-r--r--   0 root         (0) root         (0)     1909 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/export_import.py
--rw-r--r--   0 root         (0) root         (0)     1973 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/features.py
--rw-r--r--   0 root         (0) root         (0)    10283 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/files.py
--rw-r--r--   0 root         (0) root         (0)     3646 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/geo_nodes.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/group_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)    15672 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/groups.py
--rw-r--r--   0 root         (0) root         (0)     3598 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/hooks.py
--rw-r--r--   0 root         (0) root         (0)     9205 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/integrations.py
--rw-r--r--   0 root         (0) root         (0)     2734 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/invitations.py
--rw-r--r--   0 root         (0) root         (0)    10162 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/issues.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/iterations.py
--rw-r--r--   0 root         (0) root         (0)     2622 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/job_token_scope.py
--rw-r--r--   0 root         (0) root         (0)     9139 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/jobs.py
--rw-r--r--   0 root         (0) root         (0)      882 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/keys.py
--rw-r--r--   0 root         (0) root         (0)     4736 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/labels.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/ldap.py
--rw-r--r--   0 root         (0) root         (0)     3836 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/members.py
--rw-r--r--   0 root         (0) root         (0)     6146 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/merge_request_approvals.py
--rw-r--r--   0 root         (0) root         (0)    17306 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/merge_requests.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/merge_trains.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/milestones.py
--rw-r--r--   0 root         (0) root         (0)     1502 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/namespaces.py
--rw-r--r--   0 root         (0) root         (0)     8588 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/notes.py
--rw-r--r--   0 root         (0) root         (0)     2061 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/notification_settings.py
--rw-r--r--   0 root         (0) root         (0)     7187 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/packages.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/pages.py
--rw-r--r--   0 root         (0) root         (0)     1315 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/personal_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)     9778 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/pipelines.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/project_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)    44127 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/projects.py
--rw-r--r--   0 root         (0) root         (0)     3041 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/push_rules.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/releases.py
--rw-r--r--   0 root         (0) root         (0)    11048 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/repositories.py
--rw-r--r--   0 root         (0) root         (0)     1427 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/resource_groups.py
--rw-r--r--   0 root         (0) root         (0)      517 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/reviewers.py
--rw-r--r--   0 root         (0) root         (0)     4883 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/runners.py
--rw-r--r--   0 root         (0) root         (0)     2511 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/secure_files.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/settings.py
--rw-r--r--   0 root         (0) root         (0)     2956 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/sidekiq.py
--rw-r--r--   0 root         (0) root         (0)     6018 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/snippets.py
--rw-r--r--   0 root         (0) root         (0)     2638 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/statistics.py
--rw-r--r--   0 root         (0) root         (0)     1453 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/tags.py
--rw-r--r--   0 root         (0) root         (0)     1726 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/templates.py
--rw-r--r--   0 root         (0) root         (0)     1826 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/todos.py
--rw-r--r--   0 root         (0) root         (0)     2199 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/topics.py
--rw-r--r--   0 root         (0) root         (0)      824 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/triggers.py
--rw-r--r--   0 root         (0) root         (0)    21281 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/users.py
--rw-r--r--   0 root         (0) root         (0)     2627 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/variables.py
--rw-r--r--   0 root         (0) root         (0)     1775 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/wikis.py
--rw-r--r--   0 root         (0) root         (0)     4018 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.678675 python_gitlab-4.5.0/python_gitlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8223 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10674 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-docker.txt
--rw-r--r--   0 root         (0) root         (0)      115 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-docs.txt
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-lint.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-precommit.txt
--rw-r--r--   0 root         (0) root         (0)      204 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 22:19:49.682675 python_gitlab-4.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.654675 python_gitlab-4.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1090 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.654675 python_gitlab-4.5.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.658675 python_gitlab-4.5.0/tests/functional/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_boards.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_branches.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_bulk_imports.py
--rw-r--r--   0 root         (0) root         (0)      927 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_current_user.py
--rw-r--r--   0 root         (0) root         (0)      395 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_deploy_keys.py
--rw-r--r--   0 root         (0) root         (0)     1216 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_deploy_tokens.py
--rw-r--r--   0 root         (0) root         (0)      743 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_epics.py
--rw-r--r--   0 root         (0) root         (0)     7787 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)     9601 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_groups.py
--rw-r--r--   0 root         (0) root         (0)     3683 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_issues.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_keys.py
--rw-r--r--   0 root         (0) root         (0)     1290 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_lazy_objects.py
--rw-r--r--   0 root         (0) root         (0)     9723 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_merge_requests.py
--rw-r--r--   0 root         (0) root         (0)     3909 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_packages.py
--rw-r--r--   0 root         (0) root         (0)     3295 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_project_job_token_scope.py
--rw-r--r--   0 root         (0) root         (0)    10796 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_projects.py
--rw-r--r--   0 root         (0) root         (0)      710 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_push_rules.py
--rw-r--r--   0 root         (0) root         (0)     2016 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_releases.py
--rw-r--r--   0 root         (0) root         (0)     5526 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_repository.py
--rw-r--r--   0 root         (0) root         (0)      944 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_services.py
--rw-r--r--   0 root         (0) root         (0)     2117 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_snippets.py
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_statistics.py
--rw-r--r--   0 root         (0) root         (0)      971 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_topics.py
--rw-r--r--   0 root         (0) root         (0)     5007 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_users.py
--rw-r--r--   0 root         (0) root         (0)     1289 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_variables.py
--rw-r--r--   0 root         (0) root         (0)     1728 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_wikis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.662675 python_gitlab-4.5.0/tests/functional/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/conftest.py
--rw-r--r--   0 root         (0) root         (0)     7371 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2386 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1320 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_packages.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_projects.py
--rw-r--r--   0 root         (0) root         (0)     3791 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_repository.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_resource_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)      558 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_users.py
--rw-r--r--   0 root         (0) root         (0)    15703 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_v4.py
--rw-r--r--   0 root         (0) root         (0)     1416 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_variables.py
--rw-r--r--   0 root         (0) root         (0)    20667 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/conftest.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/ee-test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.662675 python_gitlab-4.5.0/tests/functional/fixtures/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/.env
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      592 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/avatar.png
--rw-r--r--   0 root         (0) root         (0)     1892 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/create_license.rb
--rw-r--r--   0 root         (0) root         (0)     1717 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      697 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/docker.py
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/invalid_auth.cfg
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/invalid_version.cfg
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/set_token.rb
--rw-r--r--   0 root         (0) root         (0)     2885 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.662675 python_gitlab-4.5.0/tests/install/
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/install/test_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.662675 python_gitlab-4.5.0/tests/smoke/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/smoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/smoke/test_dists.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/_backends/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/_backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1765 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/_backends/test_requests_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/base/
--rw-r--r--   0 root         (0) root         (0)      734 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/base/test_rest_manager.py
--rw-r--r--   0 root         (0) root         (0)    10861 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/base/test_rest_object.py
--rw-r--r--   0 root         (0) root         (0)     3194 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2695 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4353 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/meta/test_ensure_type_hints.py
--rw-r--r--   0 root         (0) root         (0)     1243 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/meta/test_imports.py
--rw-r--r--   0 root         (0) root         (0)     3996 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/meta/test_mro.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/mixins/test_meta_mixins.py
--rw-r--r--   0 root         (0) root         (0)    16409 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/mixins/test_mixin_methods.py
--rw-r--r--   0 root         (0) root         (0)     1218 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/mixins/test_object_mixins_attributes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.678675 python_gitlab-4.5.0/tests/unit/objects/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2212 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2063 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_appearance.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_applications.py
--rw-r--r--   0 root         (0) root         (0)     2928 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_audit_events.py
--rw-r--r--   0 root         (0) root         (0)     5724 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_badges.py
--rw-r--r--   0 root         (0) root         (0)     3665 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_bridges.py
--rw-r--r--   0 root         (0) root         (0)     4437 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_bulk_imports.py
--rw-r--r--   0 root         (0) root         (0)     2699 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_ci_lint.py
--rw-r--r--   0 root         (0) root         (0)     3345 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_commits.py
--rw-r--r--   0 root         (0) root         (0)     1300 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_deploy_tokens.py
--rw-r--r--   0 root         (0) root         (0)     5438 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_deployments.py
--rw-r--r--   0 root         (0) root         (0)     5089 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_draft_notes.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_environments.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_group_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)    14054 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_groups.py
--rw-r--r--   0 root         (0) root         (0)     5269 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_hooks.py
--rw-r--r--   0 root         (0) root         (0)     4748 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_invitations.py
--rw-r--r--   0 root         (0) root         (0)     3000 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_issues.py
--rw-r--r--   0 root         (0) root         (0)     1210 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_iterations.py
--rw-r--r--   0 root         (0) root         (0)     1226 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_job_artifacts.py
--rw-r--r--   0 root         (0) root         (0)     6210 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_job_token_scope.py
--rw-r--r--   0 root         (0) root         (0)     5248 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_jobs.py
--rw-r--r--   0 root         (0) root         (0)     1330 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_keys.py
--rw-r--r--   0 root         (0) root         (0)     2236 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_members.py
--rw-r--r--   0 root         (0) root         (0)     1645 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_merge_request_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     3641 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_merge_requests.py
--rw-r--r--   0 root         (0) root         (0)     2012 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_merge_trains.py
--rw-r--r--   0 root         (0) root         (0)    12878 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_packages.py
--rw-r--r--   0 root         (0) root         (0)     4464 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_personal_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)     3223 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_pipeline_schedules.py
--rw-r--r--   0 root         (0) root         (0)     5554 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_project_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)     6454 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_project_import_export.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_project_merge_request_approvals.py
--rw-r--r--   0 root         (0) root         (0)      824 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_project_statistics.py
--rw-r--r--   0 root         (0) root         (0)    21091 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_projects.py
--rw-r--r--   0 root         (0) root         (0)     2680 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_registry_repositories.py
--rw-r--r--   0 root         (0) root         (0)     4215 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_releases.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_remote_mirrors.py
--rw-r--r--   0 root         (0) root         (0)     1383 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_repositories.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_groups.py
--rw-r--r--   0 root         (0) root         (0)     1717 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_iteration_events.py
--rw-r--r--   0 root         (0) root         (0)     3424 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_label_events.py
--rw-r--r--   0 root         (0) root         (0)     2458 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_milestone_events.py
--rw-r--r--   0 root         (0) root         (0)     3195 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_state_events.py
--rw-r--r--   0 root         (0) root         (0)     8133 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_runners.py
--rw-r--r--   0 root         (0) root         (0)     2942 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_secure_files.py
--rw-r--r--   0 root         (0) root         (0)     3169 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_services.py
--rw-r--r--   0 root         (0) root         (0)     2498 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_snippets.py
--rw-r--r--   0 root         (0) root         (0)     1334 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_statistics.py
--rw-r--r--   0 root         (0) root         (0)     1455 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_submodules.py
--rw-r--r--   0 root         (0) root         (0)     2193 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_todos.py
--rw-r--r--   0 root         (0) root         (0)     3299 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_topics.py
--rw-r--r--   0 root         (0) root         (0)     8577 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_users.py
--rw-r--r--   0 root         (0) root         (0)     5173 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_variables.py
--rw-r--r--   0 root         (0) root         (0)     7536 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_cli.py
--rw-r--r--   0 root         (0) root         (0)    11083 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_config.py
--rw-r--r--   0 root         (0) root         (0)      800 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12171 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)     7347 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_gitlab_auth.py
--rw-r--r--   0 root         (0) root         (0)    25196 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_gitlab_http_methods.py
--rw-r--r--   0 root         (0) root         (0)     4011 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_types.py
--rw-r--r--   0 root         (0) root         (0)     6441 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     3423 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.355049 python_gitlab-4.6.0/
+-rw-r--r--   0 root         (0) root         (0)      526 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)   711492 2024-05-28 00:46:00.000000 python_gitlab-4.6.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     7651 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8222 2024-05-28 00:46:07.355049 python_gitlab-4.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6472 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.291049 python_gitlab-4.6.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     6790 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.279048 python_gitlab-4.6.0/docs/_static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.291049 python_gitlab-4.6.0/docs/_static/js/
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/_static/js/gitter.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.291049 python_gitlab-4.6.0/docs/api/
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/api/gitlab.rst
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/api/gitlab.v4.rst
+-rw-r--r--   0 root         (0) root         (0)     4280 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/api-levels.rst
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/api-objects.rst
+-rw-r--r--   0 root         (0) root         (0)     6622 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/api-usage-advanced.rst
+-rw-r--r--   0 root         (0) root         (0)    15176 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/api-usage.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/changelog.md
+-rw-r--r--   0 root         (0) root         (0)     7780 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/cli-examples.rst
+-rw-r--r--   0 root         (0) root         (0)      643 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/cli-objects.rst
+-rw-r--r--   0 root         (0) root         (0)    11215 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/cli-usage.rst
+-rw-r--r--   0 root         (0) root         (0)     9858 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.291049 python_gitlab-4.6.0/docs/ext/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/ext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/ext/docstrings.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/ext/manager_tmpl.j2
+-rw-r--r--   0 root         (0) root         (0)     3828 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/faq.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.307049 python_gitlab-4.6.0/docs/gl_objects/
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/access_requests.rst
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/appearance.rst
+-rw-r--r--   0 root         (0) root         (0)      619 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/applications.rst
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/badges.rst
+-rw-r--r--   0 root         (0) root         (0)     2409 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/boards.rst
+-rw-r--r--   0 root         (0) root         (0)      848 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/branches.rst
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/bulk_imports.rst
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/ci_lint.rst
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/clusters.rst
+-rw-r--r--   0 root         (0) root         (0)     3354 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/commits.rst
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/deploy_keys.rst
+-rw-r--r--   0 root         (0) root         (0)     4093 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/deploy_tokens.rst
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/deployments.rst
+-rw-r--r--   0 root         (0) root         (0)     3431 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/discussions.rst
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/draft_notes.rst
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/emojis.rst
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/environments.rst
+-rw-r--r--   0 root         (0) root         (0)     1302 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/epics.rst
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/events.rst
+-rw-r--r--   0 root         (0) root         (0)      625 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/features.rst
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/geo_nodes.rst
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/group_access_tokens.rst
+-rw-r--r--   0 root         (0) root         (0)    11232 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/groups.rst
+-rw-r--r--   0 root         (0) root         (0)     2057 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/invitations.rst
+-rw-r--r--   0 root         (0) root         (0)     7003 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/issues.rst
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/iterations.rst
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/job_token_scope.rst
+-rw-r--r--   0 root         (0) root         (0)      490 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/keys.rst
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/labels.rst
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/merge_request_approvals.rst
+-rw-r--r--   0 root         (0) root         (0)     5625 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/merge_requests.rst
+-rw-r--r--   0 root         (0) root         (0)      625 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/merge_trains.rst
+-rw-r--r--   0 root         (0) root         (0)      988 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/messages.rst
+-rw-r--r--   0 root         (0) root         (0)     2671 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/milestones.rst
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/namespaces.rst
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/notes.rst
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/notifications.rst
+-rw-r--r--   0 root         (0) root         (0)     3520 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/packages.rst
+-rw-r--r--   0 root         (0) root         (0)     1240 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/pagesdomains.rst
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/personal_access_tokens.rst
+-rw-r--r--   0 root         (0) root         (0)     9572 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/pipelines_and_jobs.rst
+-rw-r--r--   0 root         (0) root         (0)     1162 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/project_access_tokens.rst
+-rw-r--r--   0 root         (0) root         (0)    22202 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/projects.rst
+-rw-r--r--   0 root         (0) root         (0)     1456 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/protected_branches.rst
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/protected_environments.rst
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/releases.rst
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/remote_mirrors.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/repositories.rst
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/repository_tags.rst
+-rw-r--r--   0 root         (0) root         (0)      970 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/resource_groups.rst
+-rw-r--r--   0 root         (0) root         (0)     3906 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/runners.rst
+-rw-r--r--   0 root         (0) root         (0)     2351 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/search.rst
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/secure_files.rst
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/settings.rst
+-rw-r--r--   0 root         (0) root         (0)      393 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/sidekiq.rst
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/snippets.rst
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/statistics.rst
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/system_hooks.rst
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/templates.rst
+-rw-r--r--   0 root         (0) root         (0)      840 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/todos.rst
+-rw-r--r--   0 root         (0) root         (0)      969 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/topics.rst
+-rw-r--r--   0 root         (0) root         (0)    11029 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/users.rst
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/variables.rst
+-rw-r--r--   0 root         (0) root         (0)     2393 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/gl_objects/wikis.rst
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6715 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     8182 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/docs/release-notes.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.307049 python_gitlab-4.6.0/gitlab/
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.307049 python_gitlab-4.6.0/gitlab/_backends/
+-rw-r--r--   0 root         (0) root         (0)      392 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/_backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/_backends/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     5534 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/_backends/requests_backend.py
+-rw-r--r--   0 root         (0) root         (0)      249 2024-05-28 00:46:00.000000 python_gitlab-4.6.0/gitlab/_version.py
+-rw-r--r--   0 root         (0) root         (0)    13780 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/base.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/cli.py
+-rw-r--r--   0 root         (0) root         (0)    48774 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/client.py
+-rw-r--r--   0 root         (0) root         (0)     9088 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/config.py
+-rw-r--r--   0 root         (0) root         (0)     5352 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/const.py
+-rw-r--r--   0 root         (0) root         (0)     8303 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    36591 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/mixins.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3312 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/types.py
+-rw-r--r--   0 root         (0) root         (0)     6396 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.311049 python_gitlab-4.6.0/gitlab/v4/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21942 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.327049 python_gitlab-4.6.0/gitlab/v4/objects/
+-rw-r--r--   0 root         (0) root         (0)     1990 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/access_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/appearance.py
+-rw-r--r--   0 root         (0) root         (0)      591 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/applications.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/audit_events.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/award_emojis.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/badges.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/boards.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/branches.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/broadcast_messages.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/bulk_imports.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/ci_lint.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/clusters.py
+-rw-r--r--   0 root         (0) root         (0)     8292 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/commits.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/custom_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/deploy_keys.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/deploy_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/deployments.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/discussions.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/draft_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/environments.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/epics.py
+-rw-r--r--   0 root         (0) root         (0)     7067 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/events.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/export_import.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/features.py
+-rw-r--r--   0 root         (0) root         (0)    10506 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/files.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/geo_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/group_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)    15958 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/groups.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     9229 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/integrations.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/invitations.py
+-rw-r--r--   0 root         (0) root         (0)    10234 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/issues.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/iterations.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/job_token_scope.py
+-rw-r--r--   0 root         (0) root         (0)     9140 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/jobs.py
+-rw-r--r--   0 root         (0) root         (0)      882 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/keys.py
+-rw-r--r--   0 root         (0) root         (0)     4736 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/labels.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/ldap.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/members.py
+-rw-r--r--   0 root         (0) root         (0)     6400 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/merge_request_approvals.py
+-rw-r--r--   0 root         (0) root         (0)    17422 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/merge_requests.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/merge_trains.py
+-rw-r--r--   0 root         (0) root         (0)     7073 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/milestones.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/namespaces.py
+-rw-r--r--   0 root         (0) root         (0)     8588 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/notes.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/notification_settings.py
+-rw-r--r--   0 root         (0) root         (0)     7225 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/packages.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/pages.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/personal_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     9818 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/project_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)    44401 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/projects.py
+-rw-r--r--   0 root         (0) root         (0)     3041 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/push_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/releases.py
+-rw-r--r--   0 root         (0) root         (0)    11221 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/repositories.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/resource_groups.py
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/reviewers.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/runners.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/secure_files.py
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/service_accounts.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/settings.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/sidekiq.py
+-rw-r--r--   0 root         (0) root         (0)     6048 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/snippets.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/statistics.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/templates.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/todos.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/topics.py
+-rw-r--r--   0 root         (0) root         (0)      824 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/triggers.py
+-rw-r--r--   0 root         (0) root         (0)    21381 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/users.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/variables.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/gitlab/v4/objects/wikis.py
+-rw-r--r--   0 root         (0) root         (0)     4017 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.355049 python_gitlab-4.6.0/python_gitlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8222 2024-05-28 00:46:07.000000 python_gitlab-4.6.0/python_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10712 2024-05-28 00:46:07.000000 python_gitlab-4.6.0/python_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 00:46:07.000000 python_gitlab-4.6.0/python_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-28 00:46:07.000000 python_gitlab-4.6.0/python_gitlab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-28 00:46:07.000000 python_gitlab-4.6.0/python_gitlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-28 00:46:07.000000 python_gitlab-4.6.0/python_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/requirements-docker.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/requirements-docs.txt
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/requirements-lint.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/requirements-precommit.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/requirements-test.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 00:46:07.355049 python_gitlab-4.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.327049 python_gitlab-4.6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.327049 python_gitlab-4.6.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.335049 python_gitlab-4.6.0/tests/functional/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_boards.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_branches.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_bulk_imports.py
+-rw-r--r--   0 root         (0) root         (0)      927 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_current_user.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_deploy_keys.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_deploy_tokens.py
+-rw-r--r--   0 root         (0) root         (0)      743 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_epics.py
+-rw-r--r--   0 root         (0) root         (0)     7787 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     9934 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_groups.py
+-rw-r--r--   0 root         (0) root         (0)     3683 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_issues.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_keys.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_lazy_objects.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_merge_requests.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_packages.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_project_job_token_scope.py
+-rw-r--r--   0 root         (0) root         (0)    10796 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_projects.py
+-rw-r--r--   0 root         (0) root         (0)      710 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_push_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_releases.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_repository.py
+-rw-r--r--   0 root         (0) root         (0)      944 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_services.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_snippets.py
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_statistics.py
+-rw-r--r--   0 root         (0) root         (0)      971 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_topics.py
+-rw-r--r--   0 root         (0) root         (0)     5007 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_users.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_variables.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/api/test_wikis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.335049 python_gitlab-4.6.0/tests/functional/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7139 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli_artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli_packages.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli_projects.py
+-rw-r--r--   0 root         (0) root         (0)     3791 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli_resource_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli_users.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli_v4.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/cli/test_cli_variables.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/conftest.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/ee-test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.339049 python_gitlab-4.6.0/tests/functional/fixtures/
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/.env
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      592 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/avatar.png
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/create_license.rb
+-rw-r--r--   0 root         (0) root         (0)     1717 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/docker.py
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/invalid_auth.cfg
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/invalid_version.cfg
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/fixtures/set_token.rb
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/functional/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.339049 python_gitlab-4.6.0/tests/install/
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/install/test_install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.339049 python_gitlab-4.6.0/tests/smoke/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/smoke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/smoke/test_dists.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.339049 python_gitlab-4.6.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.343049 python_gitlab-4.6.0/tests/unit/_backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/_backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/_backends/test_requests_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.343049 python_gitlab-4.6.0/tests/unit/base/
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/base/test_rest_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10861 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/base/test_rest_object.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.343049 python_gitlab-4.6.0/tests/unit/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4353 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/meta/test_ensure_type_hints.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/meta/test_imports.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/meta/test_mro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.343049 python_gitlab-4.6.0/tests/unit/mixins/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/mixins/test_meta_mixins.py
+-rw-r--r--   0 root         (0) root         (0)    16409 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/mixins/test_mixin_methods.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/mixins/test_object_mixins_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 00:46:07.355049 python_gitlab-4.6.0/tests/unit/objects/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_appearance.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_applications.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_audit_events.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_badges.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_bridges.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_bulk_imports.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_ci_lint.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_commits.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_deploy_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_deployments.py
+-rw-r--r--   0 root         (0) root         (0)     5089 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_draft_notes.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_environments.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_group_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)    14876 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_groups.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_hooks.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_invitations.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_issues.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_iterations.py
+-rw-r--r--   0 root         (0) root         (0)     1226 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_job_artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     6210 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_job_token_scope.py
+-rw-r--r--   0 root         (0) root         (0)     5248 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_jobs.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_keys.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_members.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_merge_request_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_merge_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_merge_trains.py
+-rw-r--r--   0 root         (0) root         (0)    12878 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_packages.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_personal_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_pipeline_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_project_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_project_import_export.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_project_merge_request_approvals.py
+-rw-r--r--   0 root         (0) root         (0)      824 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_project_statistics.py
+-rw-r--r--   0 root         (0) root         (0)    21091 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_projects.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_registry_repositories.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_releases.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_remote_mirrors.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_repositories.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_resource_groups.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_resource_iteration_events.py
+-rw-r--r--   0 root         (0) root         (0)     3424 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_resource_label_events.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_resource_milestone_events.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_resource_state_events.py
+-rw-r--r--   0 root         (0) root         (0)     8133 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_runners.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_secure_files.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_services.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_snippets.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_submodules.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_todos.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_topics.py
+-rw-r--r--   0 root         (0) root         (0)     8577 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_users.py
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/objects/test_variables.py
+-rw-r--r--   0 root         (0) root         (0)     7536 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      800 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12171 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     7347 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/test_gitlab_auth.py
+-rw-r--r--   0 root         (0) root         (0)    25196 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/test_gitlab_http_methods.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/test_types.py
+-rw-r--r--   0 root         (0) root         (0)     6441 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tests/unit/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2024-05-28 00:45:38.000000 python_gitlab-4.6.0/tox.ini
```

### Comparing `python_gitlab-4.5.0/AUTHORS` & `python_gitlab-4.6.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/CHANGELOG.md` & `python_gitlab-4.6.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,166 @@
 # CHANGELOG
 
 
 
+## v4.6.0 (2024-05-28)
+
+### Chore
+
+* chore(deps): update python-semantic-release/upload-to-gh-release digest to 673709c ([`1b550ac`](https://github.com/python-gitlab/python-gitlab/commit/1b550ac706c8c31331a7a9dac607aed49f5e1fcf))
+
+* chore(deps): update all non-major dependencies ([`4c7014c`](https://github.com/python-gitlab/python-gitlab/commit/4c7014c13ed63f994e05b498d63b93dc8ab90c2e))
+
+* chore: update commit reference in git-blame-ignore-revs ([`d0fd5ad`](https://github.com/python-gitlab/python-gitlab/commit/d0fd5ad5a70e7eb70aedba5a0d3082418c5ffa34))
+
+* chore(cli): add ability to not add `_id_attr` as an argument
+
+In some cases we don&#39;t want to have `_id_attr` as an argument.
+
+Add ability to have it not be added as an argument. ([`2037352`](https://github.com/python-gitlab/python-gitlab/commit/20373525c1a1f98c18b953dbef896b2570d3d191))
+
+* chore: create a CustomAction dataclass ([`61d8679`](https://github.com/python-gitlab/python-gitlab/commit/61d867925772cf38f20360c9b40140ac3203efb9))
+
+* chore: add an initial .git-blame-ignore-revs
+
+This adds the `.git-blame-ignore-revs` file which allows ignoring
+certain commits when doing a `git blame --ignore-revs`
+
+Ignore the commit that requires keyword arguments for
+`register_custom_action()`
+
+https://docs.github.com/en/repositories/working-with-files/using-files/viewing-a-file#ignore-commits-in-the-blame-view ([`74db84c`](https://github.com/python-gitlab/python-gitlab/commit/74db84ca878ec7029643ff7b00db55f9ea085e9b))
+
+* chore: require keyword arguments for register_custom_action
+
+This makes it more obvious when reading the code what each argument is
+for. ([`7270523`](https://github.com/python-gitlab/python-gitlab/commit/7270523ad89a463c3542e072df73ba2255a49406))
+
+* chore: remove typing-extensions from requirements.txt
+
+We no longer support Python versions before 3.8. So it isn&#39;t needed
+anymore. ([`d569128`](https://github.com/python-gitlab/python-gitlab/commit/d56912835360a1b5a03a20390fb45cb5e8b49ce4))
+
+* chore(deps): update dependency requests to v2.32.0 [security] ([`1bc788c`](https://github.com/python-gitlab/python-gitlab/commit/1bc788ca979a36eeff2e35241bdefc764cf335ce))
+
+* chore(deps): update all non-major dependencies ([`ba1eec4`](https://github.com/python-gitlab/python-gitlab/commit/ba1eec49556ee022de471aae8d15060189f816e3))
+
+* chore(deps): update gitlab/gitlab-ee docker tag to v17 ([`5070d07`](https://github.com/python-gitlab/python-gitlab/commit/5070d07d13b9c87588dbfde3750340e322118779))
+
+* chore(cli): on the CLI help show the API endpoint of resources
+
+This makes it easier for people to map CLI command names to the API.
+
+Looks like this:
+    $ gitlab --help
+    &lt;snip&gt;
+                            The GitLab resource to manipulate.
+        application         API endpoint: /applications
+        application-appearance
+                            API endpoint: /application/appearance
+        application-settings
+                            API endpoint: /application/settings
+        application-statistics
+                            API endpoint: /application/statistics
+    &lt;snip&gt; ([`f1ef565`](https://github.com/python-gitlab/python-gitlab/commit/f1ef5650c3201f3883eb04ad90a874e8adcbcde2))
+
+* chore(cli): add some simple help for the standard operations
+
+Add help for the following standard operations:
+  * list: List the GitLab resources
+  * get: Get a GitLab resource
+  * create: Create a GitLab resource
+  * update: Update a GitLab resource
+  * delete: Delete a GitLab resource
+
+For example:
+  $ gitlab project-key --help
+  usage: gitlab project-key [-h] {list,get,create,update,delete,enable} ...
+
+  options:
+    -h, --help            show this help message and exit
+
+  action:
+    list
+    get
+    create
+    update
+    delete
+    enable
+                          Action to execute on the GitLab resource.
+      list                List the GitLab resources
+      get                 Get a GitLab resource
+      create              Create a GitLab resource
+      update              Update a GitLab resource
+      delete              Delete a GitLab resource ([`5a4a940`](https://github.com/python-gitlab/python-gitlab/commit/5a4a940f42e43ed066838503638fe612813e504f))
+
+* chore: correct type-hint for `job.trace()`
+
+Closes: #2808 ([`840572e`](https://github.com/python-gitlab/python-gitlab/commit/840572e4fa36581405b604a985d0e130fe43f4ce))
+
+* chore: add type info for ProjectFile.content
+
+Closes: #2821 ([`62fa271`](https://github.com/python-gitlab/python-gitlab/commit/62fa2719ea129b3428e5e67d3d3a493f9aead863))
+
+### Feature
+
+* feat(api):  add additional parameter to project/group iteration search (#2796)
+
+Co-authored-by: Cristiano Casella &lt;cristiano.casella@seacom.it&gt;
+Co-authored-by: Nejc Habjan &lt;hab.nejc@gmail.com&gt; ([`623dac9`](https://github.com/python-gitlab/python-gitlab/commit/623dac9c8363c61dbf53f72af58835743e96656b))
+
+* feat(api): add support for gitlab service account (#2851)
+
+
+Co-authored-by: Nejc Habjan &lt;hab.nejc@siemens.com&gt; ([`b187dea`](https://github.com/python-gitlab/python-gitlab/commit/b187deadabbfdf0326ecd79a3ee64c9de10c53e0))
+
+* feat: more usernames support for MR approvals
+
+I don&#39;t think commit a2b8c8ccfb5d went far enough to enable usernames
+support. We create and edit a lot of approval rules based on an external
+service (similar to CODE_OWNERS), but only have the usernames available,
+and currently, have to look up each user to get their user ID to populate
+user_ids for .set_approvers() calls. Would very much like to skip the
+lookup and just send the usernames, which this change should allow.
+
+See: https://docs.gitlab.com/ee/api/merge_request_approvals.html#create-project-level-rule
+
+Signed-off-by: Jarod Wilson &lt;jarod@redhat.com&gt; ([`12d195a`](https://github.com/python-gitlab/python-gitlab/commit/12d195a35a1bd14947fbd6688a8ad1bd3fc21617))
+
+### Fix
+
+* fix(deps): update minimum dependency versions in pyproject.toml
+
+Update the minimum versions of the dependencies in the pyproject.toml
+file.
+
+This is related to PR #2878 ([`37b5a70`](https://github.com/python-gitlab/python-gitlab/commit/37b5a704ef6b94774e54110ba3746a950e733986))
+
+* fix(cli): don&#39;t require `--id` when enabling a deploy key
+
+No longer require `--id` when doing:
+  gitlab project-key enable
+
+Now only the --project-id and --key-id are required. ([`98fc578`](https://github.com/python-gitlab/python-gitlab/commit/98fc5789d39b81197351660b7a3f18903c2b91ba))
+
+* fix: don&#39;t raise `RedirectError` for redirected `HEAD` requests ([`8fc13b9`](https://github.com/python-gitlab/python-gitlab/commit/8fc13b91d63d57c704d03b98920522a6469c96d7))
+
+* fix: handle large number of approval rules
+
+Use `iterator=True` when going through the list of current approval
+rules. This allows it to handle more than the default of 20 approval
+rules.
+
+Closes: #2825 ([`ef8f0e1`](https://github.com/python-gitlab/python-gitlab/commit/ef8f0e190b1add3bbba9a7b194aba2f3c1a83b2e))
+
+* fix(projects): fix &#39;import_project&#39; file argument type for typings
+
+Signed-off-by: Adrian DC &lt;radian.dc@gmail.com&gt; ([`33fbc14`](https://github.com/python-gitlab/python-gitlab/commit/33fbc14ea8432df7e637462379e567f4d0ad6c18))
+
+
 ## v4.5.0 (2024-05-13)
 
 ### Build
 
 * build: Add &#34;--no-cache-dir&#34; to pip commands in Dockerfile
 
 This would not leave cache files in the built docker image.
```

### Comparing `python_gitlab-4.5.0/COPYING` & `python_gitlab-4.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/PKG-INFO` & `python_gitlab-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gitlab
-Version: 4.5.0
+Version: 4.6.0
 Summary: A python wrapper for the GitLab API
 Author-email: Gauvain Pocentek <gauvain@pocentek.net>
 Maintainer-email: John Villalovos <john@sodarock.com>, Max Wittig <max.wittig@siemens.com>, Nejc Habjan <nejc.habjan@siemens.com>, Roger Meier <r.meier@siemens.com>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/python-gitlab/python-gitlab
 Project-URL: Changelog, https://github.com/python-gitlab/python-gitlab/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://python-gitlab.readthedocs.io
@@ -24,16 +24,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: AUTHORS
-Requires-Dist: requests>=2.25.0
-Requires-Dist: requests-toolbelt>=0.10.1
+Requires-Dist: requests>=2.32.0
+Requires-Dist: requests-toolbelt>=1.0.0
 Provides-Extra: autocompletion
 Requires-Dist: argcomplete<3,>=1.10.0; extra == "autocompletion"
 Provides-Extra: yaml
 Requires-Dist: PyYaml>=6.0.1; extra == "yaml"
 
 python-gitlab
 =============
```

### Comparing `python_gitlab-4.5.0/README.rst` & `python_gitlab-4.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/Makefile` & `python_gitlab-4.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/api/gitlab.rst` & `python_gitlab-4.6.0/docs/api/gitlab.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/api-levels.rst` & `python_gitlab-4.6.0/docs/api-levels.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/api-objects.rst` & `python_gitlab-4.6.0/docs/api-objects.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/api-usage-advanced.rst` & `python_gitlab-4.6.0/docs/api-usage-advanced.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/api-usage.rst` & `python_gitlab-4.6.0/docs/api-usage.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/cli-examples.rst` & `python_gitlab-4.6.0/docs/cli-examples.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/cli-objects.rst` & `python_gitlab-4.6.0/docs/cli-objects.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/cli-usage.rst` & `python_gitlab-4.6.0/docs/cli-usage.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/conf.py` & `python_gitlab-4.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/ext/docstrings.py` & `python_gitlab-4.6.0/docs/ext/docstrings.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/ext/manager_tmpl.j2` & `python_gitlab-4.6.0/docs/ext/manager_tmpl.j2`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/faq.rst` & `python_gitlab-4.6.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/access_requests.rst` & `python_gitlab-4.6.0/docs/gl_objects/access_requests.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/applications.rst` & `python_gitlab-4.6.0/docs/gl_objects/applications.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/badges.rst` & `python_gitlab-4.6.0/docs/gl_objects/badges.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/boards.rst` & `python_gitlab-4.6.0/docs/gl_objects/boards.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/branches.rst` & `python_gitlab-4.6.0/docs/gl_objects/branches.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/bulk_imports.rst` & `python_gitlab-4.6.0/docs/gl_objects/bulk_imports.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/ci_lint.rst` & `python_gitlab-4.6.0/docs/gl_objects/ci_lint.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/clusters.rst` & `python_gitlab-4.6.0/docs/gl_objects/clusters.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/commits.rst` & `python_gitlab-4.6.0/docs/gl_objects/commits.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/deploy_keys.rst` & `python_gitlab-4.6.0/docs/gl_objects/deploy_keys.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/deploy_tokens.rst` & `python_gitlab-4.6.0/docs/gl_objects/deploy_tokens.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/deployments.rst` & `python_gitlab-4.6.0/docs/gl_objects/deployments.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/discussions.rst` & `python_gitlab-4.6.0/docs/gl_objects/discussions.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/draft_notes.rst` & `python_gitlab-4.6.0/docs/gl_objects/draft_notes.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/emojis.rst` & `python_gitlab-4.6.0/docs/gl_objects/emojis.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/environments.rst` & `python_gitlab-4.6.0/docs/gl_objects/environments.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/epics.rst` & `python_gitlab-4.6.0/docs/gl_objects/epics.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/events.rst` & `python_gitlab-4.6.0/docs/gl_objects/events.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/features.rst` & `python_gitlab-4.6.0/docs/gl_objects/features.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/geo_nodes.rst` & `python_gitlab-4.6.0/docs/gl_objects/geo_nodes.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/group_access_tokens.rst` & `python_gitlab-4.6.0/docs/gl_objects/group_access_tokens.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/groups.rst` & `python_gitlab-4.6.0/docs/gl_objects/groups.rst`

 * *Files 3% similar despite different names*

```diff
@@ -454,7 +454,28 @@
 
     pr.branch_name_regex = '^(master|develop|support-\d+|release-\d+\..+|hotfix-.+|feature-.+)$'
     pr.save()
 
 Delete group push rules::
 
     pr.delete()
+
+Group Service Account
+=====================
+
+Reference
+---------
+
+* v4 API:
+
+  + :class:`gitlab.v4.objects.GroupServiceAccount`
+  + :class:`gitlab.v4.objects.GroupServiceAccountManager`
+  + :attr:`gitlab.v4.objects.Group.serviceaccounts`
+
+* GitLab API: https://docs.gitlab.com/ee/api/groups.html#service-accounts
+
+Examples
+---------
+
+Create group service account (only allowed at top level group)::
+
+    group.serviceaccount.create({'name': 'group-service-account', 'username': 'group-service-account'})
```

### Comparing `python_gitlab-4.5.0/docs/gl_objects/invitations.rst` & `python_gitlab-4.6.0/docs/gl_objects/invitations.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/issues.rst` & `python_gitlab-4.6.0/docs/gl_objects/issues.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/iterations.rst` & `python_gitlab-4.6.0/docs/gl_objects/iterations.rst`

 * *Files 24% similar despite different names*

```diff
@@ -27,7 +27,17 @@
 List iterations for a project's ancestor groups::
 
     iterations = project.iterations.list()
 
 List iterations for a group::
 
     iterations = group.iterations.list()
+
+Unavailable filters or keyword conflicts::
+    
+    In case you are trying to pass a parameter that collides with a python
+    keyword (i.e. `in`) or with python-gitlab's internal arguments, you'll have
+    to use the `query_parameters` argument:
+
+    ```
+    group.iterations.list(query_parameters={"in": "title"}) 
+    ```
```

### Comparing `python_gitlab-4.5.0/docs/gl_objects/job_token_scope.rst` & `python_gitlab-4.6.0/docs/gl_objects/job_token_scope.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/labels.rst` & `python_gitlab-4.6.0/docs/gl_objects/labels.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/merge_request_approvals.rst` & `python_gitlab-4.6.0/docs/gl_objects/merge_request_approvals.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/merge_requests.rst` & `python_gitlab-4.6.0/docs/gl_objects/merge_requests.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/merge_trains.rst` & `python_gitlab-4.6.0/docs/gl_objects/merge_trains.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/messages.rst` & `python_gitlab-4.6.0/docs/gl_objects/messages.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/milestones.rst` & `python_gitlab-4.6.0/docs/gl_objects/milestones.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/namespaces.rst` & `python_gitlab-4.6.0/docs/gl_objects/namespaces.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/notes.rst` & `python_gitlab-4.6.0/docs/gl_objects/notes.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/notifications.rst` & `python_gitlab-4.6.0/docs/gl_objects/notifications.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/packages.rst` & `python_gitlab-4.6.0/docs/gl_objects/packages.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/pagesdomains.rst` & `python_gitlab-4.6.0/docs/gl_objects/pagesdomains.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/personal_access_tokens.rst` & `python_gitlab-4.6.0/docs/gl_objects/personal_access_tokens.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/pipelines_and_jobs.rst` & `python_gitlab-4.6.0/docs/gl_objects/pipelines_and_jobs.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/project_access_tokens.rst` & `python_gitlab-4.6.0/docs/gl_objects/project_access_tokens.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/projects.rst` & `python_gitlab-4.6.0/docs/gl_objects/projects.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/protected_branches.rst` & `python_gitlab-4.6.0/docs/gl_objects/protected_branches.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/protected_environments.rst` & `python_gitlab-4.6.0/docs/gl_objects/protected_environments.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/releases.rst` & `python_gitlab-4.6.0/docs/gl_objects/releases.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/remote_mirrors.rst` & `python_gitlab-4.6.0/docs/gl_objects/remote_mirrors.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/repositories.rst` & `python_gitlab-4.6.0/docs/gl_objects/repositories.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/repository_tags.rst` & `python_gitlab-4.6.0/docs/gl_objects/repository_tags.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/resource_groups.rst` & `python_gitlab-4.6.0/docs/gl_objects/resource_groups.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/runners.rst` & `python_gitlab-4.6.0/docs/gl_objects/runners.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/search.rst` & `python_gitlab-4.6.0/docs/gl_objects/search.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/secure_files.rst` & `python_gitlab-4.6.0/docs/gl_objects/secure_files.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/snippets.rst` & `python_gitlab-4.6.0/docs/gl_objects/snippets.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/system_hooks.rst` & `python_gitlab-4.6.0/docs/gl_objects/system_hooks.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/templates.rst` & `python_gitlab-4.6.0/docs/gl_objects/templates.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/todos.rst` & `python_gitlab-4.6.0/docs/gl_objects/todos.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/topics.rst` & `python_gitlab-4.6.0/docs/gl_objects/topics.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/users.rst` & `python_gitlab-4.6.0/docs/gl_objects/users.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/variables.rst` & `python_gitlab-4.6.0/docs/gl_objects/variables.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/gl_objects/wikis.rst` & `python_gitlab-4.6.0/docs/gl_objects/wikis.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/make.bat` & `python_gitlab-4.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/docs/release-notes.rst` & `python_gitlab-4.6.0/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/__init__.py` & `python_gitlab-4.6.0/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/_backends/protocol.py` & `python_gitlab-4.6.0/gitlab/_backends/protocol.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/_backends/requests_backend.py` & `python_gitlab-4.6.0/gitlab/_backends/requests_backend.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/base.py` & `python_gitlab-4.6.0/gitlab/base.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/cli.py` & `python_gitlab-4.6.0/gitlab/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import dataclasses
 import functools
 import os
 import pathlib
 import re
 import sys
 import textwrap
 from types import ModuleType
@@ -25,20 +26,29 @@
 from gitlab.base import RESTObject
 
 # This regex is based on:
 # https://github.com/jpvanhal/inflection/blob/master/inflection/__init__.py
 camel_upperlower_regex = re.compile(r"([A-Z]+)([A-Z][a-z])")
 camel_lowerupper_regex = re.compile(r"([a-z\d])([A-Z])")
 
+
+@dataclasses.dataclass
+class CustomAction:
+    required: Tuple[str, ...]
+    optional: Tuple[str, ...]
+    in_object: bool
+    requires_id: bool  # if the `_id_attr` value should be a required argument
+
+
 # custom_actions = {
 #    cls: {
 #        action: (mandatory_args, optional_args, in_obj),
 #    },
 # }
-custom_actions: Dict[str, Dict[str, Tuple[Tuple[str, ...], Tuple[str, ...], bool]]] = {}
+custom_actions: Dict[str, Dict[str, CustomAction]] = {}
 
 
 # For an explanation of how these type-hints work see:
 # https://mypy.readthedocs.io/en/stable/generics.html#declaring-decorators
 #
 # The goal here is that functions which get decorated will retain their types.
 __F = TypeVar("__F", bound=Callable[..., Any])
@@ -68,18 +78,20 @@
                 choices = "\n".join(choice_list)
                 line = f"{textwrap.indent(choices, indent)}\n"
             output += line
         return output
 
 
 def register_custom_action(
+    *,
     cls_names: Union[str, Tuple[str, ...]],
-    mandatory: Tuple[str, ...] = (),
+    required: Tuple[str, ...] = (),
     optional: Tuple[str, ...] = (),
     custom_action: Optional[str] = None,
+    requires_id: bool = True,  # if the `_id_attr` value should be a required argument
 ) -> Callable[[__F], __F]:
     def wrap(f: __F) -> __F:
         @functools.wraps(f)
         def wrapped_f(*args: Any, **kwargs: Any) -> Any:
             return f(*args, **kwargs)
 
         # in_obj defines whether the method belongs to the obj or the manager
@@ -94,15 +106,20 @@
             if cls_name.endswith("Manager"):
                 final_name = cls_name.replace("Manager", "")
                 in_obj = False
             if final_name not in custom_actions:
                 custom_actions[final_name] = {}
 
             action = custom_action or f.__name__.replace("_", "-")
-            custom_actions[final_name][action] = (mandatory, optional, in_obj)
+            custom_actions[final_name][action] = CustomAction(
+                required=required,
+                optional=optional,
+                in_object=in_obj,
+                requires_id=requires_id,
+            )
 
         return cast(__F, wrapped_f)
 
     return wrap
 
 
 def die(msg: str, e: Optional[Exception] = None) -> None:
@@ -130,15 +147,14 @@
     return dasherized_lowercase.lower()
 
 
 def _get_base_parser(add_help: bool = True) -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         add_help=add_help,
         description="GitLab API Command Line Interface",
-        formatter_class=VerticalHelpFormatter,
         allow_abbrev=False,
     )
     parser.add_argument("--version", help="Display the version.", action="store_true")
     parser.add_argument(
         "-v",
         "--verbose",
         "--fancy",
```

### Comparing `python_gitlab-4.5.0/gitlab/client.py` & `python_gitlab-4.6.0/gitlab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,16 +621,16 @@
         # raise an exception with a useful error message.
         if not result.history:
             return
 
         for item in result.history:
             if item.status_code not in (301, 302):
                 continue
-            # GET methods can be redirected without issue
-            if item.request.method == "GET":
+            # GET and HEAD methods can be redirected without issue
+            if item.request.method in ("GET", "HEAD"):
                 continue
             target = item.headers.get("location")
             raise gitlab.exceptions.RedirectError(
                 REDIRECT_MSG.format(
                     status_code=item.status_code,
                     reason=item.reason,
                     source=item.url,
```

### Comparing `python_gitlab-4.5.0/gitlab/config.py` & `python_gitlab-4.6.0/gitlab/config.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/const.py` & `python_gitlab-4.6.0/gitlab/const.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/exceptions.py` & `python_gitlab-4.6.0/gitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/mixins.py` & `python_gitlab-4.6.0/gitlab/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -546,15 +546,15 @@
     _id_attr: Optional[str]
     _attrs: Dict[str, Any]
     _module: ModuleType
     _parent_attrs: Dict[str, Any]
     _updated_attrs: Dict[str, Any]
     manager: base.RESTManager
 
-    @cli.register_custom_action(("Snippet", "ProjectSnippet", "ProjectIssue"))
+    @cli.register_custom_action(cls_names=("Snippet", "ProjectSnippet", "ProjectIssue"))
     @exc.on_http_error(exc.GitlabGetError)
     def user_agent_detail(self, **kwargs: Any) -> Dict[str, Any]:
         """Get the user agent detail.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -574,15 +574,16 @@
     _attrs: Dict[str, Any]
     _module: ModuleType
     _parent_attrs: Dict[str, Any]
     _updated_attrs: Dict[str, Any]
     manager: base.RESTManager
 
     @cli.register_custom_action(
-        ("ProjectAccessRequest", "GroupAccessRequest"), (), ("access_level",)
+        cls_names=("ProjectAccessRequest", "GroupAccessRequest"),
+        optional=("access_level",),
     )
     @exc.on_http_error(exc.GitlabUpdateError)
     def approve(
         self, access_level: int = gitlab.const.DEVELOPER_ACCESS, **kwargs: Any
     ) -> None:
         """Approve an access request.
 
@@ -607,15 +608,15 @@
     _id_attr: Optional[str]
     _attrs: Dict[str, Any]
     _module: ModuleType
     _parent_attrs: Dict[str, Any]
     _updated_attrs: Dict[str, Any]
     manager: base.RESTManager
 
-    @cli.register_custom_action(("GroupExport", "ProjectExport"))
+    @cli.register_custom_action(cls_names=("GroupExport", "ProjectExport"))
     @exc.on_http_error(exc.GitlabGetError)
     def download(
         self,
         streamed: bool = False,
         action: Optional[Callable[[bytes], None]] = None,
         chunk_size: int = 1024,
         *,
@@ -717,15 +718,15 @@
     _attrs: Dict[str, Any]
     _module: ModuleType
     _parent_attrs: Dict[str, Any]
     _updated_attrs: Dict[str, Any]
     manager: base.RESTManager
 
     @cli.register_custom_action(
-        ("ProjectIssue", "ProjectMergeRequest", "ProjectLabel", "GroupLabel")
+        cls_names=("ProjectIssue", "ProjectMergeRequest", "ProjectLabel", "GroupLabel")
     )
     @exc.on_http_error(exc.GitlabSubscribeError)
     def subscribe(self, **kwargs: Any) -> None:
         """Subscribe to the object notifications.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -737,15 +738,15 @@
         path = f"{self.manager.path}/{self.encoded_id}/subscribe"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert not isinstance(server_data, requests.Response)
         self._update_attrs(server_data)
 
     @cli.register_custom_action(
-        ("ProjectIssue", "ProjectMergeRequest", "ProjectLabel", "GroupLabel")
+        cls_names=("ProjectIssue", "ProjectMergeRequest", "ProjectLabel", "GroupLabel")
     )
     @exc.on_http_error(exc.GitlabUnsubscribeError)
     def unsubscribe(self, **kwargs: Any) -> None:
         """Unsubscribe from the object notifications.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -765,15 +766,15 @@
     _id_attr: Optional[str]
     _attrs: Dict[str, Any]
     _module: ModuleType
     _parent_attrs: Dict[str, Any]
     _updated_attrs: Dict[str, Any]
     manager: base.RESTManager
 
-    @cli.register_custom_action(("ProjectIssue", "ProjectMergeRequest"))
+    @cli.register_custom_action(cls_names=("ProjectIssue", "ProjectMergeRequest"))
     @exc.on_http_error(exc.GitlabTodoError)
     def todo(self, **kwargs: Any) -> None:
         """Create a todo associated to the object.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -789,15 +790,15 @@
     _id_attr: Optional[str]
     _attrs: Dict[str, Any]
     _module: ModuleType
     _parent_attrs: Dict[str, Any]
     _updated_attrs: Dict[str, Any]
     manager: base.RESTManager
 
-    @cli.register_custom_action(("ProjectIssue", "ProjectMergeRequest"))
+    @cli.register_custom_action(cls_names=("ProjectIssue", "ProjectMergeRequest"))
     @exc.on_http_error(exc.GitlabTimeTrackingError)
     def time_stats(self, **kwargs: Any) -> Dict[str, Any]:
         """Get time stats for the object.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -815,15 +816,17 @@
 
         path = f"{self.manager.path}/{self.encoded_id}/time_stats"
         result = self.manager.gitlab.http_get(path, **kwargs)
         if TYPE_CHECKING:
             assert not isinstance(result, requests.Response)
         return result
 
-    @cli.register_custom_action(("ProjectIssue", "ProjectMergeRequest"), ("duration",))
+    @cli.register_custom_action(
+        cls_names=("ProjectIssue", "ProjectMergeRequest"), required=("duration",)
+    )
     @exc.on_http_error(exc.GitlabTimeTrackingError)
     def time_estimate(self, duration: str, **kwargs: Any) -> Dict[str, Any]:
         """Set an estimated time of work for the object.
 
         Args:
             duration: Duration in human format (e.g. 3h30)
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -835,15 +838,15 @@
         path = f"{self.manager.path}/{self.encoded_id}/time_estimate"
         data = {"duration": duration}
         result = self.manager.gitlab.http_post(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert not isinstance(result, requests.Response)
         return result
 
-    @cli.register_custom_action(("ProjectIssue", "ProjectMergeRequest"))
+    @cli.register_custom_action(cls_names=("ProjectIssue", "ProjectMergeRequest"))
     @exc.on_http_error(exc.GitlabTimeTrackingError)
     def reset_time_estimate(self, **kwargs: Any) -> Dict[str, Any]:
         """Resets estimated time for the object to 0 seconds.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -853,15 +856,17 @@
         """
         path = f"{self.manager.path}/{self.encoded_id}/reset_time_estimate"
         result = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert not isinstance(result, requests.Response)
         return result
 
-    @cli.register_custom_action(("ProjectIssue", "ProjectMergeRequest"), ("duration",))
+    @cli.register_custom_action(
+        cls_names=("ProjectIssue", "ProjectMergeRequest"), required=("duration",)
+    )
     @exc.on_http_error(exc.GitlabTimeTrackingError)
     def add_spent_time(self, duration: str, **kwargs: Any) -> Dict[str, Any]:
         """Add time spent working on the object.
 
         Args:
             duration: Duration in human format (e.g. 3h30)
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -873,15 +878,15 @@
         path = f"{self.manager.path}/{self.encoded_id}/add_spent_time"
         data = {"duration": duration}
         result = self.manager.gitlab.http_post(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert not isinstance(result, requests.Response)
         return result
 
-    @cli.register_custom_action(("ProjectIssue", "ProjectMergeRequest"))
+    @cli.register_custom_action(cls_names=("ProjectIssue", "ProjectMergeRequest"))
     @exc.on_http_error(exc.GitlabTimeTrackingError)
     def reset_spent_time(self, **kwargs: Any) -> Dict[str, Any]:
         """Resets the time spent working on the object.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -900,15 +905,15 @@
     _id_attr: Optional[str]
     _attrs: Dict[str, Any]
     _module: ModuleType
     _parent_attrs: Dict[str, Any]
     _updated_attrs: Dict[str, Any]
     manager: base.RESTManager
 
-    @cli.register_custom_action(("ProjectMergeRequest", "ProjectIssue"))
+    @cli.register_custom_action(cls_names=("ProjectMergeRequest", "ProjectIssue"))
     @exc.on_http_error(exc.GitlabListError)
     def participants(self, **kwargs: Any) -> Dict[str, Any]:
         """List the participants.
 
         Args:
             all: If True, return all the items, without pagination
             per_page: Number of items to retrieve per request
@@ -928,15 +933,16 @@
         if TYPE_CHECKING:
             assert not isinstance(result, requests.Response)
         return result
 
 
 class BadgeRenderMixin(_RestManagerBase):
     @cli.register_custom_action(
-        ("GroupBadgeManager", "ProjectBadgeManager"), ("link_url", "image_url")
+        cls_names=("GroupBadgeManager", "ProjectBadgeManager"),
+        required=("link_url", "image_url"),
     )
     @exc.on_http_error(exc.GitlabRenderError)
     def render(self, link_url: str, image_url: str, **kwargs: Any) -> Dict[str, Any]:
         """Preview link_url and image_url after interpolation.
 
         Args:
             link_url: URL of the badge link
@@ -1021,15 +1027,17 @@
             The upload path
         """
         if TYPE_CHECKING:
             assert isinstance(self._upload_path, str)
         data = self.attributes
         return self._upload_path.format(**data)
 
-    @cli.register_custom_action(("Project", "ProjectWiki"), ("filename", "filepath"))
+    @cli.register_custom_action(
+        cls_names=("Project", "ProjectWiki"), required=("filename", "filepath")
+    )
     @exc.on_http_error(exc.GitlabUploadError)
     def upload(
         self,
         filename: str,
         filedata: Optional[bytes] = None,
         filepath: Optional[str] = None,
         **kwargs: Any,
```

### Comparing `python_gitlab-4.5.0/gitlab/types.py` & `python_gitlab-4.6.0/gitlab/types.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/utils.py` & `python_gitlab-4.6.0/gitlab/utils.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/cli.py` & `python_gitlab-4.6.0/gitlab/v4/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             return getattr(self, method)()
 
         # Finally try to find custom methods
         return self.do_custom()
 
     def do_custom(self) -> Any:
         class_instance: Union[gitlab.base.RESTManager, gitlab.base.RESTObject]
-        in_obj = cli.custom_actions[self.cls_name][self.resource_action][2]
+        in_obj = cli.custom_actions[self.cls_name][self.resource_action].in_object
 
         # Get the object (lazy), then act
         if in_obj:
             data = {}
             if self.mgr._from_parent_attrs:
                 for k in self.mgr._from_parent_attrs:
                     data[k] = self.parent_args[k]
@@ -203,20 +203,28 @@
     cls: Type[gitlab.base.RESTObject],
     sub_parser: _SubparserType,
 ) -> None:
     mgr_cls_name = f"{cls.__name__}Manager"
     mgr_cls = getattr(gitlab.v4.objects, mgr_cls_name)
 
     action_parsers: Dict[str, argparse.ArgumentParser] = {}
-    for action_name in ["list", "get", "create", "update", "delete"]:
+    for action_name, help_text in [
+        ("list", "List the GitLab resources"),
+        ("get", "Get a GitLab resource"),
+        ("create", "Create a GitLab resource"),
+        ("update", "Update a GitLab resource"),
+        ("delete", "Delete a GitLab resource"),
+    ]:
         if not hasattr(mgr_cls, action_name):
             continue
 
         sub_parser_action = sub_parser.add_parser(
-            action_name, conflict_handler="resolve"
+            action_name,
+            conflict_handler="resolve",
+            help=help_text,
         )
         action_parsers[action_name] = sub_parser_action
         sub_parser_action.add_argument("--sudo", required=False)
         if mgr_cls._from_parent_attrs:
             for x in mgr_cls._from_parent_attrs:
                 sub_parser_action.add_argument(
                     f"--{x.replace('_', '-')}", required=True
@@ -303,27 +311,27 @@
             if mgr_cls._from_parent_attrs:
                 for x in mgr_cls._from_parent_attrs:
                     sub_parser_action.add_argument(
                         f"--{x.replace('_', '-')}", required=True
                     )
                 sub_parser_action.add_argument("--sudo", required=False)
 
+            custom_action = cli.custom_actions[name][action_name]
             # We need to get the object somehow
             if not issubclass(cls, gitlab.mixins.GetWithoutIdMixin):
-                if cls._id_attr is not None:
+                if cls._id_attr is not None and custom_action.requires_id:
                     id_attr = cls._id_attr.replace("_", "-")
                     sub_parser_action.add_argument(f"--{id_attr}", required=True)
 
-            required, optional, dummy = cli.custom_actions[name][action_name]
-            for x in required:
+            for x in custom_action.required:
                 if x != cls._id_attr:
                     sub_parser_action.add_argument(
                         f"--{x.replace('_', '-')}", required=True
                     )
-            for x in optional:
+            for x in custom_action.optional:
                 if x != cls._id_attr:
                     sub_parser_action.add_argument(
                         f"--{x.replace('_', '-')}", required=False
                     )
 
     if mgr_cls.__name__ in cli.custom_actions:
         name = mgr_cls.__name__
@@ -338,21 +346,21 @@
             if mgr_cls._from_parent_attrs:
                 for x in mgr_cls._from_parent_attrs:
                     sub_parser_action.add_argument(
                         f"--{x.replace('_', '-')}", required=True
                     )
                 sub_parser_action.add_argument("--sudo", required=False)
 
-            required, optional, dummy = cli.custom_actions[name][action_name]
-            for x in required:
+            custom_action = cli.custom_actions[name][action_name]
+            for x in custom_action.required:
                 if x != cls._id_attr:
                     sub_parser_action.add_argument(
                         f"--{x.replace('_', '-')}", required=True
                     )
-            for x in optional:
+            for x in custom_action.optional:
                 if x != cls._id_attr:
                     sub_parser_action.add_argument(
                         f"--{x.replace('_', '-')}", required=False
                     )
 
 
 def extend_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
@@ -370,16 +378,20 @@
             continue
         if issubclass(cls, gitlab.base.RESTManager):
             if cls._obj_cls is not None:
                 classes.add(cls._obj_cls)
 
     for cls in sorted(classes, key=operator.attrgetter("__name__")):
         arg_name = cli.cls_to_gitlab_resource(cls)
+        mgr_cls_name = f"{cls.__name__}Manager"
+        mgr_cls = getattr(gitlab.v4.objects, mgr_cls_name)
         object_group = subparsers.add_parser(
-            arg_name, formatter_class=cli.VerticalHelpFormatter
+            arg_name,
+            formatter_class=cli.VerticalHelpFormatter,
+            help=f"API endpoint: {mgr_cls._path}",
         )
 
         object_subparsers = object_group.add_subparsers(
             title="action",
             dest="resource_action",
             help="Action to execute on the GitLab resource.",
         )
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/__init__.py` & `python_gitlab-4.6.0/gitlab/v4/objects/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 from .push_rules import *
 from .releases import *
 from .repositories import *
 from .resource_groups import *
 from .reviewers import *
 from .runners import *
 from .secure_files import *
+from .service_accounts import *
 from .settings import *
 from .sidekiq import *
 from .snippets import *
 from .statistics import *
 from .tags import *
 from .templates import *
 from .todos import *
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/access_requests.py` & `python_gitlab-4.6.0/gitlab/v4/objects/access_requests.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/appearance.py` & `python_gitlab-4.6.0/gitlab/v4/objects/appearance.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/applications.py` & `python_gitlab-4.6.0/gitlab/v4/objects/applications.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/artifacts.py` & `python_gitlab-4.6.0/gitlab/v4/objects/artifacts.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,17 @@
         path = self._compute_path("/projects/{project_id}/artifacts")
 
         if TYPE_CHECKING:
             assert path is not None
         self.gitlab.http_delete(path, **kwargs)
 
     @cli.register_custom_action(
-        "ProjectArtifactManager", ("ref_name", "job"), ("job_token",)
+        cls_names="ProjectArtifactManager",
+        required=("ref_name", "job"),
+        optional=("job_token",),
     )
     @exc.on_http_error(exc.GitlabGetError)
     def download(
         self,
         ref_name: str,
         job: str,
         streamed: bool = False,
@@ -89,15 +91,16 @@
         if TYPE_CHECKING:
             assert isinstance(result, requests.Response)
         return utils.response_content(
             result, streamed, action, chunk_size, iterator=iterator
         )
 
     @cli.register_custom_action(
-        "ProjectArtifactManager", ("ref_name", "artifact_path", "job")
+        cls_names="ProjectArtifactManager",
+        required=("ref_name", "artifact_path", "job"),
     )
     @exc.on_http_error(exc.GitlabGetError)
     def raw(
         self,
         ref_name: str,
         artifact_path: str,
         job: str,
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/audit_events.py` & `python_gitlab-4.6.0/gitlab/v4/objects/audit_events.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/award_emojis.py` & `python_gitlab-4.6.0/gitlab/v4/objects/award_emojis.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/badges.py` & `python_gitlab-4.6.0/gitlab/v4/objects/badges.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/boards.py` & `python_gitlab-4.6.0/gitlab/v4/objects/boards.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/branches.py` & `python_gitlab-4.6.0/gitlab/v4/objects/branches.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/broadcast_messages.py` & `python_gitlab-4.6.0/gitlab/v4/objects/broadcast_messages.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/bulk_imports.py` & `python_gitlab-4.6.0/gitlab/v4/objects/bulk_imports.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/ci_lint.py` & `python_gitlab-4.6.0/gitlab/v4/objects/ci_lint.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     _path = "/ci/lint"
     _obj_cls = CiLint
     _create_attrs = RequiredOptional(
         required=("content",), optional=("include_merged_yaml", "include_jobs")
     )
 
     @register_custom_action(
-        "CiLintManager",
-        ("content",),
+        cls_names="CiLintManager",
+        required=("content",),
         optional=("include_merged_yaml", "include_jobs"),
     )
     def validate(self, *args: Any, **kwargs: Any) -> None:
         """Raise an error if the CI Lint results are not valid.
 
         This is a custom python-gitlab method to wrap lint endpoints."""
         result = self.create(*args, **kwargs)
@@ -59,16 +59,16 @@
         required=("content",), optional=("dry_run", "include_jobs", "ref")
     )
 
     def get(self, **kwargs: Any) -> ProjectCiLint:
         return cast(ProjectCiLint, super().get(**kwargs))
 
     @register_custom_action(
-        "ProjectCiLintManager",
-        ("content",),
+        cls_names="ProjectCiLintManager",
+        required=("content",),
         optional=("dry_run", "include_jobs", "ref"),
     )
     def validate(self, *args: Any, **kwargs: Any) -> None:
         """Raise an error if the Project CI Lint results are not valid.
 
         This is a custom python-gitlab method to wrap lint endpoints."""
         result = self.create(*args, **kwargs)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/clusters.py` & `python_gitlab-4.6.0/gitlab/v4/objects/clusters.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/commits.py` & `python_gitlab-4.6.0/gitlab/v4/objects/commits.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class ProjectCommit(RESTObject):
     _repr_attr = "title"
 
     comments: "ProjectCommitCommentManager"
     discussions: ProjectCommitDiscussionManager
     statuses: "ProjectCommitStatusManager"
 
-    @cli.register_custom_action("ProjectCommit")
+    @cli.register_custom_action(cls_names="ProjectCommit")
     @exc.on_http_error(exc.GitlabGetError)
     def diff(self, **kwargs: Any) -> Union[gitlab.GitlabList, List[Dict[str, Any]]]:
         """Generate the commit diff.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -42,15 +42,15 @@
 
         Returns:
             The changes done in this commit
         """
         path = f"{self.manager.path}/{self.encoded_id}/diff"
         return self.manager.gitlab.http_list(path, **kwargs)
 
-    @cli.register_custom_action("ProjectCommit", ("branch",))
+    @cli.register_custom_action(cls_names="ProjectCommit", required=("branch",))
     @exc.on_http_error(exc.GitlabCherryPickError)
     def cherry_pick(self, branch: str, **kwargs: Any) -> None:
         """Cherry-pick a commit into a branch.
 
         Args:
             branch: Name of target branch
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -59,15 +59,15 @@
             GitlabAuthenticationError: If authentication is not correct
             GitlabCherryPickError: If the cherry-pick could not be performed
         """
         path = f"{self.manager.path}/{self.encoded_id}/cherry_pick"
         post_data = {"branch": branch}
         self.manager.gitlab.http_post(path, post_data=post_data, **kwargs)
 
-    @cli.register_custom_action("ProjectCommit", optional=("type",))
+    @cli.register_custom_action(cls_names="ProjectCommit", optional=("type",))
     @exc.on_http_error(exc.GitlabGetError)
     def refs(
         self, type: str = "all", **kwargs: Any
     ) -> Union[gitlab.GitlabList, List[Dict[str, Any]]]:
         """List the references the commit is pushed to.
 
         Args:
@@ -81,15 +81,15 @@
         Returns:
             The references the commit is pushed to.
         """
         path = f"{self.manager.path}/{self.encoded_id}/refs"
         query_data = {"type": type}
         return self.manager.gitlab.http_list(path, query_data=query_data, **kwargs)
 
-    @cli.register_custom_action("ProjectCommit")
+    @cli.register_custom_action(cls_names="ProjectCommit")
     @exc.on_http_error(exc.GitlabGetError)
     def merge_requests(
         self, **kwargs: Any
     ) -> Union[gitlab.GitlabList, List[Dict[str, Any]]]:
         """List the merge requests related to the commit.
 
         Args:
@@ -101,15 +101,15 @@
 
         Returns:
             The merge requests related to the commit.
         """
         path = f"{self.manager.path}/{self.encoded_id}/merge_requests"
         return self.manager.gitlab.http_list(path, **kwargs)
 
-    @cli.register_custom_action("ProjectCommit", ("branch",))
+    @cli.register_custom_action(cls_names="ProjectCommit", required=("branch",))
     @exc.on_http_error(exc.GitlabRevertError)
     def revert(
         self, branch: str, **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Revert a commit on a given branch.
 
         Args:
@@ -123,15 +123,15 @@
         Returns:
             The new commit data (*not* a RESTObject)
         """
         path = f"{self.manager.path}/{self.encoded_id}/revert"
         post_data = {"branch": branch}
         return self.manager.gitlab.http_post(path, post_data=post_data, **kwargs)
 
-    @cli.register_custom_action("ProjectCommit")
+    @cli.register_custom_action(cls_names="ProjectCommit")
     @exc.on_http_error(exc.GitlabGetError)
     def signature(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Get the signature of the commit.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/container_registry.py` & `python_gitlab-4.6.0/gitlab/v4/objects/container_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 class ProjectRegistryTagManager(DeleteMixin, RetrieveMixin, RESTManager):
     _obj_cls = ProjectRegistryTag
     _from_parent_attrs = {"project_id": "project_id", "repository_id": "id"}
     _path = "/projects/{project_id}/registry/repositories/{repository_id}/tags"
 
     @cli.register_custom_action(
-        "ProjectRegistryTagManager",
-        ("name_regex_delete",),
+        cls_names="ProjectRegistryTagManager",
+        required=("name_regex_delete",),
         optional=("keep_n", "name_regex_keep", "older_than"),
     )
     @exc.on_http_error(exc.GitlabDeleteError)
     def delete_in_bulk(self, name_regex_delete: str, **kwargs: Any) -> None:
         """Delete Tag in bulk
 
         Args:
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/custom_attributes.py` & `python_gitlab-4.6.0/gitlab/v4/objects/custom_attributes.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/deploy_keys.py` & `python_gitlab-4.6.0/gitlab/v4/objects/deploy_keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 class ProjectKeyManager(CRUDMixin, RESTManager):
     _path = "/projects/{project_id}/deploy_keys"
     _obj_cls = ProjectKey
     _from_parent_attrs = {"project_id": "id"}
     _create_attrs = RequiredOptional(required=("title", "key"), optional=("can_push",))
     _update_attrs = RequiredOptional(optional=("title", "can_push"))
 
-    @cli.register_custom_action("ProjectKeyManager", ("key_id",))
+    @cli.register_custom_action(
+        cls_names="ProjectKeyManager", required=("key_id",), requires_id=False
+    )
     @exc.on_http_error(exc.GitlabProjectDeployKeyError)
     def enable(
         self, key_id: int, **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Enable a deploy key for a project.
 
         Args:
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/deploy_tokens.py` & `python_gitlab-4.6.0/gitlab/v4/objects/deploy_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/deployments.py` & `python_gitlab-4.6.0/gitlab/v4/objects/deployments.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 ]
 
 
 class ProjectDeployment(SaveMixin, RESTObject):
     mergerequests: ProjectDeploymentMergeRequestManager
 
     @cli.register_custom_action(
-        "ProjectDeployment",
-        mandatory=("status",),
+        cls_names="ProjectDeployment",
+        required=("status",),
         optional=("comment", "represented_as"),
     )
     @exc.on_http_error(exc.GitlabDeploymentApprovalError)
     def approval(
         self,
         status: str,
         comment: Optional[str] = None,
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/discussions.py` & `python_gitlab-4.6.0/gitlab/v4/objects/discussions.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/draft_notes.py` & `python_gitlab-4.6.0/gitlab/v4/objects/draft_notes.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/environments.py` & `python_gitlab-4.6.0/gitlab/v4/objects/environments.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "ProjectEnvironmentManager",
     "ProjectProtectedEnvironment",
     "ProjectProtectedEnvironmentManager",
 ]
 
 
 class ProjectEnvironment(SaveMixin, ObjectDeleteMixin, RESTObject):
-    @cli.register_custom_action("ProjectEnvironment")
+    @cli.register_custom_action(cls_names="ProjectEnvironment")
     @exc.on_http_error(exc.GitlabStopError)
     def stop(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Stop the environment.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/epics.py` & `python_gitlab-4.6.0/gitlab/v4/objects/epics.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/events.py` & `python_gitlab-4.6.0/gitlab/v4/objects/events.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/export_import.py` & `python_gitlab-4.6.0/gitlab/v4/objects/export_import.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/features.py` & `python_gitlab-4.6.0/gitlab/v4/objects/features.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/files.py` & `python_gitlab-4.6.0/gitlab/v4/objects/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 class ProjectFile(SaveMixin, ObjectDeleteMixin, RESTObject):
     _id_attr = "file_path"
     _repr_attr = "file_path"
     branch: str
     commit_message: str
     file_path: str
     manager: "ProjectFileManager"
+    content: str  # since the `decode()` method uses `self.content`
 
     def decode(self) -> bytes:
         """Returns the decoded content of the file.
 
         Returns:
             The decoded content.
         """
@@ -104,15 +105,17 @@
         optional=("encoding", "author_email", "author_name"),
     )
     _update_attrs = RequiredOptional(
         required=("file_path", "branch", "content", "commit_message"),
         optional=("encoding", "author_email", "author_name"),
     )
 
-    @cli.register_custom_action("ProjectFileManager", ("file_path", "ref"))
+    @cli.register_custom_action(
+        cls_names="ProjectFileManager", required=("file_path", "ref")
+    )
     # NOTE(jlvillal): Signature doesn't match UpdateMixin.update() so ignore
     # type error
     def get(  # type: ignore
         self, file_path: str, ref: str, **kwargs: Any
     ) -> ProjectFile:
         """Retrieve a single file.
 
@@ -127,17 +130,17 @@
 
         Returns:
             The generated RESTObject
         """
         return cast(ProjectFile, GetMixin.get(self, file_path, ref=ref, **kwargs))
 
     @cli.register_custom_action(
-        "ProjectFileManager",
-        ("file_path", "branch", "content", "commit_message"),
-        ("encoding", "author_email", "author_name"),
+        cls_names="ProjectFileManager",
+        required=("file_path", "branch", "content", "commit_message"),
+        optional=("encoding", "author_email", "author_name"),
     )
     @exc.on_http_error(exc.GitlabCreateError)
     def create(
         self, data: Optional[Dict[str, Any]] = None, **kwargs: Any
     ) -> ProjectFile:
         """Create a new object.
 
@@ -194,15 +197,16 @@
         self._update_attrs.validate_attrs(data=data)
         result = self.gitlab.http_put(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(result, dict)
         return result
 
     @cli.register_custom_action(
-        "ProjectFileManager", ("file_path", "branch", "commit_message")
+        cls_names="ProjectFileManager",
+        required=("file_path", "branch", "commit_message"),
     )
     @exc.on_http_error(exc.GitlabDeleteError)
     # NOTE(jlvillal): Signature doesn't match DeleteMixin.delete() so ignore
     # type error
     def delete(  # type: ignore
         self, file_path: str, branch: str, commit_message: str, **kwargs: Any
     ) -> None:
@@ -219,15 +223,17 @@
             GitlabDeleteError: If the server cannot perform the request
         """
         file_path = utils.EncodedId(file_path)
         path = f"{self.path}/{file_path}"
         data = {"branch": branch, "commit_message": commit_message}
         self.gitlab.http_delete(path, query_data=data, **kwargs)
 
-    @cli.register_custom_action("ProjectFileManager", ("file_path", "ref"))
+    @cli.register_custom_action(
+        cls_names="ProjectFileManager", required=("file_path", "ref")
+    )
     @exc.on_http_error(exc.GitlabGetError)
     def raw(
         self,
         file_path: str,
         ref: str,
         streamed: bool = False,
         action: Optional[Callable[..., Any]] = None,
@@ -266,15 +272,17 @@
         )
         if TYPE_CHECKING:
             assert isinstance(result, requests.Response)
         return utils.response_content(
             result, streamed, action, chunk_size, iterator=iterator
         )
 
-    @cli.register_custom_action("ProjectFileManager", ("file_path", "ref"))
+    @cli.register_custom_action(
+        cls_names="ProjectFileManager", required=("file_path", "ref")
+    )
     @exc.on_http_error(exc.GitlabListError)
     def blame(self, file_path: str, ref: str, **kwargs: Any) -> List[Dict[str, Any]]:
         """Return the content of a file for a commit.
 
         Args:
             file_path: Path of the file to retrieve
             ref: Name of the branch, tag or commit
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/geo_nodes.py` & `python_gitlab-4.6.0/gitlab/v4/objects/geo_nodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 __all__ = [
     "GeoNode",
     "GeoNodeManager",
 ]
 
 
 class GeoNode(SaveMixin, ObjectDeleteMixin, RESTObject):
-    @cli.register_custom_action("GeoNode")
+    @cli.register_custom_action(cls_names="GeoNode")
     @exc.on_http_error(exc.GitlabRepairError)
     def repair(self, **kwargs: Any) -> None:
         """Repair the OAuth authentication of the geo node.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -33,15 +33,15 @@
         """
         path = f"/geo_nodes/{self.encoded_id}/repair"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("GeoNode")
+    @cli.register_custom_action(cls_names="GeoNode")
     @exc.on_http_error(exc.GitlabGetError)
     def status(self, **kwargs: Any) -> Dict[str, Any]:
         """Get the status of the geo node.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -65,15 +65,15 @@
     _update_attrs = RequiredOptional(
         optional=("enabled", "url", "files_max_capacity", "repos_max_capacity"),
     )
 
     def get(self, id: Union[str, int], lazy: bool = False, **kwargs: Any) -> GeoNode:
         return cast(GeoNode, super().get(id=id, lazy=lazy, **kwargs))
 
-    @cli.register_custom_action("GeoNodeManager")
+    @cli.register_custom_action(cls_names="GeoNodeManager")
     @exc.on_http_error(exc.GitlabGetError)
     def status(self, **kwargs: Any) -> List[Dict[str, Any]]:
         """Get the status of all the geo nodes.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -85,15 +85,15 @@
             The status of all the geo nodes
         """
         result = self.gitlab.http_list("/geo_nodes/status", **kwargs)
         if TYPE_CHECKING:
             assert isinstance(result, list)
         return result
 
-    @cli.register_custom_action("GeoNodeManager")
+    @cli.register_custom_action(cls_names="GeoNodeManager")
     @exc.on_http_error(exc.GitlabGetError)
     def current_failures(self, **kwargs: Any) -> List[Dict[str, Any]]:
         """Get the list of failures on the current geo node.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/group_access_tokens.py` & `python_gitlab-4.6.0/gitlab/v4/objects/group_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/groups.py` & `python_gitlab-4.6.0/gitlab/v4/objects/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from .merge_requests import GroupMergeRequestManager  # noqa: F401
 from .milestones import GroupMilestoneManager  # noqa: F401
 from .notification_settings import GroupNotificationSettingsManager  # noqa: F401
 from .packages import GroupPackageManager  # noqa: F401
 from .projects import GroupProjectManager, SharedProjectManager  # noqa: F401
 from .push_rules import GroupPushRulesManager
 from .runners import GroupRunnerManager  # noqa: F401
+from .service_accounts import GroupServiceAccountManager  # noqa: F401
 from .statistics import GroupIssuesStatisticsManager  # noqa: F401
 from .variables import GroupVariableManager  # noqa: F401
 from .wikis import GroupWikiManager  # noqa: F401
 
 __all__ = [
     "Group",
     "GroupManager",
@@ -98,16 +99,17 @@
     pushrules: GroupPushRulesManager
     registry_repositories: GroupRegistryRepositoryManager
     runners: GroupRunnerManager
     subgroups: "GroupSubgroupManager"
     variables: GroupVariableManager
     wikis: GroupWikiManager
     saml_group_links: "GroupSAMLGroupLinkManager"
+    service_accounts: "GroupServiceAccountManager"
 
-    @cli.register_custom_action("Group", ("project_id",))
+    @cli.register_custom_action(cls_names="Group", required=("project_id",))
     @exc.on_http_error(exc.GitlabTransferProjectError)
     def transfer_project(self, project_id: int, **kwargs: Any) -> None:
         """Transfer a project to this group.
 
         Args:
             to_project_id: ID of the project to transfer
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -115,15 +117,15 @@
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabTransferProjectError: If the project could not be transferred
         """
         path = f"/groups/{self.encoded_id}/projects/{project_id}"
         self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("Group", (), ("group_id",))
+    @cli.register_custom_action(cls_names="Group", required=(), optional=("group_id",))
     @exc.on_http_error(exc.GitlabGroupTransferError)
     def transfer(self, group_id: Optional[int] = None, **kwargs: Any) -> None:
         """Transfer the group to a new parent group or make it a top-level group.
 
         Requires GitLab ≥14.6.
 
         Args:
@@ -137,15 +139,15 @@
         """
         path = f"/groups/{self.encoded_id}/transfer"
         post_data = {}
         if group_id is not None:
             post_data["group_id"] = group_id
         self.manager.gitlab.http_post(path, post_data=post_data, **kwargs)
 
-    @cli.register_custom_action("Group", ("scope", "search"))
+    @cli.register_custom_action(cls_names="Group", required=("scope", "search"))
     @exc.on_http_error(exc.GitlabSearchError)
     def search(
         self, scope: str, search: str, **kwargs: Any
     ) -> Union[gitlab.GitlabList, List[Dict[str, Any]]]:
         """Search the group resources matching the provided string.
 
         Args:
@@ -160,30 +162,34 @@
         Returns:
             A list of dicts describing the resources found.
         """
         data = {"scope": scope, "search": search}
         path = f"/groups/{self.encoded_id}/search"
         return self.manager.gitlab.http_list(path, query_data=data, **kwargs)
 
-    @cli.register_custom_action("Group")
+    @cli.register_custom_action(cls_names="Group")
     @exc.on_http_error(exc.GitlabCreateError)
     def ldap_sync(self, **kwargs: Any) -> None:
         """Sync LDAP groups.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabCreateError: If the server cannot perform the request
         """
         path = f"/groups/{self.encoded_id}/ldap_sync"
         self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("Group", ("group_id", "group_access"), ("expires_at",))
+    @cli.register_custom_action(
+        cls_names="Group",
+        required=("group_id", "group_access"),
+        optional=("expires_at",),
+    )
     @exc.on_http_error(exc.GitlabCreateError)
     def share(
         self,
         group_id: int,
         group_access: int,
         expires_at: Optional[str] = None,
         **kwargs: Any,
@@ -209,15 +215,15 @@
             "expires_at": expires_at,
         }
         server_data = self.manager.gitlab.http_post(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("Group", ("group_id",))
+    @cli.register_custom_action(cls_names="Group", required=("group_id",))
     @exc.on_http_error(exc.GitlabDeleteError)
     def unshare(self, group_id: int, **kwargs: Any) -> None:
         """Delete a shared group link within a group.
 
         Args:
             group_id: ID of the group.
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -225,15 +231,15 @@
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabDeleteError: If the server failed to perform the request
         """
         path = f"/groups/{self.encoded_id}/share/{group_id}"
         self.manager.gitlab.http_delete(path, **kwargs)
 
-    @cli.register_custom_action("Group")
+    @cli.register_custom_action(cls_names="Group")
     @exc.on_http_error(exc.GitlabRestoreError)
     def restore(self, **kwargs: Any) -> None:
         """Restore a  group marked for deletion..
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/hooks.py` & `python_gitlab-4.6.0/gitlab/v4/objects/hooks.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/integrations.py` & `python_gitlab-4.6.0/gitlab/v4/objects/integrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,17 @@
     }
 
     def get(
         self, id: Union[str, int], lazy: bool = False, **kwargs: Any
     ) -> ProjectIntegration:
         return cast(ProjectIntegration, super().get(id=id, lazy=lazy, **kwargs))
 
-    @cli.register_custom_action(("ProjectIntegrationManager", "ProjectServiceManager"))
+    @cli.register_custom_action(
+        cls_names=("ProjectIntegrationManager", "ProjectServiceManager")
+    )
     def available(self) -> List[str]:
         """List the services known by python-gitlab.
 
         Returns:
             The list of service code names.
         """
         return list(self._service_attrs.keys())
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/invitations.py` & `python_gitlab-4.6.0/gitlab/v4/objects/invitations.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/issues.py` & `python_gitlab-4.6.0/gitlab/v4/objects/issues.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     notes: ProjectIssueNoteManager
     resourcelabelevents: ProjectIssueResourceLabelEventManager
     resourcemilestoneevents: ProjectIssueResourceMilestoneEventManager
     resourcestateevents: ProjectIssueResourceStateEventManager
     resource_iteration_events: ProjectIssueResourceIterationEventManager
     resource_weight_events: ProjectIssueResourceWeightEventManager
 
-    @cli.register_custom_action("ProjectIssue", ("to_project_id",))
+    @cli.register_custom_action(cls_names="ProjectIssue", required=("to_project_id",))
     @exc.on_http_error(exc.GitlabUpdateError)
     def move(self, to_project_id: int, **kwargs: Any) -> None:
         """Move the issue to another project.
 
         Args:
             to_project_id: ID of the target project
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -142,15 +142,17 @@
         path = f"{self.manager.path}/{self.encoded_id}/move"
         data = {"to_project_id": to_project_id}
         server_data = self.manager.gitlab.http_post(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("ProjectIssue", ("move_after_id", "move_before_id"))
+    @cli.register_custom_action(
+        cls_names="ProjectIssue", required=("move_after_id", "move_before_id")
+    )
     @exc.on_http_error(exc.GitlabUpdateError)
     def reorder(
         self,
         move_after_id: Optional[int] = None,
         move_before_id: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
@@ -174,15 +176,15 @@
             data["move_before_id"] = move_before_id
 
         server_data = self.manager.gitlab.http_put(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("ProjectIssue")
+    @cli.register_custom_action(cls_names="ProjectIssue")
     @exc.on_http_error(exc.GitlabGetError)
     def related_merge_requests(self, **kwargs: Any) -> Dict[str, Any]:
         """List merge requests related to the issue.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -195,15 +197,15 @@
         """
         path = f"{self.manager.path}/{self.encoded_id}/related_merge_requests"
         result = self.manager.gitlab.http_get(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(result, dict)
         return result
 
-    @cli.register_custom_action("ProjectIssue")
+    @cli.register_custom_action(cls_names="ProjectIssue")
     @exc.on_http_error(exc.GitlabGetError)
     def closed_by(self, **kwargs: Any) -> Dict[str, Any]:
         """List merge requests that will close the issue when merged.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/job_token_scope.py` & `python_gitlab-4.6.0/gitlab/v4/objects/job_token_scope.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/jobs.py` & `python_gitlab-4.6.0/gitlab/v4/objects/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = [
     "ProjectJob",
     "ProjectJobManager",
 ]
 
 
 class ProjectJob(RefreshMixin, RESTObject):
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabJobCancelError)
     def cancel(self, **kwargs: Any) -> Dict[str, Any]:
         """Cancel the job.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -30,15 +30,15 @@
         """
         path = f"{self.manager.path}/{self.encoded_id}/cancel"
         result = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(result, dict)
         return result
 
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabJobRetryError)
     def retry(self, **kwargs: Any) -> Dict[str, Any]:
         """Retry the job.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -48,15 +48,15 @@
         """
         path = f"{self.manager.path}/{self.encoded_id}/retry"
         result = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(result, dict)
         return result
 
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabJobPlayError)
     def play(self, **kwargs: Any) -> None:
         """Trigger a job explicitly.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -66,60 +66,60 @@
         """
         path = f"{self.manager.path}/{self.encoded_id}/play"
         result = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(result, dict)
         self._update_attrs(result)
 
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabJobEraseError)
     def erase(self, **kwargs: Any) -> None:
         """Erase the job (remove job artifacts and trace).
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabJobEraseError: If the job could not be erased
         """
         path = f"{self.manager.path}/{self.encoded_id}/erase"
         self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabCreateError)
     def keep_artifacts(self, **kwargs: Any) -> None:
         """Prevent artifacts from being deleted when expiration is set.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabCreateError: If the request could not be performed
         """
         path = f"{self.manager.path}/{self.encoded_id}/artifacts/keep"
         self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabCreateError)
     def delete_artifacts(self, **kwargs: Any) -> None:
         """Delete artifacts of a job.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabDeleteError: If the request could not be performed
         """
         path = f"{self.manager.path}/{self.encoded_id}/artifacts"
         self.manager.gitlab.http_delete(path, **kwargs)
 
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabGetError)
     def artifacts(
         self,
         streamed: bool = False,
         action: Optional[Callable[..., Any]] = None,
         chunk_size: int = 1024,
         *,
@@ -152,15 +152,15 @@
         )
         if TYPE_CHECKING:
             assert isinstance(result, requests.Response)
         return utils.response_content(
             result, streamed, action, chunk_size, iterator=iterator
         )
 
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabGetError)
     def artifact(
         self,
         path: str,
         streamed: bool = False,
         action: Optional[Callable[..., Any]] = None,
         chunk_size: int = 1024,
@@ -195,25 +195,25 @@
         )
         if TYPE_CHECKING:
             assert isinstance(result, requests.Response)
         return utils.response_content(
             result, streamed, action, chunk_size, iterator=iterator
         )
 
-    @cli.register_custom_action("ProjectJob")
+    @cli.register_custom_action(cls_names="ProjectJob")
     @exc.on_http_error(exc.GitlabGetError)
     def trace(
         self,
         streamed: bool = False,
         action: Optional[Callable[..., Any]] = None,
         chunk_size: int = 1024,
         *,
         iterator: bool = False,
         **kwargs: Any,
-    ) -> Dict[str, Any]:
+    ) -> Optional[Union[bytes, Iterator[Any]]]:
         """Get the job trace.
 
         Args:
             streamed: If True the data will be processed by chunks of
                 `chunk_size` and each chunk is passed to `action` for
                 treatment
             iterator: If True directly return the underlying response
@@ -232,20 +232,17 @@
         """
         path = f"{self.manager.path}/{self.encoded_id}/trace"
         result = self.manager.gitlab.http_get(
             path, streamed=streamed, raw=True, **kwargs
         )
         if TYPE_CHECKING:
             assert isinstance(result, requests.Response)
-        return_value = utils.response_content(
+        return utils.response_content(
             result, streamed, action, chunk_size, iterator=iterator
         )
-        if TYPE_CHECKING:
-            assert isinstance(return_value, dict)
-        return return_value
 
 
 class ProjectJobManager(RetrieveMixin, RESTManager):
     _path = "/projects/{project_id}/jobs"
     _obj_cls = ProjectJob
     _from_parent_attrs = {"project_id": "id"}
     _list_filters = ("scope",)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/keys.py` & `python_gitlab-4.6.0/gitlab/v4/objects/keys.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/labels.py` & `python_gitlab-4.6.0/gitlab/v4/objects/labels.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/ldap.py` & `python_gitlab-4.6.0/gitlab/v4/objects/ldap.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/members.py` & `python_gitlab-4.6.0/gitlab/v4/objects/members.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/merge_request_approvals.py` & `python_gitlab-4.6.0/gitlab/v4/objects/merge_request_approvals.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,16 @@
     @exc.on_http_error(exc.GitlabUpdateError)
     def set_approvers(
         self,
         approvals_required: int,
         approver_ids: Optional[List[int]] = None,
         approver_group_ids: Optional[List[int]] = None,
         approval_rule_name: str = "name",
+        *,
+        approver_usernames: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> RESTObject:
         """Change MR-level allowed approvers and approver groups.
 
         Args:
             approvals_required: The number of required approvals for this rule
             approver_ids: User IDs that can approve MRs
@@ -100,34 +102,37 @@
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabUpdateError: If the server failed to perform the request
         """
         approver_ids = approver_ids or []
         approver_group_ids = approver_group_ids or []
+        approver_usernames = approver_usernames or []
 
         data = {
             "name": approval_rule_name,
             "approvals_required": approvals_required,
             "rule_type": "regular",
             "user_ids": approver_ids,
             "group_ids": approver_group_ids,
+            "usernames": approver_usernames,
         }
         if TYPE_CHECKING:
             assert self._parent is not None
         approval_rules: ProjectMergeRequestApprovalRuleManager = (
             self._parent.approval_rules
         )
         # update any existing approval rule matching the name
-        existing_approval_rules = approval_rules.list()
+        existing_approval_rules = approval_rules.list(iterator=True)
         for ar in existing_approval_rules:
             if ar.name == approval_rule_name:
                 ar.user_ids = data["user_ids"]
                 ar.approvals_required = data["approvals_required"]
                 ar.group_ids = data["group_ids"]
+                ar.usernames = data["usernames"]
                 ar.save()
                 return ar
         # if there was no rule matching the rule name, create a new one
         return approval_rules.create(data=data, **kwargs)
 
 
 class ProjectMergeRequestApprovalRule(SaveMixin, ObjectDeleteMixin, RESTObject):
@@ -141,22 +146,22 @@
     _update_attrs = RequiredOptional(
         required=(
             "id",
             "merge_request_iid",
             "name",
             "approvals_required",
         ),
-        optional=("user_ids", "group_ids"),
+        optional=("user_ids", "group_ids", "usernames"),
     )
     # Important: When approval_project_rule_id is set, the name, users and
     # groups of project-level rule will be copied. The approvals_required
     # specified will be used.
     _create_attrs = RequiredOptional(
         required=("name", "approvals_required"),
-        optional=("approval_project_rule_id", "user_ids", "group_ids"),
+        optional=("approval_project_rule_id", "user_ids", "group_ids", "usernames"),
     )
 
     def get(
         self, id: Union[str, int], lazy: bool = False, **kwargs: Any
     ) -> ProjectMergeRequestApprovalRule:
         return cast(
             ProjectMergeRequestApprovalRule, super().get(id=id, lazy=lazy, **kwargs)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/merge_requests.py` & `python_gitlab-4.6.0/gitlab/v4/objects/merge_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     notes: ProjectMergeRequestNoteManager
     pipelines: ProjectMergeRequestPipelineManager
     resourcelabelevents: ProjectMergeRequestResourceLabelEventManager
     resourcemilestoneevents: ProjectMergeRequestResourceMilestoneEventManager
     resourcestateevents: ProjectMergeRequestResourceStateEventManager
     reviewer_details: ProjectMergeRequestReviewerDetailManager
 
-    @cli.register_custom_action("ProjectMergeRequest")
+    @cli.register_custom_action(cls_names="ProjectMergeRequest")
     @exc.on_http_error(exc.GitlabMROnBuildSuccessError)
     def cancel_merge_when_pipeline_succeeds(self, **kwargs: Any) -> Dict[str, str]:
         """Cancel merge when the pipeline succeeds.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -193,15 +193,15 @@
         # https://docs.gitlab.com/ee/api/merge_requests.html#cancel-merge-when-pipeline-succeeds
         # are incorrect in that the return value is actually just:
         #   {'status': 'success'}  for a successful cancel.
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         return server_data
 
-    @cli.register_custom_action("ProjectMergeRequest")
+    @cli.register_custom_action(cls_names="ProjectMergeRequest")
     @exc.on_http_error(exc.GitlabListError)
     def closes_issues(self, **kwargs: Any) -> RESTObjectList:
         """List issues that will close on merge."
 
         Args:
             all: If True, return all the items, without pagination
             per_page: Number of items to retrieve per request
@@ -218,15 +218,15 @@
         path = f"{self.manager.path}/{self.encoded_id}/closes_issues"
         data_list = self.manager.gitlab.http_list(path, iterator=True, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(data_list, gitlab.GitlabList)
         manager = ProjectIssueManager(self.manager.gitlab, parent=self.manager._parent)
         return RESTObjectList(manager, ProjectIssue, data_list)
 
-    @cli.register_custom_action("ProjectMergeRequest")
+    @cli.register_custom_action(cls_names="ProjectMergeRequest")
     @exc.on_http_error(exc.GitlabListError)
     def commits(self, **kwargs: Any) -> RESTObjectList:
         """List the merge request commits.
 
         Args:
             all: If True, return all the items, without pagination
             per_page: Number of items to retrieve per request
@@ -244,15 +244,17 @@
         path = f"{self.manager.path}/{self.encoded_id}/commits"
         data_list = self.manager.gitlab.http_list(path, iterator=True, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(data_list, gitlab.GitlabList)
         manager = ProjectCommitManager(self.manager.gitlab, parent=self.manager._parent)
         return RESTObjectList(manager, ProjectCommit, data_list)
 
-    @cli.register_custom_action("ProjectMergeRequest", optional=("access_raw_diffs",))
+    @cli.register_custom_action(
+        cls_names="ProjectMergeRequest", optional=("access_raw_diffs",)
+    )
     @exc.on_http_error(exc.GitlabListError)
     def changes(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """List the merge request changes.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -262,15 +264,15 @@
 
         Returns:
             List of changes
         """
         path = f"{self.manager.path}/{self.encoded_id}/changes"
         return self.manager.gitlab.http_get(path, **kwargs)
 
-    @cli.register_custom_action("ProjectMergeRequest", (), ("sha",))
+    @cli.register_custom_action(cls_names="ProjectMergeRequest", optional=("sha",))
     @exc.on_http_error(exc.GitlabMRApprovalError)
     def approve(self, sha: Optional[str] = None, **kwargs: Any) -> Dict[str, Any]:
         """Approve the merge request.
 
         Args:
             sha: Head SHA of MR
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -291,15 +293,15 @@
 
         server_data = self.manager.gitlab.http_post(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
         return server_data
 
-    @cli.register_custom_action("ProjectMergeRequest")
+    @cli.register_custom_action(cls_names="ProjectMergeRequest")
     @exc.on_http_error(exc.GitlabMRApprovalError)
     def unapprove(self, **kwargs: Any) -> None:
         """Unapprove the merge request.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -313,15 +315,15 @@
         data: Dict[str, Any] = {}
 
         server_data = self.manager.gitlab.http_post(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("ProjectMergeRequest")
+    @cli.register_custom_action(cls_names="ProjectMergeRequest")
     @exc.on_http_error(exc.GitlabMRRebaseError)
     def rebase(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Attempt to rebase the source branch onto the target branch
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -329,15 +331,15 @@
             GitlabAuthenticationError: If authentication is not correct
             GitlabMRRebaseError: If rebasing failed
         """
         path = f"{self.manager.path}/{self.encoded_id}/rebase"
         data: Dict[str, Any] = {}
         return self.manager.gitlab.http_put(path, post_data=data, **kwargs)
 
-    @cli.register_custom_action("ProjectMergeRequest")
+    @cli.register_custom_action(cls_names="ProjectMergeRequest")
     @exc.on_http_error(exc.GitlabMRResetApprovalError)
     def reset_approvals(
         self, **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Clear all approvals of the merge request.
 
         Args:
@@ -347,15 +349,15 @@
             GitlabAuthenticationError: If authentication is not correct
             GitlabMRResetApprovalError: If reset approval failed
         """
         path = f"{self.manager.path}/{self.encoded_id}/reset_approvals"
         data: Dict[str, Any] = {}
         return self.manager.gitlab.http_put(path, post_data=data, **kwargs)
 
-    @cli.register_custom_action("ProjectMergeRequest")
+    @cli.register_custom_action(cls_names="ProjectMergeRequest")
     @exc.on_http_error(exc.GitlabGetError)
     def merge_ref(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Attempt to merge changes between source and target branches into
             `refs/merge-requests/:iid/merge`.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -363,17 +365,16 @@
         Raises:
             GitlabGetError: If cannot be merged
         """
         path = f"{self.manager.path}/{self.encoded_id}/merge_ref"
         return self.manager.gitlab.http_get(path, **kwargs)
 
     @cli.register_custom_action(
-        "ProjectMergeRequest",
-        (),
-        (
+        cls_names="ProjectMergeRequest",
+        optional=(
             "merge_commit_message",
             "should_remove_source_branch",
             "merge_when_pipeline_succeeds",
         ),
     )
     @exc.on_http_error(exc.GitlabMRClosedError)
     def merge(
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/milestones.py` & `python_gitlab-4.6.0/gitlab/v4/objects/milestones.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "ProjectMilestoneManager",
 ]
 
 
 class GroupMilestone(SaveMixin, ObjectDeleteMixin, RESTObject):
     _repr_attr = "title"
 
-    @cli.register_custom_action("GroupMilestone")
+    @cli.register_custom_action(cls_names="GroupMilestone")
     @exc.on_http_error(exc.GitlabListError)
     def issues(self, **kwargs: Any) -> RESTObjectList:
         """List issues related to this milestone.
 
         Args:
             all: If True, return all the items, without pagination
             per_page: Number of items to retrieve per request
@@ -54,15 +54,15 @@
         data_list = self.manager.gitlab.http_list(path, iterator=True, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(data_list, RESTObjectList)
         manager = GroupIssueManager(self.manager.gitlab, parent=self.manager._parent)
         # FIXME(gpocentek): the computed manager path is not correct
         return RESTObjectList(manager, GroupIssue, data_list)
 
-    @cli.register_custom_action("GroupMilestone")
+    @cli.register_custom_action(cls_names="GroupMilestone")
     @exc.on_http_error(exc.GitlabListError)
     def merge_requests(self, **kwargs: Any) -> RESTObjectList:
         """List the merge requests related to this milestone.
 
         Args:
             all: If True, return all the items, without pagination
             per_page: Number of items to retrieve per request
@@ -104,15 +104,15 @@
         return cast(GroupMilestone, super().get(id=id, lazy=lazy, **kwargs))
 
 
 class ProjectMilestone(PromoteMixin, SaveMixin, ObjectDeleteMixin, RESTObject):
     _repr_attr = "title"
     _update_method = UpdateMethod.POST
 
-    @cli.register_custom_action("ProjectMilestone")
+    @cli.register_custom_action(cls_names="ProjectMilestone")
     @exc.on_http_error(exc.GitlabListError)
     def issues(self, **kwargs: Any) -> RESTObjectList:
         """List issues related to this milestone.
 
         Args:
             all: If True, return all the items, without pagination
             per_page: Number of items to retrieve per request
@@ -131,15 +131,15 @@
         data_list = self.manager.gitlab.http_list(path, iterator=True, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(data_list, RESTObjectList)
         manager = ProjectIssueManager(self.manager.gitlab, parent=self.manager._parent)
         # FIXME(gpocentek): the computed manager path is not correct
         return RESTObjectList(manager, ProjectIssue, data_list)
 
-    @cli.register_custom_action("ProjectMilestone")
+    @cli.register_custom_action(cls_names="ProjectMilestone")
     @exc.on_http_error(exc.GitlabListError)
     def merge_requests(self, **kwargs: Any) -> RESTObjectList:
         """List the merge requests related to this milestone.
 
         Args:
             all: If True, return all the items, without pagination
             per_page: Number of items to retrieve per request
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/namespaces.py` & `python_gitlab-4.6.0/gitlab/v4/objects/namespaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,17 @@
     _path = "/namespaces"
     _obj_cls = Namespace
     _list_filters = ("search",)
 
     def get(self, id: Union[str, int], lazy: bool = False, **kwargs: Any) -> Namespace:
         return cast(Namespace, super().get(id=id, lazy=lazy, **kwargs))
 
-    @cli.register_custom_action("NamespaceManager", ("namespace", "parent_id"))
+    @cli.register_custom_action(
+        cls_names="NamespaceManager", required=("namespace", "parent_id")
+    )
     @exc.on_http_error(exc.GitlabGetError)
     def exists(self, namespace: str, **kwargs: Any) -> Namespace:
         """Get existence of a namespace by path.
 
         Args:
             namespace: The path to the namespace.
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/notes.py` & `python_gitlab-4.6.0/gitlab/v4/objects/notes.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/notification_settings.py` & `python_gitlab-4.6.0/gitlab/v4/objects/notification_settings.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/packages.py` & `python_gitlab-4.6.0/gitlab/v4/objects/packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
 class GenericPackageManager(RESTManager):
     _path = "/projects/{project_id}/packages/generic"
     _obj_cls = GenericPackage
     _from_parent_attrs = {"project_id": "id"}
 
     @cli.register_custom_action(
-        "GenericPackageManager",
-        ("package_name", "package_version", "file_name", "path"),
+        cls_names="GenericPackageManager",
+        required=("package_name", "package_version", "file_name", "path"),
     )
     @exc.on_http_error(exc.GitlabUploadError)
     def upload(
         self,
         package_name: str,
         package_version: str,
         file_name: str,
@@ -119,16 +119,16 @@
             "file_name": file_name,
             "path": path,
         }
         attrs.update(server_data)
         return self._obj_cls(self, attrs=attrs)
 
     @cli.register_custom_action(
-        "GenericPackageManager",
-        ("package_name", "package_version", "file_name"),
+        cls_names="GenericPackageManager",
+        required=("package_name", "package_version", "file_name"),
     )
     @exc.on_http_error(exc.GitlabGetError)
     def download(
         self,
         package_name: str,
         package_version: str,
         file_name: str,
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/pages.py` & `python_gitlab-4.6.0/gitlab/v4/objects/pages.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/personal_access_tokens.py` & `python_gitlab-4.6.0/gitlab/v4/objects/personal_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/pipelines.py` & `python_gitlab-4.6.0/gitlab/v4/objects/pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,30 +56,30 @@
 class ProjectPipeline(RefreshMixin, ObjectDeleteMixin, RESTObject):
     bridges: "ProjectPipelineBridgeManager"
     jobs: "ProjectPipelineJobManager"
     test_report: "ProjectPipelineTestReportManager"
     test_report_summary: "ProjectPipelineTestReportSummaryManager"
     variables: "ProjectPipelineVariableManager"
 
-    @cli.register_custom_action("ProjectPipeline")
+    @cli.register_custom_action(cls_names="ProjectPipeline")
     @exc.on_http_error(exc.GitlabPipelineCancelError)
     def cancel(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Cancel the job.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabPipelineCancelError: If the request failed
         """
         path = f"{self.manager.path}/{self.encoded_id}/cancel"
         return self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("ProjectPipeline")
+    @cli.register_custom_action(cls_names="ProjectPipeline")
     @exc.on_http_error(exc.GitlabPipelineRetryError)
     def retry(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Retry the job.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -197,15 +197,15 @@
     _from_parent_attrs = {"project_id": "project_id", "pipeline_schedule_id": "id"}
 
 
 class ProjectPipelineSchedule(SaveMixin, ObjectDeleteMixin, RESTObject):
     variables: ProjectPipelineScheduleVariableManager
     pipelines: ProjectPipelineSchedulePipelineManager
 
-    @cli.register_custom_action("ProjectPipelineSchedule")
+    @cli.register_custom_action(cls_names="ProjectPipelineSchedule")
     @exc.on_http_error(exc.GitlabOwnershipError)
     def take_ownership(self, **kwargs: Any) -> None:
         """Update the owner of a pipeline schedule.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -215,15 +215,15 @@
         """
         path = f"{self.manager.path}/{self.encoded_id}/take_ownership"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("ProjectPipelineSchedule")
+    @cli.register_custom_action(cls_names="ProjectPipelineSchedule")
     @exc.on_http_error(exc.GitlabPipelinePlayError)
     def play(self, **kwargs: Any) -> Dict[str, Any]:
         """Trigger a new scheduled pipeline, which runs immediately.
         The next scheduled run of this pipeline is not affected.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/project_access_tokens.py` & `python_gitlab-4.6.0/gitlab/v4/objects/project_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/projects.py` & `python_gitlab-4.6.0/gitlab/v4/objects/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/projects.html
 """
 
+import io
 from typing import (
     Any,
     Callable,
     cast,
     Dict,
     Iterator,
     List,
@@ -226,15 +227,15 @@
     storage: "ProjectStorageManager"
     tags: ProjectTagManager
     triggers: ProjectTriggerManager
     users: ProjectUserManager
     variables: ProjectVariableManager
     wikis: ProjectWikiManager
 
-    @cli.register_custom_action("Project", ("forked_from_id",))
+    @cli.register_custom_action(cls_names="Project", required=("forked_from_id",))
     @exc.on_http_error(exc.GitlabCreateError)
     def create_fork_relation(self, forked_from_id: int, **kwargs: Any) -> None:
         """Create a forked from/to relation between existing projects.
 
         Args:
             forked_from_id: The ID of the project that was forked from
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -242,45 +243,45 @@
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabCreateError: If the relation could not be created
         """
         path = f"/projects/{self.encoded_id}/fork/{forked_from_id}"
         self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabDeleteError)
     def delete_fork_relation(self, **kwargs: Any) -> None:
         """Delete a forked relation between existing projects.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabDeleteError: If the server failed to perform the request
         """
         path = f"/projects/{self.encoded_id}/fork"
         self.manager.gitlab.http_delete(path, **kwargs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabGetError)
     def languages(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Get languages used in the project with percentage value.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabGetError: If the server failed to perform the request
         """
         path = f"/projects/{self.encoded_id}/languages"
         return self.manager.gitlab.http_get(path, **kwargs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabCreateError)
     def star(self, **kwargs: Any) -> None:
         """Star a project.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -290,15 +291,15 @@
         """
         path = f"/projects/{self.encoded_id}/star"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabDeleteError)
     def unstar(self, **kwargs: Any) -> None:
         """Unstar a project.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -308,15 +309,15 @@
         """
         path = f"/projects/{self.encoded_id}/unstar"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabCreateError)
     def archive(self, **kwargs: Any) -> None:
         """Archive a project.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -326,15 +327,15 @@
         """
         path = f"/projects/{self.encoded_id}/archive"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabDeleteError)
     def unarchive(self, **kwargs: Any) -> None:
         """Unarchive a project.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -345,15 +346,17 @@
         path = f"/projects/{self.encoded_id}/unarchive"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(server_data, dict)
         self._update_attrs(server_data)
 
     @cli.register_custom_action(
-        "Project", ("group_id", "group_access"), ("expires_at",)
+        cls_names="Project",
+        required=("group_id", "group_access"),
+        optional=("expires_at",),
     )
     @exc.on_http_error(exc.GitlabCreateError)
     def share(
         self,
         group_id: int,
         group_access: int,
         expires_at: Optional[str] = None,
@@ -374,15 +377,15 @@
         data = {
             "group_id": group_id,
             "group_access": group_access,
             "expires_at": expires_at,
         }
         self.manager.gitlab.http_post(path, post_data=data, **kwargs)
 
-    @cli.register_custom_action("Project", ("group_id",))
+    @cli.register_custom_action(cls_names="Project", required=("group_id",))
     @exc.on_http_error(exc.GitlabDeleteError)
     def unshare(self, group_id: int, **kwargs: Any) -> None:
         """Delete a shared project link within a group.
 
         Args:
             group_id: ID of the group.
             **kwargs: Extra options to send to the server (e.g. sudo)
@@ -391,15 +394,15 @@
             GitlabAuthenticationError: If authentication is not correct
             GitlabDeleteError: If the server failed to perform the request
         """
         path = f"/projects/{self.encoded_id}/share/{group_id}"
         self.manager.gitlab.http_delete(path, **kwargs)
 
     # variables not supported in CLI
-    @cli.register_custom_action("Project", ("ref", "token"))
+    @cli.register_custom_action(cls_names="Project", required=("ref", "token"))
     @exc.on_http_error(exc.GitlabCreateError)
     def trigger_pipeline(
         self,
         ref: str,
         token: str,
         variables: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
@@ -422,15 +425,15 @@
         path = f"/projects/{self.encoded_id}/trigger/pipeline"
         post_data = {"ref": ref, "token": token, "variables": variables}
         attrs = self.manager.gitlab.http_post(path, post_data=post_data, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(attrs, dict)
         return ProjectPipeline(self.pipelines, attrs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabHousekeepingError)
     def housekeeping(self, **kwargs: Any) -> None:
         """Start the housekeeping task.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -438,30 +441,30 @@
             GitlabAuthenticationError: If authentication is not correct
             GitlabHousekeepingError: If the server failed to perform the
                                      request
         """
         path = f"/projects/{self.encoded_id}/housekeeping"
         self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabRestoreError)
     def restore(self, **kwargs: Any) -> None:
         """Restore a project marked for deletion.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabRestoreError: If the server failed to perform the request
         """
         path = f"/projects/{self.encoded_id}/restore"
         self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("Project", optional=("wiki",))
+    @cli.register_custom_action(cls_names="Project", optional=("wiki",))
     @exc.on_http_error(exc.GitlabGetError)
     def snapshot(
         self,
         wiki: bool = False,
         streamed: bool = False,
         action: Optional[Callable[[bytes], None]] = None,
         chunk_size: int = 1024,
@@ -496,15 +499,15 @@
         )
         if TYPE_CHECKING:
             assert isinstance(result, requests.Response)
         return utils.response_content(
             result, streamed, action, chunk_size, iterator=iterator
         )
 
-    @cli.register_custom_action("Project", ("scope", "search"))
+    @cli.register_custom_action(cls_names="Project", required=("scope", "search"))
     @exc.on_http_error(exc.GitlabSearchError)
     def search(
         self, scope: str, search: str, **kwargs: Any
     ) -> Union[client.GitlabList, List[Dict[str, Any]]]:
         """Search the project resources matching the provided string.'
 
         Args:
@@ -519,30 +522,30 @@
         Returns:
             A list of dicts describing the resources found.
         """
         data = {"scope": scope, "search": search}
         path = f"/projects/{self.encoded_id}/search"
         return self.manager.gitlab.http_list(path, query_data=data, **kwargs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabCreateError)
     def mirror_pull(self, **kwargs: Any) -> None:
         """Start the pull mirroring process for the project.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabCreateError: If the server failed to perform the request
         """
         path = f"/projects/{self.encoded_id}/mirror/pull"
         self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabGetError)
     def mirror_pull_details(self, **kwargs: Any) -> Dict[str, Any]:
         """Get a project's pull mirror details.
 
         Introduced in GitLab 15.5.
 
         Args:
@@ -557,15 +560,15 @@
         """
         path = f"/projects/{self.encoded_id}/mirror/pull"
         result = self.manager.gitlab.http_get(path, **kwargs)
         if TYPE_CHECKING:
             assert isinstance(result, dict)
         return result
 
-    @cli.register_custom_action("Project", ("to_namespace",))
+    @cli.register_custom_action(cls_names="Project", required=("to_namespace",))
     @exc.on_http_error(exc.GitlabTransferProjectError)
     def transfer(self, to_namespace: Union[int, str], **kwargs: Any) -> None:
         """Transfer a project to the given namespace ID
 
         Args:
             to_namespace: ID or path of the namespace to transfer the
             project to
@@ -782,15 +785,15 @@
 
     def get(self, id: Union[str, int], lazy: bool = False, **kwargs: Any) -> Project:
         return cast(Project, super().get(id=id, lazy=lazy, **kwargs))
 
     @exc.on_http_error(exc.GitlabImportError)
     def import_project(
         self,
-        file: str,
+        file: io.BufferedReader,
         path: str,
         name: Optional[str] = None,
         namespace: Optional[str] = None,
         overwrite: bool = False,
         override_params: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Union[Dict[str, Any], requests.Response]:
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/push_rules.py` & `python_gitlab-4.6.0/gitlab/v4/objects/push_rules.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/releases.py` & `python_gitlab-4.6.0/gitlab/v4/objects/releases.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/repositories.py` & `python_gitlab-4.6.0/gitlab/v4/objects/repositories.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     # When running mypy we use these as the base classes
     _RestObjectBase = gitlab.base.RESTObject
 else:
     _RestObjectBase = object
 
 
 class RepositoryMixin(_RestObjectBase):
-    @cli.register_custom_action("Project", ("submodule", "branch", "commit_sha"))
+    @cli.register_custom_action(
+        cls_names="Project", required=("submodule", "branch", "commit_sha")
+    )
     @exc.on_http_error(exc.GitlabUpdateError)
     def update_submodule(
         self, submodule: str, branch: str, commit_sha: str, **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Update a project submodule
 
         Args:
@@ -43,15 +45,17 @@
         submodule = utils.EncodedId(submodule)
         path = f"/projects/{self.encoded_id}/repository/submodules/{submodule}"
         data = {"branch": branch, "commit_sha": commit_sha}
         if "commit_message" in kwargs:
             data["commit_message"] = kwargs["commit_message"]
         return self.manager.gitlab.http_put(path, post_data=data)
 
-    @cli.register_custom_action("Project", (), ("path", "ref", "recursive"))
+    @cli.register_custom_action(
+        cls_names="Project", optional=("path", "ref", "recursive")
+    )
     @exc.on_http_error(exc.GitlabGetError)
     def repository_tree(
         self, path: str = "", ref: str = "", recursive: bool = False, **kwargs: Any
     ) -> Union[gitlab.client.GitlabList, List[Dict[str, Any]]]:
         """Return a list of files in the repository.
 
         Args:
@@ -76,15 +80,15 @@
         query_data: Dict[str, Any] = {"recursive": recursive}
         if path:
             query_data["path"] = path
         if ref:
             query_data["ref"] = ref
         return self.manager.gitlab.http_list(gl_path, query_data=query_data, **kwargs)
 
-    @cli.register_custom_action("Project", ("sha",))
+    @cli.register_custom_action(cls_names="Project", required=("sha",))
     @exc.on_http_error(exc.GitlabGetError)
     def repository_blob(
         self, sha: str, **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Return a file by blob SHA.
 
         Args:
@@ -98,15 +102,15 @@
         Returns:
             The blob content and metadata
         """
 
         path = f"/projects/{self.encoded_id}/repository/blobs/{sha}"
         return self.manager.gitlab.http_get(path, **kwargs)
 
-    @cli.register_custom_action("Project", ("sha",))
+    @cli.register_custom_action(cls_names="Project", required=("sha",))
     @exc.on_http_error(exc.GitlabGetError)
     def repository_raw_blob(
         self,
         sha: str,
         streamed: bool = False,
         action: Optional[Callable[..., Any]] = None,
         chunk_size: int = 1024,
@@ -141,15 +145,15 @@
         )
         if TYPE_CHECKING:
             assert isinstance(result, requests.Response)
         return utils.response_content(
             result, streamed, action, chunk_size, iterator=iterator
         )
 
-    @cli.register_custom_action("Project", ("from_", "to"))
+    @cli.register_custom_action(cls_names="Project", required=("from_", "to"))
     @exc.on_http_error(exc.GitlabGetError)
     def repository_compare(
         self, from_: str, to: str, **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Return a diff between two branches/commits.
 
         Args:
@@ -164,15 +168,15 @@
         Returns:
             The diff
         """
         path = f"/projects/{self.encoded_id}/repository/compare"
         query_data = {"from": from_, "to": to}
         return self.manager.gitlab.http_get(path, query_data=query_data, **kwargs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabGetError)
     def repository_contributors(
         self, **kwargs: Any
     ) -> Union[gitlab.client.GitlabList, List[Dict[str, Any]]]:
         """Return a list of contributors for the project.
 
         Args:
@@ -189,15 +193,15 @@
 
         Returns:
             The contributors
         """
         path = f"/projects/{self.encoded_id}/repository/contributors"
         return self.manager.gitlab.http_list(path, **kwargs)
 
-    @cli.register_custom_action("Project", (), ("sha", "format"))
+    @cli.register_custom_action(cls_names="Project", optional=("sha", "format"))
     @exc.on_http_error(exc.GitlabListError)
     def repository_archive(
         self,
         sha: Optional[str] = None,
         streamed: bool = False,
         action: Optional[Callable[..., Any]] = None,
         chunk_size: int = 1024,
@@ -243,15 +247,15 @@
         )
         if TYPE_CHECKING:
             assert isinstance(result, requests.Response)
         return utils.response_content(
             result, streamed, action, chunk_size, iterator=iterator
         )
 
-    @cli.register_custom_action("Project", ("refs",))
+    @cli.register_custom_action(cls_names="Project", required=("refs",))
     @exc.on_http_error(exc.GitlabGetError)
     def repository_merge_base(
         self, refs: List[str], **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Return a diff between two branches/commits.
 
         Args:
@@ -269,15 +273,15 @@
         query_data, _ = utils._transform_types(
             data={"refs": refs},
             custom_types={"refs": types.ArrayAttribute},
             transform_data=True,
         )
         return self.manager.gitlab.http_get(path, query_data=query_data, **kwargs)
 
-    @cli.register_custom_action("Project")
+    @cli.register_custom_action(cls_names="Project")
     @exc.on_http_error(exc.GitlabDeleteError)
     def delete_merged_branches(self, **kwargs: Any) -> None:
         """Delete merged branches.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/resource_groups.py` & `python_gitlab-4.6.0/gitlab/v4/objects/resource_groups.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/reviewers.py` & `python_gitlab-4.6.0/gitlab/v4/objects/reviewers.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/runners.py` & `python_gitlab-4.6.0/gitlab/v4/objects/runners.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             "access_level",
             "maximum_timeout",
         ),
     )
     _list_filters = ("scope", "type", "status", "paused", "tag_list")
     _types = {"tag_list": types.CommaSeparatedListAttribute}
 
-    @cli.register_custom_action("RunnerManager", (), ("scope",))
+    @cli.register_custom_action(cls_names="RunnerManager", optional=("scope",))
     @exc.on_http_error(exc.GitlabListError)
     def all(self, scope: Optional[str] = None, **kwargs: Any) -> List[Runner]:
         """List all the runners.
 
         Args:
             scope: The scope of runners to show, one of: specific,
                 shared, active, paused, online
@@ -99,15 +99,15 @@
         path = "/runners/all"
         query_data = {}
         if scope is not None:
             query_data["scope"] = scope
         obj = self.gitlab.http_list(path, query_data, **kwargs)
         return [self._obj_cls(self, item) for item in obj]
 
-    @cli.register_custom_action("RunnerManager", ("token",))
+    @cli.register_custom_action(cls_names="RunnerManager", required=("token",))
     @exc.on_http_error(exc.GitlabVerifyError)
     def verify(self, token: str, **kwargs: Any) -> None:
         """Validates authentication credentials for a registered Runner.
 
         Args:
             token: The runner's authentication token
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/secure_files.py` & `python_gitlab-4.6.0/gitlab/v4/objects/secure_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from gitlab.mixins import NoUpdateMixin, ObjectDeleteMixin
 from gitlab.types import FileAttribute, RequiredOptional
 
 __all__ = ["ProjectSecureFile", "ProjectSecureFileManager"]
 
 
 class ProjectSecureFile(ObjectDeleteMixin, RESTObject):
-    @cli.register_custom_action("ProjectSecureFile")
+    @cli.register_custom_action(cls_names="ProjectSecureFile")
     @exc.on_http_error(exc.GitlabGetError)
     def download(
         self,
         streamed: bool = False,
         action: Optional[Callable[[bytes], None]] = None,
         chunk_size: int = 1024,
         *,
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/settings.py` & `python_gitlab-4.6.0/gitlab/v4/objects/settings.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/sidekiq.py` & `python_gitlab-4.6.0/gitlab/v4/objects/sidekiq.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class SidekiqManager(RESTManager):
     """Manager for the Sidekiq methods.
 
     This manager doesn't actually manage objects but provides helper function
     for the sidekiq metrics API.
     """
 
-    @cli.register_custom_action("SidekiqManager")
+    @cli.register_custom_action(cls_names="SidekiqManager")
     @exc.on_http_error(exc.GitlabGetError)
     def queue_metrics(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Return the registered queues information.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -31,15 +31,15 @@
             GitlabGetError: If the information couldn't be retrieved
 
         Returns:
             Information about the Sidekiq queues
         """
         return self.gitlab.http_get("/sidekiq/queue_metrics", **kwargs)
 
-    @cli.register_custom_action("SidekiqManager")
+    @cli.register_custom_action(cls_names="SidekiqManager")
     @exc.on_http_error(exc.GitlabGetError)
     def process_metrics(
         self, **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Return the registered sidekiq workers.
 
         Args:
@@ -50,15 +50,15 @@
             GitlabGetError: If the information couldn't be retrieved
 
         Returns:
             Information about the register Sidekiq worker
         """
         return self.gitlab.http_get("/sidekiq/process_metrics", **kwargs)
 
-    @cli.register_custom_action("SidekiqManager")
+    @cli.register_custom_action(cls_names="SidekiqManager")
     @exc.on_http_error(exc.GitlabGetError)
     def job_stats(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Return statistics about the jobs performed.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -67,15 +67,15 @@
             GitlabGetError: If the information couldn't be retrieved
 
         Returns:
             Statistics about the Sidekiq jobs performed
         """
         return self.gitlab.http_get("/sidekiq/job_stats", **kwargs)
 
-    @cli.register_custom_action("SidekiqManager")
+    @cli.register_custom_action(cls_names="SidekiqManager")
     @exc.on_http_error(exc.GitlabGetError)
     def compound_metrics(
         self, **kwargs: Any
     ) -> Union[Dict[str, Any], requests.Response]:
         """Return all available metrics and statistics.
 
         Args:
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/snippets.py` & `python_gitlab-4.6.0/gitlab/v4/objects/snippets.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "ProjectSnippetManager",
 ]
 
 
 class Snippet(UserAgentDetailMixin, SaveMixin, ObjectDeleteMixin, RESTObject):
     _repr_attr = "title"
 
-    @cli.register_custom_action("Snippet")
+    @cli.register_custom_action(cls_names="Snippet")
     @exc.on_http_error(exc.GitlabGetError)
     def content(
         self,
         streamed: bool = False,
         action: Optional[Callable[..., Any]] = None,
         chunk_size: int = 1024,
         *,
@@ -85,15 +85,15 @@
             "file_name",
             "content",
             "visibility",
             "description",
         ),
     )
 
-    @cli.register_custom_action("SnippetManager")
+    @cli.register_custom_action(cls_names="SnippetManager")
     def public(self, **kwargs: Any) -> Union[RESTObjectList, List[RESTObject]]:
         """List all the public snippets.
 
         Args:
             all: If True the returned object will be a list
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -113,15 +113,15 @@
     _url = "/projects/{project_id}/snippets"
     _repr_attr = "title"
 
     awardemojis: ProjectSnippetAwardEmojiManager
     discussions: ProjectSnippetDiscussionManager
     notes: ProjectSnippetNoteManager
 
-    @cli.register_custom_action("ProjectSnippet")
+    @cli.register_custom_action(cls_names="ProjectSnippet")
     @exc.on_http_error(exc.GitlabGetError)
     def content(
         self,
         streamed: bool = False,
         action: Optional[Callable[..., Any]] = None,
         chunk_size: int = 1024,
         *,
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/statistics.py` & `python_gitlab-4.6.0/gitlab/v4/objects/statistics.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/tags.py` & `python_gitlab-4.6.0/gitlab/v4/objects/tags.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/templates.py` & `python_gitlab-4.6.0/gitlab/v4/objects/templates.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/todos.py` & `python_gitlab-4.6.0/gitlab/v4/objects/todos.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __all__ = [
     "Todo",
     "TodoManager",
 ]
 
 
 class Todo(ObjectDeleteMixin, RESTObject):
-    @cli.register_custom_action("Todo")
+    @cli.register_custom_action(cls_names="Todo")
     @exc.on_http_error(exc.GitlabTodoError)
     def mark_as_done(self, **kwargs: Any) -> Dict[str, Any]:
         """Mark the todo as done.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -36,15 +36,15 @@
 
 
 class TodoManager(ListMixin, DeleteMixin, RESTManager):
     _path = "/todos"
     _obj_cls = Todo
     _list_filters = ("action", "author_id", "project_id", "state", "type")
 
-    @cli.register_custom_action("TodoManager")
+    @cli.register_custom_action(cls_names="TodoManager")
     @exc.on_http_error(exc.GitlabTodoError)
     def mark_all_as_done(self, **kwargs: Any) -> None:
         """Mark all the todos as done.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/topics.py` & `python_gitlab-4.6.0/gitlab/v4/objects/topics.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     _update_attrs = RequiredOptional(optional=("avatar", "description", "name"))
     _types = {"avatar": types.ImageAttribute}
 
     def get(self, id: Union[str, int], lazy: bool = False, **kwargs: Any) -> Topic:
         return cast(Topic, super().get(id=id, lazy=lazy, **kwargs))
 
     @cli.register_custom_action(
-        "TopicManager",
-        mandatory=("source_topic_id", "target_topic_id"),
+        cls_names="TopicManager",
+        required=("source_topic_id", "target_topic_id"),
     )
     @exc.on_http_error(exc.GitlabMRClosedError)
     def merge(
         self,
         source_topic_id: Union[int, str],
         target_topic_id: Union[int, str],
         **kwargs: Any,
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/triggers.py` & `python_gitlab-4.6.0/gitlab/v4/objects/triggers.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/users.py` & `python_gitlab-4.6.0/gitlab/v4/objects/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     keys: "UserKeyManager"
     memberships: "UserMembershipManager"
     personal_access_tokens: UserPersonalAccessTokenManager
     projects: "UserProjectManager"
     starred_projects: "StarredProjectManager"
     status: "UserStatusManager"
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabBlockError)
     def block(self, **kwargs: Any) -> Optional[bool]:
         """Block the user.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -211,15 +211,15 @@
         server_data = cast(
             Optional[bool], self.manager.gitlab.http_post(path, **kwargs)
         )
         if server_data is True:
             self._attrs["state"] = "blocked"
         return server_data
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabFollowError)
     def follow(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Follow the user.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -229,15 +229,15 @@
 
         Returns:
             The new object data (*not* a RESTObject)
         """
         path = f"/users/{self.encoded_id}/follow"
         return self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabUnfollowError)
     def unfollow(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Unfollow the user.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -247,15 +247,15 @@
 
         Returns:
             The new object data (*not* a RESTObject)
         """
         path = f"/users/{self.encoded_id}/unfollow"
         return self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabUnblockError)
     def unblock(self, **kwargs: Any) -> Optional[bool]:
         """Unblock the user.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -272,15 +272,15 @@
         server_data = cast(
             Optional[bool], self.manager.gitlab.http_post(path, **kwargs)
         )
         if server_data is True:
             self._attrs["state"] = "active"
         return server_data
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabDeactivateError)
     def deactivate(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Deactivate the user.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -293,15 +293,15 @@
         """
         path = f"/users/{self.encoded_id}/deactivate"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if server_data:
             self._attrs["state"] = "deactivated"
         return server_data
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabActivateError)
     def activate(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Activate the user.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -314,15 +314,15 @@
         """
         path = f"/users/{self.encoded_id}/activate"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if server_data:
             self._attrs["state"] = "active"
         return server_data
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabUserApproveError)
     def approve(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Approve a user creation request.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -332,15 +332,15 @@
 
         Returns:
             The new object data (*not* a RESTObject)
         """
         path = f"/users/{self.encoded_id}/approve"
         return self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabUserRejectError)
     def reject(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Reject a user creation request.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -350,15 +350,15 @@
 
         Returns:
             The new object data (*not* a RESTObject)
         """
         path = f"/users/{self.encoded_id}/reject"
         return self.manager.gitlab.http_post(path, **kwargs)
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabBanError)
     def ban(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Ban the user.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
 
@@ -371,15 +371,15 @@
         """
         path = f"/users/{self.encoded_id}/ban"
         server_data = self.manager.gitlab.http_post(path, **kwargs)
         if server_data:
             self._attrs["state"] = "banned"
         return server_data
 
-    @cli.register_custom_action("User")
+    @cli.register_custom_action(cls_names="User")
     @exc.on_http_error(exc.GitlabUnbanError)
     def unban(self, **kwargs: Any) -> Union[Dict[str, Any], requests.Response]:
         """Unban the user.
 
         Args:
             **kwargs: Extra options to send to the server (e.g. sudo)
```

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/variables.py` & `python_gitlab-4.6.0/gitlab/v4/objects/variables.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/gitlab/v4/objects/wikis.py` & `python_gitlab-4.6.0/gitlab/v4/objects/wikis.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/pyproject.toml` & `python_gitlab-4.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     {name = "John Villalovos", email="john@sodarock.com"},
     {name = "Max Wittig", email="max.wittig@siemens.com"},
     {name = "Nejc Habjan", email="nejc.habjan@siemens.com"},
     {name = "Roger Meier", email="r.meier@siemens.com"}
 ]
 requires-python = ">=3.8.0"
 dependencies = [
-    "requests>=2.25.0",
-    "requests-toolbelt>=0.10.1",
+    "requests>=2.32.0",
+    "requests-toolbelt>=1.0.0",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Natural Language :: English",
```

### Comparing `python_gitlab-4.5.0/python_gitlab.egg-info/PKG-INFO` & `python_gitlab-4.6.0/python_gitlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gitlab
-Version: 4.5.0
+Version: 4.6.0
 Summary: A python wrapper for the GitLab API
 Author-email: Gauvain Pocentek <gauvain@pocentek.net>
 Maintainer-email: John Villalovos <john@sodarock.com>, Max Wittig <max.wittig@siemens.com>, Nejc Habjan <nejc.habjan@siemens.com>, Roger Meier <r.meier@siemens.com>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/python-gitlab/python-gitlab
 Project-URL: Changelog, https://github.com/python-gitlab/python-gitlab/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://python-gitlab.readthedocs.io
@@ -24,16 +24,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: AUTHORS
-Requires-Dist: requests>=2.25.0
-Requires-Dist: requests-toolbelt>=0.10.1
+Requires-Dist: requests>=2.32.0
+Requires-Dist: requests-toolbelt>=1.0.0
 Provides-Extra: autocompletion
 Requires-Dist: argcomplete<3,>=1.10.0; extra == "autocompletion"
 Provides-Extra: yaml
 Requires-Dist: PyYaml>=6.0.1; extra == "yaml"
 
 python-gitlab
 =============
```

### Comparing `python_gitlab-4.5.0/python_gitlab.egg-info/SOURCES.txt` & `python_gitlab-4.6.0/python_gitlab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
 gitlab/v4/objects/push_rules.py
 gitlab/v4/objects/releases.py
 gitlab/v4/objects/repositories.py
 gitlab/v4/objects/resource_groups.py
 gitlab/v4/objects/reviewers.py
 gitlab/v4/objects/runners.py
 gitlab/v4/objects/secure_files.py
+gitlab/v4/objects/service_accounts.py
 gitlab/v4/objects/settings.py
 gitlab/v4/objects/sidekiq.py
 gitlab/v4/objects/snippets.py
 gitlab/v4/objects/statistics.py
 gitlab/v4/objects/tags.py
 gitlab/v4/objects/templates.py
 gitlab/v4/objects/todos.py
```

### Comparing `python_gitlab-4.5.0/tests/conftest.py` & `python_gitlab-4.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_bulk_imports.py` & `python_gitlab-4.6.0/tests/functional/api/test_bulk_imports.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_current_user.py` & `python_gitlab-4.6.0/tests/functional/api/test_current_user.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_deploy_tokens.py` & `python_gitlab-4.6.0/tests/functional/api/test_deploy_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_epics.py` & `python_gitlab-4.6.0/tests/functional/api/test_epics.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_gitlab.py` & `python_gitlab-4.6.0/tests/functional/api/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_groups.py` & `python_gitlab-4.6.0/tests/functional/api/test_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -304,7 +304,16 @@
 
 @pytest.mark.gitlab_premium
 @pytest.mark.xfail(reason="need to setup an identity provider or it's mock")
 def test_group_saml_group_links(group):
     group.saml_group_links.create(
         {"saml_group_name": "saml-group-1", "access_level": 10}
     )
+
+
+@pytest.mark.gitlab_premium
+def test_group_service_account(group):
+    service_account = group.service_accounts.create(
+        {"name": "gitlab-service-account", "username": "gitlab-service-account"}
+    )
+    assert service_account.name == "gitlab-service-account"
+    assert service_account.username == "gitlab-service-account"
```

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_import_export.py` & `python_gitlab-4.6.0/tests/functional/api/test_import_export.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_issues.py` & `python_gitlab-4.6.0/tests/functional/api/test_issues.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_keys.py` & `python_gitlab-4.6.0/tests/functional/api/test_keys.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_lazy_objects.py` & `python_gitlab-4.6.0/tests/functional/api/test_lazy_objects.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_merge_requests.py` & `python_gitlab-4.6.0/tests/functional/api/test_merge_requests.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_packages.py` & `python_gitlab-4.6.0/tests/functional/api/test_packages.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_project_job_token_scope.py` & `python_gitlab-4.6.0/tests/functional/api/test_project_job_token_scope.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_projects.py` & `python_gitlab-4.6.0/tests/functional/api/test_projects.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_push_rules.py` & `python_gitlab-4.6.0/tests/functional/api/test_push_rules.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_releases.py` & `python_gitlab-4.6.0/tests/functional/api/test_releases.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_repository.py` & `python_gitlab-4.6.0/tests/functional/api/test_repository.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_services.py` & `python_gitlab-4.6.0/tests/functional/api/test_services.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_snippets.py` & `python_gitlab-4.6.0/tests/functional/api/test_snippets.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_topics.py` & `python_gitlab-4.6.0/tests/functional/api/test_topics.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_users.py` & `python_gitlab-4.6.0/tests/functional/api/test_users.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_variables.py` & `python_gitlab-4.6.0/tests/functional/api/test_variables.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/api/test_wikis.py` & `python_gitlab-4.6.0/tests/functional/api/test_wikis.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/conftest.py` & `python_gitlab-4.6.0/tests/functional/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,20 +30,14 @@
 
 def test_config_error_with_help_prints_help(script_runner):
     ret = script_runner.run(["gitlab", "-c", "invalid-file", "--help"])
     assert ret.stdout.startswith("usage:")
     assert ret.returncode == 0
 
 
-def test_global_help_prints_resources_vertically(script_runner):
-    ret = script_runner.run(["gitlab", "--help"])
-    assert """resource:\n  application\n  application-appearance\n""" in ret.stdout
-    assert ret.returncode == 0
-
-
 def test_resource_help_prints_actions_vertically(script_runner):
     ret = script_runner.run(["gitlab", "project", "--help"])
     assert """action:\n  list\n  get""" in ret.stdout
     assert ret.returncode == 0
 
 
 def test_resource_help_prints_actions_vertically_only_one_action(script_runner):
```

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli_artifacts.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli_artifacts.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli_packages.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli_packages.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli_projects.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli_projects.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli_repository.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli_repository.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli_resource_access_tokens.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli_resource_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli_users.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli_users.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli_v4.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli_v4.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/cli/test_cli_variables.py` & `python_gitlab-4.6.0/tests/functional/cli/test_cli_variables.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/conftest.py` & `python_gitlab-4.6.0/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/fixtures/avatar.png` & `python_gitlab-4.6.0/tests/functional/fixtures/avatar.png`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/fixtures/create_license.rb` & `python_gitlab-4.6.0/tests/functional/fixtures/create_license.rb`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/fixtures/docker-compose.yml` & `python_gitlab-4.6.0/tests/functional/fixtures/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/fixtures/docker.py` & `python_gitlab-4.6.0/tests/functional/fixtures/docker.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/functional/helpers.py` & `python_gitlab-4.6.0/tests/functional/helpers.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/smoke/test_dists.py` & `python_gitlab-4.6.0/tests/smoke/test_dists.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/_backends/test_requests_backend.py` & `python_gitlab-4.6.0/tests/unit/_backends/test_requests_backend.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/base/test_rest_manager.py` & `python_gitlab-4.6.0/tests/unit/base/test_rest_manager.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/base/test_rest_object.py` & `python_gitlab-4.6.0/tests/unit/base/test_rest_object.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/conftest.py` & `python_gitlab-4.6.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/helpers.py` & `python_gitlab-4.6.0/tests/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/meta/test_ensure_type_hints.py` & `python_gitlab-4.6.0/tests/unit/meta/test_ensure_type_hints.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/meta/test_imports.py` & `python_gitlab-4.6.0/tests/unit/meta/test_imports.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/meta/test_mro.py` & `python_gitlab-4.6.0/tests/unit/meta/test_mro.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/mixins/test_meta_mixins.py` & `python_gitlab-4.6.0/tests/unit/mixins/test_meta_mixins.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/mixins/test_mixin_methods.py` & `python_gitlab-4.6.0/tests/unit/mixins/test_mixin_methods.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/mixins/test_object_mixins_attributes.py` & `python_gitlab-4.6.0/tests/unit/mixins/test_object_mixins_attributes.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/conftest.py` & `python_gitlab-4.6.0/tests/unit/objects/conftest.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_appearance.py` & `python_gitlab-4.6.0/tests/unit/objects/test_appearance.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_applications.py` & `python_gitlab-4.6.0/tests/unit/objects/test_applications.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_audit_events.py` & `python_gitlab-4.6.0/tests/unit/objects/test_audit_events.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_badges.py` & `python_gitlab-4.6.0/tests/unit/objects/test_badges.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_bridges.py` & `python_gitlab-4.6.0/tests/unit/objects/test_bridges.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_bulk_imports.py` & `python_gitlab-4.6.0/tests/unit/objects/test_bulk_imports.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_ci_lint.py` & `python_gitlab-4.6.0/tests/unit/objects/test_ci_lint.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_commits.py` & `python_gitlab-4.6.0/tests/unit/objects/test_commits.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_deploy_tokens.py` & `python_gitlab-4.6.0/tests/unit/objects/test_deploy_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_deployments.py` & `python_gitlab-4.6.0/tests/unit/objects/test_deployments.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_draft_notes.py` & `python_gitlab-4.6.0/tests/unit/objects/test_draft_notes.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_environments.py` & `python_gitlab-4.6.0/tests/unit/objects/test_environments.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_group_access_tokens.py` & `python_gitlab-4.6.0/tests/unit/objects/test_group_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_groups.py` & `python_gitlab-4.6.0/tests/unit/objects/test_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,19 @@
     "member_check": True,
     "prevent_secrets": True,
     "author_email_regex": "^[A-Za-z0-9.]+@gitlab.com$",
     "file_name_regex": "(exe)$",
     "max_file_size": 100,
 }
 
+service_account_content = {
+    "name": "gitlab-service-account",
+    "username": "gitlab-service-account",
+}
+
 
 @pytest.fixture
 def resp_groups():
     with responses.RequestsMock(assert_all_requests_are_fired=False) as rsps:
         rsps.add(
             method=responses.GET,
             url="http://localhost/api/v4/groups/1",
@@ -321,14 +326,27 @@
             json=created_content,
             content_type="application/json",
             status=201,
         )
         yield rsps
 
 
+@pytest.fixture
+def resp_create_group_service_account():
+    with responses.RequestsMock() as rsps:
+        rsps.add(
+            method=responses.POST,
+            url="http://localhost/api/v4/groups/1/service_accounts",
+            json=service_account_content,
+            content_type="application/json",
+            status=200,
+        )
+        yield rsps
+
+
 def test_get_group(gl, resp_groups):
     data = gl.groups.get(1)
     assert isinstance(data, gitlab.v4.objects.Group)
     assert data.name == "name"
     assert data.path == "path"
     assert data.id == 1
 
@@ -462,7 +480,15 @@
 def test_delete_saml_group_link(group, resp_delete_saml_group_link):
     saml_group_link = group.saml_group_links.create(create_saml_group_link_request_body)
     saml_group_link.delete()
 
 
 def test_group_restore(group, resp_restore_group):
     group.restore()
+
+
+def test_create_group_service_account(group, resp_create_group_service_account):
+    service_account = group.service_accounts.create(
+        {"name": "gitlab-service-account", "username": "gitlab-service-account"}
+    )
+    assert service_account.name == "gitlab-service-account"
+    assert service_account.username == "gitlab-service-account"
```

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_hooks.py` & `python_gitlab-4.6.0/tests/unit/objects/test_hooks.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_invitations.py` & `python_gitlab-4.6.0/tests/unit/objects/test_invitations.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_issues.py` & `python_gitlab-4.6.0/tests/unit/objects/test_issues.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_iterations.py` & `python_gitlab-4.6.0/tests/unit/objects/test_iterations.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_job_artifacts.py` & `python_gitlab-4.6.0/tests/unit/objects/test_job_artifacts.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_job_token_scope.py` & `python_gitlab-4.6.0/tests/unit/objects/test_job_token_scope.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_jobs.py` & `python_gitlab-4.6.0/tests/unit/objects/test_jobs.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_keys.py` & `python_gitlab-4.6.0/tests/unit/objects/test_keys.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_members.py` & `python_gitlab-4.6.0/tests/unit/objects/test_members.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_merge_request_pipelines.py` & `python_gitlab-4.6.0/tests/unit/objects/test_merge_request_pipelines.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_merge_requests.py` & `python_gitlab-4.6.0/tests/unit/objects/test_merge_requests.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_merge_trains.py` & `python_gitlab-4.6.0/tests/unit/objects/test_merge_trains.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_packages.py` & `python_gitlab-4.6.0/tests/unit/objects/test_packages.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_personal_access_tokens.py` & `python_gitlab-4.6.0/tests/unit/objects/test_personal_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_pipeline_schedules.py` & `python_gitlab-4.6.0/tests/unit/objects/test_pipeline_schedules.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_pipelines.py` & `python_gitlab-4.6.0/tests/unit/objects/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_project_access_tokens.py` & `python_gitlab-4.6.0/tests/unit/objects/test_project_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_project_import_export.py` & `python_gitlab-4.6.0/tests/unit/objects/test_project_import_export.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_project_merge_request_approvals.py` & `python_gitlab-4.6.0/tests/unit/objects/test_project_merge_request_approvals.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_project_statistics.py` & `python_gitlab-4.6.0/tests/unit/objects/test_project_statistics.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_projects.py` & `python_gitlab-4.6.0/tests/unit/objects/test_projects.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_registry_repositories.py` & `python_gitlab-4.6.0/tests/unit/objects/test_registry_repositories.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_releases.py` & `python_gitlab-4.6.0/tests/unit/objects/test_releases.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_remote_mirrors.py` & `python_gitlab-4.6.0/tests/unit/objects/test_remote_mirrors.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_repositories.py` & `python_gitlab-4.6.0/tests/unit/objects/test_repositories.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_resource_groups.py` & `python_gitlab-4.6.0/tests/unit/objects/test_resource_groups.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_resource_iteration_events.py` & `python_gitlab-4.6.0/tests/unit/objects/test_resource_iteration_events.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_resource_label_events.py` & `python_gitlab-4.6.0/tests/unit/objects/test_resource_label_events.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_resource_milestone_events.py` & `python_gitlab-4.6.0/tests/unit/objects/test_resource_milestone_events.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_resource_state_events.py` & `python_gitlab-4.6.0/tests/unit/objects/test_resource_state_events.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_runners.py` & `python_gitlab-4.6.0/tests/unit/objects/test_runners.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_secure_files.py` & `python_gitlab-4.6.0/tests/unit/objects/test_secure_files.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_services.py` & `python_gitlab-4.6.0/tests/unit/objects/test_services.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_snippets.py` & `python_gitlab-4.6.0/tests/unit/objects/test_snippets.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_statistics.py` & `python_gitlab-4.6.0/tests/unit/objects/test_statistics.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_submodules.py` & `python_gitlab-4.6.0/tests/unit/objects/test_submodules.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_todos.py` & `python_gitlab-4.6.0/tests/unit/objects/test_todos.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_topics.py` & `python_gitlab-4.6.0/tests/unit/objects/test_topics.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_users.py` & `python_gitlab-4.6.0/tests/unit/objects/test_users.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/objects/test_variables.py` & `python_gitlab-4.6.0/tests/unit/objects/test_variables.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/test_cli.py` & `python_gitlab-4.6.0/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/test_config.py` & `python_gitlab-4.6.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/test_exceptions.py` & `python_gitlab-4.6.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/test_gitlab.py` & `python_gitlab-4.6.0/tests/unit/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/test_gitlab_auth.py` & `python_gitlab-4.6.0/tests/unit/test_gitlab_auth.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/test_gitlab_http_methods.py` & `python_gitlab-4.6.0/tests/unit/test_gitlab_http_methods.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/test_types.py` & `python_gitlab-4.6.0/tests/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tests/unit/test_utils.py` & `python_gitlab-4.6.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_gitlab-4.5.0/tox.ini` & `python_gitlab-4.6.0/tox.ini`

 * *Files identical despite different names*

