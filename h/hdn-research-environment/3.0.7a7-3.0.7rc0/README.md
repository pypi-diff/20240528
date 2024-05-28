# Comparing `tmp/hdn-research-environment-3.0.7a7.tar.gz` & `tmp/hdn-research-environment-3.0.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdn-research-environment-3.0.7a7.tar", last modified: Tue May 28 10:50:02 2024, max compression
+gzip compressed data, was "hdn-research-environment-3.0.7rc0.tar", last modified: Wed Apr 10 10:04:39 2024, max compression
```

## Comparing `hdn-research-environment-3.0.7a7.tar` & `hdn-research-environment-3.0.7rc0.tar`

### file list

```diff
@@ -1,109 +1,106 @@
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.434965 hdn-research-environment-3.0.7a7/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1551 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/LICENSE
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      115 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/MANIFEST.in
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      980 2024-05-28 10:50:02.435041 hdn-research-environment-3.0.7a7/PKG-INFO
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      229 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/README.md
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.421547 hdn-research-environment-3.0.7a7/environment/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/__init__.py
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.422447 hdn-research-environment-3.0.7a7/environment/api/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     8375 2024-05-27 14:48:53.000000 hdn-research-environment-3.0.7a7/environment/api/__init__.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      939 2024-04-11 13:51:03.000000 hdn-research-environment-3.0.7a7/environment/api/decorators.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      154 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/apps.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3074 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/constants.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1546 2024-04-08 12:07:08.000000 hdn-research-environment-3.0.7a7/environment/decorators.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5690 2024-05-27 14:44:42.000000 hdn-research-environment-3.0.7a7/environment/deserializers.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4513 2024-05-27 14:44:42.000000 hdn-research-environment-3.0.7a7/environment/entities.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1421 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/exceptions.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     7674 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7a7/environment/forms.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2518 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/mailers.py
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.425302 hdn-research-environment-3.0.7a7/environment/migrations/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2174 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/00012_bucketsharinginvite.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1443 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0001_initial.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1579 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      403 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      420 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2220 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0005_workflow.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      394 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2348 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      476 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      420 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1364 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      858 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/0011_refactor_workflow.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1042 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7a7/environment/migrations/0013_bucketsharinginvite_type_and_more.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/migrations/__init__.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2423 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7a7/environment/models.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    25673 2024-05-27 14:49:28.000000 hdn-research-environment-3.0.7a7/environment/services.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4519 2024-05-09 11:15:32.000000 hdn-research-environment-3.0.7a7/environment/signals.py
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.414894 hdn-research-environment-3.0.7a7/environment/static/
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.414995 hdn-research-environment-3.0.7a7/environment/static/environment/
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.426231 hdn-research-environment-3.0.7a7/environment/static/environment/css/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    11789 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/static/environment/css/bucket_files_dropzone.css
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      342 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/static/environment/css/creation_form.css
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     6583 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/static/environment/css/environment-base.css
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      117 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7a7/environment/static/environment/css/management_views.css
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       82 2024-05-27 09:03:32.000000 hdn-research-environment-3.0.7a7/environment/static/environment/css/quotas_list.css
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.427746 hdn-research-environment-3.0.7a7/environment/static/environment/js/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)   114702 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/static/environment/js/bucket_files_dropzone.min.js
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      564 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/static/environment/js/cookie.js
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      199 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/static/environment/js/destroy_shared_bucket.js
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      291 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/static/environment/js/forms.js
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2835 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3308 2024-05-09 11:15:32.000000 hdn-research-environment-3.0.7a7/environment/tasks.py
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.415218 hdn-research-environment-3.0.7a7/environment/templates/
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.430998 hdn-research-environment-3.0.7a7/environment/templates/environment/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     8013 2024-05-27 14:23:22.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3268 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2964 2024-05-23 09:29:26.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/_environment_tabs.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1269 2024-05-24 12:44:30.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/_quotas_tabs.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5553 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/_shared_buckets_list.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1073 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3847 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/bucket_files_form.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3628 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1208 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/create_shared_bucket.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1154 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/create_shared_workspace.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1630 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.431409 hdn-research-environment-3.0.7a7/environment/templates/environment/email/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      272 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      263 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/email/bucket_sharing_confirmation.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      351 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1163 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5936 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1010 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     6113 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/manage_shared_bucket.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1075 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/manage_shared_bucket_files.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1007 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/manage_shared_bucket_invitation.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      892 2024-05-24 09:19:11.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/quotas_list.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1719 2024-05-23 12:20:58.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/research_environments.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5970 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/environment/shared_bucket_files.html
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.432003 hdn-research-environment-3.0.7a7/environment/templates/tag/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1287 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/tag/bucket_modal_button.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      241 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1486 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/tag/environment_modal_button.html
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1955 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templates/tag/workspace_destroy_modal_button.html
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.432460 hdn-research-environment-3.0.7a7/environment/templatetags/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templatetags/__init__.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5724 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templatetags/action_buttons.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      136 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/templatetags/environment_templatetags.py
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.434308 hdn-research-environment-3.0.7a7/environment/tests/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/__init__.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      645 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/helpers.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    12158 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/mocks.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3007 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/test_decorators.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    10682 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/test_services.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5327 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/test_signals.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2909 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/test_utilities.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      640 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/test_validators.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3380 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/tests/test_views.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3315 2024-05-27 14:33:16.000000 hdn-research-environment-3.0.7a7/environment/urls.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1243 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/utilities.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      235 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/environment/validators.py
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    24160 2024-05-27 14:49:19.000000 hdn-research-environment-3.0.7a7/environment/views.py
-drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-05-28 10:50:02.434870 hdn-research-environment-3.0.7a7/hdn_research_environment.egg-info/
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      980 2024-05-28 10:50:02.000000 hdn-research-environment-3.0.7a7/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4154 2024-05-28 10:50:02.000000 hdn-research-environment-3.0.7a7/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        1 2024-05-28 10:50:02.000000 hdn-research-environment-3.0.7a7/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       84 2024-05-28 10:50:02.000000 hdn-research-environment-3.0.7a7/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       12 2024-05-28 10:50:02.000000 hdn-research-environment-3.0.7a7/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      109 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/pyproject.toml
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1058 2024-05-28 10:50:02.435253 hdn-research-environment-3.0.7a7/setup.cfg
--rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       38 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7a7/setup.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.023335 hdn-research-environment-3.0.7rc0/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1551 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/LICENSE
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      115 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/MANIFEST.in
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      981 2024-04-10 10:04:39.023429 hdn-research-environment-3.0.7rc0/PKG-INFO
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      229 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/README.md
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.006991 hdn-research-environment-3.0.7rc0/environment/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/__init__.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.007896 hdn-research-environment-3.0.7rc0/environment/api/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     8203 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/api/__init__.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      939 2024-03-07 11:56:49.000000 hdn-research-environment-3.0.7rc0/environment/api/decorators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      154 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/apps.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3074 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/constants.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1546 2024-04-08 12:07:08.000000 hdn-research-environment-3.0.7rc0/environment/decorators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5362 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/deserializers.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4404 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/entities.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1421 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/exceptions.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     7674 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/forms.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2518 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/mailers.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.010996 hdn-research-environment-3.0.7rc0/environment/migrations/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2174 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/00012_bucketsharinginvite.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1443 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0001_initial.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1579 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      403 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      420 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2220 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0005_workflow.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      394 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2348 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      476 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      420 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1364 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      858 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0011_refactor_workflow.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1042 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/migrations/0013_bucketsharinginvite_type_and_more.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/migrations/__init__.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2423 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/models.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    25434 2024-04-08 12:07:19.000000 hdn-research-environment-3.0.7rc0/environment/services.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4519 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/signals.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.001438 hdn-research-environment-3.0.7rc0/environment/static/
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.001535 hdn-research-environment-3.0.7rc0/environment/static/environment/
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.011779 hdn-research-environment-3.0.7rc0/environment/static/environment/css/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    11789 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/css/bucket_files_dropzone.css
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      342 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/css/creation_form.css
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     6583 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      117 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/css/management_views.css
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.013959 hdn-research-environment-3.0.7rc0/environment/static/environment/js/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)   114702 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/bucket_files_dropzone.min.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      564 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/cookie.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      199 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/destroy_shared_bucket.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      291 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/forms.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2835 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3308 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tasks.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.001729 hdn-research-environment-3.0.7rc0/environment/templates/
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.018075 hdn-research-environment-3.0.7rc0/environment/templates/environment/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     7510 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3268 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2996 2024-04-10 09:06:57.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/_environment_tabs.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5553 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/_shared_buckets_list.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1073 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3847 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/bucket_files_form.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3628 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1208 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/create_shared_bucket.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1154 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/create_shared_workspace.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1630 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.018769 hdn-research-environment-3.0.7rc0/environment/templates/environment/email/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      272 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      263 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/email/bucket_sharing_confirmation.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      351 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1163 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5936 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1010 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     6113 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1075 2024-03-14 10:19:43.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket_files.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1007 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket_invitation.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1719 2024-03-29 15:28:54.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/research_environments.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5970 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/environment/shared_bucket_files.html
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.019566 hdn-research-environment-3.0.7rc0/environment/templates/tag/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1287 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/tag/bucket_modal_button.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      241 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1486 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/tag/environment_modal_button.html
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1955 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templates/tag/workspace_destroy_modal_button.html
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.020116 hdn-research-environment-3.0.7rc0/environment/templatetags/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templatetags/__init__.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5724 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templatetags/action_buttons.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      136 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/templatetags/environment_templatetags.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.021959 hdn-research-environment-3.0.7rc0/environment/tests/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        0 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/__init__.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      645 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/helpers.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    12158 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/mocks.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3007 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_decorators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    10682 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_services.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     5327 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_signals.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     2909 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_utilities.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      640 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_validators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3380 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/tests/test_views.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     3175 2024-04-04 08:30:59.000000 hdn-research-environment-3.0.7rc0/environment/urls.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1243 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/utilities.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      235 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/environment/validators.py
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)    23604 2024-04-08 14:44:30.000000 hdn-research-environment-3.0.7rc0/environment/views.py
+drwxr-xr-x   0 mateuszkaczmarek   (501) staff       (20)        0 2024-04-10 10:04:39.023239 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      981 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     4000 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)        1 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       84 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       12 2024-04-10 10:04:38.000000 hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)      109 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/pyproject.toml
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)     1058 2024-04-10 10:04:39.023667 hdn-research-environment-3.0.7rc0/setup.cfg
+-rw-r--r--   0 mateuszkaczmarek   (501) staff       (20)       38 2024-02-15 12:24:52.000000 hdn-research-environment-3.0.7rc0/setup.py
```

### Comparing `hdn-research-environment-3.0.7a7/LICENSE` & `hdn-research-environment-3.0.7rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/PKG-INFO` & `hdn-research-environment-3.0.7rc0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdn-research-environment
-Version: 3.0.7a7
+Version: 3.0.7rc0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `hdn-research-environment-3.0.7a7/environment/api/__init__.py` & `hdn-research-environment-3.0.7rc0/environment/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,19 +81,14 @@
 
 @api_request
 def get_workspace_list(email: str) -> Request:
     return Request("GET", url=f"/workspace/{email}")
 
 
 @api_request
-def list_quotas_data(region: str, workspace_project_id: str) -> Request:
-    return Request("GET", url=f"/workspace/quotas/{region}/{workspace_project_id}")
-
-
-@api_request
 def create_workbench(
     user_email: str,
     workbench_type: str,
     machine_type: str,
     dataset_identifier: str,
     disk_size: str,
     bucket_name: str,
```

### Comparing `hdn-research-environment-3.0.7a7/environment/api/decorators.py` & `hdn-research-environment-3.0.7rc0/environment/api/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/constants.py` & `hdn-research-environment-3.0.7rc0/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/decorators.py` & `hdn-research-environment-3.0.7rc0/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/deserializers.py` & `hdn-research-environment-3.0.7rc0/environment/deserializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     WorkflowStatus,
     WorkflowType,
     WorkspaceStatus,
     SharedWorkspace,
     SharedBucket,
     SharedBucketObject,
     WorkspaceType,
-    QuotaInfo,
 )
 
 PublishedProject = apps.get_model("project", "PublishedProject")
 
 
 def _project_data_group(project: PublishedProject) -> str:
     # HACK: Use the slug and version to calculate the dataset group.
@@ -159,19 +158,7 @@
             name=bucket_object["name"],
             size=bucket_object["size"],
             modification_time=bucket_object["modification_time"],
             full_path=bucket_object["full_path"],
         )
         for bucket_object in data
     ]
-
-
-def deserialize_quotas(data) -> Iterable[QuotaInfo]:
-    return [
-        QuotaInfo(
-            metric_name=quota["metric_name"],
-            limit=quota["limit"],
-            usage=quota["usage"],
-            usage_percentage=(quota["usage"] / quota["limit"]) * 100,
-        )
-        for quota in data
-    ]
```

### Comparing `hdn-research-environment-3.0.7a7/environment/entities.py` & `hdn-research-environment-3.0.7rc0/environment/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,15 +183,7 @@
 @dataclass
 class SharedBucketObject:
     type: BucketObjectType
     name: str
     full_path: str
     size: str = None
     modification_time: str = None
-
-
-@dataclass
-class QuotaInfo:
-    metric_name: str
-    limit: int
-    usage: int
-    usage_percentage: float
```

### Comparing `hdn-research-environment-3.0.7a7/environment/exceptions.py` & `hdn-research-environment-3.0.7rc0/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/forms.py` & `hdn-research-environment-3.0.7rc0/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/mailers.py` & `hdn-research-environment-3.0.7rc0/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/migrations/00012_bucketsharinginvite.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/00012_bucketsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/migrations/0001_initial.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/migrations/0005_workflow.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/migrations/0011_refactor_workflow.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0011_refactor_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/migrations/0013_bucketsharinginvite_type_and_more.py` & `hdn-research-environment-3.0.7rc0/environment/migrations/0013_bucketsharinginvite_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/models.py` & `hdn-research-environment-3.0.7rc0/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/services.py` & `hdn-research-environment-3.0.7rc0/environment/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,21 @@
 from environment.deserializers import (
     _project_data_group,
     deserialize_research_environments,
     deserialize_workflow_details,
     deserialize_workspaces,
     deserialize_shared_workspaces,
     deserialize_shared_bucket_objects,
-    deserialize_quotas,
 )
 from environment.entities import (
     ResearchEnvironment,
     ResearchWorkspace,
     SharedWorkspace,
     SharedBucket,
     SharedBucketObject,
-    QuotaInfo,
 )
 from environment.entities import Workflow as ApiWorkflow
 from environment.exceptions import (
     BillingAccessRevokationFailed,
     BillingSharingFailed,
     ChangeEnvironmentInstanceTypeFailed,
     CreateWorkspaceFailed,
@@ -509,19 +507,14 @@
 def get_workspaces_list(user: User) -> Iterable[ResearchWorkspace]:
     email = user.cloud_identity.email
     projects = PublishedProject.objects.accessible_by(user)
     response = api.get_workspace_list(email)
     return deserialize_workspaces(response.json(), projects)
 
 
-def list_quotas_data(workspace_project_id: str, region: str) -> Iterable[QuotaInfo]:
-    response = api.list_quotas_data(workspace_project_id, region)
-    return deserialize_quotas(response.json())
-
-
 def get_shared_workspaces_list(user: User) -> Iterable[SharedWorkspace]:
     response = api.get_shared_workspaces(user.cloud_identity.email)
     return deserialize_shared_workspaces(response.json())
 
 
 def get_shared_buckets(shared_workspaces: list[SharedWorkspace]) -> list[SharedBucket]:
     return [
```

### Comparing `hdn-research-environment-3.0.7a7/environment/signals.py` & `hdn-research-environment-3.0.7rc0/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/static/environment/css/bucket_files_dropzone.css` & `hdn-research-environment-3.0.7rc0/environment/static/environment/css/bucket_files_dropzone.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/static/environment/css/environment-base.css` & `hdn-research-environment-3.0.7rc0/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/static/environment/js/bucket_files_dropzone.min.js` & `hdn-research-environment-3.0.7rc0/environment/static/environment/js/bucket_files_dropzone.min.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/static/environment/js/cookie.js` & `hdn-research-environment-3.0.7rc0/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-3.0.7rc0/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tasks.py` & `hdn-research-environment-3.0.7rc0/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/_available_environments_list.html`

 * *Files 4% similar despite different names*

```diff
@@ -27,30 +27,23 @@
                 <div class="card-header py-3" id="{{ heading }}">
                     <div class="d-flex justify-content-between">
                         <div>
                             <h6 class="mb-0">
                                 {{ workspace.gcp_project_id }}
                             </h6>
                             {% if workspace.gcp_billing_id %}
-                                <small class="d-block">
+                                <small>
                                     <span class="d-inline font-weight-bold" style="padding-top: 0.375rem;">
                                         Billing Account:
                                     </span>
                                     <span class="d-inline font-weight-normal">
                                         {{ workspace.gcp_billing_id }}
                                     </span>
                                 </small>
                             {% endif %}
-                            <small class="d-block">
-                                <span style="padding-top: 0.375rem;">
-                                    <a class="m-auto" href="{% url 'get_quotas' workspace_region=workspace.region.value|default:'us-central1' workspace_project_id=workspace.gcp_project_id %}">
-                                        Manage quotas
-                                    </a>
-                                </span>
-                            </small>
                         </div>
                         {% if not workspace.status.value == "created" %}
                             <div class="d-flex align-items-center justify-content-between">
                                 <h6 class="m-0 mr-5">
                                     {{ workspace.status.value|capfirst }}...
                                 </h6>
                                 <div class="loader" style="font-size: 3.5px; margin: 0; margin-right: 0.3rem;">Loading...</div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 { workflow_finished_message|default_if_none:"" }}
 {% endif %} {% endif %}
 _+_ _W_o_r_k_s_p_a_c_e
 {% if workspaces_with_workbenches %} {% for workspace in
 workspaces_with_workbenches %}
 ** {{{{ wwoorrkkssppaaccee..ggccpp__pprroojjeecctt__iidd }}}} **
 {% if workspace.gcp_billing_id %} Billing Account: {{ workspace.gcp_billing_id
-}} {% endif %} _M_a_n_a_g_e_ _q_u_o_t_a_s
+}} {% endif %}
 {% if not workspace.status.value == "created" %}
 ** {{{{ wwoorrkkssppaaccee..ssttaattuuss..vvaalluuee||ccaappffiirrsstt }}}}...... **
 Loading...
 {% else %} {% workspace_destroy_modal_button workspace=workspace %} {% endif %}
 {% if workspace.status.value == "created" %}
 {% if workspace.workbenches %}
     * {% for environment in workspace.workbenches %}
```

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/_environment_tabs.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/_environment_tabs.html`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         .then(({ finished }) => {
             if (finished) {
                 refreshCards(executionId);
             }
         });
     }
 
-    var socket = io("{{ websocket_url }}");
+    var socket = io("{{ websocket_url }}", { transports : ['websocket'] });
 
     socket.on('workflow_update', function(data) {
         refreshCards(data.workbench_activity_id);
     });
 
     {% for workflow in workflows %}
         socket.emit("join", "{{ workflow.execution_resource_name }}");
```

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/_shared_buckets_list.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/_shared_buckets_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/bucket_files_form.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/bucket_files_form.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/create_shared_bucket.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/create_shared_bucket.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/create_shared_workspace.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/create_shared_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/create_workspace.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/manage_shared_bucket.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/manage_shared_bucket_files.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket_files.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/manage_shared_bucket_invitation.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/manage_shared_bucket_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/research_environments.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/environment/shared_bucket_files.html` & `hdn-research-environment-3.0.7rc0/environment/templates/environment/shared_bucket_files.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/tag/bucket_modal_button.html` & `hdn-research-environment-3.0.7rc0/environment/templates/tag/bucket_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-3.0.7rc0/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templates/tag/workspace_destroy_modal_button.html` & `hdn-research-environment-3.0.7rc0/environment/templates/tag/workspace_destroy_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/templatetags/action_buttons.py` & `hdn-research-environment-3.0.7rc0/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tests/helpers.py` & `hdn-research-environment-3.0.7rc0/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tests/mocks.py` & `hdn-research-environment-3.0.7rc0/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tests/test_decorators.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tests/test_services.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tests/test_signals.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tests/test_utilities.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tests/test_validators.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/tests/test_views.py` & `hdn-research-environment-3.0.7rc0/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/urls.py` & `hdn-research-environment-3.0.7rc0/environment/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,14 @@
         "execution/check-status",
         views.check_execution_status,
         name="check_execution_status",
     ),
     path("workspace/create", views.create_workspace, name="create_workspace"),
     path("workspace/delete", views.delete_workspace, name="delete_workspace"),
     path(
-        "workspace/quotas/<workspace_region>/<workspace_project_id>",
-        views.get_quotas,
-        name="get_quotas",
-    ),
-    path(
         "sharing/workspace/create",
         views.create_shared_workspace,
         name="create_shared_workspace",
     ),
     path(
         "sharing/workspace/delete",
         views.delete_shared_workspace,
```

### Comparing `hdn-research-environment-3.0.7a7/environment/utilities.py` & `hdn-research-environment-3.0.7rc0/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-3.0.7a7/environment/views.py` & `hdn-research-environment-3.0.7rc0/environment/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -671,21 +671,7 @@
 @cloud_identity_required
 def delete_shared_bucket_content(request, bucket_name):
     data = json.loads(request.body)
     services.delete_shared_bucket_content(
         bucket_name=bucket_name, full_path=data["full_path"], user=request.user
     )
     return JsonResponse({})
-
-
-@require_http_methods(["GET"])
-@login_required
-@cloud_identity_required
-def get_quotas(request, workspace_project_id, workspace_region):
-    with concurrent.futures.ThreadPoolExecutor() as executor:
-        quotas_list_future = executor.submit(
-            services.list_quotas_data, workspace_region, workspace_project_id
-        )
-    quotas_data_list = quotas_list_future.result()
-    context = {"quotas": quotas_data_list, "workspace_project_id": workspace_project_id}
-
-    return render(request, "environment/quotas_list.html", context, status=200)
```

### Comparing `hdn-research-environment-3.0.7a7/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdn-research-environment
-Version: 3.0.7a7
+Version: 3.0.7rc0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `hdn-research-environment-3.0.7a7/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-3.0.7rc0/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,38 +37,35 @@
 environment/migrations/0011_refactor_workflow.py
 environment/migrations/0013_bucketsharinginvite_type_and_more.py
 environment/migrations/__init__.py
 environment/static/environment/css/bucket_files_dropzone.css
 environment/static/environment/css/creation_form.css
 environment/static/environment/css/environment-base.css
 environment/static/environment/css/management_views.css
-environment/static/environment/css/quotas_list.css
 environment/static/environment/js/bucket_files_dropzone.min.js
 environment/static/environment/js/cookie.js
 environment/static/environment/js/destroy_shared_bucket.js
 environment/static/environment/js/forms.js
 environment/static/environment/js/pricing_change.js
 environment/templates/environment/_available_environments_list.html
 environment/templates/environment/_billing_accounts_list.html
 environment/templates/environment/_environment_tabs.html
-environment/templates/environment/_quotas_tabs.html
 environment/templates/environment/_shared_buckets_list.html
 environment/templates/environment/base_environment_home.html
 environment/templates/environment/bucket_files_form.html
 environment/templates/environment/create_research_environment.html
 environment/templates/environment/create_shared_bucket.html
 environment/templates/environment/create_shared_workspace.html
 environment/templates/environment/create_workspace.html
 environment/templates/environment/identity_provisioning.html
 environment/templates/environment/manage_billing_account.html
 environment/templates/environment/manage_shared_billing_invitation.html
 environment/templates/environment/manage_shared_bucket.html
 environment/templates/environment/manage_shared_bucket_files.html
 environment/templates/environment/manage_shared_bucket_invitation.html
-environment/templates/environment/quotas_list.html
 environment/templates/environment/research_environments.html
 environment/templates/environment/shared_bucket_files.html
 environment/templates/environment/email/billing_sharing_confirmation.html
 environment/templates/environment/email/bucket_sharing_confirmation.html
 environment/templates/environment/email/environment_access_expired.html
 environment/templates/tag/bucket_modal_button.html
 environment/templates/tag/environment_action_button.html
```

### Comparing `hdn-research-environment-3.0.7a7/setup.cfg` & `hdn-research-environment-3.0.7rc0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 3.0.7a7
+version = 3.0.7rc
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

