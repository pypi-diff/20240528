# Comparing `tmp/django-project-base-0.75.30.tar.gz` & `tmp/django-project-base-0.75.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-base-0.75.30.tar", last modified: Tue May 21 06:04:06 2024, max compression
+gzip compressed data, was "django-project-base-0.75.32.tar", last modified: Tue May 28 14:10:11 2024, max compression
```

## Comparing `django-project-base-0.75.30.tar` & `django-project-base-0.75.32.tar`

### file list

```diff
@@ -1,222 +1,228 @@
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/
--rw-rw-r--   0 jure      (1000) jure      (1000)      116 2021-10-28 06:34:59.000000 django-project-base-0.75.30/MANIFEST.in
--rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-21 06:04:06.191960 django-project-base-0.75.30/PKG-INFO
--rw-rw-r--   0 jure      (1000) jure      (1000)     1006 2023-10-16 12:26:59.000000 django-project-base-0.75.30/README.md
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.031958 django-project-base-0.75.30/django_project_base/
--rw-r--r--   0 jure      (1000) jure      (1000)      309 2024-05-21 06:03:51.000000 django-project-base-0.75.30/django_project_base/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.035958 django-project-base-0.75.30/django_project_base/account/
--rw-rw-r--   0 jure      (1000) jure      (1000)      168 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      420 2021-12-10 13:37:27.000000 django-project-base-0.75.30/django_project_base/account/apps.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      182 2023-07-18 11:29:41.000000 django-project-base-0.75.30/django_project_base/account/constants.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.035958 django-project-base-0.75.30/django_project_base/account/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.30/django_project_base/account/management/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.035958 django-project-base-0.75.30/django_project_base/account/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.30/django_project_base/account/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1834 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/management/commands/allauth_to_social_core.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      664 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/management/commands/delete_users.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3602 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/middleware.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/account/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-08-05 09:26:32.000000 django-project-base-0.75.30/django_project_base/account/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    13904 2024-05-07 13:32:24.000000 django-project-base-0.75.30/django_project_base/account/rest/account.py
--rw-r--r--   0 jure      (1000) jure      (1000)     5208 2024-04-02 07:52:10.000000 django-project-base-0.75.30/django_project_base/account/rest/impersonate.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6815 2024-05-07 10:48:42.000000 django-project-base-0.75.30/django_project_base/account/rest/invite.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5766 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/rest/login.py
--rw-r--r--   0 jure      (1000) jure      (1000)    28708 2024-05-21 06:02:28.000000 django-project-base-0.75.30/django_project_base/account/rest/profile.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6048 2024-05-07 10:47:13.000000 django-project-base-0.75.30/django_project_base/account/rest/profile_merge.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    11582 2024-05-07 10:49:35.000000 django-project-base-0.75.30/django_project_base/account/rest/project_profiles.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6639 2024-05-16 16:41:58.000000 django-project-base-0.75.30/django_project_base/account/rest/project_profiles_utils.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6529 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/rest/reset_password.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2360 2024-03-20 13:38:09.000000 django-project-base-0.75.30/django_project_base/account/router.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/account/service/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:41.000000 django-project-base-0.75.30/django_project_base/account/service/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5836 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/service/merge_users_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1392 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/account/service/register_user_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2504 2024-04-15 14:09:15.000000 django-project-base-0.75.30/django_project_base/account/service/reset_password_email_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      216 2021-06-29 12:16:02.000000 django-project-base-0.75.30/django_project_base/account/settings.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/account/social_auth/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.30/django_project_base/account/social_auth/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1581 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/social_auth/providers.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2244 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/account/social_auth/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      226 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/account/urls.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      355 2023-07-18 11:29:41.000000 django-project-base-0.75.30/django_project_base/apps.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/auth/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.75.30/django_project_base/auth/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.75.30/django_project_base/auth/admin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      160 2023-07-18 11:29:44.000000 django-project-base-0.75.30/django_project_base/auth/apps.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/auth/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.75.30/django_project_base/auth/migrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      738 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/auth/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       74 2023-07-18 12:51:25.000000 django-project-base-0.75.30/django_project_base/auth/tests.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.75.30/django_project_base/auth/views.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/aws/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-26 14:22:46.000000 django-project-base-0.75.30/django_project_base/aws/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1769 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/aws/ses.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/base/
--rw-rw-r--   0 jure      (1000) jure      (1000)       48 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1815 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/auth_backends.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9026 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/event.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      304 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/base/exceptions.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2793 2024-02-15 14:26:52.000000 django-project-base-0.75.30/django_project_base/base/fields.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1731 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/middleware.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    12932 2024-02-15 08:50:47.000000 django-project-base-0.75.30/django_project_base/base/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3901 2024-02-20 16:52:39.000000 django-project-base-0.75.30/django_project_base/base/permissions.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1991 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/queryset_with_cache.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      494 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/base/signals.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/celery/
--rw-rw-r--   0 jure      (1000) jure      (1000)       85 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/celery/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      187 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/celery/apps.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/celery/background_tasks/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/celery/background_tasks/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1743 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/celery/background_tasks/base_task.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1721 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/celery/background_tasks/notification_tasks.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2533 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/celery/celery.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      327 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/celery/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      447 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/constants.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1336 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/country_holidays.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/licensing/
--rw-rw-r--   0 jure      (1000) jure      (1000)       98 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/licensing/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      190 2023-08-20 09:37:15.000000 django-project-base-0.75.30/django_project_base/licensing/apps.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4439 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/licensing/logic.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/licensing/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)     1767 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/licensing/migrations/0001_initial.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2065 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      550 2023-09-04 09:23:53.000000 django-project-base-0.75.30/django_project_base/licensing/migrations/0005_auto_20230901_0613.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:37:15.000000 django-project-base-0.75.30/django_project_base/licensing/migrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      940 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/licensing/models.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/licensing/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/licensing/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      944 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/licensing/rest/rest.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      243 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/licensing/rest/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      175 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/licensing/urls.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.027958 django-project-base-0.75.30/django_project_base/locale/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.027958 django-project-base-0.75.30/django_project_base/locale/en/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.047959 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/
--rw-r--r--   0 jure      (1000) jure      (1000)      380 2024-02-27 08:45:40.000000 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)    13342 2024-02-27 08:06:33.000000 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 jure      (1000) jure      (1000)       84 2024-02-27 08:45:40.000000 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     4562 2023-08-04 14:39:40.000000 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.027958 django-project-base-0.75.30/django_project_base/locale/sl/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.047959 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/
--rw-r--r--   0 jure      (1000) jure      (1000)     6828 2024-02-27 08:45:40.000000 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)    15563 2024-02-27 08:07:00.000000 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/django.po
--rw-r--r--   0 jure      (1000) jure      (1000)     3731 2024-02-27 08:45:40.000000 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     6150 2023-08-04 14:39:32.000000 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.047959 django-project-base-0.75.30/django_project_base/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/management/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.047959 django-project-base-0.75.30/django_project_base/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1791 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/management/commands/confirm_setting.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1659 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/management/commands/list_pending_settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:46:16.000000 django-project-base-0.75.30/django_project_base/models.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.051959 django-project-base-0.75.30/django_project_base/notifications/
--rw-rw-r--   0 jure      (1000) jure      (1000)      162 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/notifications/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      449 2021-09-30 06:36:03.000000 django-project-base-0.75.30/django_project_base/notifications/apps.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.051959 django-project-base-0.75.30/django_project_base/notifications/base/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/base/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.067959 django-project-base-0.75.30/django_project_base/notifications/base/channels/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    11421 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/channel.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.067959 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     4694 2024-02-26 08:15:05.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/aws_ses.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2832 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2676 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/nexmo_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2980 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/provider_integration.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    10301 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/t2.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2012 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/mail_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1321 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/sms_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/websocket_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1613 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/base/duplicate_notification_mixin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1411 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/enums.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    12558 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1581 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/phone_number_parser.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1407 2023-08-02 06:59:12.000000 django-project-base-0.75.30/django_project_base/notifications/base/queable_notification_mixin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5636 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/send_notification_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       59 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/constants.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5829 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/email_notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      975 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/notifications/maintenance_notification.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.067959 django-project-base-0.75.30/django_project_base/notifications/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/management/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.067959 django-project-base-0.75.30/django_project_base/notifications/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      900 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/management/commands/resend_notification.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.071959 django-project-base-0.75.30/django_project_base/notifications/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)     6404 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0001_initial.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1086 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      413 2023-09-04 09:23:53.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      393 2023-09-04 09:23:53.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      412 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2533 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1501 2023-09-20 12:31:19.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0005_merge_20230906_1213.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1458 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1056 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0007_auto_20231026_0555.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      448 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1410 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0009_auto_20231108_0658.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      412 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0010_djangoprojectbasenotification_extra_data.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)     9789 2024-05-04 07:03:08.000000 django-project-base-0.75.30/django_project_base/notifications/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1201 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/notifications/notification_queryset.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.183960 django-project-base-0.75.30/django_project_base/notifications/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3173 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/notifications/rest/delivery_report.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9090 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/notifications/rest/maintenance_notification.py
--rw-r--r--   0 jure      (1000) jure      (1000)    23288 2024-05-16 17:09:01.000000 django-project-base-0.75.30/django_project_base/notifications/rest/notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      934 2024-02-05 15:07:30.000000 django-project-base-0.75.30/django_project_base/notifications/rest/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      943 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/notifications/settings.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.183960 django-project-base-0.75.30/django_project_base/notifications/templates/
--rw-rw-r--   0 jure      (1000) jure      (1000)      368 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/templates/account_created.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     4339 2023-09-21 07:55:00.000000 django-project-base-0.75.30/django_project_base/notifications/templates/notification.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     2614 2023-09-21 07:55:00.000000 django-project-base-0.75.30/django_project_base/notifications/templates/notification_login.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.183960 django-project-base-0.75.30/django_project_base/notifications/tests/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/tests/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.187960 django-project-base-0.75.30/django_project_base/notifications/tests/api/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2427 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/test_create_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2196 2023-08-28 11:05:17.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/test_list_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      864 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/test_remainig_license.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1485 2023-08-28 11:05:17.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/test_retrieve_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3332 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/tests/notifications_transaction_test_case.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.187960 django-project-base-0.75.30/django_project_base/notifications/tests/unit/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/tests/unit/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2941 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/tests/unit/test_is_mail_sent.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      543 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      177 2023-08-02 05:31:11.000000 django-project-base-0.75.30/django_project_base/notifications/utils.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.187960 django-project-base-0.75.30/django_project_base/permissions/
--rw-rw-r--   0 jure      (1000) jure      (1000)     1082 2023-12-11 12:51:14.000000 django-project-base-0.75.30/django_project_base/permissions/__init__.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/profiling/
--rw-rw-r--   0 jure      (1000) jure      (1000)       89 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/profiling/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9791 2024-05-13 14:20:03.000000 django-project-base-0.75.30/django_project_base/profiling/middleware.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1040 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/profiling/performance_base_command.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3481 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/profiling/views.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-03-10 04:17:51.000000 django-project-base-0.75.30/django_project_base/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    18356 2024-05-07 10:45:40.000000 django-project-base-0.75.30/django_project_base/rest/project.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4000 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/rest/project_role.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4094 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4017 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1677 2023-11-17 14:51:19.000000 django-project-base-0.75.30/django_project_base/settings_parser.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.031958 django-project-base-0.75.30/django_project_base/static/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/static/browser-update/
--rw-rw-r--   0 jure      (1000) jure      (1000)      421 2023-07-14 12:32:29.000000 django-project-base-0.75.30/django_project_base/static/browser-update/browser-update.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     9484 2023-07-14 12:32:29.000000 django-project-base-0.75.30/django_project_base/static/browser-update/update.min.js
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.031958 django-project-base-0.75.30/django_project_base/templates/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/templates/app-debug/
--rw-rw-r--   0 jure      (1000) jure      (1000)     2169 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/templates/app-debug/main.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/templates/email/
--rw-rw-r--   0 jure      (1000) jure      (1000)      169 2023-06-20 12:45:01.000000 django-project-base-0.75.30/django_project_base/templates/email/base.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/templatetags/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2022-01-12 07:10:33.000000 django-project-base-0.75.30/django_project_base/templatetags/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      200 2022-01-12 07:10:33.000000 django-project-base-0.75.30/django_project_base/templatetags/dpb_tags.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      907 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/urls.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5824 2024-01-23 09:42:24.000000 django-project-base-0.75.30/django_project_base/utils.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      913 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/views.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.035958 django-project-base-0.75.30/django_project_base.egg-info/
--rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/PKG-INFO
--rw-r--r--   0 jure      (1000) jure      (1000)     9073 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/SOURCES.txt
--rw-r--r--   0 jure      (1000) jure      (1000)        1 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/dependency_links.txt
--rw-r--r--   0 jure      (1000) jure      (1000)      308 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/requires.txt
--rw-r--r--   0 jure      (1000) jure      (1000)       20 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/top_level.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)     1305 2023-12-14 13:42:26.000000 django-project-base-0.75.30/pyproject.toml
--rw-rw-r--   0 jure      (1000) jure      (1000)      311 2024-05-10 08:57:26.000000 django-project-base-0.75.30/requirements.txt
--rw-r--r--   0 jure      (1000) jure      (1000)       38 2024-05-21 06:04:06.191960 django-project-base-0.75.30/setup.cfg
--rwxrwxr-x   0 jure      (1000) jure      (1000)     3354 2023-10-17 07:56:43.000000 django-project-base-0.75.30/setup.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.745048 django-project-base-0.75.32/
+-rw-r--r--   0 jure      (1000) jure      (1000)      116 2024-05-28 06:15:49.000000 django-project-base-0.75.32/MANIFEST.in
+-rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-28 14:10:11.741048 django-project-base-0.75.32/PKG-INFO
+-rw-r--r--   0 jure      (1000) jure      (1000)     1006 2024-05-28 06:15:49.000000 django-project-base-0.75.32/README.md
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.429044 django-project-base-0.75.32/django_project_base/
+-rw-r--r--   0 jure      (1000) jure      (1000)      309 2024-05-28 14:09:55.000000 django-project-base-0.75.32/django_project_base/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/
+-rw-r--r--   0 jure      (1000) jure      (1000)      168 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      420 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/apps.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      182 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/constants.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/management/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.32/django_project_base/account/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/management/commands/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.32/django_project_base/account/management/commands/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1834 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/management/commands/allauth_to_social_core.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      664 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/management/commands/delete_users.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3602 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/middleware.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-08-05 09:26:32.000000 django-project-base-0.75.32/django_project_base/account/rest/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    13904 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/account.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5208 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/impersonate.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6815 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/invite.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5766 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/login.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    28708 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/profile.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6048 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/profile_merge.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    11582 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/project_profiles.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6639 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/project_profiles_utils.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6529 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/rest/reset_password.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2360 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/router.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/service/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/service/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5836 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/service/merge_users_service.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1392 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/service/register_user_service.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2504 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/service/reset_password_email_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      216 2021-06-29 12:16:02.000000 django-project-base-0.75.32/django_project_base/account/settings.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.433044 django-project-base-0.75.32/django_project_base/account/social_auth/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.32/django_project_base/account/social_auth/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1581 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/social_auth/providers.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2244 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/social_auth/settings.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      226 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/account/urls.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      355 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/auth/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)       77 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/admin.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      160 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/auth/migrations/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/migrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      738 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/models.py
+-rw-r--r--   0 jure      (1000) jure      (1000)       74 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/tests.py
+-rw-r--r--   0 jure      (1000) jure      (1000)       77 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/auth/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/aws/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/aws/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1769 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/aws/ses.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/base/
+-rw-r--r--   0 jure      (1000) jure      (1000)       48 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1815 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/auth_backends.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9026 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/event.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      304 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/exceptions.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2793 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/fields.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1731 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/middleware.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    12932 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/models.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3901 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/permissions.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1991 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/queryset_with_cache.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      494 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/base/signals.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/caching/
+-rw-r--r--   0 jure      (1000) jure      (1000)      980 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/caching/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/caching/cache_queue/
+-rw-r--r--   0 jure      (1000) jure      (1000)     2378 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/caching/cache_queue/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2084 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/caching/cache_queue/cache_queue_other.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      959 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/caching/cache_queue/cache_queue_redis.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/celery/
+-rw-r--r--   0 jure      (1000) jure      (1000)       85 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      187 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.437044 django-project-base-0.75.32/django_project_base/celery/background_tasks/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/background_tasks/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1743 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/background_tasks/base_task.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1721 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/background_tasks/notification_tasks.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2533 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/celery.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      327 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/celery/settings.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      447 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/constants.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1336 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/country_holidays.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/licensing/
+-rw-r--r--   0 jure      (1000) jure      (1000)       98 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      190 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/apps.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4439 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/logic.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/licensing/migrations/
+-rw-r--r--   0 jure      (1000) jure      (1000)     1767 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/migrations/0001_initial.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2065 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      550 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/migrations/0005_auto_20230901_0613.py
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/migrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      940 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/models.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/licensing/rest/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/rest/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      944 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/rest/rest.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      243 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/rest/router.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      175 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/licensing/urls.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.425044 django-project-base-0.75.32/django_project_base/locale/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.425044 django-project-base-0.75.32/django_project_base/locale/en/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jure      (1000) jure      (1000)      380 2024-02-27 08:45:40.000000 django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 jure      (1000) jure      (1000)    14046 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 jure      (1000) jure      (1000)     4562 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.425044 django-project-base-0.75.32/django_project_base/locale/sl/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 jure      (1000) jure      (1000)     6828 2024-02-27 08:45:40.000000 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jure      (1000) jure      (1000)    16384 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/django.po
+-rw-r--r--   0 jure      (1000) jure      (1000)     3731 2024-02-27 08:45:40.000000 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 jure      (1000) jure      (1000)     6150 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/management/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.441044 django-project-base-0.75.32/django_project_base/management/commands/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/management/commands/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1791 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/management/commands/confirm_setting.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1621 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/management/commands/list_pending_settings.py
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/models.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/
+-rw-r--r--   0 jure      (1000) jure      (1000)      162 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      449 2021-09-30 06:36:03.000000 django-project-base-0.75.32/django_project_base/notifications/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/base/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/base/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/base/channels/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    11421 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/channel.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4694 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/aws_ses.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2832 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2676 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/nexmo_sms.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2980 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/provider_integration.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    10301 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/t2.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2012 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/mail_channel.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1321 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/sms_channel.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/base/channels/websocket_channel.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1613 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/duplicate_notification_mixin.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1411 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/enums.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    12558 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1581 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/phone_number_parser.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1407 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/queable_notification_mixin.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5636 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/base/send_notification_service.py
+-rw-r--r--   0 jure      (1000) jure      (1000)       59 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/constants.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5829 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/email_notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      975 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/maintenance_notification.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/management/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.445044 django-project-base-0.75.32/django_project_base/notifications/management/commands/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/management/commands/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      900 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/management/commands/resend_notification.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/migrations/
+-rw-r--r--   0 jure      (1000) jure      (1000)     6404 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0001_initial.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1086 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      413 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      393 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options_and_more.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      412 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2533 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1501 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0005_merge_20230906_1213.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1458 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1056 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0007_auto_20231026_0555.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      448 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1410 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0009_auto_20231108_0658.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      412 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/0010_djangoprojectbasenotification_extra_data.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/migrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9789 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/models.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1201 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/notification_queryset.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/notifications/rest/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3136 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/rest/delivery_report.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9090 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/rest/maintenance_notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    23543 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/rest/notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      934 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/rest/router.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      943 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/settings.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/templates/
+-rw-r--r--   0 jure      (1000) jure      (1000)      368 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/templates/account_created.html
+-rw-r--r--   0 jure      (1000) jure      (1000)     4339 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/templates/notification.html
+-rw-r--r--   0 jure      (1000) jure      (1000)     2614 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/templates/notification_login.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/tests/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/tests/api/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2427 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/test_create_mail.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2196 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/test_list_mail.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      864 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/test_remainig_license.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1485 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/api/test_retrieve_mail.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3332 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/notifications_transaction_test_case.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.565045 django-project-base-0.75.32/django_project_base/notifications/tests/unit/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/unit/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     2941 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/unit/test_is_mail_sent.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      543 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      177 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/notifications/utils.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.569046 django-project-base-0.75.32/django_project_base/permissions/
+-rw-r--r--   0 jure      (1000) jure      (1000)     1082 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/permissions/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.569046 django-project-base-0.75.32/django_project_base/profiling/
+-rw-r--r--   0 jure      (1000) jure      (1000)       89 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/profiling/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9135 2024-05-28 14:09:12.000000 django-project-base-0.75.32/django_project_base/profiling/middleware.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1040 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/profiling/performance_base_command.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3754 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/profiling/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.569046 django-project-base-0.75.32/django_project_base/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-03-10 04:17:51.000000 django-project-base-0.75.32/django_project_base/rest/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    18501 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/rest/project.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4000 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/rest/project_role.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4094 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/router.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      705 2024-05-28 13:56:15.000000 django-project-base-0.75.32/django_project_base/serialization.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4017 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/settings.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1677 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/settings_parser.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.429044 django-project-base-0.75.32/django_project_base/static/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.569046 django-project-base-0.75.32/django_project_base/static/browser-update/
+-rw-r--r--   0 jure      (1000) jure      (1000)      421 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/static/browser-update/browser-update.js
+-rw-r--r--   0 jure      (1000) jure      (1000)     9484 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/static/browser-update/update.min.js
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.429044 django-project-base-0.75.32/django_project_base/templates/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.741048 django-project-base-0.75.32/django_project_base/templates/app-debug/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2169 2021-05-19 11:48:39.000000 django-project-base-0.75.32/django_project_base/templates/app-debug/main.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.741048 django-project-base-0.75.32/django_project_base/templates/email/
+-rw-r--r--   0 jure      (1000) jure      (1000)      169 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/templates/email/base.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.741048 django-project-base-0.75.32/django_project_base/templatetags/
+-rw-r--r--   0 jure      (1000) jure      (1000)        0 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/templatetags/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      200 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/templatetags/dpb_tags.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      907 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/urls.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5824 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/utils.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      913 2024-05-28 06:15:49.000000 django-project-base-0.75.32/django_project_base/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-28 14:10:11.429044 django-project-base-0.75.32/django_project_base.egg-info/
+-rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/PKG-INFO
+-rw-r--r--   0 jure      (1000) jure      (1000)     9270 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/SOURCES.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)        1 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/dependency_links.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)      308 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/requires.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)       20 2024-05-28 14:10:11.000000 django-project-base-0.75.32/django_project_base.egg-info/top_level.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)     1305 2024-05-28 06:15:49.000000 django-project-base-0.75.32/pyproject.toml
+-rw-r--r--   0 jure      (1000) jure      (1000)      311 2024-05-28 13:56:03.000000 django-project-base-0.75.32/requirements.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)       38 2024-05-28 14:10:11.745048 django-project-base-0.75.32/setup.cfg
+-rwxr-xr-x   0 jure      (1000) jure      (1000)     3354 2024-05-28 06:15:49.000000 django-project-base-0.75.32/setup.py
```

### Comparing `django-project-base-0.75.30/PKG-INFO` & `django-project-base-0.75.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-base
-Version: 0.75.30
+Version: 0.75.32
 Summary: Everything revolves around it: users, roles, permissions, tags, etc.
 Home-page: https://github.com/velis74/django-project-base
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-project-base-0.75.30/README.md` & `django-project-base-0.75.32/README.md`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/management/commands/allauth_to_social_core.py` & `django-project-base-0.75.32/django_project_base/account/management/commands/allauth_to_social_core.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/management/commands/delete_users.py` & `django-project-base-0.75.32/django_project_base/account/management/commands/delete_users.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/middleware.py` & `django-project-base-0.75.32/django_project_base/account/middleware.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/account.py` & `django-project-base-0.75.32/django_project_base/account/rest/account.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/impersonate.py` & `django-project-base-0.75.32/django_project_base/account/rest/impersonate.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/invite.py` & `django-project-base-0.75.32/django_project_base/account/rest/invite.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/login.py` & `django-project-base-0.75.32/django_project_base/account/rest/login.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/profile.py` & `django-project-base-0.75.32/django_project_base/account/rest/profile.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/profile_merge.py` & `django-project-base-0.75.32/django_project_base/account/rest/profile_merge.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/project_profiles.py` & `django-project-base-0.75.32/django_project_base/account/rest/project_profiles.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/project_profiles_utils.py` & `django-project-base-0.75.32/django_project_base/account/rest/project_profiles_utils.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/rest/reset_password.py` & `django-project-base-0.75.32/django_project_base/account/rest/reset_password.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/router.py` & `django-project-base-0.75.32/django_project_base/account/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/service/merge_users_service.py` & `django-project-base-0.75.32/django_project_base/account/service/merge_users_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/service/register_user_service.py` & `django-project-base-0.75.32/django_project_base/account/service/register_user_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/service/reset_password_email_service.py` & `django-project-base-0.75.32/django_project_base/account/service/reset_password_email_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/social_auth/providers.py` & `django-project-base-0.75.32/django_project_base/account/social_auth/providers.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/account/social_auth/settings.py` & `django-project-base-0.75.32/django_project_base/account/social_auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/auth/models.py` & `django-project-base-0.75.32/django_project_base/auth/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/aws/ses.py` & `django-project-base-0.75.32/django_project_base/aws/ses.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/base/auth_backends.py` & `django-project-base-0.75.32/django_project_base/base/auth_backends.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/base/event.py` & `django-project-base-0.75.32/django_project_base/base/event.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/base/fields.py` & `django-project-base-0.75.32/django_project_base/base/fields.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/base/middleware.py` & `django-project-base-0.75.32/django_project_base/base/middleware.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/base/models.py` & `django-project-base-0.75.32/django_project_base/base/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/base/permissions.py` & `django-project-base-0.75.32/django_project_base/base/permissions.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/base/queryset_with_cache.py` & `django-project-base-0.75.32/django_project_base/base/queryset_with_cache.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/celery/background_tasks/base_task.py` & `django-project-base-0.75.32/django_project_base/celery/background_tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/celery/background_tasks/notification_tasks.py` & `django-project-base-0.75.32/django_project_base/celery/background_tasks/notification_tasks.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/celery/celery.py` & `django-project-base-0.75.32/django_project_base/celery/celery.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/country_holidays.py` & `django-project-base-0.75.32/django_project_base/country_holidays.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/licensing/logic.py` & `django-project-base-0.75.32/django_project_base/licensing/logic.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/licensing/migrations/0001_initial.py` & `django-project-base-0.75.32/django_project_base/licensing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py` & `django-project-base-0.75.32/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/licensing/migrations/0005_auto_20230901_0613.py` & `django-project-base-0.75.32/django_project_base/licensing/migrations/0005_auto_20230901_0613.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/licensing/models.py` & `django-project-base-0.75.32/django_project_base/licensing/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/licensing/rest/rest.py` & `django-project-base-0.75.32/django_project_base/licensing/rest/rest.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/django.po` & `django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -4,225 +4,229 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-02-27 08:06+0000\n"
+"POT-Creation-Date: 2024-05-25 06:42+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: django_project_base/account/rest/account.py:118
+#: django_project_base/account/rest/account.py:131
 msgid "Change password"
 msgstr ""
 
-#: django_project_base/account/rest/account.py:122
+#: django_project_base/account/rest/account.py:135
 msgid "Current password"
 msgstr ""
 
-#: django_project_base/account/rest/account.py:123
+#: django_project_base/account/rest/account.py:136
 msgid "New password"
 msgstr ""
 
-#: django_project_base/account/rest/account.py:124
+#: django_project_base/account/rest/account.py:137
 msgid "Confirm new password"
 msgstr ""
 
-#: django_project_base/account/rest/account.py:222
+#: django_project_base/account/rest/account.py:240
 msgid "Code invalid"
 msgstr ""
 
-#: django_project_base/account/rest/account.py:239
-#: django_project_base/account/rest/account.py:243
+#: django_project_base/account/rest/account.py:257
+#: django_project_base/account/rest/account.py:261
 msgid "Email invalid"
 msgstr ""
 
-#: django_project_base/account/rest/account.py:318
+#: django_project_base/account/rest/account.py:336
 msgid "Add new user"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:33
+#: django_project_base/account/rest/impersonate.py:32
 msgid "User ID"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:34
+#: django_project_base/account/rest/impersonate.py:33
 msgid "User email"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:46
+#: django_project_base/account/rest/impersonate.py:45
 msgid "Select a user to impersonate"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:47
+#: django_project_base/account/rest/impersonate.py:46
 msgid "User"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:58
+#: django_project_base/account/rest/impersonate.py:57
 msgid "Impersonate a user"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:63
+#: django_project_base/account/rest/impersonate.py:62
 msgid "Cancel"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:64
+#: django_project_base/account/rest/impersonate.py:63
 msgid "Impersonate"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:88
+#: django_project_base/account/rest/impersonate.py:102
 msgid "Target user pk"
 msgstr ""
 
-#: django_project_base/account/rest/impersonate.py:112
+#: django_project_base/account/rest/impersonate.py:124
 msgid "Impersonating self is not allowed"
 msgstr ""
 
-#: django_project_base/account/rest/invite.py:42
+#: django_project_base/account/rest/invite.py:41
 msgid "Invitation text"
 msgstr ""
 
-#: django_project_base/account/rest/invite.py:44
+#: django_project_base/account/rest/invite.py:43
 msgid ""
 "Use %LINK% as a placeholder for invite link. If invite text is empty, value "
 "from settings will be used"
 msgstr ""
 
-#: django_project_base/account/rest/invite.py:52
+#: django_project_base/account/rest/invite.py:51
 msgid "Project invites"
 msgstr ""
 
-#: django_project_base/account/rest/invite.py:53
+#: django_project_base/account/rest/invite.py:52
 msgid "Inviting project member"
 msgstr ""
 
-#: django_project_base/account/rest/invite.py:58
-#: django_project_base/notifications/rest/notification.py:142
+#: django_project_base/account/rest/invite.py:57
+#: django_project_base/notifications/rest/notification.py:144
 msgid "Add"
 msgstr ""
 
-#: django_project_base/account/rest/invite.py:58
+#: django_project_base/account/rest/invite.py:57
 msgid "Add new record"
 msgstr ""
 
-#: django_project_base/account/rest/invite.py:131
+#: django_project_base/account/rest/invite.py:136
 msgid "You are invited to project"
 msgstr ""
 
 #: django_project_base/account/rest/login.py:21
 #: django_project_base/account/rest/login.py:24
 msgid "Login"
 msgstr ""
 
 #: django_project_base/account/rest/login.py:23
 msgid "Back to site"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:119
+#: django_project_base/account/rest/profile.py:120
 msgid "Full name"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:127
-#: django_project_base/account/rest/profile.py:129
+#: django_project_base/account/rest/profile.py:128
+#: django_project_base/account/rest/profile.py:130
 msgid "Specific permissions for this user"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:139
-#: django_project_base/account/rest/profile.py:145
+#: django_project_base/account/rest/profile.py:140
+#: django_project_base/account/rest/profile.py:146
 msgid ""
 "The groups this user belongs to. A user will get all permissions granted to "
 "each of their groups."
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:181
 #: django_project_base/account/rest/profile.py:182
+#: django_project_base/account/rest/profile.py:183
 #: django_project_base/account/rest/profile_merge.py:54
 #: django_project_base/account/rest/profile_merge.py:55
-#: django_project_base/account/rest/project_profiles.py:59
+#: django_project_base/account/rest/project_profiles.py:60
 msgid "Merge"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:192
 #: django_project_base/account/rest/profile.py:193
+#: django_project_base/account/rest/profile.py:194
 msgid "Export"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:236
+#: django_project_base/account/rest/profile.py:239
 msgid "Password"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:237
+#: django_project_base/account/rest/profile.py:240
 msgid "Repeat Password"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:258
+#: django_project_base/account/rest/profile.py:261
 msgid "Password is required"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:260
+#: django_project_base/account/rest/profile.py:263
 msgid "Passwords do not match"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:263
+#: django_project_base/account/rest/profile.py:266
 msgid "Email is required"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:501
+#: django_project_base/account/rest/profile.py:413
+msgid "User with this email already exists."
+msgstr ""
+
+#: django_project_base/account/rest/profile.py:521
 msgid "Code required"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:511
+#: django_project_base/account/rest/profile.py:531
 msgid "Invalid code"
 msgstr ""
 
-#: django_project_base/account/rest/profile.py:637
+#: django_project_base/account/rest/profile.py:649
 msgid "Your account was created for you"
 msgstr ""
 
 #: django_project_base/account/rest/profile_merge.py:47
 #: django_project_base/account/rest/profile_merge.py:48
 msgid "Remove"
 msgstr ""
 
 #: django_project_base/account/rest/profile_merge.py:61
 #: django_project_base/account/rest/profile_merge.py:62
 msgid "Clear all"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:53
+#: django_project_base/account/rest/project_profiles.py:54
 msgid "Reset password"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:174
+#: django_project_base/account/rest/project_profiles.py:175
 msgid "Export users"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:179
+#: django_project_base/account/rest/project_profiles.py:180
 msgid "Template"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:182
+#: django_project_base/account/rest/project_profiles.py:183
 msgid "CSV"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:183
+#: django_project_base/account/rest/project_profiles.py:184
 msgid "XLS"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:187
+#: django_project_base/account/rest/project_profiles.py:188
 msgid "Profile Fields"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:191
+#: django_project_base/account/rest/project_profiles.py:192
 msgid "Print Filter"
 msgstr ""
 
 #: django_project_base/account/rest/reset_password.py:81
 msgid "Invalidate password"
 msgstr ""
 
@@ -326,26 +330,26 @@
 msgstr ""
 
 #: django_project_base/base/models.py:243
 msgid "Custom"
 msgstr ""
 
 #: django_project_base/base/models.py:279
-#: django_project_base/rest/project.py:227
+#: django_project_base/rest/project.py:234
 msgid "Value"
 msgstr ""
 
 #: django_project_base/base/models.py:288
 msgid "Pending value"
 msgstr ""
 
 #: django_project_base/base/models.py:326
 #: django_project_base/notifications/models.py:25
 #: django_project_base/notifications/models.py:46
-#: django_project_base/notifications/models.py:250
+#: django_project_base/notifications/models.py:255
 msgid "Id"
 msgstr ""
 
 #: django_project_base/base/models.py:327
 msgid "eMail"
 msgstr ""
 
@@ -390,37 +394,33 @@
 msgid "Type"
 msgstr ""
 
 #: django_project_base/licensing/models.py:23
 msgid "Comment"
 msgstr ""
 
-#: django_project_base/management/commands/list_pending_settings.py:35
-msgid "Pending settings report"
-msgstr ""
-
 #: django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py:17
 msgid "Text for notification detail view. __LINK__ is url placeholder."
 msgstr ""
 
 #: django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py:18
 msgid "You received a notification. Clik link to view it: __LINK__"
 msgstr ""
 
 #: django_project_base/notifications/migrations/0007_auto_20231026_0555.py:17
 msgid "Send notification via EMail if user has no phone number"
 msgstr ""
 
 #: django_project_base/notifications/models.py:26
-#: django_project_base/notifications/rest/notification.py:178
+#: django_project_base/notifications/rest/notification.py:181
 msgid "Subject"
 msgstr ""
 
 #: django_project_base/notifications/models.py:27
-#: django_project_base/notifications/rest/notification.py:52
+#: django_project_base/notifications/rest/notification.py:53
 msgid "Body"
 msgstr ""
 
 #: django_project_base/notifications/models.py:28
 msgid "Footer"
 msgstr ""
 
@@ -456,66 +456,84 @@
 msgid "Delayed to"
 msgstr ""
 
 #: django_project_base/notifications/models.py:73
 msgid "Message"
 msgstr ""
 
-#: django_project_base/notifications/models.py:246
+#: django_project_base/notifications/models.py:251
 msgid "Delivered"
 msgstr ""
 
-#: django_project_base/notifications/models.py:247
+#: django_project_base/notifications/models.py:252
 msgid "Not Delivered"
 msgstr ""
 
-#: django_project_base/notifications/models.py:248
+#: django_project_base/notifications/models.py:253
 msgid "Pending delivery"
 msgstr ""
 
-#: django_project_base/notifications/models.py:259
+#: django_project_base/notifications/models.py:264
 msgid "Auxiliary notification"
 msgstr ""
 
-#: django_project_base/notifications/rest/delivery_report.py:34
-msgid "invalid"
-msgstr ""
-
 #: django_project_base/notifications/rest/maintenance_notification.py:36
 msgid ""
 "Time interval identifying at what time notification was acknowledged by user"
 msgstr ""
 
-#: django_project_base/notifications/rest/notification.py:125
-#: django_project_base/notifications/rest/notification.py:175
+#: django_project_base/notifications/rest/notification.py:109
+msgid "Messages"
+msgstr ""
+
+#: django_project_base/notifications/rest/notification.py:109
+#: django_project_base/notifications/rest/notification.py:454
+msgid "New message"
+msgstr ""
+
+#: django_project_base/notifications/rest/notification.py:127
+#: django_project_base/notifications/rest/notification.py:178
 msgid "Recipients"
 msgstr ""
 
-#: django_project_base/notifications/rest/notification.py:128
+#: django_project_base/notifications/rest/notification.py:130
 msgid "Delivery"
 msgstr ""
 
-#: django_project_base/notifications/rest/notification.py:143
+#: django_project_base/notifications/rest/notification.py:145
 msgid "Add new notification"
 msgstr ""
 
-#: django_project_base/notifications/rest/notification.py:149
-#: django_project_base/notifications/rest/notification.py:150
+#: django_project_base/notifications/rest/notification.py:151
+#: django_project_base/notifications/rest/notification.py:152
 msgid "View license"
 msgstr ""
 
-#: django_project_base/notifications/rest/notification.py:160
+#: django_project_base/notifications/rest/notification.py:156
+msgid "Edit"
+msgstr ""
+
+#: django_project_base/notifications/rest/notification.py:156
+msgid "Edit record"
+msgstr ""
+
+#: django_project_base/notifications/rest/notification.py:163
 msgid "Send"
 msgstr ""
 
-#: django_project_base/notifications/rest/notification.py:199
+#: django_project_base/notifications/rest/notification.py:185
+#: django_project_base/notifications/rest/notification.py:460
+msgid "Send on channels"
+msgstr ""
+
+#: django_project_base/notifications/rest/notification.py:203
 msgid "Send notification SMS"
 msgstr ""
 
-#: django_project_base/notifications/rest/notification.py:204
+#: django_project_base/notifications/rest/notification.py:208
 msgid "Sent"
 msgstr ""
 
 #: django_project_base/notifications/templates/account_created.html:5
 msgid ""
 "You have been invited to our application. Your credentials are listed below."
 msgstr ""
@@ -524,28 +542,40 @@
 msgid "Your username:"
 msgstr ""
 
 #: django_project_base/notifications/templates/account_created.html:11
 msgid "Have a nice day."
 msgstr ""
 
-#: django_project_base/rest/project.py:166
-#: django_project_base/rest/project.py:174
+#: django_project_base/rest/project.py:42
+msgid "Projects"
+msgstr ""
+
+#: django_project_base/rest/project.py:42
+msgid "New project"
+msgstr ""
+
+#: django_project_base/rest/project.py:42
+msgid "Edit project"
+msgstr ""
+
+#: django_project_base/rest/project.py:173
+#: django_project_base/rest/project.py:181
 msgid "Please enter value"
 msgstr ""
 
-#: django_project_base/rest/project.py:167
+#: django_project_base/rest/project.py:174
 msgid "Email sender value for notifications"
 msgstr ""
 
-#: django_project_base/rest/project.py:175
+#: django_project_base/rest/project.py:182
 msgid "Sms sender value for notifications"
 msgstr ""
 
-#: django_project_base/rest/project.py:389
+#: django_project_base/rest/project.py:396
 msgid "required"
 msgstr ""
 
 #: django_project_base/rest/project_role.py:32
 msgid "Project is required"
 msgstr ""
```

### Comparing `django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/djangojs.po` & `django-project-base-0.75.32/django_project_base/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/django.mo` & `django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/django.po` & `django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -4,228 +4,232 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-02-27 08:06+0000\n"
+"POT-Creation-Date: 2024-05-25 06:42+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
 
-#: django_project_base/account/rest/account.py:118
+#: django_project_base/account/rest/account.py:131
 msgid "Change password"
 msgstr "Spremeni geslo"
 
-#: django_project_base/account/rest/account.py:122
+#: django_project_base/account/rest/account.py:135
 msgid "Current password"
 msgstr "Trenutno geslo"
 
-#: django_project_base/account/rest/account.py:123
+#: django_project_base/account/rest/account.py:136
 msgid "New password"
 msgstr "Novo geslo"
 
-#: django_project_base/account/rest/account.py:124
+#: django_project_base/account/rest/account.py:137
 msgid "Confirm new password"
 msgstr "Potrdi novo geslo"
 
-#: django_project_base/account/rest/account.py:222
+#: django_project_base/account/rest/account.py:240
 msgid "Code invalid"
 msgstr "Napačna koda"
 
-#: django_project_base/account/rest/account.py:239
-#: django_project_base/account/rest/account.py:243
+#: django_project_base/account/rest/account.py:257
+#: django_project_base/account/rest/account.py:261
 msgid "Email invalid"
 msgstr "E-pošta ni pravilna"
 
-#: django_project_base/account/rest/account.py:318
+#: django_project_base/account/rest/account.py:336
 msgid "Add new user"
 msgstr "Dodaj novega uporabnika"
 
-#: django_project_base/account/rest/impersonate.py:33
+#: django_project_base/account/rest/impersonate.py:32
 msgid "User ID"
 msgstr "Uporabnikov ID"
 
-#: django_project_base/account/rest/impersonate.py:34
+#: django_project_base/account/rest/impersonate.py:33
 msgid "User email"
 msgstr "Uporabnikova e-pošta"
 
-#: django_project_base/account/rest/impersonate.py:46
+#: django_project_base/account/rest/impersonate.py:45
 msgid "Select a user to impersonate"
 msgstr "Izberi uporabnika za poosebljenje"
 
-#: django_project_base/account/rest/impersonate.py:47
+#: django_project_base/account/rest/impersonate.py:46
 msgid "User"
 msgstr "Uporabnik"
 
-#: django_project_base/account/rest/impersonate.py:58
+#: django_project_base/account/rest/impersonate.py:57
 msgid "Impersonate a user"
 msgstr "Poosebi uporabnika"
 
-#: django_project_base/account/rest/impersonate.py:63
+#: django_project_base/account/rest/impersonate.py:62
 msgid "Cancel"
 msgstr "Prekliči"
 
-#: django_project_base/account/rest/impersonate.py:64
+#: django_project_base/account/rest/impersonate.py:63
 msgid "Impersonate"
 msgstr "Poosebi"
 
-#: django_project_base/account/rest/impersonate.py:88
+#: django_project_base/account/rest/impersonate.py:102
 msgid "Target user pk"
 msgstr "ID uporabnika"
 
-#: django_project_base/account/rest/impersonate.py:112
+#: django_project_base/account/rest/impersonate.py:124
 msgid "Impersonating self is not allowed"
 msgstr "Ne moreš poosebljati samega sebe"
 
-#: django_project_base/account/rest/invite.py:42
+#: django_project_base/account/rest/invite.py:41
 msgid "Invitation text"
 msgstr "Tekst povabila"
 
-#: django_project_base/account/rest/invite.py:44
+#: django_project_base/account/rest/invite.py:43
 msgid ""
 "Use %LINK% as a placeholder for invite link. If invite text is empty, value "
 "from settings will be used"
 msgstr ""
 
-#: django_project_base/account/rest/invite.py:52
+#: django_project_base/account/rest/invite.py:51
 msgid "Project invites"
 msgstr "Povabila v projekt"
 
-#: django_project_base/account/rest/invite.py:53
+#: django_project_base/account/rest/invite.py:52
 msgid "Inviting project member"
 msgstr "Povabilo članu projekta"
 
-#: django_project_base/account/rest/invite.py:58
-#: django_project_base/notifications/rest/notification.py:142
+#: django_project_base/account/rest/invite.py:57
+#: django_project_base/notifications/rest/notification.py:144
 msgid "Add"
 msgstr "Dodaj"
 
-#: django_project_base/account/rest/invite.py:58
+#: django_project_base/account/rest/invite.py:57
 msgid "Add new record"
 msgstr "Dodaj nov zapis"
 
-#: django_project_base/account/rest/invite.py:131
+#: django_project_base/account/rest/invite.py:136
 msgid "You are invited to project"
 msgstr "Vabljeni ste v projekt"
 
 #: django_project_base/account/rest/login.py:21
 #: django_project_base/account/rest/login.py:24
 msgid "Login"
 msgstr "Prijava"
 
 #: django_project_base/account/rest/login.py:23
 msgid "Back to site"
 msgstr "Nazaj na aplikacijo"
 
-#: django_project_base/account/rest/profile.py:119
+#: django_project_base/account/rest/profile.py:120
 msgid "Full name"
 msgstr "Polno ime"
 
-#: django_project_base/account/rest/profile.py:127
-#: django_project_base/account/rest/profile.py:129
+#: django_project_base/account/rest/profile.py:128
+#: django_project_base/account/rest/profile.py:130
 msgid "Specific permissions for this user"
 msgstr "Pravice za tega uporabnika"
 
-#: django_project_base/account/rest/profile.py:139
-#: django_project_base/account/rest/profile.py:145
+#: django_project_base/account/rest/profile.py:140
+#: django_project_base/account/rest/profile.py:146
 msgid ""
 "The groups this user belongs to. A user will get all permissions granted to "
 "each of their groups."
 msgstr ""
 "Skupine, ki jim uprabnik pripada. Uporabnik bo imel vse pravice, dodeljene "
 "vsaki od svojih skupin"
 
-#: django_project_base/account/rest/profile.py:181
 #: django_project_base/account/rest/profile.py:182
+#: django_project_base/account/rest/profile.py:183
 #: django_project_base/account/rest/profile_merge.py:54
 #: django_project_base/account/rest/profile_merge.py:55
-#: django_project_base/account/rest/project_profiles.py:59
+#: django_project_base/account/rest/project_profiles.py:60
 msgid "Merge"
 msgstr "Združi"
 
-#: django_project_base/account/rest/profile.py:192
 #: django_project_base/account/rest/profile.py:193
+#: django_project_base/account/rest/profile.py:194
 msgid "Export"
 msgstr "Izvozi"
 
-#: django_project_base/account/rest/profile.py:236
+#: django_project_base/account/rest/profile.py:239
 msgid "Password"
 msgstr "Geslo"
 
-#: django_project_base/account/rest/profile.py:237
+#: django_project_base/account/rest/profile.py:240
 msgid "Repeat Password"
 msgstr "Ponovi geslo"
 
-#: django_project_base/account/rest/profile.py:258
+#: django_project_base/account/rest/profile.py:261
 msgid "Password is required"
 msgstr "Geslo je obvezno"
 
-#: django_project_base/account/rest/profile.py:260
+#: django_project_base/account/rest/profile.py:263
 msgid "Passwords do not match"
 msgstr "Gesli se ne ujemata"
 
-#: django_project_base/account/rest/profile.py:263
+#: django_project_base/account/rest/profile.py:266
 msgid "Email is required"
 msgstr "E-pošta je obvezen podatek"
 
-#: django_project_base/account/rest/profile.py:501
+#: django_project_base/account/rest/profile.py:413
+msgid "User with this email already exists."
+msgstr ""
+
+#: django_project_base/account/rest/profile.py:521
 msgid "Code required"
 msgstr "Koda je obvezna"
 
-#: django_project_base/account/rest/profile.py:511
+#: django_project_base/account/rest/profile.py:531
 msgid "Invalid code"
 msgstr "Napačna koda"
 
-#: django_project_base/account/rest/profile.py:637
+#: django_project_base/account/rest/profile.py:649
 msgid "Your account was created for you"
 msgstr "Zate je bil ustvarjen račun"
 
 #: django_project_base/account/rest/profile_merge.py:47
 #: django_project_base/account/rest/profile_merge.py:48
 msgid "Remove"
 msgstr "Odstrani"
 
 #: django_project_base/account/rest/profile_merge.py:61
 #: django_project_base/account/rest/profile_merge.py:62
 msgid "Clear all"
 msgstr "Zbriši vse"
 
-#: django_project_base/account/rest/project_profiles.py:53
+#: django_project_base/account/rest/project_profiles.py:54
 msgid "Reset password"
 msgstr "Ponastavi geslo"
 
-#: django_project_base/account/rest/project_profiles.py:174
+#: django_project_base/account/rest/project_profiles.py:175
 msgid "Export users"
 msgstr "Izvozi uporabnike"
 
-#: django_project_base/account/rest/project_profiles.py:179
+#: django_project_base/account/rest/project_profiles.py:180
 msgid "Template"
 msgstr "Predloga"
 
-#: django_project_base/account/rest/project_profiles.py:182
+#: django_project_base/account/rest/project_profiles.py:183
 msgid "CSV"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:183
+#: django_project_base/account/rest/project_profiles.py:184
 msgid "XLS"
 msgstr ""
 
-#: django_project_base/account/rest/project_profiles.py:187
+#: django_project_base/account/rest/project_profiles.py:188
 msgid "Profile Fields"
 msgstr "Polja iz uporabniškega profila"
 
-#: django_project_base/account/rest/project_profiles.py:191
+#: django_project_base/account/rest/project_profiles.py:192
 msgid "Print Filter"
 msgstr "Omejitev izbora"
 
 #: django_project_base/account/rest/reset_password.py:81
 msgid "Invalidate password"
 msgstr "Razveljavi geslo"
 
@@ -243,15 +247,15 @@
 
 #: django_project_base/base/models.py:24 django_project_base/base/models.py:277
 msgid "Name"
 msgstr "Ime"
 
 #: django_project_base/base/models.py:25
 msgid "Slug"
-msgstr "oznaka"
+msgstr "Oznaka"
 
 #: django_project_base/base/models.py:26 django_project_base/base/models.py:278
 msgid "Description"
 msgstr "Opis"
 
 #: django_project_base/base/models.py:27
 msgid "Logo"
@@ -306,15 +310,15 @@
 msgctxt "A tag name"
 msgid "name"
 msgstr "ime"
 
 #: django_project_base/base/models.py:158
 msgctxt "A tag slug"
 msgid "slug"
-msgstr ""
+msgstr "oznaka"
 
 #: django_project_base/base/models.py:239
 msgid "Whole number"
 msgstr "Celo število"
 
 #: django_project_base/base/models.py:240
 msgid "Decimal number"
@@ -329,32 +333,32 @@
 msgstr "Tekst"
 
 #: django_project_base/base/models.py:243
 msgid "Custom"
 msgstr "Po meri"
 
 #: django_project_base/base/models.py:279
-#: django_project_base/rest/project.py:227
+#: django_project_base/rest/project.py:234
 msgid "Value"
 msgstr "Vrednost"
 
 #: django_project_base/base/models.py:288
 msgid "Pending value"
 msgstr "Predlagana sprememba"
 
 #: django_project_base/base/models.py:326
 #: django_project_base/notifications/models.py:25
 #: django_project_base/notifications/models.py:46
-#: django_project_base/notifications/models.py:250
+#: django_project_base/notifications/models.py:255
 msgid "Id"
 msgstr "Id"
 
 #: django_project_base/base/models.py:327
 msgid "eMail"
-msgstr ""
+msgstr "ePošta"
 
 #: django_project_base/base/models.py:333
 msgid "Invitation message"
 msgstr "Sporočilo povabila"
 
 #: django_project_base/country_holidays.py:20
 msgid "Not valid country alpha 2 code"
@@ -393,37 +397,33 @@
 msgid "Type"
 msgstr "Tip"
 
 #: django_project_base/licensing/models.py:23
 msgid "Comment"
 msgstr "Opomba"
 
-#: django_project_base/management/commands/list_pending_settings.py:35
-msgid "Pending settings report"
-msgstr ""
-
 #: django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py:17
 msgid "Text for notification detail view. __LINK__ is url placeholder."
 msgstr ""
 
 #: django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py:18
 msgid "You received a notification. Clik link to view it: __LINK__"
 msgstr "Vaš klub vam je poslal obvestilo. Kliknite povezavo za ogled: __LINK__"
 
 #: django_project_base/notifications/migrations/0007_auto_20231026_0555.py:17
 msgid "Send notification via EMail if user has no phone number"
 msgstr "Pošlji obvestilo po emailu, če uporabnik nima telefonske številke"
 
 #: django_project_base/notifications/models.py:26
-#: django_project_base/notifications/rest/notification.py:178
+#: django_project_base/notifications/rest/notification.py:181
 msgid "Subject"
 msgstr "Zadeva"
 
 #: django_project_base/notifications/models.py:27
-#: django_project_base/notifications/rest/notification.py:52
+#: django_project_base/notifications/rest/notification.py:53
 msgid "Body"
 msgstr "Telo"
 
 #: django_project_base/notifications/models.py:28
 msgid "Footer"
 msgstr "Opomba"
 
@@ -459,66 +459,84 @@
 msgid "Delayed to"
 msgstr "Odloženo do"
 
 #: django_project_base/notifications/models.py:73
 msgid "Message"
 msgstr "Sporočilo"
 
-#: django_project_base/notifications/models.py:246
+#: django_project_base/notifications/models.py:251
 msgid "Delivered"
 msgstr "Dostavljeno"
 
-#: django_project_base/notifications/models.py:247
+#: django_project_base/notifications/models.py:252
 msgid "Not Delivered"
 msgstr "Ni dostavljeno"
 
-#: django_project_base/notifications/models.py:248
+#: django_project_base/notifications/models.py:253
 msgid "Pending delivery"
 msgstr "V dostavi"
 
-#: django_project_base/notifications/models.py:259
+#: django_project_base/notifications/models.py:264
 msgid "Auxiliary notification"
 msgstr "Pomožno obvestilo"
 
-#: django_project_base/notifications/rest/delivery_report.py:34
-msgid "invalid"
-msgstr ""
-
 #: django_project_base/notifications/rest/maintenance_notification.py:36
 msgid ""
 "Time interval identifying at what time notification was acknowledged by user"
 msgstr "Časovni interval, v katerem je uporabnik potrdil prejem obvestila"
 
-#: django_project_base/notifications/rest/notification.py:125
-#: django_project_base/notifications/rest/notification.py:175
+#: django_project_base/notifications/rest/notification.py:109
+msgid "Messages"
+msgstr "Sporočila"
+
+#: django_project_base/notifications/rest/notification.py:109
+#: django_project_base/notifications/rest/notification.py:454
+msgid "New message"
+msgstr "Novo sporočilo"
+
+#: django_project_base/notifications/rest/notification.py:127
+#: django_project_base/notifications/rest/notification.py:178
 msgid "Recipients"
 msgstr "Prejemniki"
 
-#: django_project_base/notifications/rest/notification.py:128
+#: django_project_base/notifications/rest/notification.py:130
 msgid "Delivery"
 msgstr "Dostavljeno"
 
-#: django_project_base/notifications/rest/notification.py:143
+#: django_project_base/notifications/rest/notification.py:145
 msgid "Add new notification"
 msgstr "Novo obvestilo"
 
-#: django_project_base/notifications/rest/notification.py:149
-#: django_project_base/notifications/rest/notification.py:150
+#: django_project_base/notifications/rest/notification.py:151
+#: django_project_base/notifications/rest/notification.py:152
 msgid "View license"
 msgstr "Poglej dobroimetje"
 
-#: django_project_base/notifications/rest/notification.py:160
+#: django_project_base/notifications/rest/notification.py:156
+msgid "Edit"
+msgstr "Uredi"
+
+#: django_project_base/notifications/rest/notification.py:156
+msgid "Edit record"
+msgstr "Uredi zapis"
+
+#: django_project_base/notifications/rest/notification.py:163
 msgid "Send"
 msgstr "Pošlji"
 
-#: django_project_base/notifications/rest/notification.py:199
+#: django_project_base/notifications/rest/notification.py:185
+#: django_project_base/notifications/rest/notification.py:460
+msgid "Send on channels"
+msgstr "Pošlji preko kanalov"
+
+#: django_project_base/notifications/rest/notification.py:203
 msgid "Send notification SMS"
 msgstr "Pošlji SMS obvestilo"
 
-#: django_project_base/notifications/rest/notification.py:204
+#: django_project_base/notifications/rest/notification.py:208
 msgid "Sent"
 msgstr "Poslano"
 
 #: django_project_base/notifications/templates/account_created.html:5
 msgid ""
 "You have been invited to our application. Your credentials are listed below."
 msgstr "Povabljen si v našo aplikacijo. Tvoje poverilnice so navedene spodaj."
@@ -527,43 +545,49 @@
 msgid "Your username:"
 msgstr "Tvoje uporabniško ime:"
 
 #: django_project_base/notifications/templates/account_created.html:11
 msgid "Have a nice day."
 msgstr "Lep dan vam želimo."
 
-#: django_project_base/rest/project.py:166
-#: django_project_base/rest/project.py:174
+#: django_project_base/rest/project.py:42
+msgid "Projects"
+msgstr "Projekti"
+
+#: django_project_base/rest/project.py:42
+msgid "New project"
+msgstr "Nov projekt"
+
+#: django_project_base/rest/project.py:42
+msgid "Edit project"
+msgstr "Uredi projekt"
+
+#: django_project_base/rest/project.py:173
+#: django_project_base/rest/project.py:181
 msgid "Please enter value"
 msgstr "Vnesi vrednost"
 
-#: django_project_base/rest/project.py:167
+#: django_project_base/rest/project.py:174
 msgid "Email sender value for notifications"
-msgstr ""
+msgstr "Nastavitev pošiljatelja ePošte za obvestila"
 
-#: django_project_base/rest/project.py:175
+#: django_project_base/rest/project.py:182
 msgid "Sms sender value for notifications"
-msgstr ""
+msgstr "Nastavitev pošiljatelja SMS za obvestila"
 
-#: django_project_base/rest/project.py:389
+#: django_project_base/rest/project.py:396
 msgid "required"
 msgstr "E-pošta je obvezen podatek"
 
 #: django_project_base/rest/project_role.py:32
 msgid "Project is required"
 msgstr "Projekt je obvezen podatek"
 
 #: example/demo_django_base/migrations/0008_projectinvite.py:23
 msgid ""
 "Text for invite notification view. __LINK__ is url to invite confirmation "
 "placeholder."
-msgstr ""
+msgstr "Tekst za povabilo k pridružitvi. Dodaj __LINK__ za url za potrditev."
 
 #: example/demo_django_base/migrations/0008_projectinvite.py:25
 msgid "Click link to join project: __LINK__"
-msgstr ""
-
-#~ msgid "On first login you will be prompted to change your password."
-#~ msgstr "Pri prvi prijavi bo sistem zahteval spremembo gesla"
-
-#~ msgid "Your password:"
-#~ msgstr "Tvoje geslo:"
+msgstr "Klikni povezavo, da se pridružiš: __LINK__"
```

### Comparing `django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo` & `django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/djangojs.po` & `django-project-base-0.75.32/django_project_base/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/management/commands/confirm_setting.py` & `django-project-base-0.75.32/django_project_base/management/commands/confirm_setting.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/management/commands/list_pending_settings.py` & `django-project-base-0.75.32/django_project_base/management/commands/list_pending_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import json
 
-from gettext import gettext
-
 import swapper
 
 from django.conf import settings
 from django.core.management.base import BaseCommand
 
 from django_project_base.notifications.email_notification import SystemEMailNotificationWithListOfEmails
 from django_project_base.notifications.models import DjangoProjectBaseMessage
@@ -28,15 +26,15 @@
                     "value": setting.python_value,
                     "pending_value": setting.python_pending_value,
                 }
 
         if to := getattr(settings, "ADMINS", getattr(settings, "MANAGERS", [])) and result:
             SystemEMailNotificationWithListOfEmails(
                 message=DjangoProjectBaseMessage(
-                    subject=gettext("Pending settings report"),
+                    subject="Pending settings report",
                     body=json.dumps(result),
                     footer="",
                     content_type=DjangoProjectBaseMessage.HTML,
                 ),
                 recipients=to,
             ).send()
```

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/channels/channel.py` & `django-project-base-0.75.32/django_project_base/notifications/base/channels/channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/aws_ses.py` & `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/aws_ses.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py` & `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/nexmo_sms.py` & `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/nexmo_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/provider_integration.py` & `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/provider_integration.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/t2.py` & `django-project-base-0.75.32/django_project_base/notifications/base/channels/integrations/t2.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/channels/mail_channel.py` & `django-project-base-0.75.32/django_project_base/notifications/base/channels/mail_channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/channels/sms_channel.py` & `django-project-base-0.75.32/django_project_base/notifications/base/channels/sms_channel.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/duplicate_notification_mixin.py` & `django-project-base-0.75.32/django_project_base/notifications/base/duplicate_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/enums.py` & `django-project-base-0.75.32/django_project_base/notifications/base/enums.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/notification.py` & `django-project-base-0.75.32/django_project_base/notifications/base/notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/phone_number_parser.py` & `django-project-base-0.75.32/django_project_base/notifications/base/phone_number_parser.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/queable_notification_mixin.py` & `django-project-base-0.75.32/django_project_base/notifications/base/queable_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/base/send_notification_service.py` & `django-project-base-0.75.32/django_project_base/notifications/base/send_notification_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/email_notification.py` & `django-project-base-0.75.32/django_project_base/notifications/email_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/maintenance_notification.py` & `django-project-base-0.75.32/django_project_base/notifications/maintenance_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/management/commands/resend_notification.py` & `django-project-base-0.75.32/django_project_base/notifications/management/commands/resend_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/migrations/0001_initial.py` & `django-project-base-0.75.32/django_project_base/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py` & `django-project-base-0.75.32/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py` & `django-project-base-0.75.32/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/migrations/0005_merge_20230906_1213.py` & `django-project-base-0.75.32/django_project_base/notifications/migrations/0005_merge_20230906_1213.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py` & `django-project-base-0.75.32/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/migrations/0007_auto_20231026_0555.py` & `django-project-base-0.75.32/django_project_base/notifications/migrations/0007_auto_20231026_0555.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/migrations/0009_auto_20231108_0658.py` & `django-project-base-0.75.32/django_project_base/notifications/migrations/0009_auto_20231108_0658.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/models.py` & `django-project-base-0.75.32/django_project_base/notifications/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/notification_queryset.py` & `django-project-base-0.75.32/django_project_base/notifications/notification_queryset.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/rest/delivery_report.py` & `django-project-base-0.75.32/django_project_base/notifications/rest/delivery_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import logging
 import uuid
 
-from gettext import gettext
 from typing import Optional
 
 from django.utils.module_loading import import_string
 from rest_framework import viewsets
 from rest_framework.authentication import BasicAuthentication, TokenAuthentication
 from rest_framework.exceptions import ErrorDetail, ValidationError
 from rest_framework.permissions import IsAuthenticated, SAFE_METHODS
@@ -27,15 +26,15 @@
     def __find_dlr_id(self, params: dict) -> Optional[str]:
         id = next(filter(lambda i: i.lower() in self._primary_key_names, params.keys()), None)
         if id and params.get(id):
             uid = str(params[id])
             try:
                 uuid.UUID(uid)
             except ValueError:
-                raise ValidationError(ErrorDetail(string="Invalid identifier", code=gettext("invalid")))
+                raise ValidationError(ErrorDetail(string="Invalid identifier", code="invalid"))
             return uid
         logger = logging.getLogger("django")
         logger.exception(
             f"Id not found for delivery report {self.request.query_params} {self.request.data} {self.request.user}"
         )
         return None
```

### Comparing `django-project-base-0.75.30/django_project_base/notifications/rest/maintenance_notification.py` & `django-project-base-0.75.32/django_project_base/notifications/rest/maintenance_notification.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/rest/notification.py` & `django-project-base-0.75.32/django_project_base/notifications/rest/notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,17 @@
                         str,
                         MessageToListField().parse(val=json.loads(value), return_instances=True),
                     )
                 )
             )
             if (
                 self.parent
-                and self.parent.instance  # noqa: W503
-                and not isinstance(self.parent.instance, QuerySet)  # noqa: W503
-                and not self.parent.instance.recipients_original_payload_search  # noqa: W503
+                and self.parent.instance
+                and not isinstance(self.parent.instance, QuerySet)
+                and not self.parent.instance.recipients_original_payload_search
             ):
                 self.parent.instance.recipients_original_payload_search = search_str
                 self.parent.instance.save(update_fields=["recipients_original_payload_search"])
             # TODO: THIS SOLUTION FOR SEARCH IS BAD; BAD; -> MAKE BETTER ONE
             if row_data and not row_data.recipients_original_payload_search:
                 row_data.recipients_original_payload_search = search_str
                 row_data.save(update_fields=["recipients_original_payload_search"])
@@ -102,14 +102,15 @@
         if value:
             return datetime.datetime.fromtimestamp(value).astimezone(pytz.utc)
         return value
 
 
 class NotificationSerializer(ModelSerializer):
     template_context = dict(url_reverse="notification")
+    form_titles = {"table": _("Messages"), "edit": _("New message")}
 
     def __init__(self, *args, is_filter: bool = False, **kwds):
         super().__init__(*args, is_filter=is_filter, **kwds)
         self.fields.fields["level"].display_form = DisplayMode.HIDDEN
         self.fields.fields["type"].display_form = DisplayMode.HIDDEN
         self.fields.fields["project_slug"].display = DisplayMode.HIDDEN
         self.fields.fields["message_to"].child_relation.queryset = SearchItems.objects.get_queryset(
@@ -177,14 +178,15 @@
         label=_("Recipients"),
     )
 
     message_subject = fields.CharField(write_only=True, label=_("Subject"), display_table=DisplayMode.HIDDEN)
     message_body = MessageBodyField()
 
     send_on_channels = fields.MultipleChoiceField(
+        label=_("Send on channels"),
         allow_empty=False,
         display_table=DisplayMode.SUPPRESS,
         display_form=DisplayMode.FULL,
         choices=[(c.name, c.name) for c in ChannelIdentifier.supported_channels()],
         write_only=True,
     )
 
@@ -360,14 +362,15 @@
 class NotificationViewset(ModelViewSet):
     authentication_classes = [
         SessionAuthentication,
         BasicAuthentication,
         TokenAuthentication,
     ]
     permission_classes = [IsAuthenticated]
+    pagination_class = ModelViewSet.generate_paged_loader(ordering=["-created_at"])
 
     def get_permissions(self):
         if self.action in ("notification_login", "notification_view"):
             return []
         else:
             return super().get_permissions()
 
@@ -444,18 +447,21 @@
             return queryset.filter(**{"recipients_original_payload_search__icontains": value})
         return super().filter_queryset_field(queryset, field, value)
 
     def get_serializer_class(self):
         if self.action in ("create", "update"):
 
             class NewMessageSerializer(Serializer):
+                form_titles = {"edit": _("New message")}
+
                 message_body = NotificationSerializer().fields.fields["message_body"]
                 message_subject = NotificationSerializer().fields.fields["message_subject"]
                 message_to = MessageToListField(allow_null=False, allow_empty=False)
                 send_on_channels = fields.ListField(
+                    label=_("Send on channels"),
                     child=fields.CharField(),
                     required=True,
                     display_table=DisplayMode.SUPPRESS,
                     display_form=DisplayMode.SUPPRESS,
                 )
                 send_notification_sms = fields.BooleanField(default=False, allow_null=False)
```

### Comparing `django-project-base-0.75.30/django_project_base/notifications/rest/router.py` & `django-project-base-0.75.32/django_project_base/notifications/rest/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/settings.py` & `django-project-base-0.75.32/django_project_base/notifications/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/templates/notification.html` & `django-project-base-0.75.32/django_project_base/notifications/templates/notification.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/templates/notification_login.html` & `django-project-base-0.75.32/django_project_base/notifications/templates/notification_login.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/tests/api/test_create_mail.py` & `django-project-base-0.75.32/django_project_base/notifications/tests/api/test_create_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/tests/api/test_list_mail.py` & `django-project-base-0.75.32/django_project_base/notifications/tests/api/test_list_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/tests/api/test_remainig_license.py` & `django-project-base-0.75.32/django_project_base/notifications/tests/api/test_remainig_license.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/tests/api/test_retrieve_mail.py` & `django-project-base-0.75.32/django_project_base/notifications/tests/api/test_retrieve_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/tests/notifications_transaction_test_case.py` & `django-project-base-0.75.32/django_project_base/notifications/tests/notifications_transaction_test_case.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/tests/unit/test_is_mail_sent.py` & `django-project-base-0.75.32/django_project_base/notifications/tests/unit/test_is_mail_sent.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py` & `django-project-base-0.75.32/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/permissions/__init__.py` & `django-project-base-0.75.32/django_project_base/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/profiling/middleware.py` & `django-project-base-0.75.32/django_project_base/profiling/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,42 +9,25 @@
 
 from typing import Optional
 
 from django.conf import settings
 from django.core.cache import cache
 from django.db import connections
 
+from django_project_base.caching import CacheCounter
+from django_project_base.caching.cache_queue import CacheQueue
+
 DEFAULT_MAX_LOG_FILE_SIZE = 10000000
 MAX_DATA_LOGGING_FILE_SIZE = 3000000
 
 MATCH_DETAIL_QUERIES = re.compile(
     r"(rest/\w+)/((?:[0-9a-f]{8}(?:-[0-9a-f]{4}){3}-[0-9a-f]{12})|" r"(?:(?:[0-9a-f]{2}:){5}[0-9a-f]{2})|\d+)(/.*)?"
 )
 
 
-class CacheLock(object):
-    def __init__(self, name):
-        self.name = "CacheLock." + name
-
-    def __enter__(self):
-        while True:
-            cache.add(self.name, 0)
-            try:
-                res = cache.incr(self.name, 1)
-            except ValueError:
-                # This happens if another thread just deleted the cache entry after our .add and before our .incr
-                res = 0
-            if res == 1:
-                break
-            time.sleep(0.1)
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        cache.delete(self.name)
-
-
 class ProfileRequest(object):
     response: object
     _start_time: tuple
     _end_time: tuple
     _process_function: callable
     _process_function_args: tuple
     _process_function_kwargs: dict
@@ -144,24 +127,24 @@
                                 "duration": duration[0],
                                 "queries": queries,
                                 "PATH_INFO": path_info,
                             }
                             r_data.update(
                                 {i: str(self._settings[i]) for i in ("HTTP_HOST", "REQUEST_METHOD", "QUERY_STRING")}
                             )
-                            with CacheLock("long_running_cmds"):
-                                cache_ptr = (cache.get("long_running_cmds_pointer", -1) + 1) % 50
-                                cache.set("long_running_cmds_pointer", cache_ptr, timeout=86400)
+                            cache_ptr = CacheCounter("long_running_cmds_pointer", timeout=86400).incr(start=-1) % 50
+
                             cache.set("long_running_cmds_data%d" % cache_ptr, r_data, timeout=86400)
-                        with CacheLock("last_hour_running_cmds"):
-                            r_data = (path_info, duration[0], duration[1], duration[2])
-                            # get cache entries in the last 10 seconds
-                            cache_ptr = cache.get("last_hour_running_cmds%d" % (int(time.time()) // 10), [])
-                            cache_ptr.append(r_data)
-                            cache.set("last_hour_running_cmds%d" % (int(time.time()) // 10), cache_ptr, timeout=3600)
+
+                        r_data = [path_info, duration[0], duration[1], duration[2]]
+                        last_hour_running_cmds_key = f"last_hour_running_cmds{int(time.time()) // 10}"
+                        last_hour_running_cmds_queue = CacheQueue.get_cache_queue(
+                            last_hour_running_cmds_key, timeout=3600
+                        )
+                        last_hour_running_cmds_queue.rpush(json.dumps(r_data))
 
                     req_data = dict(
                         code=getattr(response, "status_code", None),
                         method=self._settings["REQUEST_METHOD"],
                         duration=duration[0],
                         timestamp=end_time[0] / 1000,
                         path_info=path_info,
```

### Comparing `django-project-base-0.75.30/django_project_base/profiling/performance_base_command.py` & `django-project-base-0.75.32/django_project_base/profiling/performance_base_command.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/profiling/views.py` & `django-project-base-0.75.32/django_project_base/profiling/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import json
 import random
 
 from datetime import datetime
 
 from django.core.cache import cache
 from django.shortcuts import render
 from dynamicforms.struct import Struct
 
+from django_project_base.caching.cache_queue import CacheQueue
 from django_project_base.settings import PROFILER_LOG_LONG_REQUESTS_COUNT
 
 
 def app_debug_view(request):
     # if not getattr(request, 'user', None) or request.user.pk not in POWER_USERS:
     if not getattr(request, "user", None):
         raise PermissionError
@@ -64,16 +66,19 @@
         result_data.append(item)
 
     result_data.sort(key=lambda f: f.get("r_data", {}).get("duration", 0) or 0, reverse=True)
     spenders = list(sorted(totals.values(), key=lambda x: x.time, reverse=True))
 
     totals = {}
     for interval in range(int((time.time()) - 3600) // 10, int(time.time()) // 10 + 1):
-        cache_ptr = cache.get("last_hour_running_cmds%d" % interval, [])
-        for item in cache_ptr:
+        last_hour_running_cmds_key = f"last_hour_running_cmds{interval}"
+        last_hour_running_cmds_queue = CacheQueue.get_cache_queue(last_hour_running_cmds_key, timeout=3600)
+
+        cache_ptr = last_hour_running_cmds_queue.lrange()
+        for item in [json.loads(item) for item in cache_ptr]:
             totals.setdefault(item[0], Struct(count=0, wall_time=0, path="", user_time=0, sys_time=0, cpu_time=0))
             total = totals[item[0]]
             total.count += 1
             total.wall_time += item[1]
             total.user_time += item[2]
             total.sys_time += item[3]
             total.cpu_time += item[2] + item[3]
```

### Comparing `django-project-base-0.75.30/django_project_base/rest/project.py` & `django-project-base-0.75.32/django_project_base/rest/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import swapper
 
 from django.conf import settings
 from django.core.management import call_command
 from django.db import transaction
 from django.http import Http404
 from django.shortcuts import get_object_or_404
+from django.utils.translation import gettext as _
 from drf_spectacular.utils import extend_schema, OpenApiResponse
 from dynamicforms import fields
 from dynamicforms.action import TableAction, TablePosition
 from dynamicforms.mixins import DisplayMode
 from dynamicforms.serializers import ModelSerializer
 from dynamicforms.template_render.layout import Column, Layout, Row
 from dynamicforms.viewsets import ModelViewSet
@@ -34,14 +35,15 @@
 from django_project_base.base.permissions import CreateAny, IsProjectOwnerOrReadOnly
 from django_project_base.constants import EMAIL_SENDER_ID_SETTING_NAME, SMS_SENDER_ID_SETTING_NAME
 from django_project_base.utils import get_pk_name
 
 
 class ProjectSerializer(ModelSerializer):
     template_context = dict(url_reverse="project-base-project")
+    form_titles = {"table": _("Projects"), "new": _("New project"), "edit": _("Edit project")}
 
     def __init__(self, *args, is_filter: bool = False, **kwds):
         super().__init__(*args, is_filter=is_filter, **kwds)
 
         if self.context.get("view") and self.context["view"].format_kwarg == "componentdef":
             self.fields.fields["owner"].display_table = DisplayMode.SUPPRESS
             if self.context["view"].detail and self.instance.pk is None:
```

### Comparing `django-project-base-0.75.30/django_project_base/rest/project_role.py` & `django-project-base-0.75.32/django_project_base/rest/project_role.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/router.py` & `django-project-base-0.75.32/django_project_base/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/settings.py` & `django-project-base-0.75.32/django_project_base/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/settings_parser.py` & `django-project-base-0.75.32/django_project_base/settings_parser.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/static/browser-update/update.min.js` & `django-project-base-0.75.32/django_project_base/static/browser-update/update.min.js`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/templates/app-debug/main.html` & `django-project-base-0.75.32/django_project_base/templates/app-debug/main.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/urls.py` & `django-project-base-0.75.32/django_project_base/urls.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/utils.py` & `django-project-base-0.75.32/django_project_base/utils.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base/views.py` & `django-project-base-0.75.32/django_project_base/views.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/django_project_base.egg-info/PKG-INFO` & `django-project-base-0.75.32/django_project_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-base
-Version: 0.75.30
+Version: 0.75.32
 Summary: Everything revolves around it: users, roles, permissions, tags, etc.
 Home-page: https://github.com/velis74/django-project-base
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-project-base-0.75.30/django_project_base.egg-info/SOURCES.txt` & `django-project-base-0.75.32/django_project_base.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 django_project_base/__init__.py
 django_project_base/apps.py
 django_project_base/constants.py
 django_project_base/country_holidays.py
 django_project_base/models.py
 django_project_base/router.py
+django_project_base/serialization.py
 django_project_base/settings.py
 django_project_base/settings_parser.py
 django_project_base/urls.py
 django_project_base/utils.py
 django_project_base/views.py
 django_project_base.egg-info/PKG-INFO
 django_project_base.egg-info/SOURCES.txt
@@ -62,14 +63,18 @@
 django_project_base/base/exceptions.py
 django_project_base/base/fields.py
 django_project_base/base/middleware.py
 django_project_base/base/models.py
 django_project_base/base/permissions.py
 django_project_base/base/queryset_with_cache.py
 django_project_base/base/signals.py
+django_project_base/caching/__init__.py
+django_project_base/caching/cache_queue/__init__.py
+django_project_base/caching/cache_queue/cache_queue_other.py
+django_project_base/caching/cache_queue/cache_queue_redis.py
 django_project_base/celery/__init__.py
 django_project_base/celery/apps.py
 django_project_base/celery/celery.py
 django_project_base/celery/settings.py
 django_project_base/celery/background_tasks/__init__.py
 django_project_base/celery/background_tasks/base_task.py
 django_project_base/celery/background_tasks/notification_tasks.py
@@ -83,15 +88,14 @@
 django_project_base/licensing/migrations/0005_auto_20230901_0613.py
 django_project_base/licensing/migrations/__init__.py
 django_project_base/licensing/rest/__init__.py
 django_project_base/licensing/rest/rest.py
 django_project_base/licensing/rest/router.py
 django_project_base/locale/en/LC_MESSAGES/django.mo
 django_project_base/locale/en/LC_MESSAGES/django.po
-django_project_base/locale/en/LC_MESSAGES/djangojs.mo
 django_project_base/locale/en/LC_MESSAGES/djangojs.po
 django_project_base/locale/sl/LC_MESSAGES/django.mo
 django_project_base/locale/sl/LC_MESSAGES/django.po
 django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
 django_project_base/locale/sl/LC_MESSAGES/djangojs.po
 django_project_base/management/__init__.py
 django_project_base/management/commands/__init__.py
```

### Comparing `django-project-base-0.75.30/pyproject.toml` & `django-project-base-0.75.32/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-project-base-0.75.30/setup.py` & `django-project-base-0.75.32/setup.py`

 * *Files identical despite different names*

