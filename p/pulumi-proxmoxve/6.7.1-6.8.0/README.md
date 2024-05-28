# Comparing `tmp/pulumi_proxmoxve-6.7.1.tar.gz` & `tmp/pulumi_proxmoxve-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-6.7.1.tar", last modified: Wed May 22 16:13:12 2024, max compression
+gzip compressed data, was "pulumi_proxmoxve-6.8.0.tar", last modified: Tue May 28 09:20:39 2024, max compression
```

## Comparing `pulumi_proxmoxve-6.7.1.tar` & `pulumi_proxmoxve-6.8.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.031790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29531 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.031790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.031790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36258 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64491 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/download/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38006 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/download/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/get_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/get_vm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/ha_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/get_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/get_pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/get_usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.039790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    32979 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24800 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/network_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/network_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16471 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.039790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25525 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.039790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/user/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16708 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/user/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87349 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    75190 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   123851 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.031790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33026 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37116 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64491 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32310 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.659774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38006 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/get_vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.659774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/ha_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.659774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/get_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.659774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/get_pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/get_usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.663775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32979 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24800 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/network_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/network_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25525 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16708 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/user/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90275 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77594 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123851 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25922 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:20:39.655774 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:20:39.667775 pulumi_proxmoxve-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-28 09:20:39.000000 pulumi_proxmoxve-6.8.0/setup.py
```

### Comparing `pulumi_proxmoxve-6.7.1/PKG-INFO` & `pulumi_proxmoxve-6.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 6.7.1
+Version: 6.8.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.7.1/README.md` & `pulumi_proxmoxve-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/_inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 __all__ = [
     'HostsEntryArgs',
     'ProviderSshArgs',
     'ProviderSshNodeArgs',
     'Vm2CloneArgs',
     'Vm2CpuArgs',
     'Vm2TimeoutsArgs',
+    'Vm2VgaArgs',
     'GetVm2CloneArgs',
     'GetVm2CpuArgs',
     'GetVm2TimeoutsArgs',
+    'GetVm2VgaArgs',
 ]
 
 @pulumi.input_type
 class HostsEntryArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
                  hostnames: pulumi.Input[Sequence[pulumi.Input[str]]]):
@@ -535,14 +537,69 @@
 
     @update.setter
     def update(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "update", value)
 
 
 @pulumi.input_type
+class Vm2VgaArgs:
+    def __init__(__self__, *,
+                 clipboard: Optional[pulumi.Input[str]] = None,
+                 memory: Optional[pulumi.Input[int]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] clipboard: Enable a specific clipboard. If not set, depending on the display type the SPICE one will be added. Currently only `vnc` is available. Migration with VNC clipboard is not supported by Proxmox.
+        :param pulumi.Input[int] memory: The VGA memory in megabytes (4-512 MB). Has no effect with serial display.
+        :param pulumi.Input[str] type: The VGA type (defaults to `std`).
+        """
+        if clipboard is not None:
+            pulumi.set(__self__, "clipboard", clipboard)
+        if memory is not None:
+            pulumi.set(__self__, "memory", memory)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def clipboard(self) -> Optional[pulumi.Input[str]]:
+        """
+        Enable a specific clipboard. If not set, depending on the display type the SPICE one will be added. Currently only `vnc` is available. Migration with VNC clipboard is not supported by Proxmox.
+        """
+        return pulumi.get(self, "clipboard")
+
+    @clipboard.setter
+    def clipboard(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "clipboard", value)
+
+    @property
+    @pulumi.getter
+    def memory(self) -> Optional[pulumi.Input[int]]:
+        """
+        The VGA memory in megabytes (4-512 MB). Has no effect with serial display.
+        """
+        return pulumi.get(self, "memory")
+
+    @memory.setter
+    def memory(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "memory", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The VGA type (defaults to `std`).
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+
+@pulumi.input_type
 class GetVm2CloneArgs:
     def __init__(__self__, *,
                  id: int,
                  retries: int):
         """
         :param int id: The ID of the VM to clone.
         :param int retries: The number of retries to perform when cloning the VM (default: 3).
@@ -751,7 +808,59 @@
         return pulumi.get(self, "read")
 
     @read.setter
     def read(self, value: Optional[str]):
         pulumi.set(self, "read", value)
 
 
+@pulumi.input_type
+class GetVm2VgaArgs:
+    def __init__(__self__, *,
+                 clipboard: str,
+                 memory: int,
+                 type: str):
+        """
+        :param str clipboard: Enable a specific clipboard.
+        :param int memory: The VGA memory in megabytes (4-512 MB). Has no effect with serial display.
+        :param str type: The VGA type.
+        """
+        pulumi.set(__self__, "clipboard", clipboard)
+        pulumi.set(__self__, "memory", memory)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def clipboard(self) -> str:
+        """
+        Enable a specific clipboard.
+        """
+        return pulumi.get(self, "clipboard")
+
+    @clipboard.setter
+    def clipboard(self, value: str):
+        pulumi.set(self, "clipboard", value)
+
+    @property
+    @pulumi.getter
+    def memory(self) -> int:
+        """
+        The VGA memory in megabytes (4-512 MB). Has no effect with serial display.
+        """
+        return pulumi.get(self, "memory")
+
+    @memory.setter
+    def memory(self, value: int):
+        pulumi.set(self, "memory", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        The VGA type.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: str):
+        pulumi.set(self, "type", value)
+
+
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/acl.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/_inputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/options.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/cluster/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,17 +392,19 @@
 @pulumi.input_type
 class ContainerInitializationDnsArgs:
     def __init__(__self__, *,
                  domain: Optional[pulumi.Input[str]] = None,
                  server: Optional[pulumi.Input[str]] = None,
                  servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[str] domain: The DNS search domain
-        :param pulumi.Input[str] server: The DNS server
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The list of DNS servers
+        :param pulumi.Input[str] domain: The DNS search domain.
+        :param pulumi.Input[str] server: The DNS server. The `server` attribute is
+               deprecated and will be removed in a future release. Please use
+               the `servers` attribute instead.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The list of DNS servers.
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if server is not None:
             warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
             pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
         if server is not None:
@@ -410,198 +412,208 @@
         if servers is not None:
             pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS search domain
+        The DNS search domain.
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter
     def server(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS server
+        The DNS server. The `server` attribute is
+        deprecated and will be removed in a future release. Please use
+        the `servers` attribute instead.
         """
         warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
         pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
 
         return pulumi.get(self, "server")
 
     @server.setter
     def server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server", value)
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The list of DNS servers
+        The list of DNS servers.
         """
         return pulumi.get(self, "servers")
 
     @servers.setter
     def servers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "servers", value)
 
 
 @pulumi.input_type
 class ContainerInitializationIpConfigArgs:
     def __init__(__self__, *,
                  ipv4: Optional[pulumi.Input['ContainerInitializationIpConfigIpv4Args']] = None,
                  ipv6: Optional[pulumi.Input['ContainerInitializationIpConfigIpv6Args']] = None):
         """
-        :param pulumi.Input['ContainerInitializationIpConfigIpv4Args'] ipv4: The IPv4 configuration
-        :param pulumi.Input['ContainerInitializationIpConfigIpv6Args'] ipv6: The IPv6 configuration
+        :param pulumi.Input['ContainerInitializationIpConfigIpv4Args'] ipv4: The IPv4 configuration.
+        :param pulumi.Input['ContainerInitializationIpConfigIpv6Args'] ipv6: The IPv4 configuration.
         """
         if ipv4 is not None:
             pulumi.set(__self__, "ipv4", ipv4)
         if ipv6 is not None:
             pulumi.set(__self__, "ipv6", ipv6)
 
     @property
     @pulumi.getter
     def ipv4(self) -> Optional[pulumi.Input['ContainerInitializationIpConfigIpv4Args']]:
         """
-        The IPv4 configuration
+        The IPv4 configuration.
         """
         return pulumi.get(self, "ipv4")
 
     @ipv4.setter
     def ipv4(self, value: Optional[pulumi.Input['ContainerInitializationIpConfigIpv4Args']]):
         pulumi.set(self, "ipv4", value)
 
     @property
     @pulumi.getter
     def ipv6(self) -> Optional[pulumi.Input['ContainerInitializationIpConfigIpv6Args']]:
         """
-        The IPv6 configuration
+        The IPv4 configuration.
         """
         return pulumi.get(self, "ipv6")
 
     @ipv6.setter
     def ipv6(self, value: Optional[pulumi.Input['ContainerInitializationIpConfigIpv6Args']]):
         pulumi.set(self, "ipv6", value)
 
 
 @pulumi.input_type
 class ContainerInitializationIpConfigIpv4Args:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  gateway: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: The IPv4 address
-        :param pulumi.Input[str] gateway: The IPv4 gateway
+        :param pulumi.Input[str] address: The IPv4 address (use `dhcp` for
+               autodiscovery).
+        :param pulumi.Input[str] gateway: The IPv4 gateway (must be omitted
+               when `dhcp` is used as the address).
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv4 address
+        The IPv4 address (use `dhcp` for
+        autodiscovery).
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv4 gateway
+        The IPv4 gateway (must be omitted
+        when `dhcp` is used as the address).
         """
         return pulumi.get(self, "gateway")
 
     @gateway.setter
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
 
 @pulumi.input_type
 class ContainerInitializationIpConfigIpv6Args:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  gateway: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: The IPv6 address
-        :param pulumi.Input[str] gateway: The IPv6 gateway
+        :param pulumi.Input[str] address: The IPv6 address (use `dhcp` for
+               autodiscovery).
+        :param pulumi.Input[str] gateway: The IPv6 gateway (must be omitted
+               when `dhcp` is used as the address).
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 address
+        The IPv6 address (use `dhcp` for
+        autodiscovery).
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 gateway
+        The IPv6 gateway (must be omitted
+        when `dhcp` is used as the address).
         """
         return pulumi.get(self, "gateway")
 
     @gateway.setter
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
 
 @pulumi.input_type
 class ContainerInitializationUserAccountArgs:
     def __init__(__self__, *,
                  keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  password: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: The SSH keys
-        :param pulumi.Input[str] password: The SSH password
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: The SSH keys for the root account.
+        :param pulumi.Input[str] password: The password for the root account.
         """
         if keys is not None:
             pulumi.set(__self__, "keys", keys)
         if password is not None:
             pulumi.set(__self__, "password", password)
 
     @property
     @pulumi.getter
     def keys(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The SSH keys
+        The SSH keys for the root account.
         """
         return pulumi.get(self, "keys")
 
     @keys.setter
     def keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "keys", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH password
+        The password for the root account.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
@@ -663,15 +675,15 @@
         """
         :param pulumi.Input[str] path: Path to the mount point as seen from inside the
                container.
         :param pulumi.Input[str] volume: Volume, device or directory to mount into the
                container.
         :param pulumi.Input[bool] acl: Explicitly enable or disable ACL support.
         :param pulumi.Input[bool] backup: Whether to include the mount point in backups (only
-               used for volume mount points).
+               used for volume mount points, defaults to `false`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] mount_options: List of extra mount options.
         :param pulumi.Input[bool] quota: Enable user quotas inside the container (not supported
                with ZFS subvolumes).
         :param pulumi.Input[bool] read_only: Read-only mount point.
         :param pulumi.Input[bool] replicate: Will include this volume to a storage replica job.
         :param pulumi.Input[bool] shared: Mark this non-volume mount point as available on all
                nodes.
@@ -736,15 +748,15 @@
         pulumi.set(self, "acl", value)
 
     @property
     @pulumi.getter
     def backup(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to include the mount point in backups (only
-        used for volume mount points).
+        used for volume mount points, defaults to `false`).
         """
         return pulumi.get(self, "backup")
 
     @backup.setter
     def backup(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "backup", value)
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -391,173 +391,185 @@
 @pulumi.output_type
 class ContainerInitializationDns(dict):
     def __init__(__self__, *,
                  domain: Optional[str] = None,
                  server: Optional[str] = None,
                  servers: Optional[Sequence[str]] = None):
         """
-        :param str domain: The DNS search domain
-        :param str server: The DNS server
-        :param Sequence[str] servers: The list of DNS servers
+        :param str domain: The DNS search domain.
+        :param str server: The DNS server. The `server` attribute is
+               deprecated and will be removed in a future release. Please use
+               the `servers` attribute instead.
+        :param Sequence[str] servers: The list of DNS servers.
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if server is not None:
             pulumi.set(__self__, "server", server)
         if servers is not None:
             pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
         """
-        The DNS search domain
+        The DNS search domain.
         """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def server(self) -> Optional[str]:
         """
-        The DNS server
+        The DNS server. The `server` attribute is
+        deprecated and will be removed in a future release. Please use
+        the `servers` attribute instead.
         """
         warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
         pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
 
         return pulumi.get(self, "server")
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[Sequence[str]]:
         """
-        The list of DNS servers
+        The list of DNS servers.
         """
         return pulumi.get(self, "servers")
 
 
 @pulumi.output_type
 class ContainerInitializationIpConfig(dict):
     def __init__(__self__, *,
                  ipv4: Optional['outputs.ContainerInitializationIpConfigIpv4'] = None,
                  ipv6: Optional['outputs.ContainerInitializationIpConfigIpv6'] = None):
         """
-        :param 'ContainerInitializationIpConfigIpv4Args' ipv4: The IPv4 configuration
-        :param 'ContainerInitializationIpConfigIpv6Args' ipv6: The IPv6 configuration
+        :param 'ContainerInitializationIpConfigIpv4Args' ipv4: The IPv4 configuration.
+        :param 'ContainerInitializationIpConfigIpv6Args' ipv6: The IPv4 configuration.
         """
         if ipv4 is not None:
             pulumi.set(__self__, "ipv4", ipv4)
         if ipv6 is not None:
             pulumi.set(__self__, "ipv6", ipv6)
 
     @property
     @pulumi.getter
     def ipv4(self) -> Optional['outputs.ContainerInitializationIpConfigIpv4']:
         """
-        The IPv4 configuration
+        The IPv4 configuration.
         """
         return pulumi.get(self, "ipv4")
 
     @property
     @pulumi.getter
     def ipv6(self) -> Optional['outputs.ContainerInitializationIpConfigIpv6']:
         """
-        The IPv6 configuration
+        The IPv4 configuration.
         """
         return pulumi.get(self, "ipv6")
 
 
 @pulumi.output_type
 class ContainerInitializationIpConfigIpv4(dict):
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  gateway: Optional[str] = None):
         """
-        :param str address: The IPv4 address
-        :param str gateway: The IPv4 gateway
+        :param str address: The IPv4 address (use `dhcp` for
+               autodiscovery).
+        :param str gateway: The IPv4 gateway (must be omitted
+               when `dhcp` is used as the address).
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
         """
-        The IPv4 address
+        The IPv4 address (use `dhcp` for
+        autodiscovery).
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[str]:
         """
-        The IPv4 gateway
+        The IPv4 gateway (must be omitted
+        when `dhcp` is used as the address).
         """
         return pulumi.get(self, "gateway")
 
 
 @pulumi.output_type
 class ContainerInitializationIpConfigIpv6(dict):
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  gateway: Optional[str] = None):
         """
-        :param str address: The IPv6 address
-        :param str gateway: The IPv6 gateway
+        :param str address: The IPv6 address (use `dhcp` for
+               autodiscovery).
+        :param str gateway: The IPv6 gateway (must be omitted
+               when `dhcp` is used as the address).
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
         """
-        The IPv6 address
+        The IPv6 address (use `dhcp` for
+        autodiscovery).
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[str]:
         """
-        The IPv6 gateway
+        The IPv6 gateway (must be omitted
+        when `dhcp` is used as the address).
         """
         return pulumi.get(self, "gateway")
 
 
 @pulumi.output_type
 class ContainerInitializationUserAccount(dict):
     def __init__(__self__, *,
                  keys: Optional[Sequence[str]] = None,
                  password: Optional[str] = None):
         """
-        :param Sequence[str] keys: The SSH keys
-        :param str password: The SSH password
+        :param Sequence[str] keys: The SSH keys for the root account.
+        :param str password: The password for the root account.
         """
         if keys is not None:
             pulumi.set(__self__, "keys", keys)
         if password is not None:
             pulumi.set(__self__, "password", password)
 
     @property
     @pulumi.getter
     def keys(self) -> Optional[Sequence[str]]:
         """
-        The SSH keys
+        The SSH keys for the root account.
         """
         return pulumi.get(self, "keys")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         """
-        The SSH password
+        The password for the root account.
         """
         return pulumi.get(self, "password")
 
 
 @pulumi.output_type
 class ContainerMemory(dict):
     def __init__(__self__, *,
@@ -626,15 +638,15 @@
         """
         :param str path: Path to the mount point as seen from inside the
                container.
         :param str volume: Volume, device or directory to mount into the
                container.
         :param bool acl: Explicitly enable or disable ACL support.
         :param bool backup: Whether to include the mount point in backups (only
-               used for volume mount points).
+               used for volume mount points, defaults to `false`).
         :param Sequence[str] mount_options: List of extra mount options.
         :param bool quota: Enable user quotas inside the container (not supported
                with ZFS subvolumes).
         :param bool read_only: Read-only mount point.
         :param bool replicate: Will include this volume to a storage replica job.
         :param bool shared: Mark this non-volume mount point as available on all
                nodes.
@@ -687,15 +699,15 @@
         return pulumi.get(self, "acl")
 
     @property
     @pulumi.getter
     def backup(self) -> Optional[bool]:
         """
         Whether to include the mount point in backups (only
-        used for volume mount points).
+        used for volume mount points, defaults to `false`).
         """
         return pulumi.get(self, "backup")
 
     @property
     @pulumi.getter(name="mountOptions")
     def mount_options(self) -> Optional[Sequence[str]]:
         """
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/download/file.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/download/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/get_node.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/get_vm2.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/get_vm2.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 
 @pulumi.output_type
 class GetVm2Result:
     """
     A collection of values returned by getVm2.
     """
-    def __init__(__self__, clone=None, cpu=None, description=None, id=None, name=None, node_name=None, tags=None, template=None, timeouts=None):
+    def __init__(__self__, clone=None, cpu=None, description=None, id=None, name=None, node_name=None, tags=None, template=None, timeouts=None, vga=None):
         if clone and not isinstance(clone, dict):
             raise TypeError("Expected argument 'clone' to be a dict")
         pulumi.set(__self__, "clone", clone)
         if cpu and not isinstance(cpu, dict):
             raise TypeError("Expected argument 'cpu' to be a dict")
         pulumi.set(__self__, "cpu", cpu)
         if description and not isinstance(description, str):
@@ -47,14 +47,17 @@
         pulumi.set(__self__, "tags", tags)
         if template and not isinstance(template, bool):
             raise TypeError("Expected argument 'template' to be a bool")
         pulumi.set(__self__, "template", template)
         if timeouts and not isinstance(timeouts, dict):
             raise TypeError("Expected argument 'timeouts' to be a dict")
         pulumi.set(__self__, "timeouts", timeouts)
+        if vga and not isinstance(vga, dict):
+            raise TypeError("Expected argument 'vga' to be a dict")
+        pulumi.set(__self__, "vga", vga)
 
     @property
     @pulumi.getter
     def clone(self) -> Optional['outputs.GetVm2CloneResult']:
         """
         The cloning configuration.
         """
@@ -117,14 +120,22 @@
         return pulumi.get(self, "template")
 
     @property
     @pulumi.getter
     def timeouts(self) -> Optional['outputs.GetVm2TimeoutsResult']:
         return pulumi.get(self, "timeouts")
 
+    @property
+    @pulumi.getter
+    def vga(self) -> 'outputs.GetVm2VgaResult':
+        """
+        The VGA configuration.
+        """
+        return pulumi.get(self, "vga")
+
 
 class AwaitableGetVm2Result(GetVm2Result):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetVm2Result(
@@ -132,85 +143,92 @@
             cpu=self.cpu,
             description=self.description,
             id=self.id,
             name=self.name,
             node_name=self.node_name,
             tags=self.tags,
             template=self.template,
-            timeouts=self.timeouts)
+            timeouts=self.timeouts,
+            vga=self.vga)
 
 
 def get_vm2(clone: Optional[pulumi.InputType['GetVm2CloneArgs']] = None,
             cpu: Optional[pulumi.InputType['GetVm2CpuArgs']] = None,
             description: Optional[str] = None,
             id: Optional[int] = None,
             name: Optional[str] = None,
             node_name: Optional[str] = None,
             tags: Optional[Sequence[str]] = None,
             template: Optional[bool] = None,
             timeouts: Optional[pulumi.InputType['GetVm2TimeoutsArgs']] = None,
+            vga: Optional[pulumi.InputType['GetVm2VgaArgs']] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVm2Result:
     """
     !> **DO NOT USE**
     This is an experimental implementation of a Proxmox VM datasource using Plugin Framework.
 
 
     :param pulumi.InputType['GetVm2CloneArgs'] clone: The cloning configuration.
     :param pulumi.InputType['GetVm2CpuArgs'] cpu: The CPU configuration.
     :param str description: The description of the VM.
     :param int id: The unique identifier of the VM in the Proxmox cluster.
     :param str name: The name of the VM.
     :param str node_name: The name of the node where the VM is provisioned.
     :param Sequence[str] tags: The tags assigned to the VM.
     :param bool template: Whether the VM is a template.
+    :param pulumi.InputType['GetVm2VgaArgs'] vga: The VGA configuration.
     """
     __args__ = dict()
     __args__['clone'] = clone
     __args__['cpu'] = cpu
     __args__['description'] = description
     __args__['id'] = id
     __args__['name'] = name
     __args__['nodeName'] = node_name
     __args__['tags'] = tags
     __args__['template'] = template
     __args__['timeouts'] = timeouts
+    __args__['vga'] = vga
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:index/getVm2:getVm2', __args__, opts=opts, typ=GetVm2Result).value
 
     return AwaitableGetVm2Result(
         clone=pulumi.get(__ret__, 'clone'),
         cpu=pulumi.get(__ret__, 'cpu'),
         description=pulumi.get(__ret__, 'description'),
         id=pulumi.get(__ret__, 'id'),
         name=pulumi.get(__ret__, 'name'),
         node_name=pulumi.get(__ret__, 'node_name'),
         tags=pulumi.get(__ret__, 'tags'),
         template=pulumi.get(__ret__, 'template'),
-        timeouts=pulumi.get(__ret__, 'timeouts'))
+        timeouts=pulumi.get(__ret__, 'timeouts'),
+        vga=pulumi.get(__ret__, 'vga'))
 
 
 @_utilities.lift_output_func(get_vm2)
 def get_vm2_output(clone: Optional[pulumi.Input[Optional[pulumi.InputType['GetVm2CloneArgs']]]] = None,
                    cpu: Optional[pulumi.Input[Optional[pulumi.InputType['GetVm2CpuArgs']]]] = None,
                    description: Optional[pulumi.Input[Optional[str]]] = None,
                    id: Optional[pulumi.Input[int]] = None,
                    name: Optional[pulumi.Input[Optional[str]]] = None,
                    node_name: Optional[pulumi.Input[str]] = None,
                    tags: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                    template: Optional[pulumi.Input[Optional[bool]]] = None,
                    timeouts: Optional[pulumi.Input[Optional[pulumi.InputType['GetVm2TimeoutsArgs']]]] = None,
+                   vga: Optional[pulumi.Input[Optional[pulumi.InputType['GetVm2VgaArgs']]]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVm2Result]:
     """
     !> **DO NOT USE**
     This is an experimental implementation of a Proxmox VM datasource using Plugin Framework.
 
 
     :param pulumi.InputType['GetVm2CloneArgs'] clone: The cloning configuration.
     :param pulumi.InputType['GetVm2CpuArgs'] cpu: The CPU configuration.
     :param str description: The description of the VM.
     :param int id: The unique identifier of the VM in the Proxmox cluster.
     :param str name: The name of the VM.
     :param str node_name: The name of the node where the VM is provisioned.
     :param Sequence[str] tags: The tags assigned to the VM.
     :param bool template: Whether the VM is a template.
+    :param pulumi.InputType['GetVm2VgaArgs'] vga: The VGA configuration.
     """
     ...
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_group.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_groups.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_resource.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_resources.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/get_ha_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/ha_group.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/ha_resource.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/ha/ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/__init__.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/get_mappings.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/get_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/_inputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/get_pci.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/get_pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/get_usb.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/get_usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/pci.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/usb.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/mapping/usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hardware/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/__init__.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_dns.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_hosts.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_time.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_version.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/network_bridge.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/network_bridge.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/network_vlan.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/network_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 from . import _utilities
 
 __all__ = [
     'HostsEntry',
     'Vm2Clone',
     'Vm2Cpu',
     'Vm2Timeouts',
+    'Vm2Vga',
     'GetVm2CloneResult',
     'GetVm2CpuResult',
     'GetVm2TimeoutsResult',
+    'GetVm2VgaResult',
 ]
 
 @pulumi.output_type
 class HostsEntry(dict):
     def __init__(__self__, *,
                  address: str,
                  hostnames: Sequence[str]):
@@ -257,14 +259,57 @@
         """
         A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours).
         """
         return pulumi.get(self, "update")
 
 
 @pulumi.output_type
+class Vm2Vga(dict):
+    def __init__(__self__, *,
+                 clipboard: Optional[str] = None,
+                 memory: Optional[int] = None,
+                 type: Optional[str] = None):
+        """
+        :param str clipboard: Enable a specific clipboard. If not set, depending on the display type the SPICE one will be added. Currently only `vnc` is available. Migration with VNC clipboard is not supported by Proxmox.
+        :param int memory: The VGA memory in megabytes (4-512 MB). Has no effect with serial display.
+        :param str type: The VGA type (defaults to `std`).
+        """
+        if clipboard is not None:
+            pulumi.set(__self__, "clipboard", clipboard)
+        if memory is not None:
+            pulumi.set(__self__, "memory", memory)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def clipboard(self) -> Optional[str]:
+        """
+        Enable a specific clipboard. If not set, depending on the display type the SPICE one will be added. Currently only `vnc` is available. Migration with VNC clipboard is not supported by Proxmox.
+        """
+        return pulumi.get(self, "clipboard")
+
+    @property
+    @pulumi.getter
+    def memory(self) -> Optional[int]:
+        """
+        The VGA memory in megabytes (4-512 MB). Has no effect with serial display.
+        """
+        return pulumi.get(self, "memory")
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[str]:
+        """
+        The VGA type (defaults to `std`).
+        """
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
 class GetVm2CloneResult(dict):
     def __init__(__self__, *,
                  id: int,
                  retries: int):
         """
         :param int id: The ID of the VM to clone.
         :param int retries: The number of retries to perform when cloning the VM (default: 3).
@@ -421,7 +466,47 @@
     def read(self) -> Optional[str]:
         """
         A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
         """
         return pulumi.get(self, "read")
 
 
+@pulumi.output_type
+class GetVm2VgaResult(dict):
+    def __init__(__self__, *,
+                 clipboard: str,
+                 memory: int,
+                 type: str):
+        """
+        :param str clipboard: Enable a specific clipboard.
+        :param int memory: The VGA memory in megabytes (4-512 MB). Has no effect with serial display.
+        :param str type: The VGA type.
+        """
+        pulumi.set(__self__, "clipboard", clipboard)
+        pulumi.set(__self__, "memory", memory)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def clipboard(self) -> str:
+        """
+        Enable a specific clipboard.
+        """
+        return pulumi.get(self, "clipboard")
+
+    @property
+    @pulumi.getter
+    def memory(self) -> int:
+        """
+        The VGA memory in megabytes (4-512 MB). Has no effect with serial display.
+        """
+        return pulumi.get(self, "memory")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        The VGA type.
+        """
+        return pulumi.get(self, "type")
+
+
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/user/token.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/user/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,17 @@
 class VirtualMachineAudioDeviceArgs:
     def __init__(__self__, *,
                  device: Optional[pulumi.Input[str]] = None,
                  driver: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] device: The device (defaults to `intel-hda`).
+               - `AC97` - Intel 82801AA AC97 Audio.
+               - `ich9-intel-hda` - Intel HD Audio Controller (ich9).
+               - `intel-hda` - Intel HD Audio.
         :param pulumi.Input[str] driver: The driver (defaults to `spice`).
         :param pulumi.Input[bool] enabled: Whether to enable the audio device (defaults
                to `true`).
         """
         if device is not None:
             pulumi.set(__self__, "device", device)
         if driver is not None:
@@ -134,14 +137,17 @@
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def device(self) -> Optional[pulumi.Input[str]]:
         """
         The device (defaults to `intel-hda`).
+        - `AC97` - Intel 82801AA AC97 Audio.
+        - `ich9-intel-hda` - Intel HD Audio Controller (ich9).
+        - `intel-hda` - Intel HD Audio.
         """
         return pulumi.get(self, "device")
 
     @device.setter
     def device(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "device", value)
 
@@ -813,22 +819,24 @@
                  iops_write: Optional[pulumi.Input[int]] = None,
                  iops_write_burstable: Optional[pulumi.Input[int]] = None,
                  read: Optional[pulumi.Input[int]] = None,
                  read_burstable: Optional[pulumi.Input[int]] = None,
                  write: Optional[pulumi.Input[int]] = None,
                  write_burstable: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[int] iops_read: The maximum read I/O in operations per second
-        :param pulumi.Input[int] iops_read_burstable: The maximum unthrottled read I/O pool in operations per second
-        :param pulumi.Input[int] iops_write: The maximum write I/O in operations per second
-        :param pulumi.Input[int] iops_write_burstable: The maximum unthrottled write I/O pool in operations per second
-        :param pulumi.Input[int] read: The maximum read speed in megabytes per second
-        :param pulumi.Input[int] read_burstable: The maximum burstable read speed in megabytes per second
-        :param pulumi.Input[int] write: The maximum write speed in megabytes per second
-        :param pulumi.Input[int] write_burstable: The maximum burstable write speed in megabytes per second
+        :param pulumi.Input[int] iops_read: The maximum read I/O in operations per second.
+        :param pulumi.Input[int] iops_read_burstable: The maximum unthrottled read I/O pool in operations per second.
+        :param pulumi.Input[int] iops_write: The maximum write I/O in operations per second.
+        :param pulumi.Input[int] iops_write_burstable: The maximum unthrottled write I/O pool in operations per second.
+        :param pulumi.Input[int] read: The maximum read speed in megabytes per second.
+        :param pulumi.Input[int] read_burstable: The maximum burstable read speed in
+               megabytes per second.
+        :param pulumi.Input[int] write: The maximum write speed in megabytes per second.
+        :param pulumi.Input[int] write_burstable: The maximum burstable write speed in
+               megabytes per second.
         """
         if iops_read is not None:
             pulumi.set(__self__, "iops_read", iops_read)
         if iops_read_burstable is not None:
             pulumi.set(__self__, "iops_read_burstable", iops_read_burstable)
         if iops_write is not None:
             pulumi.set(__self__, "iops_write", iops_write)
@@ -843,99 +851,101 @@
         if write_burstable is not None:
             pulumi.set(__self__, "write_burstable", write_burstable)
 
     @property
     @pulumi.getter(name="iopsRead")
     def iops_read(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum read I/O in operations per second
+        The maximum read I/O in operations per second.
         """
         return pulumi.get(self, "iops_read")
 
     @iops_read.setter
     def iops_read(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "iops_read", value)
 
     @property
     @pulumi.getter(name="iopsReadBurstable")
     def iops_read_burstable(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum unthrottled read I/O pool in operations per second
+        The maximum unthrottled read I/O pool in operations per second.
         """
         return pulumi.get(self, "iops_read_burstable")
 
     @iops_read_burstable.setter
     def iops_read_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "iops_read_burstable", value)
 
     @property
     @pulumi.getter(name="iopsWrite")
     def iops_write(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum write I/O in operations per second
+        The maximum write I/O in operations per second.
         """
         return pulumi.get(self, "iops_write")
 
     @iops_write.setter
     def iops_write(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "iops_write", value)
 
     @property
     @pulumi.getter(name="iopsWriteBurstable")
     def iops_write_burstable(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum unthrottled write I/O pool in operations per second
+        The maximum unthrottled write I/O pool in operations per second.
         """
         return pulumi.get(self, "iops_write_burstable")
 
     @iops_write_burstable.setter
     def iops_write_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "iops_write_burstable", value)
 
     @property
     @pulumi.getter
     def read(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum read speed in megabytes per second
+        The maximum read speed in megabytes per second.
         """
         return pulumi.get(self, "read")
 
     @read.setter
     def read(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "read", value)
 
     @property
     @pulumi.getter(name="readBurstable")
     def read_burstable(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum burstable read speed in megabytes per second
+        The maximum burstable read speed in
+        megabytes per second.
         """
         return pulumi.get(self, "read_burstable")
 
     @read_burstable.setter
     def read_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "read_burstable", value)
 
     @property
     @pulumi.getter
     def write(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum write speed in megabytes per second
+        The maximum write speed in megabytes per second.
         """
         return pulumi.get(self, "write")
 
     @write.setter
     def write(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "write", value)
 
     @property
     @pulumi.getter(name="writeBurstable")
     def write_burstable(self) -> Optional[pulumi.Input[int]]:
         """
-        The maximum burstable write speed in megabytes per second
+        The maximum burstable write speed in
+        megabytes per second.
         """
         return pulumi.get(self, "write_burstable")
 
     @write_burstable.setter
     def write_burstable(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "write_burstable", value)
 
@@ -1391,17 +1401,19 @@
 @pulumi.input_type
 class VirtualMachineInitializationDnsArgs:
     def __init__(__self__, *,
                  domain: Optional[pulumi.Input[str]] = None,
                  server: Optional[pulumi.Input[str]] = None,
                  servers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[str] domain: The DNS search domain
-        :param pulumi.Input[str] server: The DNS server
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The list of DNS servers
+        :param pulumi.Input[str] domain: The DNS search domain.
+        :param pulumi.Input[str] server: The DNS server. The `server` attribute is
+               deprecated and will be removed in a future release. Please use the
+               `servers` attribute instead.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] servers: The list of DNS servers.
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if server is not None:
             warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
             pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
         if server is not None:
@@ -1409,159 +1421,173 @@
         if servers is not None:
             pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS search domain
+        The DNS search domain.
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter
     def server(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS server
+        The DNS server. The `server` attribute is
+        deprecated and will be removed in a future release. Please use the
+        `servers` attribute instead.
         """
         warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
         pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
 
         return pulumi.get(self, "server")
 
     @server.setter
     def server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server", value)
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The list of DNS servers
+        The list of DNS servers.
         """
         return pulumi.get(self, "servers")
 
     @servers.setter
     def servers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "servers", value)
 
 
 @pulumi.input_type
 class VirtualMachineInitializationIpConfigArgs:
     def __init__(__self__, *,
                  ipv4: Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args']] = None,
                  ipv6: Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args']] = None):
         """
-        :param pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args'] ipv4: The IPv4 configuration
-        :param pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args'] ipv6: The IPv6 configuration
+        :param pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args'] ipv4: The IPv4 configuration.
+        :param pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args'] ipv6: The IPv4 configuration.
         """
         if ipv4 is not None:
             pulumi.set(__self__, "ipv4", ipv4)
         if ipv6 is not None:
             pulumi.set(__self__, "ipv6", ipv6)
 
     @property
     @pulumi.getter
     def ipv4(self) -> Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args']]:
         """
-        The IPv4 configuration
+        The IPv4 configuration.
         """
         return pulumi.get(self, "ipv4")
 
     @ipv4.setter
     def ipv4(self, value: Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv4Args']]):
         pulumi.set(self, "ipv4", value)
 
     @property
     @pulumi.getter
     def ipv6(self) -> Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args']]:
         """
-        The IPv6 configuration
+        The IPv4 configuration.
         """
         return pulumi.get(self, "ipv6")
 
     @ipv6.setter
     def ipv6(self, value: Optional[pulumi.Input['VirtualMachineInitializationIpConfigIpv6Args']]):
         pulumi.set(self, "ipv6", value)
 
 
 @pulumi.input_type
 class VirtualMachineInitializationIpConfigIpv4Args:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  gateway: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: The IPv4 address
-        :param pulumi.Input[str] gateway: The IPv4 gateway
+        :param pulumi.Input[str] address: The IPv4 address in CIDR notation
+               (e.g. 192.168.2.2/24). Alternatively, set this to `dhcp` for
+               autodiscovery.
+        :param pulumi.Input[str] gateway: The IPv4 gateway (must be omitted
+               when `dhcp` is used as the address).
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv4 address
+        The IPv4 address in CIDR notation
+        (e.g. 192.168.2.2/24). Alternatively, set this to `dhcp` for
+        autodiscovery.
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv4 gateway
+        The IPv4 gateway (must be omitted
+        when `dhcp` is used as the address).
         """
         return pulumi.get(self, "gateway")
 
     @gateway.setter
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
 
 @pulumi.input_type
 class VirtualMachineInitializationIpConfigIpv6Args:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  gateway: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: The IPv6 address
-        :param pulumi.Input[str] gateway: The IPv6 gateway
+        :param pulumi.Input[str] address: The IPv6 address in CIDR notation
+               (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
+               to `dhcp` for autodiscovery.
+        :param pulumi.Input[str] gateway: The IPv6 gateway (must be omitted
+               when `dhcp` is used as the address).
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 address
+        The IPv6 address in CIDR notation
+        (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
+        to `dhcp` for autodiscovery.
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv6 gateway
+        The IPv6 gateway (must be omitted
+        when `dhcp` is used as the address).
         """
         return pulumi.get(self, "gateway")
 
     @gateway.setter
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
@@ -1569,54 +1595,54 @@
 @pulumi.input_type
 class VirtualMachineInitializationUserAccountArgs:
     def __init__(__self__, *,
                  keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: The SSH keys
-        :param pulumi.Input[str] password: The SSH password
-        :param pulumi.Input[str] username: The SSH username
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: The SSH keys.
+        :param pulumi.Input[str] password: The SSH password.
+        :param pulumi.Input[str] username: The SSH username.
         """
         if keys is not None:
             pulumi.set(__self__, "keys", keys)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def keys(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The SSH keys
+        The SSH keys.
         """
         return pulumi.get(self, "keys")
 
     @keys.setter
     def keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "keys", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH password
+        The SSH password.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH username
+        The SSH username.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
@@ -2321,37 +2347,57 @@
     def usb3(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "usb3", value)
 
 
 @pulumi.input_type
 class VirtualMachineVgaArgs:
     def __init__(__self__, *,
+                 clipboard: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  memory: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] enabled: Whether to enable the VGA device (defaults
-               to `true`).
+        :param pulumi.Input[str] clipboard: Enable VNC clipboard by setting to `vnc`. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information.
+        :param pulumi.Input[bool] enabled: Whether to enable the VGA device
         :param pulumi.Input[int] memory: The VGA memory in megabytes (defaults to `16`).
         :param pulumi.Input[str] type: The VGA type (defaults to `std`).
         """
+        if clipboard is not None:
+            pulumi.set(__self__, "clipboard", clipboard)
+        if enabled is not None:
+            warnings.warn("""The `enabled` attribute is deprecated and will be removed in a future release. Use type `none` instead.""", DeprecationWarning)
+            pulumi.log.warn("""enabled is deprecated: The `enabled` attribute is deprecated and will be removed in a future release. Use type `none` instead.""")
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if memory is not None:
             pulumi.set(__self__, "memory", memory)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
+    def clipboard(self) -> Optional[pulumi.Input[str]]:
+        """
+        Enable VNC clipboard by setting to `vnc`. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information.
+        """
+        return pulumi.get(self, "clipboard")
+
+    @clipboard.setter
+    def clipboard(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "clipboard", value)
+
+    @property
+    @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to enable the VGA device (defaults
-        to `true`).
+        Whether to enable the VGA device
         """
+        warnings.warn("""The `enabled` attribute is deprecated and will be removed in a future release. Use type `none` instead.""", DeprecationWarning)
+        pulumi.log.warn("""enabled is deprecated: The `enabled` attribute is deprecated and will be removed in a future release. Use type `none` instead.""")
+
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
 class VirtualMachineAudioDevice(dict):
     def __init__(__self__, *,
                  device: Optional[str] = None,
                  driver: Optional[str] = None,
                  enabled: Optional[bool] = None):
         """
         :param str device: The device (defaults to `intel-hda`).
+               - `AC97` - Intel 82801AA AC97 Audio.
+               - `ich9-intel-hda` - Intel HD Audio Controller (ich9).
+               - `intel-hda` - Intel HD Audio.
         :param str driver: The driver (defaults to `spice`).
         :param bool enabled: Whether to enable the audio device (defaults
                to `true`).
         """
         if device is not None:
             pulumi.set(__self__, "device", device)
         if driver is not None:
@@ -120,14 +123,17 @@
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def device(self) -> Optional[str]:
         """
         The device (defaults to `intel-hda`).
+        - `AC97` - Intel 82801AA AC97 Audio.
+        - `ich9-intel-hda` - Intel HD Audio Controller (ich9).
+        - `intel-hda` - Intel HD Audio.
         """
         return pulumi.get(self, "device")
 
     @property
     @pulumi.getter
     def driver(self) -> Optional[str]:
         """
@@ -747,22 +753,24 @@
                  iops_write: Optional[int] = None,
                  iops_write_burstable: Optional[int] = None,
                  read: Optional[int] = None,
                  read_burstable: Optional[int] = None,
                  write: Optional[int] = None,
                  write_burstable: Optional[int] = None):
         """
-        :param int iops_read: The maximum read I/O in operations per second
-        :param int iops_read_burstable: The maximum unthrottled read I/O pool in operations per second
-        :param int iops_write: The maximum write I/O in operations per second
-        :param int iops_write_burstable: The maximum unthrottled write I/O pool in operations per second
-        :param int read: The maximum read speed in megabytes per second
-        :param int read_burstable: The maximum burstable read speed in megabytes per second
-        :param int write: The maximum write speed in megabytes per second
-        :param int write_burstable: The maximum burstable write speed in megabytes per second
+        :param int iops_read: The maximum read I/O in operations per second.
+        :param int iops_read_burstable: The maximum unthrottled read I/O pool in operations per second.
+        :param int iops_write: The maximum write I/O in operations per second.
+        :param int iops_write_burstable: The maximum unthrottled write I/O pool in operations per second.
+        :param int read: The maximum read speed in megabytes per second.
+        :param int read_burstable: The maximum burstable read speed in
+               megabytes per second.
+        :param int write: The maximum write speed in megabytes per second.
+        :param int write_burstable: The maximum burstable write speed in
+               megabytes per second.
         """
         if iops_read is not None:
             pulumi.set(__self__, "iops_read", iops_read)
         if iops_read_burstable is not None:
             pulumi.set(__self__, "iops_read_burstable", iops_read_burstable)
         if iops_write is not None:
             pulumi.set(__self__, "iops_write", iops_write)
@@ -777,71 +785,73 @@
         if write_burstable is not None:
             pulumi.set(__self__, "write_burstable", write_burstable)
 
     @property
     @pulumi.getter(name="iopsRead")
     def iops_read(self) -> Optional[int]:
         """
-        The maximum read I/O in operations per second
+        The maximum read I/O in operations per second.
         """
         return pulumi.get(self, "iops_read")
 
     @property
     @pulumi.getter(name="iopsReadBurstable")
     def iops_read_burstable(self) -> Optional[int]:
         """
-        The maximum unthrottled read I/O pool in operations per second
+        The maximum unthrottled read I/O pool in operations per second.
         """
         return pulumi.get(self, "iops_read_burstable")
 
     @property
     @pulumi.getter(name="iopsWrite")
     def iops_write(self) -> Optional[int]:
         """
-        The maximum write I/O in operations per second
+        The maximum write I/O in operations per second.
         """
         return pulumi.get(self, "iops_write")
 
     @property
     @pulumi.getter(name="iopsWriteBurstable")
     def iops_write_burstable(self) -> Optional[int]:
         """
-        The maximum unthrottled write I/O pool in operations per second
+        The maximum unthrottled write I/O pool in operations per second.
         """
         return pulumi.get(self, "iops_write_burstable")
 
     @property
     @pulumi.getter
     def read(self) -> Optional[int]:
         """
-        The maximum read speed in megabytes per second
+        The maximum read speed in megabytes per second.
         """
         return pulumi.get(self, "read")
 
     @property
     @pulumi.getter(name="readBurstable")
     def read_burstable(self) -> Optional[int]:
         """
-        The maximum burstable read speed in megabytes per second
+        The maximum burstable read speed in
+        megabytes per second.
         """
         return pulumi.get(self, "read_burstable")
 
     @property
     @pulumi.getter
     def write(self) -> Optional[int]:
         """
-        The maximum write speed in megabytes per second
+        The maximum write speed in megabytes per second.
         """
         return pulumi.get(self, "write")
 
     @property
     @pulumi.getter(name="writeBurstable")
     def write_burstable(self) -> Optional[int]:
         """
-        The maximum burstable write speed in megabytes per second
+        The maximum burstable write speed in
+        megabytes per second.
         """
         return pulumi.get(self, "write_burstable")
 
 
 @pulumi.output_type
 class VirtualMachineEfiDisk(dict):
     @staticmethod
@@ -1265,185 +1275,201 @@
 @pulumi.output_type
 class VirtualMachineInitializationDns(dict):
     def __init__(__self__, *,
                  domain: Optional[str] = None,
                  server: Optional[str] = None,
                  servers: Optional[Sequence[str]] = None):
         """
-        :param str domain: The DNS search domain
-        :param str server: The DNS server
-        :param Sequence[str] servers: The list of DNS servers
+        :param str domain: The DNS search domain.
+        :param str server: The DNS server. The `server` attribute is
+               deprecated and will be removed in a future release. Please use the
+               `servers` attribute instead.
+        :param Sequence[str] servers: The list of DNS servers.
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if server is not None:
             pulumi.set(__self__, "server", server)
         if servers is not None:
             pulumi.set(__self__, "servers", servers)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
         """
-        The DNS search domain
+        The DNS search domain.
         """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def server(self) -> Optional[str]:
         """
-        The DNS server
+        The DNS server. The `server` attribute is
+        deprecated and will be removed in a future release. Please use the
+        `servers` attribute instead.
         """
         warnings.warn("""The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""", DeprecationWarning)
         pulumi.log.warn("""server is deprecated: The `server` attribute is deprecated and will be removed in a future release. Please use the `servers` attribute instead.""")
 
         return pulumi.get(self, "server")
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[Sequence[str]]:
         """
-        The list of DNS servers
+        The list of DNS servers.
         """
         return pulumi.get(self, "servers")
 
 
 @pulumi.output_type
 class VirtualMachineInitializationIpConfig(dict):
     def __init__(__self__, *,
                  ipv4: Optional['outputs.VirtualMachineInitializationIpConfigIpv4'] = None,
                  ipv6: Optional['outputs.VirtualMachineInitializationIpConfigIpv6'] = None):
         """
-        :param 'VirtualMachineInitializationIpConfigIpv4Args' ipv4: The IPv4 configuration
-        :param 'VirtualMachineInitializationIpConfigIpv6Args' ipv6: The IPv6 configuration
+        :param 'VirtualMachineInitializationIpConfigIpv4Args' ipv4: The IPv4 configuration.
+        :param 'VirtualMachineInitializationIpConfigIpv6Args' ipv6: The IPv4 configuration.
         """
         if ipv4 is not None:
             pulumi.set(__self__, "ipv4", ipv4)
         if ipv6 is not None:
             pulumi.set(__self__, "ipv6", ipv6)
 
     @property
     @pulumi.getter
     def ipv4(self) -> Optional['outputs.VirtualMachineInitializationIpConfigIpv4']:
         """
-        The IPv4 configuration
+        The IPv4 configuration.
         """
         return pulumi.get(self, "ipv4")
 
     @property
     @pulumi.getter
     def ipv6(self) -> Optional['outputs.VirtualMachineInitializationIpConfigIpv6']:
         """
-        The IPv6 configuration
+        The IPv4 configuration.
         """
         return pulumi.get(self, "ipv6")
 
 
 @pulumi.output_type
 class VirtualMachineInitializationIpConfigIpv4(dict):
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  gateway: Optional[str] = None):
         """
-        :param str address: The IPv4 address
-        :param str gateway: The IPv4 gateway
+        :param str address: The IPv4 address in CIDR notation
+               (e.g. 192.168.2.2/24). Alternatively, set this to `dhcp` for
+               autodiscovery.
+        :param str gateway: The IPv4 gateway (must be omitted
+               when `dhcp` is used as the address).
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
         """
-        The IPv4 address
+        The IPv4 address in CIDR notation
+        (e.g. 192.168.2.2/24). Alternatively, set this to `dhcp` for
+        autodiscovery.
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[str]:
         """
-        The IPv4 gateway
+        The IPv4 gateway (must be omitted
+        when `dhcp` is used as the address).
         """
         return pulumi.get(self, "gateway")
 
 
 @pulumi.output_type
 class VirtualMachineInitializationIpConfigIpv6(dict):
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  gateway: Optional[str] = None):
         """
-        :param str address: The IPv6 address
-        :param str gateway: The IPv6 gateway
+        :param str address: The IPv6 address in CIDR notation
+               (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
+               to `dhcp` for autodiscovery.
+        :param str gateway: The IPv6 gateway (must be omitted
+               when `dhcp` is used as the address).
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
         """
-        The IPv6 address
+        The IPv6 address in CIDR notation
+        (e.g. fd1c:000:0000::0000:000:7334/64). Alternatively, set this
+        to `dhcp` for autodiscovery.
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def gateway(self) -> Optional[str]:
         """
-        The IPv6 gateway
+        The IPv6 gateway (must be omitted
+        when `dhcp` is used as the address).
         """
         return pulumi.get(self, "gateway")
 
 
 @pulumi.output_type
 class VirtualMachineInitializationUserAccount(dict):
     def __init__(__self__, *,
                  keys: Optional[Sequence[str]] = None,
                  password: Optional[str] = None,
                  username: Optional[str] = None):
         """
-        :param Sequence[str] keys: The SSH keys
-        :param str password: The SSH password
-        :param str username: The SSH username
+        :param Sequence[str] keys: The SSH keys.
+        :param str password: The SSH password.
+        :param str username: The SSH username.
         """
         if keys is not None:
             pulumi.set(__self__, "keys", keys)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def keys(self) -> Optional[Sequence[str]]:
         """
-        The SSH keys
+        The SSH keys.
         """
         return pulumi.get(self, "keys")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         """
-        The SSH password
+        The SSH password.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
         """
-        The SSH username
+        The SSH username.
         """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class VirtualMachineMemory(dict):
     @staticmethod
@@ -2066,37 +2092,50 @@
         """
         return pulumi.get(self, "usb3")
 
 
 @pulumi.output_type
 class VirtualMachineVga(dict):
     def __init__(__self__, *,
+                 clipboard: Optional[str] = None,
                  enabled: Optional[bool] = None,
                  memory: Optional[int] = None,
                  type: Optional[str] = None):
         """
-        :param bool enabled: Whether to enable the VGA device (defaults
-               to `true`).
+        :param str clipboard: Enable VNC clipboard by setting to `vnc`. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information.
+        :param bool enabled: Whether to enable the VGA device
         :param int memory: The VGA memory in megabytes (defaults to `16`).
         :param str type: The VGA type (defaults to `std`).
         """
+        if clipboard is not None:
+            pulumi.set(__self__, "clipboard", clipboard)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if memory is not None:
             pulumi.set(__self__, "memory", memory)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
+    def clipboard(self) -> Optional[str]:
+        """
+        Enable VNC clipboard by setting to `vnc`. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information.
+        """
+        return pulumi.get(self, "clipboard")
+
+    @property
+    @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
-        Whether to enable the VGA device (defaults
-        to `true`).
+        Whether to enable the VGA device
         """
+        warnings.warn("""The `enabled` attribute is deprecated and will be removed in a future release. Use type `none` instead.""", DeprecationWarning)
+        pulumi.log.warn("""enabled is deprecated: The `enabled` attribute is deprecated and will be removed in a future release. Use type `none` instead.""")
+
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def memory(self) -> Optional[int]:
         """
         The VGA memory in megabytes (defaults to `16`).
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm2.py` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve/vm2.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,24 +19,26 @@
                  node_name: pulumi.Input[str],
                  clone: Optional[pulumi.Input['Vm2CloneArgs']] = None,
                  cpu: Optional[pulumi.Input['Vm2CpuArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[bool]] = None,
-                 timeouts: Optional[pulumi.Input['Vm2TimeoutsArgs']] = None):
+                 timeouts: Optional[pulumi.Input['Vm2TimeoutsArgs']] = None,
+                 vga: Optional[pulumi.Input['Vm2VgaArgs']] = None):
         """
         The set of arguments for constructing a Vm2 resource.
         :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
         :param pulumi.Input['Vm2CloneArgs'] clone: The cloning configuration.
         :param pulumi.Input['Vm2CpuArgs'] cpu: The CPU configuration.
         :param pulumi.Input[str] description: The description of the VM.
         :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the VM.
         :param pulumi.Input[bool] template: Set to true to create a VM template.
+        :param pulumi.Input['Vm2VgaArgs'] vga: Configure the VGA Hardware. If you want to use high resolution modes (>= 1280x1024x16) you may need to increase the vga memory option. Since QEMU 2.9 the default VGA display type is `std` for all OS types besides some Windows versions (XP and older) which use `cirrus`. The `qxl` option enables the SPICE display server. For win* OS you can select how many independent displays you want, Linux guests can add displays themself. You can also run without any graphic card, using a serial device as terminal. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information and available configuration parameters.
         """
         pulumi.set(__self__, "node_name", node_name)
         if clone is not None:
             pulumi.set(__self__, "clone", clone)
         if cpu is not None:
             pulumi.set(__self__, "cpu", cpu)
         if description is not None:
@@ -45,14 +47,16 @@
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if template is not None:
             pulumi.set(__self__, "template", template)
         if timeouts is not None:
             pulumi.set(__self__, "timeouts", timeouts)
+        if vga is not None:
+            pulumi.set(__self__, "vga", vga)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> pulumi.Input[str]:
         """
         The name of the node where the VM is provisioned.
         """
@@ -139,35 +143,49 @@
     def timeouts(self) -> Optional[pulumi.Input['Vm2TimeoutsArgs']]:
         return pulumi.get(self, "timeouts")
 
     @timeouts.setter
     def timeouts(self, value: Optional[pulumi.Input['Vm2TimeoutsArgs']]):
         pulumi.set(self, "timeouts", value)
 
+    @property
+    @pulumi.getter
+    def vga(self) -> Optional[pulumi.Input['Vm2VgaArgs']]:
+        """
+        Configure the VGA Hardware. If you want to use high resolution modes (>= 1280x1024x16) you may need to increase the vga memory option. Since QEMU 2.9 the default VGA display type is `std` for all OS types besides some Windows versions (XP and older) which use `cirrus`. The `qxl` option enables the SPICE display server. For win* OS you can select how many independent displays you want, Linux guests can add displays themself. You can also run without any graphic card, using a serial device as terminal. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information and available configuration parameters.
+        """
+        return pulumi.get(self, "vga")
+
+    @vga.setter
+    def vga(self, value: Optional[pulumi.Input['Vm2VgaArgs']]):
+        pulumi.set(self, "vga", value)
+
 
 @pulumi.input_type
 class _Vm2State:
     def __init__(__self__, *,
                  clone: Optional[pulumi.Input['Vm2CloneArgs']] = None,
                  cpu: Optional[pulumi.Input['Vm2CpuArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[bool]] = None,
-                 timeouts: Optional[pulumi.Input['Vm2TimeoutsArgs']] = None):
+                 timeouts: Optional[pulumi.Input['Vm2TimeoutsArgs']] = None,
+                 vga: Optional[pulumi.Input['Vm2VgaArgs']] = None):
         """
         Input properties used for looking up and filtering Vm2 resources.
         :param pulumi.Input['Vm2CloneArgs'] clone: The cloning configuration.
         :param pulumi.Input['Vm2CpuArgs'] cpu: The CPU configuration.
         :param pulumi.Input[str] description: The description of the VM.
         :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
         :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the VM.
         :param pulumi.Input[bool] template: Set to true to create a VM template.
+        :param pulumi.Input['Vm2VgaArgs'] vga: Configure the VGA Hardware. If you want to use high resolution modes (>= 1280x1024x16) you may need to increase the vga memory option. Since QEMU 2.9 the default VGA display type is `std` for all OS types besides some Windows versions (XP and older) which use `cirrus`. The `qxl` option enables the SPICE display server. For win* OS you can select how many independent displays you want, Linux guests can add displays themself. You can also run without any graphic card, using a serial device as terminal. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information and available configuration parameters.
         """
         if clone is not None:
             pulumi.set(__self__, "clone", clone)
         if cpu is not None:
             pulumi.set(__self__, "cpu", cpu)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -177,14 +195,16 @@
             pulumi.set(__self__, "node_name", node_name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if template is not None:
             pulumi.set(__self__, "template", template)
         if timeouts is not None:
             pulumi.set(__self__, "timeouts", timeouts)
+        if vga is not None:
+            pulumi.set(__self__, "vga", vga)
 
     @property
     @pulumi.getter
     def clone(self) -> Optional[pulumi.Input['Vm2CloneArgs']]:
         """
         The cloning configuration.
         """
@@ -271,28 +291,41 @@
     def timeouts(self) -> Optional[pulumi.Input['Vm2TimeoutsArgs']]:
         return pulumi.get(self, "timeouts")
 
     @timeouts.setter
     def timeouts(self, value: Optional[pulumi.Input['Vm2TimeoutsArgs']]):
         pulumi.set(self, "timeouts", value)
 
+    @property
+    @pulumi.getter
+    def vga(self) -> Optional[pulumi.Input['Vm2VgaArgs']]:
+        """
+        Configure the VGA Hardware. If you want to use high resolution modes (>= 1280x1024x16) you may need to increase the vga memory option. Since QEMU 2.9 the default VGA display type is `std` for all OS types besides some Windows versions (XP and older) which use `cirrus`. The `qxl` option enables the SPICE display server. For win* OS you can select how many independent displays you want, Linux guests can add displays themself. You can also run without any graphic card, using a serial device as terminal. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information and available configuration parameters.
+        """
+        return pulumi.get(self, "vga")
+
+    @vga.setter
+    def vga(self, value: Optional[pulumi.Input['Vm2VgaArgs']]):
+        pulumi.set(self, "vga", value)
+
 
 class Vm2(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  clone: Optional[pulumi.Input[pulumi.InputType['Vm2CloneArgs']]] = None,
                  cpu: Optional[pulumi.Input[pulumi.InputType['Vm2CpuArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[bool]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None,
+                 vga: Optional[pulumi.Input[pulumi.InputType['Vm2VgaArgs']]] = None,
                  __props__=None):
         """
         !> **DO NOT USE**
         This is an experimental implementation of a Proxmox VM resource using Plugin Framework.<br><br>It is a Proof of Concept, highly experimental and **will** change in future. It does not support all features of the Proxmox API for VMs and **MUST NOT** be used in production.
 
         > Many attributes are marked as **optional** _and_ **computed** in the schema,
         hence you may seem added to the plan with "(known after apply)" status, even if they are not set in the configuration.
@@ -306,14 +339,15 @@
         :param pulumi.Input[pulumi.InputType['Vm2CloneArgs']] clone: The cloning configuration.
         :param pulumi.Input[pulumi.InputType['Vm2CpuArgs']] cpu: The CPU configuration.
         :param pulumi.Input[str] description: The description of the VM.
         :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
         :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the VM.
         :param pulumi.Input[bool] template: Set to true to create a VM template.
+        :param pulumi.Input[pulumi.InputType['Vm2VgaArgs']] vga: Configure the VGA Hardware. If you want to use high resolution modes (>= 1280x1024x16) you may need to increase the vga memory option. Since QEMU 2.9 the default VGA display type is `std` for all OS types besides some Windows versions (XP and older) which use `cirrus`. The `qxl` option enables the SPICE display server. For win* OS you can select how many independent displays you want, Linux guests can add displays themself. You can also run without any graphic card, using a serial device as terminal. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information and available configuration parameters.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Vm2Args,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -347,14 +381,15 @@
                  cpu: Optional[pulumi.Input[pulumi.InputType['Vm2CpuArgs']]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[bool]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None,
+                 vga: Optional[pulumi.Input[pulumi.InputType['Vm2VgaArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -366,14 +401,15 @@
             __props__.__dict__["name"] = name
             if node_name is None and not opts.urn:
                 raise TypeError("Missing required property 'node_name'")
             __props__.__dict__["node_name"] = node_name
             __props__.__dict__["tags"] = tags
             __props__.__dict__["template"] = template
             __props__.__dict__["timeouts"] = timeouts
+            __props__.__dict__["vga"] = vga
         super(Vm2, __self__).__init__(
             'proxmoxve:index/vm2:Vm2',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -383,42 +419,45 @@
             clone: Optional[pulumi.Input[pulumi.InputType['Vm2CloneArgs']]] = None,
             cpu: Optional[pulumi.Input[pulumi.InputType['Vm2CpuArgs']]] = None,
             description: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             node_name: Optional[pulumi.Input[str]] = None,
             tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             template: Optional[pulumi.Input[bool]] = None,
-            timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None) -> 'Vm2':
+            timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None,
+            vga: Optional[pulumi.Input[pulumi.InputType['Vm2VgaArgs']]] = None) -> 'Vm2':
         """
         Get an existing Vm2 resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['Vm2CloneArgs']] clone: The cloning configuration.
         :param pulumi.Input[pulumi.InputType['Vm2CpuArgs']] cpu: The CPU configuration.
         :param pulumi.Input[str] description: The description of the VM.
         :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
         :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the VM.
         :param pulumi.Input[bool] template: Set to true to create a VM template.
+        :param pulumi.Input[pulumi.InputType['Vm2VgaArgs']] vga: Configure the VGA Hardware. If you want to use high resolution modes (>= 1280x1024x16) you may need to increase the vga memory option. Since QEMU 2.9 the default VGA display type is `std` for all OS types besides some Windows versions (XP and older) which use `cirrus`. The `qxl` option enables the SPICE display server. For win* OS you can select how many independent displays you want, Linux guests can add displays themself. You can also run without any graphic card, using a serial device as terminal. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information and available configuration parameters.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _Vm2State.__new__(_Vm2State)
 
         __props__.__dict__["clone"] = clone
         __props__.__dict__["cpu"] = cpu
         __props__.__dict__["description"] = description
         __props__.__dict__["name"] = name
         __props__.__dict__["node_name"] = node_name
         __props__.__dict__["tags"] = tags
         __props__.__dict__["template"] = template
         __props__.__dict__["timeouts"] = timeouts
+        __props__.__dict__["vga"] = vga
         return Vm2(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def clone(self) -> pulumi.Output[Optional['outputs.Vm2Clone']]:
         """
         The cloning configuration.
@@ -474,7 +513,15 @@
         return pulumi.get(self, "template")
 
     @property
     @pulumi.getter
     def timeouts(self) -> pulumi.Output[Optional['outputs.Vm2Timeouts']]:
         return pulumi.get(self, "timeouts")
 
+    @property
+    @pulumi.getter
+    def vga(self) -> pulumi.Output['outputs.Vm2Vga']:
+        """
+        Configure the VGA Hardware. If you want to use high resolution modes (>= 1280x1024x16) you may need to increase the vga memory option. Since QEMU 2.9 the default VGA display type is `std` for all OS types besides some Windows versions (XP and older) which use `cirrus`. The `qxl` option enables the SPICE display server. For win* OS you can select how many independent displays you want, Linux guests can add displays themself. You can also run without any graphic card, using a serial device as terminal. See the [Proxmox documentation](https://pve.proxmox.com/pve-docs/pve-admin-guide.html#qm_virtual_machines_settings) section 10.2.8 for more information and available configuration parameters.
+        """
+        return pulumi.get(self, "vga")
+
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 6.7.1
+Version: 6.8.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-6.8.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.1/setup.py` & `pulumi_proxmoxve-6.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.7.1"
+VERSION = "6.8.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
```

