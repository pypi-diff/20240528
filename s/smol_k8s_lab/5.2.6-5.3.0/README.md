# Comparing `tmp/smol_k8s_lab-5.2.6.tar.gz` & `tmp/smol_k8s_lab-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_k8s_lab-5.2.6.tar", max compression
+gzip compressed data, was "smol_k8s_lab-5.3.0.tar", max compression
```

## Comparing `smol_k8s_lab-5.2.6.tar` & `smol_k8s_lab-5.3.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    34260 2024-05-25 14:18:06.244552 smol_k8s_lab-5.2.6/LICENSE
--rw-r--r--   0        0        0    29423 2024-05-25 14:18:06.244552 smol_k8s_lab-5.2.6/README.md
--rw-r--r--   0        0        0     3323 2024-05-25 14:18:06.512550 smol_k8s_lab-5.2.6/pyproject.toml
--rwxr-xr-x   0        0        0    16188 2024-05-25 14:18:06.512550 smol_k8s_lab-5.2.6/smol_k8s_lab/__init__.py
--rw-r--r--   0        0        0  5853144 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/audio/audio-en.tar.gz
--rwxr-xr-x   0        0        0    12759 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/bw_cli.py
--rw-r--r--   0        0        0     1679 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden.css
--rw-r--r--   0        0        0     2093 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
--rw-r--r--   0        0        0     4524 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
--rw-r--r--   0        0        0     2395 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
--rw-r--r--   0        0        0     6916 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
--rw-r--r--   0        0        0    17031 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/config/audio/en.yml
--rw-r--r--   0        0        0     2364 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/config/audio/nl.yml
--rw-r--r--   0        0        0    79433 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/config/default_config.yaml
--rw-r--r--   0        0        0     5666 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/config/keycloak_config.json
--rw-r--r--   0        0        0      237 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/config/kind/kind-config-cilium.yaml
--rw-r--r--   0        0        0      385 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/config/kind/kind_cluster_config.yaml
--rw-r--r--   0        0        0      831 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
--rwxr-xr-x   0        0        0     3008 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/constants.py
--rwxr-xr-x   0        0        0    12945 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/env_config.py
--rw-r--r--   0        0        0     9821 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/__init__.py
--rw-r--r--   0        0        0     7789 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/argocd.py
--rw-r--r--   0        0        0        0 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
--rw-r--r--   0        0        0     6581 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
--rw-r--r--   0        0        0     9763 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
--rw-r--r--   0        0        0    19076 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
--rw-r--r--   0        0        0    20511 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
--rw-r--r--   0        0        0     3372 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
--rw-r--r--   0        0        0     1285 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
--rw-r--r--   0        0        0     9134 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/initial_special.py
--rw-r--r--   0        0        0        0 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/networking/__init__.py
--rw-r--r--   0        0        0     1766 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/networking/cilium.py
--rw-r--r--   0        0        0     2318 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/networking/metallb.py
--rw-r--r--   0        0        0    10977 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/networking/netmaker.py
--rw-r--r--   0        0        0     2383 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/operators/__init__.py
--rw-r--r--   0        0        0     8381 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/operators/minio.py
--rw-r--r--   0        0        0     3617 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
--rw-r--r--   0        0        0     4286 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
--rw-r--r--   0        0        0        0 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
--rw-r--r--   0        0        0     2675 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
--rw-r--r--   0        0        0     3759 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
--rw-r--r--   0        0        0     4805 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/secrets_management/vault.py
--rw-r--r--   0        0        0    11623 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/home_assistant.py
--rw-r--r--   0        0        0    21465 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/mastodon.py
--rwxr-xr-x   0        0        0     1706 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
--rw-r--r--   0        0        0    24586 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/matrix.py
--rw-r--r--   0        0        0    20726 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/nextcloud.py
--rwxr-xr-x   0        0        0     6182 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
--rw-r--r--   0        0        0     8034 2024-05-25 14:18:06.524550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_distros/__init__.py
--rw-r--r--   0        0        0     3755 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_distros/k3d.py
--rw-r--r--   0        0        0     8481 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_distros/k3s.py
--rw-r--r--   0        0        0     4821 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_distros/kind.py
--rw-r--r--   0        0        0        1 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/__init__.py
--rw-r--r--   0        0        0     8642 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/argocd_util.py
--rw-r--r--   0        0        0     8689 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/backup.py
--rwxr-xr-x   0        0        0     8607 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/helm.py
--rw-r--r--   0        0        0    14252 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/k8s_lib.py
--rw-r--r--   0        0        0    22222 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/restores.py
--rw-r--r--   0        0        0     1358 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/__init__.py
--rw-r--r--   0        0        0    14333 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
--rw-r--r--   0        0        0     9712 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
--rw-r--r--   0        0        0    18578 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
--rw-r--r--   0        0        0    14373 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/input_widgets.py
--rwxr-xr-x   0        0        0     4002 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/invalid_apps.py
--rw-r--r--   0        0        0     6970 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/modify_globals.py
--rw-r--r--   0        0        0     3697 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/new_app_modal.py
--rwxr-xr-x   0        0        0    17593 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/apps_screen.py
--rw-r--r--   0        0        0    12891 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/base.py
--rw-r--r--   0        0        0    33063 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/base_widgets/audio_widget.py
--rw-r--r--   0        0        0     7189 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/base_widgets/cluster_modal.py
--rw-r--r--   0        0        0     3384 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
--rwxr-xr-x   0        0        0     8926 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/confirm_screen.py
--rw-r--r--   0        0        0     1546 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/add_nodes_widget.tcss
--rw-r--r--   0        0        0     7174 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/apps_config.tcss
--rw-r--r--   0        0        0     1184 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/apps_init_config.tcss
--rw-r--r--   0        0        0     6681 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/base.tcss
--rw-r--r--   0        0        0      988 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/base_modal.tcss
--rw-r--r--   0        0        0     1371 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/cluster_modal.tcss
--rw-r--r--   0        0        0     1278 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/confirm.tcss
--rw-r--r--   0        0        0     1564 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/distro_config.tcss
--rw-r--r--   0        0        0      927 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/help.tcss
--rw-r--r--   0        0        0      984 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/invalid_apps.tcss
--rw-r--r--   0        0        0     2198 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/k3s.tcss
--rw-r--r--   0        0        0     1901 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/kind.tcss
--rw-r--r--   0        0        0     1259 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/modify_globals_modal.tcss
--rw-r--r--   0        0        0      770 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/new_app_modal.tcss
--rw-r--r--   0        0        0      112 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/new_option_modal.tcss
--rw-r--r--   0        0        0     1168 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/node_inputs_widget.tcss
--rw-r--r--   0        0        0     1101 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/node_modal.tcss
--rw-r--r--   0        0        0     3433 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
--rw-r--r--   0        0        0     2554 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/tui_config.tcss
--rwxr-xr-x   0        0        0    10391 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_screen.py
--rw-r--r--   0        0        0        0 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/__init__.py
--rw-r--r--   0        0        0    17214 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/add_nodes.py
--rw-r--r--   0        0        0    14337 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/k3s_config.py
--rw-r--r--   0        0        0     6754 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/kind_config.py
--rw-r--r--   0        0        0     6060 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
--rw-r--r--   0        0        0     4359 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
--rw-r--r--   0        0        0     4669 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
--rw-r--r--   0        0        0     4193 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/help_screen.py
--rwxr-xr-x   0        0        0     4020 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/make_screenshots.py
--rwxr-xr-x   0        0        0    11139 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/smol_k8s_config_screen.py
--rwxr-xr-x   0        0        0     8811 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/tui_config_screen.py
--rw-r--r--   0        0        0     9901 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/util.py
--rw-r--r--   0        0        0        0 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/validators/__init__.py
--rw-r--r--   0        0        0      579 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/tui/validators/already_exists.py
--rw-r--r--   0        0        0        0 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/__init__.py
--rw-r--r--   0        0        0    16300 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/minio_lib.py
--rw-r--r--   0        0        0     1184 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/passwords.py
--rwxr-xr-x   0        0        0     2423 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/rich_cli/console_logging.py
--rwxr-xr-x   0        0        0     4720 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/rich_cli/help_text.py
--rw-r--r--   0        0        0     2610 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/run/final_cmd.py
--rwxr-xr-x   0        0        0     7483 2024-05-25 14:18:06.528550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/run/subproc.py
--rw-r--r--   0        0        0     2837 2024-05-25 14:18:06.532550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/value_from.py
--rw-r--r--   0        0        0      315 2024-05-25 14:18:06.532550 smol_k8s_lab-5.2.6/smol_k8s_lab/utils/yaml_with_comments.py
--rw-r--r--   0        0        0    31153 1970-01-01 00:00:00.000000 smol_k8s_lab-5.2.6/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-05-28 09:38:58.664504 smol_k8s_lab-5.3.0/LICENSE
+-rw-r--r--   0        0        0    29423 2024-05-28 09:38:58.664504 smol_k8s_lab-5.3.0/README.md
+-rw-r--r--   0        0        0     3326 2024-05-28 09:38:58.928506 smol_k8s_lab-5.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0    16188 2024-05-28 09:38:58.932506 smol_k8s_lab-5.3.0/smol_k8s_lab/__init__.py
+-rw-r--r--   0        0        0  5853144 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/audio/audio-en.tar.gz
+-rwxr-xr-x   0        0        0    12759 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/bw_cli.py
+-rw-r--r--   0        0        0     1679 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden.css
+-rw-r--r--   0        0        0     2093 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
+-rw-r--r--   0        0        0     4524 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
+-rw-r--r--   0        0        0     2395 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
+-rw-r--r--   0        0        0     6916 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
+-rw-r--r--   0        0        0    17031 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/config/audio/en.yml
+-rw-r--r--   0        0        0     2364 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/config/audio/nl.yml
+-rw-r--r--   0        0        0    79454 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/config/default_config.yaml
+-rw-r--r--   0        0        0     5666 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/config/keycloak_config.json
+-rw-r--r--   0        0        0      237 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/config/kind/kind-config-cilium.yaml
+-rw-r--r--   0        0        0      385 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/config/kind/kind_cluster_config.yaml
+-rw-r--r--   0        0        0      831 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
+-rwxr-xr-x   0        0        0     3008 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/constants.py
+-rwxr-xr-x   0        0        0    12945 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/env_config.py
+-rw-r--r--   0        0        0     9821 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/__init__.py
+-rw-r--r--   0        0        0     7789 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/argocd.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
+-rw-r--r--   0        0        0     6581 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
+-rw-r--r--   0        0        0     9763 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
+-rw-r--r--   0        0        0    19076 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
+-rw-r--r--   0        0        0    20511 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
+-rw-r--r--   0        0        0     3372 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
+-rw-r--r--   0        0        0     1285 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
+-rw-r--r--   0        0        0     9134 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/initial_special.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/networking/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/networking/cilium.py
+-rw-r--r--   0        0        0     2318 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/networking/metallb.py
+-rw-r--r--   0        0        0    10977 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/networking/netmaker.py
+-rw-r--r--   0        0        0     2383 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/operators/__init__.py
+-rw-r--r--   0        0        0     8381 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/operators/minio.py
+-rw-r--r--   0        0        0     3617 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
+-rw-r--r--   0        0        0     4286 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
+-rw-r--r--   0        0        0     2675 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
+-rw-r--r--   0        0        0     3759 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
+-rw-r--r--   0        0        0     4805 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py
+-rw-r--r--   0        0        0    11623 2024-05-28 09:38:58.940506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/home_assistant.py
+-rw-r--r--   0        0        0    21465 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/mastodon.py
+-rwxr-xr-x   0        0        0     1706 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
+-rw-r--r--   0        0        0    24926 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/matrix.py
+-rw-r--r--   0        0        0    20726 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/nextcloud.py
+-rwxr-xr-x   0        0        0     6182 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
+-rw-r--r--   0        0        0     8034 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_distros/__init__.py
+-rw-r--r--   0        0        0     3755 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_distros/k3d.py
+-rw-r--r--   0        0        0     8481 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_distros/k3s.py
+-rw-r--r--   0        0        0     4821 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_distros/kind.py
+-rw-r--r--   0        0        0        1 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/__init__.py
+-rw-r--r--   0        0        0     8642 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/argocd_util.py
+-rw-r--r--   0        0        0     8689 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/backup.py
+-rwxr-xr-x   0        0        0     8607 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/helm.py
+-rw-r--r--   0        0        0    14252 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/k8s_lib.py
+-rw-r--r--   0        0        0    22222 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/restores.py
+-rw-r--r--   0        0        0     1358 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/__init__.py
+-rw-r--r--   0        0        0    14333 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
+-rw-r--r--   0        0        0     9712 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
+-rw-r--r--   0        0        0    18578 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
+-rw-r--r--   0        0        0    14373 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/input_widgets.py
+-rwxr-xr-x   0        0        0     4002 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py
+-rw-r--r--   0        0        0     6970 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/modify_globals.py
+-rw-r--r--   0        0        0     3697 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py
+-rwxr-xr-x   0        0        0    17593 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/apps_screen.py
+-rw-r--r--   0        0        0    12891 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/base.py
+-rw-r--r--   0        0        0    33063 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/base_widgets/audio_widget.py
+-rw-r--r--   0        0        0     7189 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py
+-rw-r--r--   0        0        0     3384 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
+-rwxr-xr-x   0        0        0     8926 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/confirm_screen.py
+-rw-r--r--   0        0        0     1546 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss
+-rw-r--r--   0        0        0     7174 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/apps_config.tcss
+-rw-r--r--   0        0        0     1184 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/apps_init_config.tcss
+-rw-r--r--   0        0        0     6701 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/base.tcss
+-rw-r--r--   0        0        0      988 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/base_modal.tcss
+-rw-r--r--   0        0        0     1371 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/cluster_modal.tcss
+-rw-r--r--   0        0        0     1278 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/confirm.tcss
+-rw-r--r--   0        0        0     1564 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/distro_config.tcss
+-rw-r--r--   0        0        0      927 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/help.tcss
+-rw-r--r--   0        0        0      984 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/invalid_apps.tcss
+-rw-r--r--   0        0        0     2198 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/k3s.tcss
+-rw-r--r--   0        0        0     1901 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/kind.tcss
+-rw-r--r--   0        0        0     1259 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss
+-rw-r--r--   0        0        0      770 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/new_app_modal.tcss
+-rw-r--r--   0        0        0      112 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/new_option_modal.tcss
+-rw-r--r--   0        0        0     1168 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss
+-rw-r--r--   0        0        0     1101 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/node_modal.tcss
+-rw-r--r--   0        0        0     3433 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
+-rw-r--r--   0        0        0     2554 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/tui_config.tcss
+-rwxr-xr-x   0        0        0    10391 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_screen.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/__init__.py
+-rw-r--r--   0        0        0    17214 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py
+-rw-r--r--   0        0        0    14337 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py
+-rw-r--r--   0        0        0     6754 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/kind_config.py
+-rw-r--r--   0        0        0     6060 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
+-rw-r--r--   0        0        0     4359 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
+-rw-r--r--   0        0        0     4669 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
+-rw-r--r--   0        0        0     4193 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/help_screen.py
+-rwxr-xr-x   0        0        0     4020 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/make_screenshots.py
+-rwxr-xr-x   0        0        0    11139 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/smol_k8s_config_screen.py
+-rwxr-xr-x   0        0        0     8811 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/tui_config_screen.py
+-rw-r--r--   0        0        0     9901 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/util.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/validators/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-28 09:38:58.944506 smol_k8s_lab-5.3.0/smol_k8s_lab/tui/validators/already_exists.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/__init__.py
+-rw-r--r--   0        0        0    16300 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/minio_lib.py
+-rw-r--r--   0        0        0     1184 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/passwords.py
+-rwxr-xr-x   0        0        0     2423 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/rich_cli/console_logging.py
+-rwxr-xr-x   0        0        0     4720 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/rich_cli/help_text.py
+-rw-r--r--   0        0        0     2610 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/run/final_cmd.py
+-rwxr-xr-x   0        0        0     7483 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/run/subproc.py
+-rw-r--r--   0        0        0     2837 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/value_from.py
+-rw-r--r--   0        0        0      315 2024-05-28 09:38:58.948506 smol_k8s_lab-5.3.0/smol_k8s_lab/utils/yaml_with_comments.py
+-rw-r--r--   0        0        0    31145 1970-01-01 00:00:00.000000 smol_k8s_lab-5.3.0/PKG-INFO
```

### Comparing `smol_k8s_lab-5.2.6/LICENSE` & `smol_k8s_lab-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/README.md` & `smol_k8s_lab-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/pyproject.toml` & `smol_k8s_lab-5.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "smol_k8s_lab"
-version       = "5.2.6"
+version       = "5.3.0"
 description   = "CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD"
 authors       = ["Jesse Hitch <jessebot@linux.com>",
                  "Max Roby <emax@cloudydev.net>"]
 readme        = "README.md"
 packages      = [{include = "smol_k8s_lab"}]
 license       = "AGPL-3.0-or-later"
 homepage      = "https://small-hack.github.io/smol-k8s-lab"
@@ -41,16 +41,16 @@
 pyyaml             = "^6.0"
 requests           = "^2.32"
 rich               = "^13.0"
 ruamel-yaml        = "^0.18"
 ruamel-yaml-string = "^0.1"
 textual            = "^0.63"
 xdg-base-dirs      = "^6.0"
-pygame             = "^2.5.2"
-python-ulid = "^2.5.0"
+pygame             = "^2.5"
+python-ulid        = "^2.6"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.5"
 mkdocs-video    = "^1.5"
@@ -71,15 +71,15 @@
 # categories = "ConsoleOnly;"
 
 [tool.poetry.group.audio]
 optional = true
 
 # this group is only needed for development
 [tool.poetry.group.audio.dependencies]
-coqui-tts     = "^0.23.1"
+coqui-tts     = "^0.24.0"
 # note: this still requires you to install ffmpeg
 pydub         = "^0.25.1"
 
 [tool.poetry.plugins."smol-k8s-lab.application.plugin"]
 "smol-k8s-lab" = "smol_k8s_lab:main"
 "smol-tts"     = "smol_tts:tts_gen"
```

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/__init__.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/audio/audio-en.tar.gz` & `smol_k8s_lab-5.3.0/smol_k8s_lab/audio/audio-en.tar.gz`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/bw_cli.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/bw_cli.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden.css` & `smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden.css`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden_app.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/config/audio/en.yml` & `smol_k8s_lab-5.3.0/smol_k8s_lab/config/audio/en.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/config/audio/nl.yml` & `smol_k8s_lab-5.3.0/smol_k8s_lab/config/audio/nl.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/config/default_config.yaml` & `smol_k8s_lab-5.3.0/smol_k8s_lab/config/default_config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -949,15 +949,15 @@
       secret_keys:
         # hostname of the synapse matrix server
         hostname: ""
         # the hostname of the element web interface
         element_hostname: ""
         # hostname for federation, that others can see you on the fediverse
         federation_hostname: ""
-        # sliding sync hostname to use for beta features
+        # sliding sync hostname to use for beta features. currently on syncv3
         sliding_sync_hostname: "sliding sync hostname to use for beta features"
         # auth hostname to use for beta features
         auth_hostname: "auth hostname to use for beta features"
         # email for of the admin user
         admin_email: ""
         # enable persistent volume claim for matrix media storage
         media_pvc_enabled: "true"
```

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/config/keycloak_config.json` & `smol_k8s_lab-5.3.0/smol_k8s_lab/config/keycloak_config.json`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/config/smol-k8s-lab.appdata.xml` & `smol_k8s_lab-5.3.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/constants.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/constants.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/env_config.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/env_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/__init__.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/argocd.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/argocd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/vouch.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/ingress/cert_manager.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/initial_special.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/initial_special.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/networking/cilium.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/networking/cilium.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/networking/metallb.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/networking/metallb.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/networking/netmaker.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/networking/netmaker.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/operators/__init__.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/operators/minio.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/operators/minio.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/operators/postgres_operators.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/operators/seaweedfs.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/secrets_management/infisical.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/secrets_management/vault.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/home_assistant.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/home_assistant.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/mastodon.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/mastodon.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/mastodon_rake.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/matrix.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,31 +80,34 @@
         mail_user = init_values['smtp_user']
         mail_pass = extract_secret(init_values['smtp_password'])
         mail_host = init_values['smtp_host']
 
         # create a local alias to check and make sure matrix is functional
         create_minio_alias("matrix", s3_endpoint, "matrix", s3_access_key)
 
+        # secret for the token header for matrix to talk to sliding sync
+        syncv3_secret = create_password()
+
         # create Matrix OIDC Application
         if zitadel and not restore_enabled:
-            log.debug("Creating a Matrix OIDC application in Zitadel...")
-            redirect_uris = f"https://{matrix_hostname}/_synapse/client/oidc/callback"
+            log.debug("Creating an OIDC application in Zitadel...")
+            mas_issuer = f"https://{zitadel.hostname}"
+            mas_client_id = str(ULID())
+            mas_provider_ulid = str(ULID())
+            mas_client_secret = create_password()
+            mas_admin_token = create_password()
+            matrix_auth_hostname = secrets.get("auth_hostname", "")
+            zitadel_hostname = zitadel.hostname
             logout_uris = [f"https://{matrix_hostname}"]
+            redirect_uris = f"https://{matrix_auth_hostname}/upstream/callback/{mas_provider_ulid}"
             oidc_creds = zitadel.create_application("matrix",
                                                     redirect_uris,
                                                     logout_uris)
             zitadel.create_role("matrix_users", "Matrix Users", "matrix_users")
             zitadel.update_user_grant(['matrix_users'])
-            zitadel_hostname = zitadel.hostname
-            mas_issuer = f"https://{zitadel.hostname}"
-            mas_client_id = str(ULID())
-            mas_provider_ulid = str(ULID())
-            mas_client_secret = create_password()
-            mas_admin_token = create_password()
-            sliding_sync_secret = create_password()
         else:
             zitadel_hostname = ""
 
         # if the user has bitwarden enabled
         if bitwarden and not restore_enabled:
             setup_bitwarden_items(argocd,
                                   matrix_hostname,
@@ -122,15 +125,15 @@
                                   zitadel_hostname,
                                   oidc_creds,
                                   mas_provider_ulid,
                                   mas_issuer,
                                   mas_client_id,
                                   mas_client_secret,
                                   mas_admin_token,
-                                  sliding_sync_secret,
+                                  syncv3_secret,
                                   bitwarden)
 
         # else create these as Kubernetes secrets
         elif not bitwarden and not restore_enabled:
             # postgresql credentials
             argocd.k8s.create_secret(
                     'matrix-pgsql-credentials',
@@ -144,20 +147,23 @@
                     'mas-pgsql-credentials',
                     'matrix',
                     {"password": "we-use-tls-instead-of-password-now",
                      "database": "mas",
                      "hostname": f"mas-rw.{matrix_namespace}.svc"}
                     )
 
+            pgconnstr = ("user=syncv3 dbname=syncv3 "
+                         f"host=mas-rw.{matrix_namespace}.svc "
+                         "sslmode=verify-full sslkey=/etc/secrets/synvcv3/tls.key"
+                         " sslcert=/etc/secrets/syncv3/tls.crt "
+                         "sslrootcert=/etc/secrets/ca/ca.crt")
             argocd.k8s.create_secret(
-                    'sliding-sync-pgsql-credentials',
+                    'syncv3-pgsql-credentials',
                     'matrix',
-                    {"password": "we-use-tls-instead-of-password-now",
-                     "database": "syncv3",
-                     "hostname": f"syncv3-rw.{matrix_namespace}.svc"}
+                    {"password": pgconnstr}
                     )
 
             # registation key
             matrix_registration_key = create_password()
             argocd.k8s.create_secret(
                     'matrix-registration',
                     'matrix',
@@ -253,15 +259,15 @@
             )[0]['id']
 
     mas_id = bitwarden.get_item(
             f"matrix-authentication-service-credentials-{matrix_hostname}", False
             )[0]['id']
 
     sync_id = bitwarden.get_item(
-            f"matrix-sliding-sync-credentials-{matrix_hostname}", False
+            f"matrix-syncv3-credentials-{matrix_hostname}", False
             )[0]['id']
 
     oidc_id = bitwarden.get_item(
             f"matrix-oidc-credentials-{matrix_hostname}", False
             )[0]
 
     # identity provider name and id are nested in the oidc item fields
@@ -304,15 +310,15 @@
                           zitadel_hostname: str,
                           oidc_creds: str,
                           mas_provider_ulid: str,
                           mas_issuer: str,
                           mas_client_id: str,
                           mas_client_secret: str,
                           mas_admin_token: str,
-                          sliding_sync_secret: str,
+                          syncv3_secret: str,
                           bitwarden: BwCLI):
     """
     setup all the required secrets as items in bitwarden
     """
     sub_header("Creating matrix secrets in Bitwarden")
 
     # S3 credentials
@@ -373,27 +379,29 @@
             fields=[db_host_obj, db_obj]
             )
 
     # postgres matrix authentication service credentials
     mas_db_host_obj = create_custom_field("hostname",
                                           f"mas-postgres-rw.{matrix_namespace}.svc")
     mas_db_obj = create_custom_field("database", "mas")
+    # MAS doesn't support TLS auth to databases yet
+    mas_db_pw = create_password()
     mas_db_id = bitwarden.create_login(
             name='mas-pgsql-credentials',
             item_url=matrix_hostname,
             user='mas',
-            password="we-use-tls-instead-of-password-now",
+            password=mas_db_pw,
             fields=[mas_db_host_obj, mas_db_obj]
             )
 
     # postgres sliding sync connection string
     conn_str = ("user=syncv3 dbname=syncv3 "
-                f"host=syncv3-postgres-rw.{matrix_namespace}.svc sslmode=require"
-                "sslkey=/etc/secrets/sliding-sync/tls.key "
-                "sslcert=/etc/secrets/sliding-sync/tls.crt "
+                f"host=syncv3-postgres-rw.{matrix_namespace}.svc sslmode=require "
+                "sslkey=/etc/secrets/syncv3/tls.key "
+                "sslcert=/etc/secrets/syncv3/tls.crt "
                 "sslrootcert=/etc/secrets/ca/ca.crt")
     sync_db_id = bitwarden.create_login(
             name='syncv3-pgsql-credentials',
             item_url=matrix_hostname,
             user='syncv3',
             password=conn_str,
             )
@@ -415,18 +423,18 @@
             item_url=matrix_hostname,
             user="admin",
             password=matrix_registration_key
             )
 
     # matrix sliding sync
     sync_id = bitwarden.create_login(
-            name='matrix-sliding-sync-credentials',
+            name='matrix-syncv3-credentials',
             item_url=matrix_hostname,
             user="syncv3",
-            password=sliding_sync_secret
+            password=syncv3_secret
             )
 
     # OIDC credentials
     log.info("Creating OIDC credentials for Matrix in Bitwarden")
     if zitadel_hostname:
         idp_id = "zitadel"
         idp_name = "Zitadel Auth"
```

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/nextcloud.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/nextcloud.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_distros/__init__.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_distros/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_distros/k3d.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_distros/k3d.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_distros/k3s.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_distros/k3s.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_distros/kind.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_distros/kind.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/argocd_util.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/argocd_util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/backup.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/backup.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/helm.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/helm.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/k8s_lib.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/k8s_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/k8s_tools/restores.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/k8s_tools/restores.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/__init__.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/argocd_widgets.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/backup_and_restore.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/input_widgets.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/input_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/invalid_apps.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/modify_globals.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/modify_globals.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/app_widgets/new_app_modal.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/apps_screen.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/apps_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/base.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/base.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/base_widgets/audio_widget.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/base_widgets/audio_widget.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/base_widgets/cluster_modal.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/base_widgets/new_cluster_input.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/confirm_screen.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/confirm_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/add_nodes_widget.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/apps_config.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/apps_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/apps_init_config.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/apps_init_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/base.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/base.tcss`

 * *Files 14% similar despite different names*

```diff
@@ -54,32 +54,32 @@
 }
 
 /* Matches the bottom footer text on every page */
 Footer {
     background: $background 1%;
 }
 
-Footer .footer--description {
-    color: $light_cornflower;
-    background: $navy 50%;
-}
-
-Footer .footer--key {
-    color: $navy;
-    background: $light_cornflower;
-}
 
-Footer .footer--highlight {
-    color: $orange;
+Footer > FooterKey {
     background: $navy 50%;
-}
-
-Footer .footer--highlight-key {
-    color: $navy;
-    background: $orange;
+    color: $light_cornflower;
+    .footer-key--key {
+        background: $light_cornflower;
+        color: $navy;
+    }
+
+    &:hover {
+        color: $orange;
+        background: $navy 50%;
+
+       .footer-key--key {
+            color: $navy;
+            background: $orange;
+        }
+    }
 }
 
 /* sets the init switch slider color only when it's on */
 Switch.-on > .switch--slider {
     color: $spacechalk_lime 90%;
 }
```

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/base_modal.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/base_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/cluster_modal.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/cluster_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/confirm.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/confirm.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/distro_config.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/distro_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/help.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/help.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/invalid_apps.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/invalid_apps.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/k3s.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/k3s.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/kind.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/kind.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/modify_globals_modal.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/new_app_modal.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/new_app_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/node_inputs_widget.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/node_modal.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/node_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/css/tui_config.tcss` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/css/tui_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_screen.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/add_nodes.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/k3s_config.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/kind_config.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/kind_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/kubelet_config.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/distro_widgets/node_adjustment.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/help_screen.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/help_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/make_screenshots.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/make_screenshots.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/smol_k8s_config_screen.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/smol_k8s_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/tui_config_screen.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/tui_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/util.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/tui/validators/already_exists.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/tui/validators/already_exists.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/utils/minio_lib.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/utils/minio_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/utils/passwords.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/utils/passwords.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/utils/rich_cli/console_logging.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/utils/rich_cli/console_logging.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/utils/rich_cli/help_text.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/utils/rich_cli/help_text.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/utils/run/final_cmd.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/utils/run/final_cmd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/utils/run/subproc.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/utils/run/subproc.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/smol_k8s_lab/utils/value_from.py` & `smol_k8s_lab-5.3.0/smol_k8s_lab/utils/value_from.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.2.6/PKG-INFO` & `smol_k8s_lab-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smol_k8s_lab
-Version: 5.2.6
+Version: 5.3.0
 Summary: CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD
 Home-page: https://small-hack.github.io/smol-k8s-lab
 License: AGPL-3.0-or-later
 Keywords: kubernetes,homelab,kind,k3s,k8s
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<3.13
@@ -19,17 +19,17 @@
 Classifier: Topic :: System :: Installation/Setup
 Requires-Dist: bcrypt (>=4.1,<5.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: cryptography (>=42.0,<43.0)
 Requires-Dist: kubernetes (>=29,<30)
 Requires-Dist: minio (>=7.2,<8.0)
 Requires-Dist: pyfiglet (>=1.0,<2.0)
-Requires-Dist: pygame (>=2.5.2,<3.0.0)
+Requires-Dist: pygame (>=2.5,<3.0)
 Requires-Dist: pyjwt (>=2.8,<3.0)
-Requires-Dist: python-ulid (>=2.5.0,<3.0.0)
+Requires-Dist: python-ulid (>=2.6,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.32,<3.0)
 Requires-Dist: rich (>=13.0,<14.0)
 Requires-Dist: ruamel-yaml (>=0.18,<0.19)
 Requires-Dist: ruamel-yaml-string (>=0.1,<0.2)
 Requires-Dist: textual (>=0.63,<0.64)
 Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.2.6 Summary: CLI and TUI to
+Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.3.0 Summary: CLI and TUI to
 quickly install slimmer Kubernetes distros and then manage apps declaratively
 using Argo CD Home-page: https://small-hack.github.io/smol-k8s-lab License:
 AGPL-3.0-or-later Keywords: kubernetes,homelab,kind,k3s,k8s Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: System ::
 Installation/Setup Requires-Dist: bcrypt (>=4.1,<5.0) Requires-Dist: click
 (>=8.1,<9.0) Requires-Dist: cryptography (>=42.0,<43.0) Requires-Dist:
 kubernetes (>=29,<30) Requires-Dist: minio (>=7.2,<8.0) Requires-Dist: pyfiglet
-(>=1.0,<2.0) Requires-Dist: pygame (>=2.5.2,<3.0.0) Requires-Dist: pyjwt
-(>=2.8,<3.0) Requires-Dist: python-ulid (>=2.5.0,<3.0.0) Requires-Dist: pyyaml
+(>=1.0,<2.0) Requires-Dist: pygame (>=2.5,<3.0) Requires-Dist: pyjwt
+(>=2.8,<3.0) Requires-Dist: python-ulid (>=2.6,<3.0) Requires-Dist: pyyaml
 (>=6.0,<7.0) Requires-Dist: requests (>=2.32,<3.0) Requires-Dist: rich
 (>=13.0,<14.0) Requires-Dist: ruamel-yaml (>=0.18,<0.19) Requires-Dist: ruamel-
 yaml-string (>=0.1,<0.2) Requires-Dist: textual (>=0.63,<0.64) Requires-Dist:
 xdg-base-dirs (>=6.0,<7.0) Project-URL: Bug Tracker, http://github.com/small-
 hack/smol-k8s-lab/issues Project-URL: Documentation, https://small-
 hack.github.io/smol-k8s-lab Project-URL: Repository, http://github.com/small-
 hack/smol-k8s-lab Description-Content-Type: text/markdown
```

