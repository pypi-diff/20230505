# Comparing `tmp/pyroute2-0.7.7.tar.gz` & `tmp/pyroute2-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroute2-0.7.7.tar", last modified: Fri Apr 14 19:19:17 2023, max compression
+gzip compressed data, was "pyroute2-0.7.8.tar", last modified: Fri May  5 11:34:45 2023, max compression
```

## Comparing `pyroute2-0.7.7.tar` & `pyroute2-0.7.8.tar`

### file list

```diff
@@ -1,354 +1,354 @@
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.496275 pyroute2-0.7.7/
--rw-r--r--   0 peet      (1001) peet      (1001)    28610 2023-04-14 19:01:53.000000 pyroute2-0.7.7/CHANGELOG.rst
--rw-r--r--   0 peet      (1001) peet      (1001)       31 2023-03-15 10:10:02.000000 pyroute2-0.7.7/LICENSE
--rw-r--r--   0 peet      (1001) peet      (1001)    11348 2023-03-15 10:10:02.000000 pyroute2-0.7.7/LICENSE.Apache-2.0
--rw-r--r--   0 peet      (1001) peet      (1001)    18092 2023-03-15 10:10:02.000000 pyroute2-0.7.7/LICENSE.GPL-2.0-or-later
--rw-r--r--   0 peet      (1001) peet      (1001)      237 2023-03-15 10:10:02.000000 pyroute2-0.7.7/MANIFEST.in
--rw-r--r--   0 peet      (1001) peet      (1001)     8172 2023-04-14 19:19:17.496275 pyroute2-0.7.7/PKG-INFO
--rw-r--r--   0 peet      (1001) peet      (1001)     2198 2023-03-15 10:10:02.000000 pyroute2-0.7.7/README.contribute.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      340 2023-03-15 10:10:02.000000 pyroute2-0.7.7/README.license.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      397 2023-03-15 10:10:02.000000 pyroute2-0.7.7/README.minimal.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      757 2023-03-15 10:10:02.000000 pyroute2-0.7.7/README.report.rst
--rw-r--r--   0 peet      (1001) peet      (1001)     6853 2023-03-15 10:10:02.000000 pyroute2-0.7.7/README.rst
--rw-r--r--   0 peet      (1001) peet      (1001)        6 2023-04-14 19:19:05.000000 pyroute2-0.7.7/VERSION
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.449275 pyroute2-0.7.7/examples/
--rw-r--r--   0 peet      (1001) peet      (1001)       18 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/README.md
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.450275 pyroute2-0.7.7/examples/devlink/
--rw-r--r--   0 peet      (1001) peet      (1001)      224 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/devlink/devlink_list.py
--rw-r--r--   0 peet      (1001) peet      (1001)       80 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/devlink/devlink_monitor.py
--rw-r--r--   0 peet      (1001) peet      (1001)      284 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/devlink/devlink_port_list.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.451275 pyroute2-0.7.7/examples/ethtool/
--rw-r--r--   0 peet      (1001) peet      (1001)      816 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ethtool/ethtool-ioctl_get_infos.py
--rw-r--r--   0 peet      (1001) peet      (1001)      496 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ethtool/ethtool-netlink_get_infos.py
--rw-r--r--   0 peet      (1001) peet      (1001)      391 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ethtool/ethtool_get_infos.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.451275 pyroute2-0.7.7/examples/generic/
--rw-r--r--   0 peet      (1001) peet      (1001)      155 2022-05-21 16:48:21.000000 pyroute2-0.7.7/examples/generic/Makefile
--rw-r--r--   0 peet      (1001) peet      (1001)     3561 2022-05-21 16:48:21.000000 pyroute2-0.7.7/examples/generic/netl.c
--rwxr-xr-x   0 peet      (1001) peet      (1001)     1179 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/generic/netl.py
--rw-r--r--   0 peet      (1001) peet      (1001)      391 2022-05-21 16:48:21.000000 pyroute2-0.7.7/examples/ipq.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.451275 pyroute2-0.7.7/examples/iproute/
--rw-r--r--   0 peet      (1001) peet      (1001)      187 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/iproute/ip_monitor.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1523 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ipset.py
--rw-r--r--   0 peet      (1001) peet      (1001)      127 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/kobject_uevent.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.451275 pyroute2-0.7.7/examples/lab/
--rw-r--r--   0 peet      (1001) peet      (1001)      462 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/README.rst
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.452275 pyroute2-0.7.7/examples/lab/iproute_get_addr/
--rw-r--r--   0 peet      (1001) peet      (1001)      162 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/iproute_get_addr/README.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      323 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/iproute_get_addr/check.py
--rw-r--r--   0 peet      (1001) peet      (1001)       64 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/iproute_get_addr/setup.py
--rw-r--r--   0 peet      (1001) peet      (1001)      102 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/iproute_get_addr/task.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.452275 pyroute2-0.7.7/examples/lab/iproute_get_attr/
--rw-r--r--   0 peet      (1001) peet      (1001)      341 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/iproute_get_attr/README.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      252 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/iproute_get_attr/check.py
--rw-r--r--   0 peet      (1001) peet      (1001)       64 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/iproute_get_attr/setup.py
--rw-r--r--   0 peet      (1001) peet      (1001)      308 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/lab/iproute_get_attr/task.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.453275 pyroute2-0.7.7/examples/ndb/
--rw-r--r--   0 peet      (1001) peet      (1001)      752 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ndb/create_bond.py
--rw-r--r--   0 peet      (1001) peet      (1001)      643 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ndb/create_interface.py
--rw-r--r--   0 peet      (1001) peet      (1001)      684 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ndb/create_vlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3546 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ndb/keystone_auth.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2188 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/ndb/radius_auth.py
--rwxr-xr-x   0 peet      (1001) peet      (1001)      444 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/nftables.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1522 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/nftables_sets.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.454275 pyroute2-0.7.7/examples/policy/
--rwxr-xr-x   0 peet      (1001) peet      (1001)      536 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/policy/policy.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.454275 pyroute2-0.7.7/examples/processes/
--rw-r--r--   0 peet      (1001) peet      (1001)      414 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/processes/pmonitor.py
--rw-r--r--   0 peet      (1001) peet      (1001)      246 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/processes/taskstats.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.455275 pyroute2-0.7.7/examples/pyroute2-cli/
--rw-r--r--   0 peet      (1001) peet      (1001)      300 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/pyroute2-cli/comments
--rw-r--r--   0 peet      (1001) peet      (1001)     1869 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/pyroute2-cli/create_bridge
--rw-r--r--   0 peet      (1001) peet      (1001)      723 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/pyroute2-cli/create_dummy
--rw-r--r--   0 peet      (1001) peet      (1001)       87 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/pyroute2-cli/dump_lo
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.455275 pyroute2-0.7.7/examples/wifi/
--rw-r--r--   0 peet      (1001) peet      (1001)      464 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/wifi/nl80211_interface_type.py
--rw-r--r--   0 peet      (1001) peet      (1001)      422 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/wifi/nl80211_interfaces.py
--rw-r--r--   0 peet      (1001) peet      (1001)      113 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/wifi/nl80211_monitor.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2504 2023-03-15 10:10:02.000000 pyroute2-0.7.7/examples/wifi/nl80211_scan_dump.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.455275 pyroute2-0.7.7/pr2modules/
--rw-r--r--   0 peet      (1001) peet      (1001)      568 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pr2modules/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)       90 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyproject.toml
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.457275 pyroute2-0.7.7/pyroute2/
--rw-r--r--   0 peet      (1001) peet      (1001)     2876 2023-04-05 11:12:40.000000 pyroute2-0.7.7/pyroute2/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2474 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/arp.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.458275 pyroute2-0.7.7/pyroute2/bsd/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2-0.7.7/pyroute2/bsd/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.459275 pyroute2-0.7.7/pyroute2/bsd/pf_route/
--rw-r--r--   0 peet      (1001) peet      (1001)     4186 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/bsd/pf_route/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3270 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/bsd/pf_route/freebsd.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3607 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/bsd/pf_route/openbsd.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.459275 pyroute2-0.7.7/pyroute2/bsd/rtmsocket/
--rw-r--r--   0 peet      (1001) peet      (1001)     4287 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/bsd/rtmsocket/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1382 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/bsd/rtmsocket/freebsd.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1423 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/bsd/rtmsocket/openbsd.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8136 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/bsd/util.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.460275 pyroute2-0.7.7/pyroute2/cli/
--rw-r--r--   0 peet      (1001) peet      (1001)     2991 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/cli/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.460275 pyroute2-0.7.7/pyroute2/cli/auth/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/cli/auth/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1194 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/cli/auth/auth_keystone.py
--rw-r--r--   0 peet      (1001) peet      (1001)      774 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/cli/auth/auth_radius.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3296 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/cli/console.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5586 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/cli/parser.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3188 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/cli/server.py
--rw-r--r--   0 peet      (1001) peet      (1001)     9156 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/cli/session.py
--rw-r--r--   0 peet      (1001) peet      (1001)    17833 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/common.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.461275 pyroute2-0.7.7/pyroute2/config/
--rw-r--r--   0 peet      (1001) peet      (1001)     1365 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/config/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2340 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/config/asyncio.py
--rw-r--r--   0 peet      (1001) peet      (1001)      258 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/config/eventlet.py
--rw-r--r--   0 peet      (1001) peet      (1001)      541 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/config/log.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8497 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/config/test_platform.py
--rw-r--r--   0 peet      (1001) peet      (1001)       22 2023-04-14 19:19:05.000000 pyroute2-0.7.7/pyroute2/config/version.py
--rw-r--r--   0 peet      (1001) peet      (1001)     6845 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/conntrack.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2071 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/devlink.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.462275 pyroute2-0.7.7/pyroute2/dhcp/
--rw-r--r--   0 peet      (1001) peet      (1001)    10048 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/dhcp/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1896 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/dhcp/client.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2066 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/dhcp/dhcp4msg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     4120 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/dhcp/dhcp4socket.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.463275 pyroute2-0.7.7/pyroute2/ethtool/
--rw-r--r--   0 peet      (1001) peet      (1001)       50 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ethtool/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     6700 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ethtool/common.py
--rw-r--r--   0 peet      (1001) peet      (1001)    11964 2023-03-16 09:44:55.000000 pyroute2-0.7.7/pyroute2/ethtool/ethtool.py
--rw-r--r--   0 peet      (1001) peet      (1001)    18285 2023-03-16 09:44:55.000000 pyroute2-0.7.7/pyroute2/ethtool/ioctl.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.463275 pyroute2-0.7.7/pyroute2/ext/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ext/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)      318 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ext/icmp.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3853 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ext/rawsocket.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.463275 pyroute2-0.7.7/pyroute2/inotify/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/inotify/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2403 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/inotify/inotify_fd.py
--rw-r--r--   0 peet      (1001) peet      (1001)      539 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/inotify/inotify_msg.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.465275 pyroute2-0.7.7/pyroute2/ipdb/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2-0.7.7/pyroute2/ipdb/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)      237 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipdb/exceptions.py
--rw-r--r--   0 peet      (1001) peet      (1001)    53683 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipdb/interfaces.py
--rw-r--r--   0 peet      (1001) peet      (1001)     9458 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipdb/linkedset.py
--rw-r--r--   0 peet      (1001) peet      (1001)    49046 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipdb/main.py
--rw-r--r--   0 peet      (1001) peet      (1001)    46123 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipdb/routes.py
--rw-r--r--   0 peet      (1001) peet      (1001)     9617 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipdb/rules.py
--rw-r--r--   0 peet      (1001) peet      (1001)    16515 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipdb/transactional.py
--rw-r--r--   0 peet      (1001) peet      (1001)      222 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipdb/utils.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.467275 pyroute2-0.7.7/pyroute2/iproute/
--rw-r--r--   0 peet      (1001) peet      (1001)     4920 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/iproute/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    10532 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/iproute/bsd.py
--rw-r--r--   0 peet      (1001) peet      (1001)    23630 2023-04-05 11:12:44.000000 pyroute2-0.7.7/pyroute2/iproute/ipmock.py
--rw-r--r--   0 peet      (1001) peet      (1001)    82477 2023-03-16 14:35:20.000000 pyroute2-0.7.7/pyroute2/iproute/linux.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1313 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/iproute/parsers.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8082 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/iproute/windows.py
--rw-r--r--   0 peet      (1001) peet      (1001)    24131 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ipset.py
--rw-r--r--   0 peet      (1001) peet      (1001)    22019 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/iwutil.py
--rw-r--r--   0 peet      (1001) peet      (1001)      419 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/lab.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1139 2023-04-05 11:12:40.000000 pyroute2-0.7.7/pyroute2/loader.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1834 2023-04-05 11:12:40.000000 pyroute2-0.7.7/pyroute2/minimal.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.470275 pyroute2-0.7.7/pyroute2/ndb/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:43:06.000000 pyroute2-0.7.7/pyroute2/ndb/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2647 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/auth_manager.py
--rwxr-xr-x   0 peet      (1001) peet      (1001)     2163 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/cli.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1003 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/cluster.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1352 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/compat.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2067 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/events.py
--rw-r--r--   0 peet      (1001) peet      (1001)    21420 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/main.py
--rw-r--r--   0 peet      (1001) peet      (1001)      246 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/messages.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5147 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/noipdb.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.471275 pyroute2-0.7.7/pyroute2/ndb/objects/
--rw-r--r--   0 peet      (1001) peet      (1001)    37851 2023-04-05 11:12:44.000000 pyroute2-0.7.7/pyroute2/ndb/objects/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     9028 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/objects/address.py
--rw-r--r--   0 peet      (1001) peet      (1001)    34524 2023-04-05 11:12:44.000000 pyroute2-0.7.7/pyroute2/ndb/objects/interface.py
--rw-r--r--   0 peet      (1001) peet      (1001)     4832 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/objects/neighbour.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1977 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/objects/netns.py
--rw-r--r--   0 peet      (1001) peet      (1001)    28891 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/objects/route.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2440 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/objects/rule.py
--rw-r--r--   0 peet      (1001) peet      (1001)     4867 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/query.py
--rw-r--r--   0 peet      (1001) peet      (1001)    11291 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/report.py
--rw-r--r--   0 peet      (1001) peet      (1001)    32754 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/schema.py
--rw-r--r--   0 peet      (1001) peet      (1001)    16500 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/source.py
--rw-r--r--   0 peet      (1001) peet      (1001)     9808 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/task_manager.py
--rw-r--r--   0 peet      (1001) peet      (1001)    11313 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/transaction.py
--rw-r--r--   0 peet      (1001) peet      (1001)     6350 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/ndb/transport.py
--rw-r--r--   0 peet      (1001) peet      (1001)    15974 2023-04-05 11:12:44.000000 pyroute2-0.7.7/pyroute2/ndb/view.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.472275 pyroute2-0.7.7/pyroute2/netlink/
--rw-r--r--   0 peet      (1001) peet      (1001)    72813 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1947 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/buffer.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.473275 pyroute2-0.7.7/pyroute2/netlink/connector/
--rw-r--r--   0 peet      (1001) peet      (1001)      405 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/connector/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3998 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/connector/cn_proc.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.473275 pyroute2-0.7.7/pyroute2/netlink/devlink/
--rw-r--r--   0 peet      (1001) peet      (1001)    23285 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/devlink/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.473275 pyroute2-0.7.7/pyroute2/netlink/diag/
--rw-r--r--   0 peet      (1001) peet      (1001)    10423 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/diag/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    18650 2023-04-14 07:32:11.000000 pyroute2-0.7.7/pyroute2/netlink/diag/ss2.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.474275 pyroute2-0.7.7/pyroute2/netlink/event/
--rw-r--r--   0 peet      (1001) peet      (1001)      714 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/event/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2078 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/event/acpi_event.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2034 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/event/dquot.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2594 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/event/thermal.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1616 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/exceptions.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.475275 pyroute2-0.7.7/pyroute2/netlink/generic/
--rw-r--r--   0 peet      (1001) peet      (1001)     3910 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/generic/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     7467 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/generic/ethtool.py
--rw-r--r--   0 peet      (1001) peet      (1001)    19073 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/generic/l2tp.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3928 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/generic/mptcp.py
--rw-r--r--   0 peet      (1001) peet      (1001)    12476 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/generic/wireguard.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.475275 pyroute2-0.7.7/pyroute2/netlink/ipq/
--rw-r--r--   0 peet      (1001) peet      (1001)     3315 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/ipq/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.475275 pyroute2-0.7.7/pyroute2/netlink/nfnetlink/
--rw-r--r--   0 peet      (1001) peet      (1001)     1036 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/nfnetlink/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     7145 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/nfnetlink/ipset.py
--rw-r--r--   0 peet      (1001) peet      (1001)    27707 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/nfnetlink/nfctsocket.py
--rw-r--r--   0 peet      (1001) peet      (1001)    43123 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/nfnetlink/nftsocket.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.476275 pyroute2-0.7.7/pyroute2/netlink/nl80211/
--rw-r--r--   0 peet      (1001) peet      (1001)    61729 2023-04-05 11:25:50.000000 pyroute2-0.7.7/pyroute2/netlink/nl80211/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    49725 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/nlsocket.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2317 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/proxy.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.478275 pyroute2-0.7.7/pyroute2/netlink/rtnl/
--rw-r--r--   0 peet      (1001) peet      (1001)     5988 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)      155 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/errmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2428 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/fibmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2799 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifaddrmsg.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.479275 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/
--rw-r--r--   0 peet      (1001) peet      (1001)    43260 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    10801 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/compat.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.482275 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1747 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/bond.py
--rw-r--r--   0 peet      (1001) peet      (1001)      776 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/geneve.py
--rw-r--r--   0 peet      (1001) peet      (1001)      227 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/gtp.py
--rwxr-xr-x   0 peet      (1001) peet      (1001)      376 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/ipoib.py
--rw-r--r--   0 peet      (1001) peet      (1001)      291 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/ipvlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)      151 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/team.py
--rw-r--r--   0 peet      (1001) peet      (1001)      494 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/tun.py
--rw-r--r--   0 peet      (1001) peet      (1001)      569 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/tuntap.py
--rw-r--r--   0 peet      (1001) peet      (1001)      751 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/vlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)      146 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/vrf.py
--rw-r--r--   0 peet      (1001) peet      (1001)      317 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/vti.py
--rw-r--r--   0 peet      (1001) peet      (1001)      357 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/vti6.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1417 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/vxlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)      189 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/xfrm.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3428 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/proxy.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1974 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/sync.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3875 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/tuntap.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2583 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ifstatsmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5802 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/iprsocket.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3244 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/iw_event.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2018 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/marshal.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2607 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ndmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2188 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/ndtmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)      321 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/nsidmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)      522 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/nsinfmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)      366 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/p2pmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)      523 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/riprsocket.py
--rw-r--r--   0 peet      (1001) peet      (1001)      114 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/rtgenmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)    26078 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/rtmsg.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.487275 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/
--rw-r--r--   0 peet      (1001) peet      (1001)     2743 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)      979 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_bpf.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1234 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_connmark.py
--rw-r--r--   0 peet      (1001) peet      (1001)      709 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_gact.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1725 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_mirred.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1866 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_police.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3338 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_skbedit.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1465 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_vlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8478 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_basic.py
--rw-r--r--   0 peet      (1001) peet      (1001)     4613 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_flow.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1427 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_fw.py
--rw-r--r--   0 peet      (1001) peet      (1001)      986 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_matchall.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8033 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_u32.py
--rw-r--r--   0 peet      (1001) peet      (1001)    10724 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/common.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2063 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/common_act.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3148 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/common_ematch.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2776 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/em_cmp.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1741 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/em_ipset.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5933 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/em_meta.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2571 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_bpf.py
--rw-r--r--   0 peet      (1001) peet      (1001)    12834 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_cake.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3431 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_choke.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1010 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_clsact.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1607 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_codel.py
--rw-r--r--   0 peet      (1001) peet      (1001)      754 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_drr.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2658 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_fq_codel.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2352 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_hfsc.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5738 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_htb.py
--rw-r--r--   0 peet      (1001) peet      (1001)      214 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_ingress.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5111 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_netem.py
--rw-r--r--   0 peet      (1001) peet      (1001)      196 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_pfifo.py
--rw-r--r--   0 peet      (1001) peet      (1001)      215 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_pfifo_fast.py
--rw-r--r--   0 peet      (1001) peet      (1001)      446 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_plug.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2717 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_sfq.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1087 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_tbf.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1249 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_template.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.487275 pyroute2-0.7.7/pyroute2/netlink/taskstats/
--rw-r--r--   0 peet      (1001) peet      (1001)     4920 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/taskstats/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.487275 pyroute2-0.7.7/pyroute2/netlink/uevent/
--rw-r--r--   0 peet      (1001) peet      (1001)     1096 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netlink/uevent/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.488275 pyroute2-0.7.7/pyroute2/netns/
--rw-r--r--   0 peet      (1001) peet      (1001)    10678 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netns/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3803 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/netns/manager.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.488275 pyroute2-0.7.7/pyroute2/nftables/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2-0.7.7/pyroute2/nftables/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2530 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nftables/expressions.py
--rw-r--r--   0 peet      (1001) peet      (1001)    12712 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nftables/main.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.489275 pyroute2-0.7.7/pyroute2/nftables/parser/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nftables/parser/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    10530 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nftables/parser/expr.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2394 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nftables/parser/parser.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3892 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nftables/rule.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.490275 pyroute2-0.7.7/pyroute2/nslink/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nslink/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     6785 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nslink/nslink.py
--rw-r--r--   0 peet      (1001) peet      (1001)    11393 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/nslink/nspopen.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.490275 pyroute2-0.7.7/pyroute2/protocols/
--rw-r--r--   0 peet      (1001) peet      (1001)     8716 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/protocols/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.490275 pyroute2-0.7.7/pyroute2/remote/
--rw-r--r--   0 peet      (1001) peet      (1001)      206 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/remote/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)      111 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/remote/__main__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     4503 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/remote/iproute.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2084 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/remote/shell.py
--rw-r--r--   0 peet      (1001) peet      (1001)    11899 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/remote/transport.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.494275 pyroute2-0.7.7/pyroute2/requests/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3430 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/address.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5195 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/bridge.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5083 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/common.py
--rw-r--r--   0 peet      (1001) peet      (1001)     9174 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/link.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2005 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/main.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1241 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/neighbour.py
--rw-r--r--   0 peet      (1001) peet      (1001)      107 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/netns.py
--rw-r--r--   0 peet      (1001) peet      (1001)    19591 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/route.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1229 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/requests/rule.py
--rw-r--r--   0 peet      (1001) peet      (1001)    19622 2023-03-15 10:10:02.000000 pyroute2-0.7.7/pyroute2/wiset.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.458275 pyroute2-0.7.7/pyroute2.egg-info/
--rw-r--r--   0 peet      (1001) peet      (1001)     8172 2023-04-14 19:19:17.000000 pyroute2-0.7.7/pyroute2.egg-info/PKG-INFO
--rw-r--r--   0 peet      (1001) peet      (1001)     9472 2023-04-14 19:19:17.000000 pyroute2-0.7.7/pyroute2.egg-info/SOURCES.txt
--rw-r--r--   0 peet      (1001) peet      (1001)        1 2023-04-14 19:19:17.000000 pyroute2-0.7.7/pyroute2.egg-info/dependency_links.txt
--rw-r--r--   0 peet      (1001) peet      (1001)      206 2023-04-14 19:19:17.000000 pyroute2-0.7.7/pyroute2.egg-info/entry_points.txt
--rw-r--r--   0 peet      (1001) peet      (1001)       93 2023-04-14 19:19:17.000000 pyroute2-0.7.7/pyroute2.egg-info/requires.txt
--rw-r--r--   0 peet      (1001) peet      (1001)       20 2023-04-14 19:19:17.000000 pyroute2-0.7.7/pyroute2.egg-info/top_level.txt
--rw-r--r--   0 peet      (1001) peet      (1001)     1525 2023-04-14 19:19:17.496275 pyroute2-0.7.7/setup.cfg
--rw-r--r--   0 peet      (1001) peet      (1001)       38 2023-03-15 10:10:02.000000 pyroute2-0.7.7/setup.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.446275 pyroute2-0.7.7/tests/
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.494275 pyroute2-0.7.7/tests/test_unit/
--rw-r--r--   0 peet      (1001) peet      (1001)     2096 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_addr_pool.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1892 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_buffer.py
--rw-r--r--   0 peet      (1001) peet      (1001)      891 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_common.py
--rw-r--r--   0 peet      (1001) peet      (1001)      422 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_config.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.494275 pyroute2-0.7.7/tests/test_unit/test_entry_points/
--rw-r--r--   0 peet      (1001) peet      (1001)      379 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_entry_points/test_basic.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.494275 pyroute2-0.7.7/tests/test_unit/test_iproute_match/
--rw-r--r--   0 peet      (1001) peet      (1001)    50363 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_iproute_match/links.dump
--rw-r--r--   0 peet      (1001) peet      (1001)     2175 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_iproute_match/test_match.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.495275 pyroute2-0.7.7/tests/test_unit/test_nlmsg/
--rw-r--r--   0 peet      (1001) peet      (1001)     1308 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_nlmsg/addrmsg_ipv4.dump
--rw-r--r--   0 peet      (1001) peet      (1001)     4287 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_nlmsg/gre_01.dump
--rw-r--r--   0 peet      (1001) peet      (1001)     1395 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_nlmsg/iw_info_rsp.dump
--rw-r--r--   0 peet      (1001) peet      (1001)    32910 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_nlmsg/iw_scan_rsp.dump
--rw-r--r--   0 peet      (1001) peet      (1001)      722 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_nlmsg/test_attr.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1819 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_nlmsg/test_map_adapter.py
--rw-r--r--   0 peet      (1001) peet      (1001)     4154 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_nlmsg/test_marshal.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-04-14 19:19:17.496275 pyroute2-0.7.7/tests/test_unit/test_requests/
--rw-r--r--   0 peet      (1001) peet      (1001)      375 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_requests/common.py
--rw-r--r--   0 peet      (1001) peet      (1001)     6431 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_requests/test_address.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2515 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_requests/test_link.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2960 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_requests/test_neighbour.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3938 2023-03-15 10:10:02.000000 pyroute2-0.7.7/tests/test_unit/test_requests/test_route.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.658496 pyroute2-0.7.8/
+-rw-r--r--   0 peet      (1001) peet      (1001)    28688 2023-05-05 08:37:53.000000 pyroute2-0.7.8/CHANGELOG.rst
+-rw-r--r--   0 peet      (1001) peet      (1001)       31 2023-03-15 10:10:02.000000 pyroute2-0.7.8/LICENSE
+-rw-r--r--   0 peet      (1001) peet      (1001)    11348 2023-03-15 10:10:02.000000 pyroute2-0.7.8/LICENSE.Apache-2.0
+-rw-r--r--   0 peet      (1001) peet      (1001)    18092 2023-03-15 10:10:02.000000 pyroute2-0.7.8/LICENSE.GPL-2.0-or-later
+-rw-r--r--   0 peet      (1001) peet      (1001)      237 2023-03-15 10:10:02.000000 pyroute2-0.7.8/MANIFEST.in
+-rw-r--r--   0 peet      (1001) peet      (1001)     8172 2023-05-05 11:34:45.658496 pyroute2-0.7.8/PKG-INFO
+-rw-r--r--   0 peet      (1001) peet      (1001)     2198 2023-03-15 10:10:02.000000 pyroute2-0.7.8/README.contribute.rst
+-rw-r--r--   0 peet      (1001) peet      (1001)      340 2023-03-15 10:10:02.000000 pyroute2-0.7.8/README.license.rst
+-rw-r--r--   0 peet      (1001) peet      (1001)      397 2023-03-15 10:10:02.000000 pyroute2-0.7.8/README.minimal.rst
+-rw-r--r--   0 peet      (1001) peet      (1001)      757 2023-03-15 10:10:02.000000 pyroute2-0.7.8/README.report.rst
+-rw-r--r--   0 peet      (1001) peet      (1001)     6853 2023-03-15 10:10:02.000000 pyroute2-0.7.8/README.rst
+-rw-r--r--   0 peet      (1001) peet      (1001)        6 2023-05-05 11:34:23.000000 pyroute2-0.7.8/VERSION
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.594496 pyroute2-0.7.8/examples/
+-rw-r--r--   0 peet      (1001) peet      (1001)       18 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/README.md
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.594496 pyroute2-0.7.8/examples/devlink/
+-rw-r--r--   0 peet      (1001) peet      (1001)      224 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/devlink/devlink_list.py
+-rw-r--r--   0 peet      (1001) peet      (1001)       80 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/devlink/devlink_monitor.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      284 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/devlink/devlink_port_list.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.596496 pyroute2-0.7.8/examples/ethtool/
+-rw-r--r--   0 peet      (1001) peet      (1001)      816 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ethtool/ethtool-ioctl_get_infos.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      496 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ethtool/ethtool-netlink_get_infos.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      391 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ethtool/ethtool_get_infos.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.596496 pyroute2-0.7.8/examples/generic/
+-rw-r--r--   0 peet      (1001) peet      (1001)      155 2022-05-21 16:48:21.000000 pyroute2-0.7.8/examples/generic/Makefile
+-rw-r--r--   0 peet      (1001) peet      (1001)     3561 2022-05-21 16:48:21.000000 pyroute2-0.7.8/examples/generic/netl.c
+-rwxr-xr-x   0 peet      (1001) peet      (1001)     1179 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/generic/netl.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      391 2022-05-21 16:48:21.000000 pyroute2-0.7.8/examples/ipq.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.596496 pyroute2-0.7.8/examples/iproute/
+-rw-r--r--   0 peet      (1001) peet      (1001)      187 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/iproute/ip_monitor.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1523 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ipset.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      127 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/kobject_uevent.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.597496 pyroute2-0.7.8/examples/lab/
+-rw-r--r--   0 peet      (1001) peet      (1001)      462 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/README.rst
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.598496 pyroute2-0.7.8/examples/lab/iproute_get_addr/
+-rw-r--r--   0 peet      (1001) peet      (1001)      162 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/iproute_get_addr/README.rst
+-rw-r--r--   0 peet      (1001) peet      (1001)      323 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/iproute_get_addr/check.py
+-rw-r--r--   0 peet      (1001) peet      (1001)       64 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/iproute_get_addr/setup.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      102 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/iproute_get_addr/task.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.599496 pyroute2-0.7.8/examples/lab/iproute_get_attr/
+-rw-r--r--   0 peet      (1001) peet      (1001)      341 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/iproute_get_attr/README.rst
+-rw-r--r--   0 peet      (1001) peet      (1001)      252 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/iproute_get_attr/check.py
+-rw-r--r--   0 peet      (1001) peet      (1001)       64 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/iproute_get_attr/setup.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      308 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/lab/iproute_get_attr/task.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.600496 pyroute2-0.7.8/examples/ndb/
+-rw-r--r--   0 peet      (1001) peet      (1001)      752 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ndb/create_bond.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      643 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ndb/create_interface.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      684 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ndb/create_vlan.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3546 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ndb/keystone_auth.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2188 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/ndb/radius_auth.py
+-rwxr-xr-x   0 peet      (1001) peet      (1001)      444 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/nftables.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1522 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/nftables_sets.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.600496 pyroute2-0.7.8/examples/policy/
+-rwxr-xr-x   0 peet      (1001) peet      (1001)      536 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/policy/policy.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.600496 pyroute2-0.7.8/examples/processes/
+-rw-r--r--   0 peet      (1001) peet      (1001)      414 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/processes/pmonitor.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      246 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/processes/taskstats.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.601496 pyroute2-0.7.8/examples/pyroute2-cli/
+-rw-r--r--   0 peet      (1001) peet      (1001)      300 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/pyroute2-cli/comments
+-rw-r--r--   0 peet      (1001) peet      (1001)     1869 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/pyroute2-cli/create_bridge
+-rw-r--r--   0 peet      (1001) peet      (1001)      723 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/pyroute2-cli/create_dummy
+-rw-r--r--   0 peet      (1001) peet      (1001)       87 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/pyroute2-cli/dump_lo
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.602496 pyroute2-0.7.8/examples/wifi/
+-rw-r--r--   0 peet      (1001) peet      (1001)      464 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/wifi/nl80211_interface_type.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      422 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/wifi/nl80211_interfaces.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      113 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/wifi/nl80211_monitor.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2504 2023-03-15 10:10:02.000000 pyroute2-0.7.8/examples/wifi/nl80211_scan_dump.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.602496 pyroute2-0.7.8/pr2modules/
+-rw-r--r--   0 peet      (1001) peet      (1001)      568 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pr2modules/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)       90 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyproject.toml
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.605496 pyroute2-0.7.8/pyroute2/
+-rw-r--r--   0 peet      (1001) peet      (1001)     2876 2023-04-05 11:12:40.000000 pyroute2-0.7.8/pyroute2/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2474 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/arp.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.607496 pyroute2-0.7.8/pyroute2/bsd/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2-0.7.8/pyroute2/bsd/__init__.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.608496 pyroute2-0.7.8/pyroute2/bsd/pf_route/
+-rw-r--r--   0 peet      (1001) peet      (1001)     4186 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/bsd/pf_route/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3270 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/bsd/pf_route/freebsd.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3607 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/bsd/pf_route/openbsd.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.608496 pyroute2-0.7.8/pyroute2/bsd/rtmsocket/
+-rw-r--r--   0 peet      (1001) peet      (1001)     4287 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/bsd/rtmsocket/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1382 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/bsd/rtmsocket/freebsd.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1423 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/bsd/rtmsocket/openbsd.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     8136 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/bsd/util.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.609496 pyroute2-0.7.8/pyroute2/cli/
+-rw-r--r--   0 peet      (1001) peet      (1001)     2991 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/cli/__init__.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.610496 pyroute2-0.7.8/pyroute2/cli/auth/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/cli/auth/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1194 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/cli/auth/auth_keystone.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      774 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/cli/auth/auth_radius.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3296 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/cli/console.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     5586 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/cli/parser.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3188 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/cli/server.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     9156 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/cli/session.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    17833 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/common.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.610496 pyroute2-0.7.8/pyroute2/config/
+-rw-r--r--   0 peet      (1001) peet      (1001)     1365 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/config/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2340 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/config/asyncio.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      258 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/config/eventlet.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      541 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/config/log.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     8497 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/config/test_platform.py
+-rw-r--r--   0 peet      (1001) peet      (1001)       22 2023-05-05 11:34:23.000000 pyroute2-0.7.8/pyroute2/config/version.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     6845 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/conntrack.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2071 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/devlink.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.611496 pyroute2-0.7.8/pyroute2/dhcp/
+-rw-r--r--   0 peet      (1001) peet      (1001)    10048 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/dhcp/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1896 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/dhcp/client.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2066 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/dhcp/dhcp4msg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     4120 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/dhcp/dhcp4socket.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.613496 pyroute2-0.7.8/pyroute2/ethtool/
+-rw-r--r--   0 peet      (1001) peet      (1001)       50 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ethtool/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     6700 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ethtool/common.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    11964 2023-03-16 09:44:55.000000 pyroute2-0.7.8/pyroute2/ethtool/ethtool.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    18285 2023-03-16 09:44:55.000000 pyroute2-0.7.8/pyroute2/ethtool/ioctl.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.613496 pyroute2-0.7.8/pyroute2/ext/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ext/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      318 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ext/icmp.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3853 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ext/rawsocket.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.614496 pyroute2-0.7.8/pyroute2/inotify/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/inotify/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2403 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/inotify/inotify_fd.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      539 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/inotify/inotify_msg.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.616496 pyroute2-0.7.8/pyroute2/ipdb/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2-0.7.8/pyroute2/ipdb/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      237 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipdb/exceptions.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    53683 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipdb/interfaces.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     9458 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipdb/linkedset.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    49046 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipdb/main.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    46123 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipdb/routes.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     9617 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipdb/rules.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    16515 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipdb/transactional.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      222 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipdb/utils.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.618496 pyroute2-0.7.8/pyroute2/iproute/
+-rw-r--r--   0 peet      (1001) peet      (1001)     4920 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/iproute/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    10532 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/iproute/bsd.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    23630 2023-04-05 11:12:44.000000 pyroute2-0.7.8/pyroute2/iproute/ipmock.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    82477 2023-03-16 14:35:20.000000 pyroute2-0.7.8/pyroute2/iproute/linux.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1313 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/iproute/parsers.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     8082 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/iproute/windows.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    24131 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ipset.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    22019 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/iwutil.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      419 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/lab.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1139 2023-04-05 11:12:40.000000 pyroute2-0.7.8/pyroute2/loader.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1834 2023-04-05 11:12:40.000000 pyroute2-0.7.8/pyroute2/minimal.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.621496 pyroute2-0.7.8/pyroute2/ndb/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:43:06.000000 pyroute2-0.7.8/pyroute2/ndb/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2647 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/auth_manager.py
+-rwxr-xr-x   0 peet      (1001) peet      (1001)     2163 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/cli.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1003 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/cluster.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1352 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/compat.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2067 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/events.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    21420 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/main.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      246 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/messages.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     5147 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/noipdb.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.622496 pyroute2-0.7.8/pyroute2/ndb/objects/
+-rw-r--r--   0 peet      (1001) peet      (1001)    37851 2023-04-05 11:12:44.000000 pyroute2-0.7.8/pyroute2/ndb/objects/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     9028 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/objects/address.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    34524 2023-04-05 11:12:44.000000 pyroute2-0.7.8/pyroute2/ndb/objects/interface.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     4832 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/objects/neighbour.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1977 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/objects/netns.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    28891 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/objects/route.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2440 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/objects/rule.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     4867 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/query.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    11291 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/report.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    32754 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/schema.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    16500 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/source.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     9808 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/task_manager.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    11313 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/transaction.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     6350 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/ndb/transport.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    15974 2023-04-05 11:12:44.000000 pyroute2-0.7.8/pyroute2/ndb/view.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.625496 pyroute2-0.7.8/pyroute2/netlink/
+-rw-r--r--   0 peet      (1001) peet      (1001)    72813 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1947 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/buffer.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.625496 pyroute2-0.7.8/pyroute2/netlink/connector/
+-rw-r--r--   0 peet      (1001) peet      (1001)      405 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/connector/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3998 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/connector/cn_proc.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.626496 pyroute2-0.7.8/pyroute2/netlink/devlink/
+-rw-r--r--   0 peet      (1001) peet      (1001)    23285 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/devlink/__init__.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.626496 pyroute2-0.7.8/pyroute2/netlink/diag/
+-rw-r--r--   0 peet      (1001) peet      (1001)    10423 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/diag/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    18781 2023-05-05 08:37:08.000000 pyroute2-0.7.8/pyroute2/netlink/diag/ss2.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.627496 pyroute2-0.7.8/pyroute2/netlink/event/
+-rw-r--r--   0 peet      (1001) peet      (1001)      714 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/event/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2078 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/event/acpi_event.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2034 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/event/dquot.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2594 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/event/thermal.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1616 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/exceptions.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.628496 pyroute2-0.7.8/pyroute2/netlink/generic/
+-rw-r--r--   0 peet      (1001) peet      (1001)     3910 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/generic/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     7467 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/generic/ethtool.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    19073 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/generic/l2tp.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3928 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/generic/mptcp.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    12476 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/generic/wireguard.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.628496 pyroute2-0.7.8/pyroute2/netlink/ipq/
+-rw-r--r--   0 peet      (1001) peet      (1001)     3315 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/ipq/__init__.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.629496 pyroute2-0.7.8/pyroute2/netlink/nfnetlink/
+-rw-r--r--   0 peet      (1001) peet      (1001)     1036 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/nfnetlink/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     7145 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/nfnetlink/ipset.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    27707 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/nfnetlink/nfctsocket.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    43123 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/nfnetlink/nftsocket.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.629496 pyroute2-0.7.8/pyroute2/netlink/nl80211/
+-rw-r--r--   0 peet      (1001) peet      (1001)    61729 2023-04-05 11:25:50.000000 pyroute2-0.7.8/pyroute2/netlink/nl80211/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    49725 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/nlsocket.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2317 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/proxy.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.631496 pyroute2-0.7.8/pyroute2/netlink/rtnl/
+-rw-r--r--   0 peet      (1001) peet      (1001)     5988 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      155 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/errmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2428 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/fibmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2799 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifaddrmsg.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.633496 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/
+-rw-r--r--   0 peet      (1001) peet      (1001)    43260 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    10801 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/compat.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.637496 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1747 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/bond.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      776 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/geneve.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      227 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/gtp.py
+-rwxr-xr-x   0 peet      (1001) peet      (1001)      376 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/ipoib.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      291 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/ipvlan.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      151 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/team.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      494 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/tun.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      569 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/tuntap.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      751 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vlan.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      146 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vrf.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      317 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vti.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      357 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vti6.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1417 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vxlan.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      189 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/xfrm.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3428 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/proxy.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1974 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/sync.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3875 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/tuntap.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2583 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ifstatsmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     5802 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/iprsocket.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3244 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/iw_event.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2018 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/marshal.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2607 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ndmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2188 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/ndtmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      321 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/nsidmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      522 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/nsinfmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      366 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/p2pmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      523 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/riprsocket.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      114 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/rtgenmsg.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    26078 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/rtmsg.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.646496 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/
+-rw-r--r--   0 peet      (1001) peet      (1001)     2743 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      979 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_bpf.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1234 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_connmark.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      709 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_gact.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1725 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_mirred.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1866 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_police.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3338 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_skbedit.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1465 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_vlan.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     8478 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_basic.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     4613 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_flow.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1427 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_fw.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      986 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_matchall.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     8033 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_u32.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    10724 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/common.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2063 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/common_act.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3148 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/common_ematch.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2776 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_cmp.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1741 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_ipset.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     5933 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_meta.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2571 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_bpf.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    12834 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_cake.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3431 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_choke.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1010 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_clsact.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1607 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_codel.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      754 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_drr.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2658 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_fq_codel.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2352 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_hfsc.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     5738 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_htb.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      214 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_ingress.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     5111 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_netem.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      196 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_pfifo.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      215 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_pfifo_fast.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      446 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_plug.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2717 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_sfq.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1087 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_tbf.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1249 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_template.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.646496 pyroute2-0.7.8/pyroute2/netlink/taskstats/
+-rw-r--r--   0 peet      (1001) peet      (1001)     4920 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/taskstats/__init__.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.646496 pyroute2-0.7.8/pyroute2/netlink/uevent/
+-rw-r--r--   0 peet      (1001) peet      (1001)     1096 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netlink/uevent/__init__.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.647496 pyroute2-0.7.8/pyroute2/netns/
+-rw-r--r--   0 peet      (1001) peet      (1001)    10678 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netns/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3803 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/netns/manager.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.647496 pyroute2-0.7.8/pyroute2/nftables/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2-0.7.8/pyroute2/nftables/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2530 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nftables/expressions.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    12712 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nftables/main.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.649496 pyroute2-0.7.8/pyroute2/nftables/parser/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nftables/parser/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    10530 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nftables/parser/expr.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2394 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nftables/parser/parser.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3892 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nftables/rule.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.649496 pyroute2-0.7.8/pyroute2/nslink/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nslink/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     6785 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nslink/nslink.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    11393 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/nslink/nspopen.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.650496 pyroute2-0.7.8/pyroute2/protocols/
+-rw-r--r--   0 peet      (1001) peet      (1001)     8716 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/protocols/__init__.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.650496 pyroute2-0.7.8/pyroute2/remote/
+-rw-r--r--   0 peet      (1001) peet      (1001)      206 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/remote/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      111 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/remote/__main__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     4503 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/remote/iproute.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2084 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/remote/shell.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    11899 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/remote/transport.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.653496 pyroute2-0.7.8/pyroute2/requests/
+-rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/__init__.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3430 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/address.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     5195 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/bridge.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     5083 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/common.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     9174 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/link.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2005 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/main.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1241 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/neighbour.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      107 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/netns.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    19591 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/route.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1229 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/requests/rule.py
+-rw-r--r--   0 peet      (1001) peet      (1001)    19622 2023-03-15 10:10:02.000000 pyroute2-0.7.8/pyroute2/wiset.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.607496 pyroute2-0.7.8/pyroute2.egg-info/
+-rw-r--r--   0 peet      (1001) peet      (1001)     8172 2023-05-05 11:34:45.000000 pyroute2-0.7.8/pyroute2.egg-info/PKG-INFO
+-rw-r--r--   0 peet      (1001) peet      (1001)     9472 2023-05-05 11:34:45.000000 pyroute2-0.7.8/pyroute2.egg-info/SOURCES.txt
+-rw-r--r--   0 peet      (1001) peet      (1001)        1 2023-05-05 11:34:45.000000 pyroute2-0.7.8/pyroute2.egg-info/dependency_links.txt
+-rw-r--r--   0 peet      (1001) peet      (1001)      206 2023-05-05 11:34:45.000000 pyroute2-0.7.8/pyroute2.egg-info/entry_points.txt
+-rw-r--r--   0 peet      (1001) peet      (1001)       93 2023-05-05 11:34:45.000000 pyroute2-0.7.8/pyroute2.egg-info/requires.txt
+-rw-r--r--   0 peet      (1001) peet      (1001)       20 2023-05-05 11:34:45.000000 pyroute2-0.7.8/pyroute2.egg-info/top_level.txt
+-rw-r--r--   0 peet      (1001) peet      (1001)     1525 2023-05-05 11:34:45.659496 pyroute2-0.7.8/setup.cfg
+-rw-r--r--   0 peet      (1001) peet      (1001)       38 2023-03-15 10:10:02.000000 pyroute2-0.7.8/setup.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.589496 pyroute2-0.7.8/tests/
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.654496 pyroute2-0.7.8/tests/test_unit/
+-rw-r--r--   0 peet      (1001) peet      (1001)     2096 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_addr_pool.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1892 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_buffer.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      891 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_common.py
+-rw-r--r--   0 peet      (1001) peet      (1001)      422 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_config.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.654496 pyroute2-0.7.8/tests/test_unit/test_entry_points/
+-rw-r--r--   0 peet      (1001) peet      (1001)      379 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_entry_points/test_basic.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.655496 pyroute2-0.7.8/tests/test_unit/test_iproute_match/
+-rw-r--r--   0 peet      (1001) peet      (1001)    50363 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_iproute_match/links.dump
+-rw-r--r--   0 peet      (1001) peet      (1001)     2175 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_iproute_match/test_match.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.657496 pyroute2-0.7.8/tests/test_unit/test_nlmsg/
+-rw-r--r--   0 peet      (1001) peet      (1001)     1308 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_nlmsg/addrmsg_ipv4.dump
+-rw-r--r--   0 peet      (1001) peet      (1001)     4287 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_nlmsg/gre_01.dump
+-rw-r--r--   0 peet      (1001) peet      (1001)     1395 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_nlmsg/iw_info_rsp.dump
+-rw-r--r--   0 peet      (1001) peet      (1001)    32910 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_nlmsg/iw_scan_rsp.dump
+-rw-r--r--   0 peet      (1001) peet      (1001)      722 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_nlmsg/test_attr.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     1819 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_nlmsg/test_map_adapter.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     4154 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_nlmsg/test_marshal.py
+drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-05-05 11:34:45.657496 pyroute2-0.7.8/tests/test_unit/test_requests/
+-rw-r--r--   0 peet      (1001) peet      (1001)      375 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_requests/common.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     6431 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_requests/test_address.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2515 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_requests/test_link.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     2960 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_requests/test_neighbour.py
+-rw-r--r--   0 peet      (1001) peet      (1001)     3938 2023-03-15 10:10:02.000000 pyroute2-0.7.8/tests/test_unit/test_requests/test_route.py
```

### Comparing `pyroute2-0.7.7/CHANGELOG.rst` & `pyroute2-0.7.8/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Changelog
 =========
 
+* 0.7.8
+    * ss2: more fixes <https://github.com/svinota/pyroute2/pull/1088>
 * 0.7.7
     * ss2: user context patch <https://github.com/svinota/pyroute2/pull/1087>
     * ndb: basic altname support
     * nl80211: decoder improvements <https://github.com/svinota/pyroute2/pull/1086>
 * 0.7.6
     * setup: static loader <https://github.com/svinota/pyroute2/issues/1076>
     * iproute: support altname in link_lookup()
```

### Comparing `pyroute2-0.7.7/LICENSE.Apache-2.0` & `pyroute2-0.7.8/LICENSE.Apache-2.0`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/LICENSE.GPL-2.0-or-later` & `pyroute2-0.7.8/LICENSE.GPL-2.0-or-later`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/PKG-INFO` & `pyroute2-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroute2
-Version: 0.7.7
+Version: 0.7.8
 Summary: Python Netlink library
 Home-page: https://github.com/svinota/pyroute2
 Author: Peter Saveliev
 Author-email: peter@svinota.eu
 License: GPL-2.0-or-later OR Apache-2.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyroute2-0.7.7/README.contribute.rst` & `pyroute2-0.7.8/README.contribute.rst`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/README.report.rst` & `pyroute2-0.7.8/README.report.rst`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/README.rst` & `pyroute2-0.7.8/README.rst`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/ethtool/ethtool-ioctl_get_infos.py` & `pyroute2-0.7.8/examples/ethtool/ethtool-ioctl_get_infos.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/generic/netl.c` & `pyroute2-0.7.8/examples/generic/netl.c`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/generic/netl.py` & `pyroute2-0.7.8/examples/generic/netl.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/ipset.py` & `pyroute2-0.7.8/examples/ipset.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/ndb/create_bond.py` & `pyroute2-0.7.8/examples/ndb/create_bond.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/ndb/create_interface.py` & `pyroute2-0.7.8/examples/ndb/create_interface.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/ndb/create_vlan.py` & `pyroute2-0.7.8/examples/ndb/create_vlan.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/ndb/keystone_auth.py` & `pyroute2-0.7.8/examples/ndb/keystone_auth.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/ndb/radius_auth.py` & `pyroute2-0.7.8/examples/ndb/radius_auth.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/nftables_sets.py` & `pyroute2-0.7.8/examples/nftables_sets.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/policy/policy.py` & `pyroute2-0.7.8/examples/policy/policy.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/pyroute2-cli/create_bridge` & `pyroute2-0.7.8/examples/pyroute2-cli/create_bridge`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/pyroute2-cli/create_dummy` & `pyroute2-0.7.8/examples/pyroute2-cli/create_dummy`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/examples/wifi/nl80211_scan_dump.py` & `pyroute2-0.7.8/examples/wifi/nl80211_scan_dump.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pr2modules/__init__.py` & `pyroute2-0.7.8/pr2modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/__init__.py` & `pyroute2-0.7.8/pyroute2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/arp.py` & `pyroute2-0.7.8/pyroute2/arp.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/bsd/pf_route/__init__.py` & `pyroute2-0.7.8/pyroute2/bsd/pf_route/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/bsd/pf_route/freebsd.py` & `pyroute2-0.7.8/pyroute2/bsd/pf_route/freebsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/bsd/pf_route/openbsd.py` & `pyroute2-0.7.8/pyroute2/bsd/pf_route/openbsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/bsd/rtmsocket/__init__.py` & `pyroute2-0.7.8/pyroute2/bsd/rtmsocket/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/bsd/rtmsocket/freebsd.py` & `pyroute2-0.7.8/pyroute2/bsd/rtmsocket/freebsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/bsd/rtmsocket/openbsd.py` & `pyroute2-0.7.8/pyroute2/bsd/rtmsocket/openbsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/bsd/util.py` & `pyroute2-0.7.8/pyroute2/bsd/util.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/cli/__init__.py` & `pyroute2-0.7.8/pyroute2/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/cli/auth/auth_keystone.py` & `pyroute2-0.7.8/pyroute2/cli/auth/auth_keystone.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/cli/auth/auth_radius.py` & `pyroute2-0.7.8/pyroute2/cli/auth/auth_radius.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/cli/console.py` & `pyroute2-0.7.8/pyroute2/cli/console.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/cli/parser.py` & `pyroute2-0.7.8/pyroute2/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/cli/server.py` & `pyroute2-0.7.8/pyroute2/cli/server.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/cli/session.py` & `pyroute2-0.7.8/pyroute2/cli/session.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/common.py` & `pyroute2-0.7.8/pyroute2/common.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/config/__init__.py` & `pyroute2-0.7.8/pyroute2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/config/asyncio.py` & `pyroute2-0.7.8/pyroute2/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/config/log.py` & `pyroute2-0.7.8/pyroute2/config/log.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/config/test_platform.py` & `pyroute2-0.7.8/pyroute2/config/test_platform.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/conntrack.py` & `pyroute2-0.7.8/pyroute2/conntrack.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/devlink.py` & `pyroute2-0.7.8/pyroute2/devlink.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/dhcp/__init__.py` & `pyroute2-0.7.8/pyroute2/dhcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/dhcp/client.py` & `pyroute2-0.7.8/pyroute2/dhcp/client.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/dhcp/dhcp4msg.py` & `pyroute2-0.7.8/pyroute2/dhcp/dhcp4msg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/dhcp/dhcp4socket.py` & `pyroute2-0.7.8/pyroute2/dhcp/dhcp4socket.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ethtool/common.py` & `pyroute2-0.7.8/pyroute2/ethtool/common.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ethtool/ethtool.py` & `pyroute2-0.7.8/pyroute2/ethtool/ethtool.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ethtool/ioctl.py` & `pyroute2-0.7.8/pyroute2/ethtool/ioctl.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ext/rawsocket.py` & `pyroute2-0.7.8/pyroute2/ext/rawsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/inotify/inotify_fd.py` & `pyroute2-0.7.8/pyroute2/inotify/inotify_fd.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/inotify/inotify_msg.py` & `pyroute2-0.7.8/pyroute2/inotify/inotify_msg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ipdb/interfaces.py` & `pyroute2-0.7.8/pyroute2/ipdb/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ipdb/linkedset.py` & `pyroute2-0.7.8/pyroute2/ipdb/linkedset.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ipdb/main.py` & `pyroute2-0.7.8/pyroute2/ipdb/main.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ipdb/routes.py` & `pyroute2-0.7.8/pyroute2/ipdb/routes.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ipdb/rules.py` & `pyroute2-0.7.8/pyroute2/ipdb/rules.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ipdb/transactional.py` & `pyroute2-0.7.8/pyroute2/ipdb/transactional.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/iproute/__init__.py` & `pyroute2-0.7.8/pyroute2/iproute/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/iproute/bsd.py` & `pyroute2-0.7.8/pyroute2/iproute/bsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/iproute/ipmock.py` & `pyroute2-0.7.8/pyroute2/iproute/ipmock.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/iproute/linux.py` & `pyroute2-0.7.8/pyroute2/iproute/linux.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/iproute/parsers.py` & `pyroute2-0.7.8/pyroute2/iproute/parsers.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/iproute/windows.py` & `pyroute2-0.7.8/pyroute2/iproute/windows.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ipset.py` & `pyroute2-0.7.8/pyroute2/ipset.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/iwutil.py` & `pyroute2-0.7.8/pyroute2/iwutil.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/loader.py` & `pyroute2-0.7.8/pyroute2/loader.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/minimal.py` & `pyroute2-0.7.8/pyroute2/minimal.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/auth_manager.py` & `pyroute2-0.7.8/pyroute2/ndb/auth_manager.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/cli.py` & `pyroute2-0.7.8/pyroute2/ndb/cli.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/cluster.py` & `pyroute2-0.7.8/pyroute2/ndb/cluster.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/compat.py` & `pyroute2-0.7.8/pyroute2/ndb/compat.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/events.py` & `pyroute2-0.7.8/pyroute2/ndb/events.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/main.py` & `pyroute2-0.7.8/pyroute2/ndb/main.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/noipdb.py` & `pyroute2-0.7.8/pyroute2/ndb/noipdb.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/objects/__init__.py` & `pyroute2-0.7.8/pyroute2/ndb/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/objects/address.py` & `pyroute2-0.7.8/pyroute2/ndb/objects/address.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/objects/interface.py` & `pyroute2-0.7.8/pyroute2/ndb/objects/interface.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/objects/neighbour.py` & `pyroute2-0.7.8/pyroute2/ndb/objects/neighbour.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/objects/netns.py` & `pyroute2-0.7.8/pyroute2/ndb/objects/netns.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/objects/route.py` & `pyroute2-0.7.8/pyroute2/ndb/objects/route.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/objects/rule.py` & `pyroute2-0.7.8/pyroute2/ndb/objects/rule.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/query.py` & `pyroute2-0.7.8/pyroute2/ndb/query.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/report.py` & `pyroute2-0.7.8/pyroute2/ndb/report.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/schema.py` & `pyroute2-0.7.8/pyroute2/ndb/schema.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/source.py` & `pyroute2-0.7.8/pyroute2/ndb/source.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/task_manager.py` & `pyroute2-0.7.8/pyroute2/ndb/task_manager.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/transaction.py` & `pyroute2-0.7.8/pyroute2/ndb/transaction.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/transport.py` & `pyroute2-0.7.8/pyroute2/ndb/transport.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/ndb/view.py` & `pyroute2-0.7.8/pyroute2/ndb/view.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/buffer.py` & `pyroute2-0.7.8/pyroute2/netlink/buffer.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/connector/cn_proc.py` & `pyroute2-0.7.8/pyroute2/netlink/connector/cn_proc.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/devlink/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/devlink/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/diag/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/diag/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/diag/ss2.py` & `pyroute2-0.7.8/pyroute2/netlink/diag/ss2.py`

 * *Files 17% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     _BUILD_RECURS_PATH = ["inode", "usr", "pid", "fd"]
 
     def _parse_inode(self, sconn):
         sk_path = self._proc_sk_fd_cast % (sconn.pid, sconn.fd)
         inode = None
 
         sk_inode_raw = os.readlink(sk_path)
-        inode = self._sk_inode_re.search(sk_inode_raw).group('ino')
+        inode = self._sk_inode_re.search(sk_inode_raw).group("ino")
 
         if not inode:
             raise RuntimeError("Unexpected kernel sk inode outline")
 
         return inode
 
     def __recurs_enter(
@@ -137,22 +137,26 @@
             _pid=flow.pid,
             _ctxt=ctxt,
             _recurs_path=recurs_path,
         )
 
     def _build(self):
         for flow in psutil.net_connections(kind="all"):
-            proc = psutil.Process(flow.pid)
-            usr = proc.username()
+            try:
+                proc = psutil.Process(flow.pid)
+                usr = proc.username()
 
-            ctxt = {"cmd": proc.exe(), "full_cmd": proc.cmdline(), "fds": []}
+                ctxt = {
+                    "cmd": proc.exe(),
+                    "full_cmd": proc.cmdline(),
+                    "fds": [],
+                }
 
-            try:
                 self._enter_item(usr, flow, ctxt)
-            except FileNotFoundError:
+            except (FileNotFoundError, AttributeError, psutil.NoSuchProcess):
                 # Handling edge case of race condition between build and parse
                 # time. That's for very volatile, shortlived flows that can
                 # exist during build but are gone once we want to parse the
                 # inode.
                 pass
 
     def __init__(self):
@@ -179,99 +183,99 @@
                 data = socket.gethostbyaddr(ip)
                 host = str(data[0])
                 return host
             except Exception:
                 # gracefully
                 return None
 
-    def __init__(self, sk_states, fmt='json'):
+    def __init__(self, sk_states, fmt="json"):
         self._states = sk_states
 
         fmter = "_fmt_%s" % fmt
         self._fmt = getattr(self, fmter, None)
 
         def __call__(self, nl_diag_sk, args, usr_ctxt):
-            raise RuntimeError('not implemented')
+            raise RuntimeError("not implemented")
 
     def _fmt_json(self, refined_stats):
         return json.dumps(refined_stats, indent=4)
 
 
 class UNIX(Protocol):
-    def __init__(self, sk_states=SS_CONN, _fmt='json'):
+    def __init__(self, sk_states=SS_CONN, _fmt="json"):
         super(UNIX, self).__init__(sk_states, fmt=_fmt)
 
     def __call__(self, nl_diag_sk, args, usr_ctxt):
         sstats = nl_diag_sk.get_sock_stats(
             states=self._states,
             family=AF_UNIX,
             show=(UDIAG_SHOW_NAME | UDIAG_SHOW_VFS | UDIAG_SHOW_PEER),
         )
         refined_stats = self._refine_diag_raw(sstats, usr_ctxt)
         printable = self._fmt(refined_stats)
 
         print(printable)
 
     def _refine_diag_raw(self, raw_stats, usr_ctxt):
-        refined = {'UNIX': {'flows': []}}
+        refined = {"UNIX": {"flows": []}}
 
         def vfs_cb(raw_val):
             out = {}
-            out['inode'] = raw_val['udiag_vfs_ino']
-            out['dev'] = raw_val['udiag_vfs_dev']
+            out["inode"] = raw_val["udiag_vfs_ino"]
+            out["dev"] = raw_val["udiag_vfs_dev"]
 
             return out
 
         k_idx = 0
         val_idx = 1
         cb_idx = 1
 
         idiag_attr_refine_map = {
-            'UNIX_DIAG_NAME': ('path_name', None),
-            'UNIX_DIAG_VFS': ('vfs', vfs_cb),
-            'UNIX_DIAG_PEER': ('peer_inode', None),
-            'UNIX_DIAG_SHUTDOWN': ('shutdown', None),
+            "UNIX_DIAG_NAME": ("path_name", None),
+            "UNIX_DIAG_VFS": ("vfs", vfs_cb),
+            "UNIX_DIAG_PEER": ("peer_inode", None),
+            "UNIX_DIAG_SHUTDOWN": ("shutdown", None),
         }
 
         for raw_flow in raw_stats:
             vessel = {}
-            vessel['inode'] = raw_flow['udiag_ino']
+            vessel["inode"] = raw_flow["udiag_ino"]
 
-            for attr in raw_flow['attrs']:
+            for attr in raw_flow["attrs"]:
                 attr_k = attr[k_idx]
                 attr_val = attr[val_idx]
                 k = idiag_attr_refine_map[attr_k][k_idx]
                 cb = idiag_attr_refine_map[attr_k][cb_idx]
 
                 if cb:
                     attr_val = cb(attr_val)
 
                 vessel[k] = attr_val
 
-            refined['UNIX']['flows'].append(vessel)
+            refined["UNIX"]["flows"].append(vessel)
 
         if usr_ctxt:
-            for flow in refined['UNIX']['flows']:
+            for flow in refined["UNIX"]["flows"]:
                 try:
-                    sk_inode = flow['inode']
-                    flow['usr_ctxt'] = usr_ctxt[sk_inode]
+                    sk_inode = flow["inode"]
+                    flow["usr_ctxt"] = usr_ctxt[sk_inode]
                 except KeyError:
                     # might define sentinel val
                     pass
 
         return refined
 
 
 class TCP(Protocol):
     INET_DIAG_MEMINFO = 1
     INET_DIAG_INFO = 2
     INET_DIAG_VEGASINFO = 3
     INET_DIAG_CONG = 4
 
-    def __init__(self, sk_states=SS_CONN, _fmt='json'):
+    def __init__(self, sk_states=SS_CONN, _fmt="json"):
         super(TCP, self).__init__(sk_states, fmt=_fmt)
 
         IDIAG_EXT_FLAGS = [
             self.INET_DIAG_MEMINFO,
             self.INET_DIAG_INFO,
             self.INET_DIAG_VEGASINFO,
             self.INET_DIAG_CONG,
@@ -287,81 +291,81 @@
         )
         refined_stats = self._refine_diag_raw(sstats, args.resolve, usr_ctxt)
         printable = self._fmt(refined_stats)
 
         print(printable)
 
     def _refine_diag_raw(self, raw_stats, do_resolve, usr_ctxt):
-        refined = {'TCP': {'flows': []}}
+        refined = {"TCP": {"flows": []}}
 
         idiag_refine_map = {
-            'src': 'idiag_src',
-            'dst': 'idiag_dst',
-            'src_port': 'idiag_sport',
-            'dst_port': 'idiag_dport',
-            'inode': 'idiag_inode',
-            'iface_idx': 'idiag_if',
-            'retrans': 'idiag_retrans',
+            "src": "idiag_src",
+            "dst": "idiag_dst",
+            "src_port": "idiag_sport",
+            "dst_port": "idiag_dport",
+            "inode": "idiag_inode",
+            "iface_idx": "idiag_if",
+            "retrans": "idiag_retrans",
         }
 
         for raw_flow in raw_stats:
             vessel = {}
             for k1, k2 in idiag_refine_map.items():
                 vessel[k1] = raw_flow[k2]
 
-            for ext_bundle in raw_flow['attrs']:
+            for ext_bundle in raw_flow["attrs"]:
                 vessel = self._refine_extension(vessel, ext_bundle)
 
-            refined['TCP']['flows'].append(vessel)
+            refined["TCP"]["flows"].append(vessel)
 
         if usr_ctxt:
-            for flow in refined['TCP']['flows']:
+            for flow in refined["TCP"]["flows"]:
                 try:
-                    sk_inode = flow['inode']
-                    flow['usr_ctxt'] = usr_ctxt[sk_inode]
+                    sk_inode = flow["inode"]
+                    flow["usr_ctxt"] = usr_ctxt[sk_inode]
                 except KeyError:
                     # might define sentinel val
                     pass
 
         if do_resolve:
-            for flow in refined['TCP']['flows']:
-                src_host = Protocol.Resolver.getHost(flow['src'])
+            for flow in refined["TCP"]["flows"]:
+                src_host = Protocol.Resolver.getHost(flow["src"])
                 if src_host:
-                    flow['src_host'] = src_host
+                    flow["src_host"] = src_host
 
-                dst_host = Protocol.Resolver.getHost(flow['dst'])
+                dst_host = Protocol.Resolver.getHost(flow["dst"])
                 if dst_host:
-                    flow['dst_host'] = dst_host
+                    flow["dst_host"] = dst_host
 
         return refined
 
     def _refine_extension(self, vessel, raw_ext):
         k, content = raw_ext
         ext_refine_map = {
-            'meminfo': {
-                'r': 'idiag_rmem',
-                'w': 'idiag_wmem',
-                'f': 'idiag_fmem',
-                't': 'idiag_tmem',
+            "meminfo": {
+                "r": "idiag_rmem",
+                "w": "idiag_wmem",
+                "f": "idiag_fmem",
+                "t": "idiag_tmem",
             }
         }
 
-        if k == 'INET_DIAG_MEMINFO':
-            mem_k = 'meminfo'
+        if k == "INET_DIAG_MEMINFO":
+            mem_k = "meminfo"
             vessel[mem_k] = {}
             for k1, k2 in ext_refine_map[mem_k].items():
                 vessel[mem_k][k1] = content[k2]
 
-        elif k == 'INET_DIAG_CONG':
-            vessel['cong_algo'] = content
+        elif k == "INET_DIAG_CONG":
+            vessel["cong_algo"] = content
 
-        elif k == 'INET_DIAG_INFO':
+        elif k == "INET_DIAG_INFO":
             vessel = self._refine_tcp_info(vessel, content)
 
-        elif k == 'INET_DIAG_SHUTDOWN':
+        elif k == "INET_DIAG_SHUTDOWN":
             pass
 
         return vessel
 
     # interim approach
     # tcpinfo call backs
     class InfoCbCore:
@@ -384,27 +388,27 @@
             if value < 0xFFFF:
                 return value
 
             return None
 
         @staticmethod
         def rtt_p_cb(key, value, **ctx):
-            tcp_info_raw = ctx['raw']
+            tcp_info_raw = ctx["raw"]
 
             try:
                 if (
-                    tcp_info_raw['tcpv_enabled'] != 0
-                    and tcp_info_raw['tcpv_rtt'] != 0x7FFFFFFF
+                    tcp_info_raw["tcpv_enabled"] != 0
+                    and tcp_info_raw["tcpv_rtt"] != 0x7FFFFFFF
                 ):
-                    return tcp_info_raw['tcpv_rtt']
+                    return tcp_info_raw["tcpv_rtt"]
             except KeyError:
                 # ill practice, yet except quicker path
                 pass
 
-            return tcp_info_raw['tcpi_rtt'] / 1000.0
+            return tcp_info_raw["tcpi_rtt"] / 1000.0
 
         # converter
         @staticmethod
         def state_c_cb(key, value, **ctx):
             state_str_map = {
                 SS_ESTABLISHED: "established",
                 SS_SYN_SENT: "syn-sent",
@@ -419,127 +423,127 @@
                 SS_CLOSING: "closing",
             }
 
             return state_str_map[value]
 
         @staticmethod
         def opts_c_cb(key, value, **ctx):
-            tcp_info_raw = ctx['raw']
+            tcp_info_raw = ctx["raw"]
 
             # tcp_info opt flags
             TCPI_OPT_TIMESTAMPS = 1
             TCPI_OPT_SACK = 2
             TCPI_OPT_ECN = 8
 
             out = []
 
-            opts = tcp_info_raw['tcpi_options']
+            opts = tcp_info_raw["tcpi_options"]
             if opts & TCPI_OPT_TIMESTAMPS:
                 out.append("ts")
             if opts & TCPI_OPT_SACK:
                 out.append("sack")
             if opts & TCPI_OPT_ECN:
                 out.append("ecn")
 
             return out
 
     def _refine_tcp_info(self, vessel, tcp_info_raw):
         ti = TCP.InfoCbCore
 
         info_refine_tabl = {
-            'tcpi_state': ('state', ti.state_c_cb),
-            'tcpi_pmtu': ('pmtu', None),
-            'tcpi_retrans': ('retrans', None),
-            'tcpi_ato': ('ato', ti.generic_1k_n_cb),
-            'tcpi_rto': ('rto', ti.rto_n_cb),
+            "tcpi_state": ("state", ti.state_c_cb),
+            "tcpi_pmtu": ("pmtu", None),
+            "tcpi_retrans": ("retrans", None),
+            "tcpi_ato": ("ato", ti.generic_1k_n_cb),
+            "tcpi_rto": ("rto", ti.rto_n_cb),
             # TODO consider wscale baking
-            'tcpi_snd_wscale': ('snd_wscale', None),
-            'tcpi_rcv_wscale': ('rcv_wscale', None),
+            "tcpi_snd_wscale": ("snd_wscale", None),
+            "tcpi_rcv_wscale": ("rcv_wscale", None),
             # TODO bps baking
-            'tcpi_snd_mss': ('snd_mss', None),
-            'tcpi_snd_cwnd': ('snd_cwnd', None),
-            'tcpi_snd_ssthresh': ('snd_ssthresh', ti.snd_thresh_p_cb),
+            "tcpi_snd_mss": ("snd_mss", None),
+            "tcpi_snd_cwnd": ("snd_cwnd", None),
+            "tcpi_snd_ssthresh": ("snd_ssthresh", ti.snd_thresh_p_cb),
             # TODO consider rtt agglomeration - needs nesting
-            'tcpi_rtt': ('rtt', ti.rtt_p_cb),
-            'tcpi_rttvar': ('rttvar', ti.generic_1k_n_cb),
-            'tcpi_rcv_rtt': ('rcv_rtt', ti.generic_1k_n_cb),
-            'tcpi_rcv_space': ('rcv_space', None),
-            'tcpi_options': ('opts', ti.opts_c_cb),
+            "tcpi_rtt": ("rtt", ti.rtt_p_cb),
+            "tcpi_rttvar": ("rttvar", ti.generic_1k_n_cb),
+            "tcpi_rcv_rtt": ("rcv_rtt", ti.generic_1k_n_cb),
+            "tcpi_rcv_space": ("rcv_space", None),
+            "tcpi_options": ("opts", ti.opts_c_cb),
             # unclear, NB not in use by iproute2 ss latest
-            'tcpi_last_data_sent': ('last_data_sent', None),
-            'tcpi_rcv_ssthresh': ('rcv_ssthresh', None),
-            'tcpi_rcv_ssthresh': ('rcv_ssthresh', None),
-            'tcpi_segs_in': ('segs_in', None),
-            'tcpi_segs_out': ('segs_out', None),
-            'tcpi_data_segs_in': ('data_segs_in', None),
-            'tcpi_data_segs_out': ('data_segs_out', None),
-            'tcpi_lost': ('lost', None),
-            'tcpi_notsent_bytes': ('notsent_bytes', None),
-            'tcpi_rcv_mss': ('rcv_mss', None),
-            'tcpi_pacing_rate': ('pacing_rate', None),
-            'tcpi_retransmits': ('retransmits', None),
-            'tcpi_min_rtt': ('min_rtt', None),
-            'tcpi_rwnd_limited': ('rwnd_limited', None),
-            'tcpi_max_pacing_rate': ('max_pacing_rate', None),
-            'tcpi_probes': ('probes', None),
-            'tcpi_reordering': ('reordering', None),
-            'tcpi_last_data_recv': ('last_data_recv', None),
-            'tcpi_bytes_received': ('bytes_received', None),
-            'tcpi_fackets': ('fackets', None),
-            'tcpi_last_ack_recv': ('last_ack_recv', None),
-            'tcpi_last_ack_sent': ('last_ack_sent', None),
-            'tcpi_unacked': ('unacked', None),
-            'tcpi_sacked': ('sacked', None),
-            'tcpi_bytes_acked': ('bytes_acked', None),
-            'tcpi_delivery_rate_app_limited': (
-                'delivery_rate_app_limited',
+            "tcpi_last_data_sent": ("last_data_sent", None),
+            "tcpi_rcv_ssthresh": ("rcv_ssthresh", None),
+            "tcpi_rcv_ssthresh": ("rcv_ssthresh", None),
+            "tcpi_segs_in": ("segs_in", None),
+            "tcpi_segs_out": ("segs_out", None),
+            "tcpi_data_segs_in": ("data_segs_in", None),
+            "tcpi_data_segs_out": ("data_segs_out", None),
+            "tcpi_lost": ("lost", None),
+            "tcpi_notsent_bytes": ("notsent_bytes", None),
+            "tcpi_rcv_mss": ("rcv_mss", None),
+            "tcpi_pacing_rate": ("pacing_rate", None),
+            "tcpi_retransmits": ("retransmits", None),
+            "tcpi_min_rtt": ("min_rtt", None),
+            "tcpi_rwnd_limited": ("rwnd_limited", None),
+            "tcpi_max_pacing_rate": ("max_pacing_rate", None),
+            "tcpi_probes": ("probes", None),
+            "tcpi_reordering": ("reordering", None),
+            "tcpi_last_data_recv": ("last_data_recv", None),
+            "tcpi_bytes_received": ("bytes_received", None),
+            "tcpi_fackets": ("fackets", None),
+            "tcpi_last_ack_recv": ("last_ack_recv", None),
+            "tcpi_last_ack_sent": ("last_ack_sent", None),
+            "tcpi_unacked": ("unacked", None),
+            "tcpi_sacked": ("sacked", None),
+            "tcpi_bytes_acked": ("bytes_acked", None),
+            "tcpi_delivery_rate_app_limited": (
+                "delivery_rate_app_limited",
                 None,
             ),
-            'tcpi_delivery_rate': ('delivery_rate', None),
-            'tcpi_sndbuf_limited': ('sndbuf_limited', None),
-            'tcpi_ca_state': ('ca_state', None),
-            'tcpi_busy_time': ('busy_time', None),
-            'tcpi_total_retrans': ('total_retrans', None),
-            'tcpi_advmss': ('advmss', None),
-            'tcpi_backoff': (None, None),
-            'tcpv_enabled': (None, 'skip'),
-            'tcpv_rttcnt': (None, 'skip'),
-            'tcpv_rtt': (None, 'skip'),
-            'tcpv_minrtt': (None, 'skip'),
+            "tcpi_delivery_rate": ("delivery_rate", None),
+            "tcpi_sndbuf_limited": ("sndbuf_limited", None),
+            "tcpi_ca_state": ("ca_state", None),
+            "tcpi_busy_time": ("busy_time", None),
+            "tcpi_total_retrans": ("total_retrans", None),
+            "tcpi_advmss": ("advmss", None),
+            "tcpi_backoff": (None, None),
+            "tcpv_enabled": (None, "skip"),
+            "tcpv_rttcnt": (None, "skip"),
+            "tcpv_rtt": (None, "skip"),
+            "tcpv_minrtt": (None, "skip"),
             # BBR
-            'bbr_bw_lo': ('bbr_bw_lo', None),
-            'bbr_bw_hi': ('bbr_bw_hi', None),
-            'bbr_min_rtt': ('bbr_min_rtt', None),
-            'bbr_pacing_gain': ('bbr_pacing_gain', None),
-            'bbr_cwnd_gain': ('bbr_cwnd_gain', None),
+            "bbr_bw_lo": ("bbr_bw_lo", None),
+            "bbr_bw_hi": ("bbr_bw_hi", None),
+            "bbr_min_rtt": ("bbr_min_rtt", None),
+            "bbr_pacing_gain": ("bbr_pacing_gain", None),
+            "bbr_cwnd_gain": ("bbr_cwnd_gain", None),
             # DCTCP
-            'dctcp_enabled': ('dctcp_enabled', None),
-            'dctcp_ce_state': ('dctcp_ce_state', None),
-            'dctcp_alpha': ('dctcp_alpha', None),
-            'dctcp_ab_ecn': ('dctcp_ab_ecn', None),
-            'dctcp_ab_tot': ('dctcp_ab_tot', None),
+            "dctcp_enabled": ("dctcp_enabled", None),
+            "dctcp_ce_state": ("dctcp_ce_state", None),
+            "dctcp_alpha": ("dctcp_alpha", None),
+            "dctcp_ab_ecn": ("dctcp_ab_ecn", None),
+            "dctcp_ab_tot": ("dctcp_ab_tot", None),
         }
         k_idx = 0
         cb_idx = 1
 
-        info_k = 'tcp_info'
+        info_k = "tcp_info"
         vessel[info_k] = {}
 
         # BUG - pyroute2 diag - seems always last info instance from kernel
         if type(tcp_info_raw) != str:
             for k, v in tcp_info_raw.items():
                 if k not in info_refine_tabl:
                     continue
                 refined_k = info_refine_tabl[k][k_idx]
                 cb = info_refine_tabl[k][cb_idx]
                 refined_v = v
-                if cb and cb == 'skip':
+                if cb and cb == "skip":
                     continue
                 elif cb:
-                    ctx = {'raw': tcp_info_raw}
+                    ctx = {"raw": tcp_info_raw}
                     refined_v = cb(k, v, **ctx)
 
                 vessel[info_k][refined_k] = refined_v
 
         return vessel
 
 
@@ -547,52 +551,52 @@
     parser = argparse.ArgumentParser(
         description="""
                                      ss2 - socket statistics depictor meant as
                                      a complete and convenient surrogate for
                                      iproute2/misc/ss2"""
     )
     parser.add_argument(
-        '-x',
-        '--unix',
-        help='Display Unix domain sockets.',
-        action='store_true',
+        "-x",
+        "--unix",
+        help="Display Unix domain sockets.",
+        action="store_true",
     )
     parser.add_argument(
-        '-t', '--tcp', help='Display TCP sockets.', action='store_true'
+        "-t", "--tcp", help="Display TCP sockets.", action="store_true"
     )
     parser.add_argument(
-        '-l',
-        '--listen',
-        help='Display listening sockets.',
-        action='store_true',
+        "-l",
+        "--listen",
+        help="Display listening sockets.",
+        action="store_true",
     )
     parser.add_argument(
-        '-a', '--all', help='Display all sockets.', action='store_true'
+        "-a", "--all", help="Display all sockets.", action="store_true"
     )
     parser.add_argument(
-        '-p',
-        '--process',
-        help='show socket holding context',
-        action='store_true',
+        "-p",
+        "--process",
+        help="show socket holding context",
+        action="store_true",
     )
     parser.add_argument(
-        '-r',
-        '--resolve',
-        help='resolve host names in addition',
-        action='store_true',
+        "-r",
+        "--resolve",
+        help="resolve host names in addition",
+        action="store_true",
     )
 
     args = parser.parse_args()
 
     return args
 
 
 def run(args=None):
     if psutil is None:
-        raise RuntimeError('ss2 requires python-psutil >= 5.0 to run')
+        raise RuntimeError("ss2 requires python-psutil >= 5.0 to run")
 
     if not args:
         args = prepare_args()
 
     _states = SS_CONN
     if args.listen:
         _states = 1 << SS_LISTEN
@@ -603,15 +607,15 @@
     if args.tcp:
         protocols.append(TCP(sk_states=_states))
 
     if args.unix:
         protocols.append(UNIX(sk_states=_states))
 
     if not protocols:
-        raise RuntimeError('not implemented - ss2 in fledging mode')
+        raise RuntimeError("not implemented - ss2 in fledging mode")
 
     _user_ctxt_map = None
     if args.process:
         _user_ctxt_map = UserCtxtMap()
 
     with DiagSocket() as ds:
         ds.bind()
```

### Comparing `pyroute2-0.7.7/pyroute2/netlink/event/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/event/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/event/acpi_event.py` & `pyroute2-0.7.8/pyroute2/netlink/event/acpi_event.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/event/dquot.py` & `pyroute2-0.7.8/pyroute2/netlink/event/dquot.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/event/thermal.py` & `pyroute2-0.7.8/pyroute2/netlink/event/thermal.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/exceptions.py` & `pyroute2-0.7.8/pyroute2/netlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/generic/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/generic/ethtool.py` & `pyroute2-0.7.8/pyroute2/netlink/generic/ethtool.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/generic/l2tp.py` & `pyroute2-0.7.8/pyroute2/netlink/generic/l2tp.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/generic/mptcp.py` & `pyroute2-0.7.8/pyroute2/netlink/generic/mptcp.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/generic/wireguard.py` & `pyroute2-0.7.8/pyroute2/netlink/generic/wireguard.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/ipq/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/ipq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/nfnetlink/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/nfnetlink/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/nfnetlink/ipset.py` & `pyroute2-0.7.8/pyroute2/netlink/nfnetlink/ipset.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/nfnetlink/nfctsocket.py` & `pyroute2-0.7.8/pyroute2/netlink/nfnetlink/nfctsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/nfnetlink/nftsocket.py` & `pyroute2-0.7.8/pyroute2/netlink/nfnetlink/nftsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/nl80211/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/nl80211/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/nlsocket.py` & `pyroute2-0.7.8/pyroute2/netlink/nlsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/proxy.py` & `pyroute2-0.7.8/pyroute2/netlink/proxy.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/fibmsg.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/fibmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifaddrmsg.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifaddrmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/compat.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/compat.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/bond.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/bond.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/geneve.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/geneve.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/tuntap.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/tuntap.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/vlan.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vlan.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/plugins/vxlan.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vxlan.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/proxy.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/proxy.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/sync.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/sync.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifinfmsg/tuntap.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/tuntap.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ifstatsmsg.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ifstatsmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/iprsocket.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/iprsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/iw_event.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/iw_event.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/marshal.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/marshal.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ndmsg.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ndmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/ndtmsg.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/ndtmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/nsinfmsg.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/nsinfmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/riprsocket.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/riprsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/rtmsg.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/rtmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_bpf.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_bpf.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_connmark.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_connmark.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_gact.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_gact.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_mirred.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_mirred.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_police.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_police.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_skbedit.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_skbedit.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/act_vlan.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_vlan.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_basic.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_basic.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_flow.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_flow.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_fw.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_fw.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_matchall.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_matchall.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/cls_u32.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_u32.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/common.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/common.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/common_act.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/common_act.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/common_ematch.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/common_ematch.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/em_cmp.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_cmp.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/em_ipset.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_ipset.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/em_meta.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_meta.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_bpf.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_bpf.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_cake.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_cake.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_choke.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_choke.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_clsact.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_clsact.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_codel.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_codel.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_drr.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_drr.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_fq_codel.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_fq_codel.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_hfsc.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_hfsc.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_htb.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_htb.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_netem.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_netem.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_sfq.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_sfq.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_tbf.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_tbf.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/rtnl/tcmsg/sched_template.py` & `pyroute2-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_template.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/taskstats/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/taskstats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netlink/uevent/__init__.py` & `pyroute2-0.7.8/pyroute2/netlink/uevent/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netns/__init__.py` & `pyroute2-0.7.8/pyroute2/netns/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/netns/manager.py` & `pyroute2-0.7.8/pyroute2/netns/manager.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/nftables/expressions.py` & `pyroute2-0.7.8/pyroute2/nftables/expressions.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/nftables/main.py` & `pyroute2-0.7.8/pyroute2/nftables/main.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/nftables/parser/expr.py` & `pyroute2-0.7.8/pyroute2/nftables/parser/expr.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/nftables/parser/parser.py` & `pyroute2-0.7.8/pyroute2/nftables/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/nftables/rule.py` & `pyroute2-0.7.8/pyroute2/nftables/rule.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/nslink/nslink.py` & `pyroute2-0.7.8/pyroute2/nslink/nslink.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/nslink/nspopen.py` & `pyroute2-0.7.8/pyroute2/nslink/nspopen.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/protocols/__init__.py` & `pyroute2-0.7.8/pyroute2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/remote/iproute.py` & `pyroute2-0.7.8/pyroute2/remote/iproute.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/remote/shell.py` & `pyroute2-0.7.8/pyroute2/remote/shell.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/remote/transport.py` & `pyroute2-0.7.8/pyroute2/remote/transport.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/requests/address.py` & `pyroute2-0.7.8/pyroute2/requests/address.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/requests/bridge.py` & `pyroute2-0.7.8/pyroute2/requests/bridge.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/requests/common.py` & `pyroute2-0.7.8/pyroute2/requests/common.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/requests/link.py` & `pyroute2-0.7.8/pyroute2/requests/link.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/requests/main.py` & `pyroute2-0.7.8/pyroute2/requests/main.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/requests/neighbour.py` & `pyroute2-0.7.8/pyroute2/requests/neighbour.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/requests/route.py` & `pyroute2-0.7.8/pyroute2/requests/route.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/requests/rule.py` & `pyroute2-0.7.8/pyroute2/requests/rule.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2/wiset.py` & `pyroute2-0.7.8/pyroute2/wiset.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/pyroute2.egg-info/PKG-INFO` & `pyroute2-0.7.8/pyroute2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroute2
-Version: 0.7.7
+Version: 0.7.8
 Summary: Python Netlink library
 Home-page: https://github.com/svinota/pyroute2
 Author: Peter Saveliev
 Author-email: peter@svinota.eu
 License: GPL-2.0-or-later OR Apache-2.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyroute2-0.7.7/pyroute2.egg-info/SOURCES.txt` & `pyroute2-0.7.8/pyroute2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/setup.cfg` & `pyroute2-0.7.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_addr_pool.py` & `pyroute2-0.7.8/tests/test_unit/test_addr_pool.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_buffer.py` & `pyroute2-0.7.8/tests/test_unit/test_buffer.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_common.py` & `pyroute2-0.7.8/tests/test_unit/test_common.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_iproute_match/links.dump` & `pyroute2-0.7.8/tests/test_unit/test_iproute_match/links.dump`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_iproute_match/test_match.py` & `pyroute2-0.7.8/tests/test_unit/test_iproute_match/test_match.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_nlmsg/addrmsg_ipv4.dump` & `pyroute2-0.7.8/tests/test_unit/test_nlmsg/addrmsg_ipv4.dump`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_nlmsg/gre_01.dump` & `pyroute2-0.7.8/tests/test_unit/test_nlmsg/gre_01.dump`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_nlmsg/iw_info_rsp.dump` & `pyroute2-0.7.8/tests/test_unit/test_nlmsg/iw_info_rsp.dump`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_nlmsg/iw_scan_rsp.dump` & `pyroute2-0.7.8/tests/test_unit/test_nlmsg/iw_scan_rsp.dump`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_nlmsg/test_attr.py` & `pyroute2-0.7.8/tests/test_unit/test_nlmsg/test_attr.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_nlmsg/test_map_adapter.py` & `pyroute2-0.7.8/tests/test_unit/test_nlmsg/test_map_adapter.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_nlmsg/test_marshal.py` & `pyroute2-0.7.8/tests/test_unit/test_nlmsg/test_marshal.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_requests/test_address.py` & `pyroute2-0.7.8/tests/test_unit/test_requests/test_address.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_requests/test_link.py` & `pyroute2-0.7.8/tests/test_unit/test_requests/test_link.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_requests/test_neighbour.py` & `pyroute2-0.7.8/tests/test_unit/test_requests/test_neighbour.py`

 * *Files identical despite different names*

### Comparing `pyroute2-0.7.7/tests/test_unit/test_requests/test_route.py` & `pyroute2-0.7.8/tests/test_unit/test_requests/test_route.py`

 * *Files identical despite different names*

