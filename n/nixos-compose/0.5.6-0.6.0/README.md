# Comparing `tmp/nixos_compose-0.5.6.tar.gz` & `tmp/nixos_compose-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixos_compose-0.5.6.tar", max compression
+gzip compressed data, was "nixos_compose-0.6.0.tar", max compression
```

## Comparing `nixos_compose-0.5.6.tar` & `nixos_compose-0.6.0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     1094 2024-01-11 17:28:25.788006 nixos_compose-0.5.6/LICENSE
--rw-r--r--   0        0        0      216 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic/composition.nix
--rw-r--r--   0        0        0      561 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic/flake.nix
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic/nxc.json
--rw-r--r--   0        0        0      216 2024-01-11 17:28:25.797006 nixos_compose-0.5.6/examples/basic-nur/composition.nix
--rw-r--r--   0        0        0     1043 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic-nur/flake.nix
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic-nur/nxc.json
--rw-r--r--   0        0        0      214 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/execo/composition.nix
--rw-r--r--   0        0        0     2964 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/execo/execo_script.py
--rw-r--r--   0        0        0      963 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/execo/flake.nix
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/execo/nxc.json
--rw-r--r--   0        0        0      569 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/flake.lock
--rw-r--r--   0        0        0       96 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/compositions.nix
--rw-r--r--   0        0        0      577 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/flake.nix
--rw-r--r--   0        0        0      200 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/linux_5_4.nix
--rw-r--r--   0        0        0      907 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/linux_ipanema_5_4.nix
--rw-r--r--   0        0        0       51 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/nxc.json
--rw-r--r--   0        0        0      132 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/bar-composition.nix
--rw-r--r--   0        0        0       80 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/compositions.nix
--rw-r--r--   0        0        0      571 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/flake.nix
--rw-r--r--   0        0        0      132 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/foo-composition.nix
--rw-r--r--   0        0        0       51 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/nxc.json
--rw-r--r--   0        0        0      569 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nbp-mpi/composition.nix
--rw-r--r--   0        0        0      807 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nbp-mpi/flake.nix
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nbp-mpi/nxc.json
--rw-r--r--   0        0        0     1113 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nix_flake_templates.nix
--rw-r--r--   0        0        0     2141 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/composition.nix
--rw-r--r--   0        0        0      703 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/flake.nix
--rw-r--r--   0        0        0       49 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/nodes.yaml
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/nxc.json
--rw-r--r--   0        0        0     4455 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/ssh-keys.nix
--rw-r--r--   0        0        0      499 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/composition.nix
--rw-r--r--   0        0        0      563 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/flake.nix
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/nxc.json
--rw-r--r--   0        0        0      484 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/scripts/scripts.nix
--rw-r--r--   0        0        0       83 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/scripts/test_python.py
--rw-r--r--   0        0        0      465 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/setup/composition.nix
--rw-r--r--   0        0        0      593 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/setup/flake.nix
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/setup/nxc.json
--rw-r--r--   0        0        0     2917 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/setup/setup.toml
--rw-r--r--   0        0        0      691 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/shared-directories-users/composition.nix
--rw-r--r--   0        0        0      807 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/shared-directories-users/flake.nix
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/shared-directories-users/nxc.json
--rw-r--r--   0        0        0      600 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/webserver/composition.nix
--rw-r--r--   0        0        0      571 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/webserver/flake.nix
--rw-r--r--   0        0        0       60 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/webserver/nxc.json
--rw-r--r--   0        0        0     1262 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/all-in-one.nix
--rw-r--r--   0        0        0     4160 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/compose.nix
--rw-r--r--   0        0        0     3246 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/docker/generate_docker_compose.nix
--rw-r--r--   0        0        0      569 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/docker/generate_image.nix
--rw-r--r--   0        0        0      816 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/docker/nxc-shared-dirs-docker.nix
--rw-r--r--   0        0        0      864 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/docker/systemd.nix
--rw-r--r--   0        0        0      229 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/flavours/docker.nix
--rw-r--r--   0        0        0      731 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/g5k-image.nix
--rw-r--r--   0        0        0     1966 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/g5k-nfs-store.nix
--rw-r--r--   0        0        0      273 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/g5k-ramdisk.nix
--rw-r--r--   0        0        0      533 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/nspawn/base.nix
--rw-r--r--   0        0        0     1982 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/nspawn/generate_nspawn_compose.nix
--rw-r--r--   0        0        0      469 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/nspawn.nix
--rw-r--r--   0        0        0     1572 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/base-hardware.nix
--rw-r--r--   0        0        0     1595 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/base-vm.nix
--rw-r--r--   0        0        0      233 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/base.nix
--rw-r--r--   0        0        0     5217 2024-03-24 20:19:40.908081 nixos_compose-0.5.6/nix/flavours/shared/common.nix
--rw-r--r--   0        0        0     1081 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/g5k-common.nix
--rw-r--r--   0        0        0     1034 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/g5k-ssh-host-keys.nix
--rw-r--r--   0        0        0     3548 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/installation-device.nix
--rw-r--r--   0        0        0     2164 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/netboot.nix
--rw-r--r--   0        0        0     1117 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/nxc-shared-dirs-nfs.nix
--rw-r--r--   0        0        0     6708 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/nxc.nix
--rw-r--r--   0        0        0     4183 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/ssh-keys.nix
--rw-r--r--   0        0        0     6531 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/stage-1-cmds.nix
--rw-r--r--   0        0        0     4044 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/vm-stage-1-cmds.nix
--rw-r--r--   0        0        0      435 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/vm-ramdisk.nix
--rw-r--r--   0        0        0     1440 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/vm.nix
--rw-r--r--   0        0        0     1076 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/flavours.json
--rw-r--r--   0        0        0      321 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/flavours.nix
--rw-r--r--   0        0        0      485 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours2json.nix
--rw-r--r--   0        0        0     1970 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/generate_one_composition_info.nix
--rw-r--r--   0        0        0     1830 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/helpers.nix
--rw-r--r--   0        0        0      421 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/lib.nix
--rw-r--r--   0        0        0     1625 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/make-system-tarball.nix
--rw-r--r--   0        0        0     1540 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/make-system-tarball.sh
--rw-r--r--   0        0        0     6485 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/multiple_compositions.nix
--rw-r--r--   0        0        0      989 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/nur.nix
--rw-r--r--   0        0        0      973 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nix/one_composition.nix
--rw-r--r--   0        0        0     7234 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nix/setup.nix
--rw-r--r--   0        0        0        0 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nixos_compose/__init__.py
--rw-r--r--   0        0        0    32412 2024-04-24 15:55:13.623282 nixos_compose-0.5.6/nixos_compose/actions.py
--rw-r--r--   0        0        0     1851 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/cli.py
--rw-r--r--   0        0        0        0 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nixos_compose/commands/__init__.py
--rw-r--r--   0        0        0     9271 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/commands/cmd_build.py
--rw-r--r--   0        0        0      553 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nixos_compose/commands/cmd_clean.py
--rw-r--r--   0        0        0     2800 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/commands/cmd_connect.py
--rw-r--r--   0        0        0     3455 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/commands/cmd_driver.py
--rw-r--r--   0        0        0     2646 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/commands/cmd_helper.py
--rw-r--r--   0        0        0     4974 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/commands/cmd_init.py
--rw-r--r--   0        0        0    15072 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/commands/cmd_start.py
--rw-r--r--   0        0        0     1829 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/commands/cmd_stop.py
--rw-r--r--   0        0        0     9518 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/context.py
--rw-r--r--   0        0        0      391 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/default_role.py
--rwxr-xr-x   0        0        0      522 2024-01-11 17:28:25.805006 nixos_compose-0.5.6/nixos_compose/driver/__init__.py
--rw-r--r--   0        0        0     5389 2024-01-11 17:28:25.805006 nixos_compose-0.5.6/nixos_compose/driver/driver.py
--rw-r--r--   0        0        0     3250 2024-01-11 17:28:25.805006 nixos_compose-0.5.6/nixos_compose/driver/logger.py
--rw-r--r--   0        0        0    31276 2024-01-11 17:28:25.805006 nixos_compose-0.5.6/nixos_compose/driver/machine.py
--rw-r--r--   0        0        0     3424 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/driver/vlan.py
--rw-r--r--   0        0        0      869 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/flavour.py
--rw-r--r--   0        0        0     1606 2024-01-11 17:28:25.806006 nixos_compose-0.5.6/nixos_compose/flavours/__init__.py
--rw-r--r--   0        0        0     9876 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/flavours/docker.py
--rw-r--r--   0        0        0     8030 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/flavours/grid5000.py
--rwxr-xr-x   0        0        0     1799 2024-01-11 17:28:25.806006 nixos_compose-0.5.6/nixos_compose/flavours/nspawn/machine-dir.sh
--rwxr-xr-x   0        0        0     8836 2024-01-11 17:28:25.806006 nixos_compose-0.5.6/nixos_compose/flavours/nspawn/nxc-net.sh
--rw-r--r--   0        0        0    11435 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/flavours/nspawn.py
--rw-r--r--   0        0        0     7158 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/flavours/vm.py
--rw-r--r--   0        0        0      602 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/g5k.py
--rw-r--r--   0        0        0     2187 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/httpd.py
--rw-r--r--   0        0        0     4273 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/nxc_execo.py
--rw-r--r--   0        0        0     3747 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/platform.py
--rw-r--r--   0        0        0     4033 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/setup.py
--rw-r--r--   0        0        0      953 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/state.py
--rw-r--r--   0        0        0        0 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/tools/__init__.py
--rwxr-xr-x   0        0        0      248 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/tools/g5k_set_pub_key_sleep.sh
--rwxr-xr-x   0        0        0     5009 2024-01-11 17:28:25.808006 nixos_compose-0.5.6/nixos_compose/tools/kataract.py
--rw-r--r--   0        0        0     5916 2024-01-11 17:28:25.808006 nixos_compose-0.5.6/nixos_compose/tools/nested_deployment.py
--rw-r--r--   0        0        0     2372 2024-01-11 17:28:25.808006 nixos_compose-0.5.6/nixos_compose/utils.py
--rw-r--r--   0        0        0     1064 2024-04-24 17:51:32.404552 nixos_compose-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 nixos_compose-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-01-11 17:28:25.788006 nixos_compose-0.6.0/LICENSE
+-rw-r--r--   0        0        0      216 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/basic/composition.nix
+-rw-r--r--   0        0        0      561 2024-05-28 08:47:45.283995 nixos_compose-0.6.0/examples/basic/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/basic/nxc.json
+-rw-r--r--   0        0        0      216 2024-01-11 17:28:25.797006 nixos_compose-0.6.0/examples/basic-nur/composition.nix
+-rw-r--r--   0        0        0     1043 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/basic-nur/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/basic-nur/nxc.json
+-rw-r--r--   0        0        0      214 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/execo/composition.nix
+-rw-r--r--   0        0        0     5009 2024-05-28 08:47:48.796988 nixos_compose-0.6.0/examples/execo/execo_script.py
+-rw-r--r--   0        0        0      963 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/execo/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/execo/nxc.json
+-rw-r--r--   0        0        0      569 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/flake.lock
+-rw-r--r--   0        0        0       96 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/kernel/compositions.nix
+-rw-r--r--   0        0        0      577 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/kernel/flake.nix
+-rw-r--r--   0        0        0      200 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/kernel/linux_5_4.nix
+-rw-r--r--   0        0        0      907 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/kernel/linux_ipanema_5_4.nix
+-rw-r--r--   0        0        0       51 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/kernel/nxc.json
+-rw-r--r--   0        0        0      132 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/multi-compositions/bar-composition.nix
+-rw-r--r--   0        0        0       80 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/multi-compositions/compositions.nix
+-rw-r--r--   0        0        0      571 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/multi-compositions/flake.nix
+-rw-r--r--   0        0        0      132 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/multi-compositions/foo-composition.nix
+-rw-r--r--   0        0        0       51 2024-01-11 17:28:25.798006 nixos_compose-0.6.0/examples/multi-compositions/nxc.json
+-rw-r--r--   0        0        0      569 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nbp-mpi/composition.nix
+-rw-r--r--   0        0        0      807 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nbp-mpi/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nbp-mpi/nxc.json
+-rw-r--r--   0        0        0     1113 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nix_flake_templates.nix
+-rw-r--r--   0        0        0     2141 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nixos-cluster/composition.nix
+-rw-r--r--   0        0        0      703 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nixos-cluster/flake.nix
+-rw-r--r--   0        0        0       49 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nixos-cluster/nodes.yaml
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nixos-cluster/nxc.json
+-rw-r--r--   0        0        0     4455 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/nixos-cluster/ssh-keys.nix
+-rw-r--r--   0        0        0      499 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/scripts/composition.nix
+-rw-r--r--   0        0        0      563 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/scripts/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/scripts/nxc.json
+-rw-r--r--   0        0        0      484 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/scripts/scripts/scripts.nix
+-rw-r--r--   0        0        0       83 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/scripts/scripts/test_python.py
+-rw-r--r--   0        0        0      465 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/setup/composition.nix
+-rw-r--r--   0        0        0      593 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/setup/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.6.0/examples/setup/nxc.json
+-rw-r--r--   0        0        0     2917 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/examples/setup/setup.toml
+-rw-r--r--   0        0        0      691 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/examples/shared-directories-users/composition.nix
+-rw-r--r--   0        0        0      807 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/examples/shared-directories-users/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/examples/shared-directories-users/nxc.json
+-rw-r--r--   0        0        0      600 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/examples/webserver/composition.nix
+-rw-r--r--   0        0        0      571 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/examples/webserver/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/examples/webserver/nxc.json
+-rw-r--r--   0        0        0     1262 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/nix/all-in-one.nix
+-rw-r--r--   0        0        0     4160 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/nix/compose.nix
+-rw-r--r--   0        0        0     3246 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/docker/generate_docker_compose.nix
+-rw-r--r--   0        0        0      569 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/docker/generate_image.nix
+-rw-r--r--   0        0        0      816 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/docker/nxc-shared-dirs-docker.nix
+-rw-r--r--   0        0        0      864 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/docker/systemd.nix
+-rw-r--r--   0        0        0      229 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/nix/flavours/docker.nix
+-rw-r--r--   0        0        0      731 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/g5k-image.nix
+-rw-r--r--   0        0        0     1966 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/g5k-nfs-store.nix
+-rw-r--r--   0        0        0      273 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/g5k-ramdisk.nix
+-rw-r--r--   0        0        0      533 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/nspawn/base.nix
+-rw-r--r--   0        0        0     1982 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/nspawn/generate_nspawn_compose.nix
+-rw-r--r--   0        0        0      469 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/nspawn.nix
+-rw-r--r--   0        0        0     1572 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/shared/base-hardware.nix
+-rw-r--r--   0        0        0     1595 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/shared/base-vm.nix
+-rw-r--r--   0        0        0      233 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/shared/base.nix
+-rw-r--r--   0        0        0     5217 2024-03-24 20:19:40.908081 nixos_compose-0.6.0/nix/flavours/shared/common.nix
+-rw-r--r--   0        0        0     1081 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/shared/g5k-common.nix
+-rw-r--r--   0        0        0     1034 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/shared/g5k-ssh-host-keys.nix
+-rw-r--r--   0        0        0     3548 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/shared/installation-device.nix
+-rw-r--r--   0        0        0     2164 2024-01-11 17:28:25.801006 nixos_compose-0.6.0/nix/flavours/shared/netboot.nix
+-rw-r--r--   0        0        0     1117 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/flavours/shared/nxc-shared-dirs-nfs.nix
+-rw-r--r--   0        0        0     6708 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/flavours/shared/nxc.nix
+-rw-r--r--   0        0        0     4183 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/flavours/shared/ssh-keys.nix
+-rw-r--r--   0        0        0     6531 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/flavours/shared/stage-1-cmds.nix
+-rw-r--r--   0        0        0     4044 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/flavours/shared/vm-stage-1-cmds.nix
+-rw-r--r--   0        0        0      435 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/flavours/vm-ramdisk.nix
+-rw-r--r--   0        0        0     1440 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/flavours/vm.nix
+-rw-r--r--   0        0        0     1076 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/nix/flavours.json
+-rw-r--r--   0        0        0      321 2024-01-11 17:28:25.800006 nixos_compose-0.6.0/nix/flavours.nix
+-rw-r--r--   0        0        0      485 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/flavours2json.nix
+-rw-r--r--   0        0        0     1970 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/generate_one_composition_info.nix
+-rw-r--r--   0        0        0     1830 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/helpers.nix
+-rw-r--r--   0        0        0      421 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/lib.nix
+-rw-r--r--   0        0        0     1625 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/make-system-tarball.nix
+-rw-r--r--   0        0        0     1540 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/make-system-tarball.sh
+-rw-r--r--   0        0        0     6485 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/multiple_compositions.nix
+-rw-r--r--   0        0        0      989 2024-01-11 17:28:25.802006 nixos_compose-0.6.0/nix/nur.nix
+-rw-r--r--   0        0        0      973 2024-01-11 17:28:25.803006 nixos_compose-0.6.0/nix/one_composition.nix
+-rw-r--r--   0        0        0     7234 2024-01-11 17:28:25.803006 nixos_compose-0.6.0/nix/setup.nix
+-rw-r--r--   0        0        0        0 2024-01-11 17:28:25.803006 nixos_compose-0.6.0/nixos_compose/__init__.py
+-rw-r--r--   0        0        0    32408 2024-05-28 08:47:48.798987 nixos_compose-0.6.0/nixos_compose/actions.py
+-rw-r--r--   0        0        0     1851 2024-03-24 20:20:27.989890 nixos_compose-0.6.0/nixos_compose/cli.py
+-rw-r--r--   0        0        0        0 2024-01-11 17:28:25.803006 nixos_compose-0.6.0/nixos_compose/commands/__init__.py
+-rw-r--r--   0        0        0     9271 2024-03-24 20:20:27.989890 nixos_compose-0.6.0/nixos_compose/commands/cmd_build.py
+-rw-r--r--   0        0        0      553 2024-01-11 17:28:25.803006 nixos_compose-0.6.0/nixos_compose/commands/cmd_clean.py
+-rw-r--r--   0        0        0     2800 2024-03-24 20:20:27.989890 nixos_compose-0.6.0/nixos_compose/commands/cmd_connect.py
+-rw-r--r--   0        0        0     3455 2024-03-24 20:20:27.989890 nixos_compose-0.6.0/nixos_compose/commands/cmd_driver.py
+-rw-r--r--   0        0        0     2646 2024-01-11 17:28:25.804006 nixos_compose-0.6.0/nixos_compose/commands/cmd_helper.py
+-rw-r--r--   0        0        0     4974 2024-01-11 17:28:25.804006 nixos_compose-0.6.0/nixos_compose/commands/cmd_init.py
+-rw-r--r--   0        0        0    15305 2024-05-28 08:47:48.799987 nixos_compose-0.6.0/nixos_compose/commands/cmd_start.py
+-rw-r--r--   0        0        0     1829 2024-01-11 17:28:25.804006 nixos_compose-0.6.0/nixos_compose/commands/cmd_stop.py
+-rw-r--r--   0        0        0     9518 2024-01-11 17:28:25.804006 nixos_compose-0.6.0/nixos_compose/context.py
+-rw-r--r--   0        0        0      391 2024-01-11 17:28:25.804006 nixos_compose-0.6.0/nixos_compose/default_role.py
+-rwxr-xr-x   0        0        0      522 2024-01-11 17:28:25.805006 nixos_compose-0.6.0/nixos_compose/driver/__init__.py
+-rw-r--r--   0        0        0     5389 2024-01-11 17:28:25.805006 nixos_compose-0.6.0/nixos_compose/driver/driver.py
+-rw-r--r--   0        0        0     3250 2024-01-11 17:28:25.805006 nixos_compose-0.6.0/nixos_compose/driver/logger.py
+-rw-r--r--   0        0        0    31276 2024-01-11 17:28:25.805006 nixos_compose-0.6.0/nixos_compose/driver/machine.py
+-rw-r--r--   0        0        0     3424 2024-03-24 20:20:27.989890 nixos_compose-0.6.0/nixos_compose/driver/vlan.py
+-rw-r--r--   0        0        0      869 2024-03-24 20:20:27.989890 nixos_compose-0.6.0/nixos_compose/flavour.py
+-rw-r--r--   0        0        0     1606 2024-01-11 17:28:25.806006 nixos_compose-0.6.0/nixos_compose/flavours/__init__.py
+-rw-r--r--   0        0        0     9876 2024-03-24 20:20:27.990890 nixos_compose-0.6.0/nixos_compose/flavours/docker.py
+-rw-r--r--   0        0        0     8092 2024-05-28 08:47:48.800988 nixos_compose-0.6.0/nixos_compose/flavours/grid5000.py
+-rwxr-xr-x   0        0        0     1799 2024-01-11 17:28:25.806006 nixos_compose-0.6.0/nixos_compose/flavours/nspawn/machine-dir.sh
+-rwxr-xr-x   0        0        0     8836 2024-01-11 17:28:25.806006 nixos_compose-0.6.0/nixos_compose/flavours/nspawn/nxc-net.sh
+-rw-r--r--   0        0        0    11435 2024-03-24 20:20:27.990890 nixos_compose-0.6.0/nixos_compose/flavours/nspawn.py
+-rw-r--r--   0        0        0     7158 2024-03-24 20:20:27.990890 nixos_compose-0.6.0/nixos_compose/flavours/vm.py
+-rw-r--r--   0        0        0      602 2024-01-11 17:28:25.807006 nixos_compose-0.6.0/nixos_compose/g5k.py
+-rw-r--r--   0        0        0     2187 2024-01-11 17:28:25.807006 nixos_compose-0.6.0/nixos_compose/httpd.py
+-rw-r--r--   0        0        0     3568 2024-05-28 08:47:48.801988 nixos_compose-0.6.0/nixos_compose/nxc_execo.py
+-rw-r--r--   0        0        0     3747 2024-01-11 17:28:25.807006 nixos_compose-0.6.0/nixos_compose/platform.py
+-rw-r--r--   0        0        0     4033 2024-01-11 17:28:25.807006 nixos_compose-0.6.0/nixos_compose/setup.py
+-rw-r--r--   0        0        0      953 2024-01-11 17:28:25.807006 nixos_compose-0.6.0/nixos_compose/state.py
+-rw-r--r--   0        0        0        0 2024-01-11 17:28:25.807006 nixos_compose-0.6.0/nixos_compose/tools/__init__.py
+-rwxr-xr-x   0        0        0      248 2024-01-11 17:28:25.807006 nixos_compose-0.6.0/nixos_compose/tools/g5k_set_pub_key_sleep.sh
+-rwxr-xr-x   0        0        0     5009 2024-01-11 17:28:25.808006 nixos_compose-0.6.0/nixos_compose/tools/kataract.py
+-rw-r--r--   0        0        0     5916 2024-01-11 17:28:25.808006 nixos_compose-0.6.0/nixos_compose/tools/nested_deployment.py
+-rw-r--r--   0        0        0     2372 2024-01-11 17:28:25.808006 nixos_compose-0.6.0/nixos_compose/utils.py
+-rw-r--r--   0        0        0     1064 2024-05-28 08:47:48.801988 nixos_compose-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 nixos_compose-0.6.0/PKG-INFO
```

### Comparing `nixos_compose-0.5.6/LICENSE` & `nixos_compose-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/basic/flake.nix` & `nixos_compose-0.6.0/examples/basic/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/basic-nur/flake.nix` & `nixos_compose-0.6.0/examples/basic-nur/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/execo/flake.nix` & `nixos_compose-0.6.0/examples/execo/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/flake.lock` & `nixos_compose-0.6.0/examples/flake.lock`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/kernel/flake.nix` & `nixos_compose-0.6.0/examples/kernel/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/kernel/linux_ipanema_5_4.nix` & `nixos_compose-0.6.0/examples/kernel/linux_ipanema_5_4.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/multi-compositions/flake.nix` & `nixos_compose-0.6.0/examples/multi-compositions/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/nbp-mpi/composition.nix` & `nixos_compose-0.6.0/examples/nbp-mpi/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/nbp-mpi/flake.nix` & `nixos_compose-0.6.0/examples/nbp-mpi/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/nix_flake_templates.nix` & `nixos_compose-0.6.0/examples/nix_flake_templates.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/nixos-cluster/composition.nix` & `nixos_compose-0.6.0/examples/nixos-cluster/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/nixos-cluster/flake.nix` & `nixos_compose-0.6.0/examples/nixos-cluster/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/nixos-cluster/ssh-keys.nix` & `nixos_compose-0.6.0/examples/nixos-cluster/ssh-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/scripts/flake.nix` & `nixos_compose-0.6.0/examples/scripts/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/setup/flake.nix` & `nixos_compose-0.6.0/examples/setup/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/setup/setup.toml` & `nixos_compose-0.6.0/examples/setup/setup.toml`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/shared-directories-users/composition.nix` & `nixos_compose-0.6.0/examples/shared-directories-users/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/shared-directories-users/flake.nix` & `nixos_compose-0.6.0/examples/shared-directories-users/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/webserver/composition.nix` & `nixos_compose-0.6.0/examples/webserver/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/examples/webserver/flake.nix` & `nixos_compose-0.6.0/examples/webserver/flake.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/all-in-one.nix` & `nixos_compose-0.6.0/nix/all-in-one.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/compose.nix` & `nixos_compose-0.6.0/nix/compose.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/docker/generate_docker_compose.nix` & `nixos_compose-0.6.0/nix/flavours/docker/generate_docker_compose.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/docker/generate_image.nix` & `nixos_compose-0.6.0/nix/flavours/docker/generate_image.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/docker/nxc-shared-dirs-docker.nix` & `nixos_compose-0.6.0/nix/flavours/docker/nxc-shared-dirs-docker.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/docker/systemd.nix` & `nixos_compose-0.6.0/nix/flavours/docker/systemd.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/g5k-image.nix` & `nixos_compose-0.6.0/nix/flavours/g5k-image.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/g5k-nfs-store.nix` & `nixos_compose-0.6.0/nix/flavours/g5k-nfs-store.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/nspawn/base.nix` & `nixos_compose-0.6.0/nix/flavours/nspawn/base.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/nspawn/generate_nspawn_compose.nix` & `nixos_compose-0.6.0/nix/flavours/nspawn/generate_nspawn_compose.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/base-hardware.nix` & `nixos_compose-0.6.0/nix/flavours/shared/base-hardware.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/base-vm.nix` & `nixos_compose-0.6.0/nix/flavours/shared/base-vm.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/common.nix` & `nixos_compose-0.6.0/nix/flavours/shared/common.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/g5k-common.nix` & `nixos_compose-0.6.0/nix/flavours/shared/g5k-common.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/g5k-ssh-host-keys.nix` & `nixos_compose-0.6.0/nix/flavours/shared/g5k-ssh-host-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/installation-device.nix` & `nixos_compose-0.6.0/nix/flavours/shared/installation-device.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/netboot.nix` & `nixos_compose-0.6.0/nix/flavours/shared/netboot.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/nxc-shared-dirs-nfs.nix` & `nixos_compose-0.6.0/nix/flavours/shared/nxc-shared-dirs-nfs.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/nxc.nix` & `nixos_compose-0.6.0/nix/flavours/shared/nxc.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/ssh-keys.nix` & `nixos_compose-0.6.0/nix/flavours/shared/ssh-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/stage-1-cmds.nix` & `nixos_compose-0.6.0/nix/flavours/shared/stage-1-cmds.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/shared/vm-stage-1-cmds.nix` & `nixos_compose-0.6.0/nix/flavours/shared/vm-stage-1-cmds.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours/vm.nix` & `nixos_compose-0.6.0/nix/flavours/vm.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/flavours.json` & `nixos_compose-0.6.0/nix/flavours.json`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/generate_one_composition_info.nix` & `nixos_compose-0.6.0/nix/generate_one_composition_info.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/helpers.nix` & `nixos_compose-0.6.0/nix/helpers.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/make-system-tarball.nix` & `nixos_compose-0.6.0/nix/make-system-tarball.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/make-system-tarball.sh` & `nixos_compose-0.6.0/nix/make-system-tarball.sh`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/multiple_compositions.nix` & `nixos_compose-0.6.0/nix/multiple_compositions.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/nur.nix` & `nixos_compose-0.6.0/nix/nur.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/one_composition.nix` & `nixos_compose-0.6.0/nix/one_composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nix/setup.nix` & `nixos_compose-0.6.0/nix/setup.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/actions.py` & `nixos_compose-0.6.0/nixos_compose/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     with open(realpath_from_store(ctx, filename), "r") as f:
         test_script = f.read()
         return test_script
 
 
 def read_compose_info(ctx):
     if not op.isfile(ctx.compose_info_file):
-        raise click.ClickException(f"{ctx.compose_info_filename} does not exist")
+        raise click.ClickException(f"{ctx.compose_info_file} does not exist")
     with open(ctx.compose_info_file, "r") as f:
         compose_info = json.load(f)
 
     if "compositions_info" in compose_info:
         ctx.compositions_info = compose_info
 
         if len(compose_info["compositions_info"]) > 1:
```

### Comparing `nixos_compose-0.5.6/nixos_compose/cli.py` & `nixos_compose-0.6.0/nixos_compose/cli.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/commands/cmd_build.py` & `nixos_compose-0.6.0/nixos_compose/commands/cmd_build.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/commands/cmd_clean.py` & `nixos_compose-0.6.0/nixos_compose/commands/cmd_clean.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/commands/cmd_connect.py` & `nixos_compose-0.6.0/nixos_compose/commands/cmd_connect.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/commands/cmd_driver.py` & `nixos_compose-0.6.0/nixos_compose/commands/cmd_driver.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/commands/cmd_helper.py` & `nixos_compose-0.6.0/nixos_compose/commands/cmd_helper.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/commands/cmd_init.py` & `nixos_compose-0.6.0/nixos_compose/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/commands/cmd_start.py` & `nixos_compose-0.6.0/nixos_compose/commands/cmd_start.py`

 * *Files 2% similar despite different names*

```diff
@@ -494,21 +494,26 @@
         ctx.compose_info_file = realpath_from_store(ctx, compose_info)
         ctx.composition_flavour_prefix = op.basename(compose_info)
         ctx.composition_name = "composition"
         ctx.composition_basename_file = ctx.composition_name
     else:
         ctx.compose_info_file = realpath_from_store(ctx, build_path)
 
-    if ctx.platform:
-        if reuse:
-            (ssh, sudo, push_path) = ctx.platform.subsequent_start_values
-        else:
-            (ssh, sudo, push_path) = ctx.platform.first_start_values
-        if ctx.push_path is None:
-            ctx.push_path = push_path
+    #
+    # ssh not used, subsequent_start_values and first_start_values not use w/
+    # nfs mount on g5k. If not need on other platform to REMOVE (see also platform.py
+    # Only depends of flavours or plaforms
+    #
+    # if ctx.platform:
+    #     if reuse:
+    #         (ssh, sudo, push_path) = ctx.platform.subsequent_start_values
+    #     else:
+    #         (ssh, sudo, push_path) = ctx.platform.first_start_values
+    #     if ctx.push_path is None:
+    #         ctx.push_path = push_path
 
     if machine_file:
         machines = read_hosts(machine_file)
         if not machines:
             ctx.elog(f"Machine file '{machine_file}' is empty")
             sys.exit(1)
```

### Comparing `nixos_compose-0.5.6/nixos_compose/commands/cmd_stop.py` & `nixos_compose-0.6.0/nixos_compose/commands/cmd_stop.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/context.py` & `nixos_compose-0.6.0/nixos_compose/context.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/driver/__init__.py` & `nixos_compose-0.6.0/nixos_compose/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/driver/driver.py` & `nixos_compose-0.6.0/nixos_compose/driver/driver.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/driver/logger.py` & `nixos_compose-0.6.0/nixos_compose/driver/logger.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/driver/machine.py` & `nixos_compose-0.6.0/nixos_compose/driver/machine.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/driver/vlan.py` & `nixos_compose-0.6.0/nixos_compose/driver/vlan.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/flavour.py` & `nixos_compose-0.6.0/nixos_compose/flavour.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/flavours/__init__.py` & `nixos_compose-0.6.0/nixos_compose/flavours/__init__.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/flavours/docker.py` & `nixos_compose-0.6.0/nixos_compose/flavours/docker.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/flavours/grid5000.py` & `nixos_compose-0.6.0/nixos_compose/flavours/grid5000.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
             kernel_params=f"boot.shell_on_fail console=tty0 console=ttyS0,115200 deploy={deploy} {additional_kernel_params} {kernel_params}",
         )
         kaenv_file.write(kaenv)
 
 
 class G5kKexecBasedFlavour(Flavour):
     def __init__(self, ctx):
+        if ctx.ssh == "":
+            ctx.ssh = "ssh -l root"
         super().__init__(ctx)
 
     def generate_deployment_info(self, ssh_pub_key_file=None):
         generate_deployment_info(self.ctx, ssh_pub_key_file)
 
     def generate_kexec_scripts(self):
         generate_kexec_scripts(self.ctx)
```

### Comparing `nixos_compose-0.5.6/nixos_compose/flavours/nspawn/machine-dir.sh` & `nixos_compose-0.6.0/nixos_compose/flavours/nspawn/machine-dir.sh`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/flavours/nspawn/nxc-net.sh` & `nixos_compose-0.6.0/nixos_compose/flavours/nspawn/nxc-net.sh`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/flavours/nspawn.py` & `nixos_compose-0.6.0/nixos_compose/flavours/nspawn.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/flavours/vm.py` & `nixos_compose-0.6.0/nixos_compose/flavours/vm.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/g5k.py` & `nixos_compose-0.6.0/nixos_compose/g5k.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/httpd.py` & `nixos_compose-0.6.0/nixos_compose/httpd.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/nxc_execo.py` & `nixos_compose-0.6.0/nixos_compose/nxc_execo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,17 @@
-# import execo
-# import execo_g5k
-# import execo_engine
-# from execo import Process, Host, Remote, SshProcess, Report
 from execo import Host
 from execo_g5k import get_oar_job_nodes
 
-#     get_oar_job_nodes,
-#     oarsub,
-#     oardel,
-#     OarSubmission,
-#     wait_oar_job_start,
-# )
-# from execo_engine import Engine
 import os
 import os.path as op
 
-# import time
-# import logging
 import tempfile
 from .context import Context
 from .actions import realpath_from_store, translate_hosts2ip
-from .flavours.grid5000 import G5kRamdiskFlavour, G5KImageFlavour, G5kNfsStoreFlavour
+from .flavours import get_flavour_by_name
 
 # from .g5k import key_sleep_script
 from .httpd import HTTPDaemon
 
 
 def get_envdir(ctx):
     if os.path.isfile("nxc.json"):
@@ -40,71 +27,59 @@
         raise Exception("Cannot find `nxc.json`")
 
 
 def get_oar_job_nodes_nxc(
     oar_job_id,
     site,
     compose_info_file=None,
-    flavour_name="g5k-ramdisk",
+    flavour_name="g5k-nfs-store",
     composition_name="composition",
     roles_quantities={},
     port=0,
 ):
     """
     Brother of the "get_oar_job_nodes" function from execo
     but does the mapping with roles from NXC
     """
     ctx = Context()
     # TODO: kaberk
     ctx.composition_name = composition_name
     ctx.flavour_name = flavour_name
+    ctx.composition_flavour_prefix = f"{composition_name}::{flavour_name}"
     ctx.roles_distribution = roles_quantities
 
     ctx.envdir = None
     get_envdir(ctx)
 
     if compose_info_file:
         ctx.compose_info_file = compose_info_file
     else:
         build_folder = op.join(ctx.envdir, "build")
         simlink_build = op.join(
             build_folder, f"{ctx.composition_name}::{ctx.flavour_name}"
         )
         ctx.compose_info_file = realpath_from_store(ctx, simlink_build)
 
+    flavour = get_flavour_by_name(flavour_name)(ctx)
+    ctx.flavour = flavour
+
     # print(f"compose info file: {ctx.compose_info_file}")
 
     g5k_nodes = get_oar_job_nodes(oar_job_id, site)
     print(f"G5K nodes: {g5k_nodes}")
     machines = [node.address for node in g5k_nodes]
     if len(machines) > 4:
         ctx.use_http = True
         ctx.httpd = HTTPDaemon(ctx=ctx, port=port)
         ctx.httpd.start(directory=ctx.envdir)
     translate_hosts2ip(ctx, machines)
 
-    if flavour_name == "g5k-ramdisk":
-        flavour = G5kRamdiskFlavour(ctx)
-    elif flavour_name == "g5k-nfs-store":
-        flavour = G5kNfsStoreFlavour(ctx)
-    elif flavour_name == "g5k-image":
-        flavour = G5KImageFlavour(ctx)
-    else:
-        raise Exception(f"'{flavour_name}' is not an available flavour")
-    # ?!
-    flavour.ctx.flavour = flavour
-
-    print("generating deploy info")
     flavour.generate_deployment_info()
 
-    # flavour.ctx.ssh = f"OAR_JOB_ID={oar_job_id} oarsh"
-    flavour.ctx.ssh = "ssh"
-    flavour.ctx.sudo = "sudo-g5k"
-
-    flavour.ctx.log("Deploying")
+    ctx.log("Deploying")
     if hasattr(flavour, "generate_kexec_scripts"):
         flavour.generate_kexec_scripts()
         flavour.launch()
     else:
         user = os.environ["USER"]
         tempfile.tempdir = f"/home/{user}/public"
         tmp = tempfile.NamedTemporaryFile(delete=False)
```

### Comparing `nixos_compose-0.5.6/nixos_compose/platform.py` & `nixos_compose-0.6.0/nixos_compose/platform.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/setup.py` & `nixos_compose-0.6.0/nixos_compose/setup.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/state.py` & `nixos_compose-0.6.0/nixos_compose/state.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/tools/kataract.py` & `nixos_compose-0.6.0/nixos_compose/tools/kataract.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/tools/nested_deployment.py` & `nixos_compose-0.6.0/nixos_compose/tools/nested_deployment.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/nixos_compose/utils.py` & `nixos_compose-0.6.0/nixos_compose/utils.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.6/pyproject.toml` & `nixos_compose-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nixos-compose"
-version = "0.5.6"
+version = "0.6.0"
 description = ""
 authors = ["Olivier Richard <olivier.richard@imag.fr>"]
 license = "MIT"
 include = [
      { path = 'examples', format = 'wheel' },
      { path = 'nix', format = 'wheel' },
      #{ path = 'tools', format = 'wheel' }
```

### Comparing `nixos_compose-0.5.6/PKG-INFO` & `nixos_compose-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nixos-compose
-Version: 0.5.6
+Version: 0.6.0
 Summary: 
 License: MIT
 Author: Olivier Richard
 Author-email: olivier.richard@imag.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

