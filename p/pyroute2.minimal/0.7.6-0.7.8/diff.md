# Comparing `tmp/pyroute2.minimal-0.7.6.tar.gz` & `tmp/pyroute2.minimal-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroute2.minimal-0.7.6.tar", last modified: Sun Mar 19 16:57:39 2023, max compression
+gzip compressed data, was "pyroute2.minimal-0.7.8.tar", last modified: Fri May  5 08:51:26 2023, max compression
```

## Comparing `pyroute2.minimal-0.7.6.tar` & `pyroute2.minimal-0.7.8.tar`

### file list

```diff
@@ -1,271 +1,271 @@
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.961918 pyroute2.minimal-0.7.6/
--rw-r--r--   0 peet      (1001) peet      (1001)    28407 2023-03-19 15:35:19.000000 pyroute2.minimal-0.7.6/CHANGELOG.rst
--rw-r--r--   0 peet      (1001) peet      (1001)       31 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/LICENSE
--rw-r--r--   0 peet      (1001) peet      (1001)    11348 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/LICENSE.Apache-2.0
--rw-r--r--   0 peet      (1001) peet      (1001)    18092 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/LICENSE.GPL-2.0-or-later
--rw-r--r--   0 peet      (1001) peet      (1001)      237 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/MANIFEST.in
--rw-r--r--   0 peet      (1001) peet      (1001)     1746 2023-03-19 16:57:39.961918 pyroute2.minimal-0.7.6/PKG-INFO
--rw-r--r--   0 peet      (1001) peet      (1001)     2198 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/README.contribute.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      340 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/README.license.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      397 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/README.minimal.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      757 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/README.report.rst
--rw-r--r--   0 peet      (1001) peet      (1001)     6853 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/README.rst
--rw-r--r--   0 peet      (1001) peet      (1001)        6 2023-03-19 16:57:20.000000 pyroute2.minimal-0.7.6/VERSION
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.937918 pyroute2.minimal-0.7.6/examples/
--rw-r--r--   0 peet      (1001) peet      (1001)       18 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/README.md
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.937918 pyroute2.minimal-0.7.6/examples/devlink/
--rw-r--r--   0 peet      (1001) peet      (1001)      224 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/devlink/devlink_list.py
--rw-r--r--   0 peet      (1001) peet      (1001)       80 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/devlink/devlink_monitor.py
--rw-r--r--   0 peet      (1001) peet      (1001)      284 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/devlink/devlink_port_list.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.937918 pyroute2.minimal-0.7.6/examples/ethtool/
--rw-r--r--   0 peet      (1001) peet      (1001)      816 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ethtool/ethtool-ioctl_get_infos.py
--rw-r--r--   0 peet      (1001) peet      (1001)      496 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ethtool/ethtool-netlink_get_infos.py
--rw-r--r--   0 peet      (1001) peet      (1001)      391 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ethtool/ethtool_get_infos.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.938918 pyroute2.minimal-0.7.6/examples/generic/
--rw-r--r--   0 peet      (1001) peet      (1001)      155 2022-05-21 16:48:21.000000 pyroute2.minimal-0.7.6/examples/generic/Makefile
--rw-r--r--   0 peet      (1001) peet      (1001)     3561 2022-05-21 16:48:21.000000 pyroute2.minimal-0.7.6/examples/generic/netl.c
--rwxr-xr-x   0 peet      (1001) peet      (1001)     1179 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/generic/netl.py
--rw-r--r--   0 peet      (1001) peet      (1001)      391 2022-05-21 16:48:21.000000 pyroute2.minimal-0.7.6/examples/ipq.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.938918 pyroute2.minimal-0.7.6/examples/iproute/
--rw-r--r--   0 peet      (1001) peet      (1001)      187 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/iproute/ip_monitor.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1523 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ipset.py
--rw-r--r--   0 peet      (1001) peet      (1001)      127 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/kobject_uevent.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.938918 pyroute2.minimal-0.7.6/examples/lab/
--rw-r--r--   0 peet      (1001) peet      (1001)      462 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/README.rst
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.938918 pyroute2.minimal-0.7.6/examples/lab/iproute_get_addr/
--rw-r--r--   0 peet      (1001) peet      (1001)      162 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/iproute_get_addr/README.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      323 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/iproute_get_addr/check.py
--rw-r--r--   0 peet      (1001) peet      (1001)       64 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/iproute_get_addr/setup.py
--rw-r--r--   0 peet      (1001) peet      (1001)      102 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/iproute_get_addr/task.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.939918 pyroute2.minimal-0.7.6/examples/lab/iproute_get_attr/
--rw-r--r--   0 peet      (1001) peet      (1001)      341 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/iproute_get_attr/README.rst
--rw-r--r--   0 peet      (1001) peet      (1001)      252 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/iproute_get_attr/check.py
--rw-r--r--   0 peet      (1001) peet      (1001)       64 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/iproute_get_attr/setup.py
--rw-r--r--   0 peet      (1001) peet      (1001)      308 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/lab/iproute_get_attr/task.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.939918 pyroute2.minimal-0.7.6/examples/ndb/
--rw-r--r--   0 peet      (1001) peet      (1001)      752 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ndb/create_bond.py
--rw-r--r--   0 peet      (1001) peet      (1001)      643 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ndb/create_interface.py
--rw-r--r--   0 peet      (1001) peet      (1001)      684 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ndb/create_vlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3546 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ndb/keystone_auth.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2188 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/ndb/radius_auth.py
--rwxr-xr-x   0 peet      (1001) peet      (1001)      444 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/nftables.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1522 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/nftables_sets.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.939918 pyroute2.minimal-0.7.6/examples/policy/
--rwxr-xr-x   0 peet      (1001) peet      (1001)      536 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/policy/policy.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.940918 pyroute2.minimal-0.7.6/examples/processes/
--rw-r--r--   0 peet      (1001) peet      (1001)      414 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/processes/pmonitor.py
--rw-r--r--   0 peet      (1001) peet      (1001)      246 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/processes/taskstats.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.940918 pyroute2.minimal-0.7.6/examples/pyroute2-cli/
--rw-r--r--   0 peet      (1001) peet      (1001)      300 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/pyroute2-cli/comments
--rw-r--r--   0 peet      (1001) peet      (1001)     1869 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/pyroute2-cli/create_bridge
--rw-r--r--   0 peet      (1001) peet      (1001)      723 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/pyroute2-cli/create_dummy
--rw-r--r--   0 peet      (1001) peet      (1001)       87 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/pyroute2-cli/dump_lo
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.940918 pyroute2.minimal-0.7.6/examples/wifi/
--rw-r--r--   0 peet      (1001) peet      (1001)      464 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/wifi/nl80211_interface_type.py
--rw-r--r--   0 peet      (1001) peet      (1001)      422 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/wifi/nl80211_interfaces.py
--rw-r--r--   0 peet      (1001) peet      (1001)      113 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/wifi/nl80211_monitor.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2504 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/examples/wifi/nl80211_scan_dump.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.941918 pyroute2.minimal-0.7.6/pr2modules/
--rw-r--r--   0 peet      (1001) peet      (1001)      568 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pr2modules/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)       90 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyproject.toml
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.942918 pyroute2.minimal-0.7.6/pyroute2/
--rw-r--r--   0 peet      (1001) peet      (1001)     1834 2023-03-19 16:57:37.000000 pyroute2.minimal-0.7.6/pyroute2/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2474 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/arp.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.943918 pyroute2.minimal-0.7.6/pyroute2/bsd/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2.minimal-0.7.6/pyroute2/bsd/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.943918 pyroute2.minimal-0.7.6/pyroute2/bsd/pf_route/
--rw-r--r--   0 peet      (1001) peet      (1001)     4186 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/bsd/pf_route/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3270 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/bsd/pf_route/freebsd.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3607 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/bsd/pf_route/openbsd.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.943918 pyroute2.minimal-0.7.6/pyroute2/bsd/rtmsocket/
--rw-r--r--   0 peet      (1001) peet      (1001)     4287 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/bsd/rtmsocket/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1382 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/bsd/rtmsocket/freebsd.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1423 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/bsd/rtmsocket/openbsd.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8136 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/bsd/util.py
--rw-r--r--   0 peet      (1001) peet      (1001)    17833 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/common.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.944918 pyroute2.minimal-0.7.6/pyroute2/config/
--rw-r--r--   0 peet      (1001) peet      (1001)     1365 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/config/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2340 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/config/asyncio.py
--rw-r--r--   0 peet      (1001) peet      (1001)      258 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/config/eventlet.py
--rw-r--r--   0 peet      (1001) peet      (1001)      541 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/config/log.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8497 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/config/test_platform.py
--rw-r--r--   0 peet      (1001) peet      (1001)       22 2023-03-19 16:57:20.000000 pyroute2.minimal-0.7.6/pyroute2/config/version.py
--rw-r--r--   0 peet      (1001) peet      (1001)     6845 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/conntrack.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2071 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/devlink.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.944918 pyroute2.minimal-0.7.6/pyroute2/inotify/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/inotify/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2403 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/inotify/inotify_fd.py
--rw-r--r--   0 peet      (1001) peet      (1001)      539 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/inotify/inotify_msg.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.945918 pyroute2.minimal-0.7.6/pyroute2/iproute/
--rw-r--r--   0 peet      (1001) peet      (1001)     4920 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/iproute/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    10532 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/iproute/bsd.py
--rw-r--r--   0 peet      (1001) peet      (1001)    23547 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/iproute/ipmock.py
--rw-r--r--   0 peet      (1001) peet      (1001)    82477 2023-03-16 14:35:20.000000 pyroute2.minimal-0.7.6/pyroute2/iproute/linux.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1313 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/iproute/parsers.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8082 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/iproute/windows.py
--rw-r--r--   0 peet      (1001) peet      (1001)    24131 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/ipset.py
--rw-r--r--   0 peet      (1001) peet      (1001)    22019 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/iwutil.py
--rw-r--r--   0 peet      (1001) peet      (1001)      419 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/lab.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1139 2023-03-18 20:08:16.000000 pyroute2.minimal-0.7.6/pyroute2/loader.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1834 2023-03-18 20:08:16.000000 pyroute2.minimal-0.7.6/pyroute2/minimal.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.946918 pyroute2.minimal-0.7.6/pyroute2/netlink/
--rw-r--r--   0 peet      (1001) peet      (1001)    72813 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1947 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/buffer.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.946918 pyroute2.minimal-0.7.6/pyroute2/netlink/devlink/
--rw-r--r--   0 peet      (1001) peet      (1001)    23285 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/devlink/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.946918 pyroute2.minimal-0.7.6/pyroute2/netlink/diag/
--rw-r--r--   0 peet      (1001) peet      (1001)    10423 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/diag/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    18314 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/diag/ss2.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.947918 pyroute2.minimal-0.7.6/pyroute2/netlink/event/
--rw-r--r--   0 peet      (1001) peet      (1001)      714 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/event/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2078 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/event/acpi_event.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2034 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/event/dquot.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2594 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/event/thermal.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1616 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/exceptions.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.947918 pyroute2.minimal-0.7.6/pyroute2/netlink/generic/
--rw-r--r--   0 peet      (1001) peet      (1001)     3910 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/generic/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     7467 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/generic/ethtool.py
--rw-r--r--   0 peet      (1001) peet      (1001)    19073 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/generic/l2tp.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3928 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/generic/mptcp.py
--rw-r--r--   0 peet      (1001) peet      (1001)    12476 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/generic/wireguard.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.947918 pyroute2.minimal-0.7.6/pyroute2/netlink/ipq/
--rw-r--r--   0 peet      (1001) peet      (1001)     3315 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/ipq/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.948918 pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/
--rw-r--r--   0 peet      (1001) peet      (1001)     1036 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     7145 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/ipset.py
--rw-r--r--   0 peet      (1001) peet      (1001)    27707 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/nfctsocket.py
--rw-r--r--   0 peet      (1001) peet      (1001)    43123 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/nftsocket.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.948918 pyroute2.minimal-0.7.6/pyroute2/netlink/nl80211/
--rw-r--r--   0 peet      (1001) peet      (1001)    57760 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/nl80211/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    49725 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/nlsocket.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2317 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/proxy.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.950918 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/
--rw-r--r--   0 peet      (1001) peet      (1001)     5988 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)      155 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/errmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2428 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/fibmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2799 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifaddrmsg.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.951918 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/
--rw-r--r--   0 peet      (1001) peet      (1001)    43260 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)    10801 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/compat.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.952918 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-14 18:41:13.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1747 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/bond.py
--rw-r--r--   0 peet      (1001) peet      (1001)      776 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/geneve.py
--rw-r--r--   0 peet      (1001) peet      (1001)      227 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/gtp.py
--rwxr-xr-x   0 peet      (1001) peet      (1001)      376 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/ipoib.py
--rw-r--r--   0 peet      (1001) peet      (1001)      291 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/ipvlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)      151 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/team.py
--rw-r--r--   0 peet      (1001) peet      (1001)      494 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/tun.py
--rw-r--r--   0 peet      (1001) peet      (1001)      569 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/tuntap.py
--rw-r--r--   0 peet      (1001) peet      (1001)      751 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/vlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)      146 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/vrf.py
--rw-r--r--   0 peet      (1001) peet      (1001)      317 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/vti.py
--rw-r--r--   0 peet      (1001) peet      (1001)      357 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/vti6.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1417 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/vxlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)      189 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/xfrm.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3428 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/proxy.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1974 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/sync.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3875 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/tuntap.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2583 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifstatsmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5802 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/iprsocket.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3244 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/iw_event.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2018 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/marshal.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2607 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ndmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2188 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ndtmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)      321 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/nsidmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)      522 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/nsinfmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)      366 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/p2pmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)      523 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/riprsocket.py
--rw-r--r--   0 peet      (1001) peet      (1001)      114 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/rtgenmsg.py
--rw-r--r--   0 peet      (1001) peet      (1001)    26078 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/rtmsg.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.957918 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/
--rw-r--r--   0 peet      (1001) peet      (1001)     2743 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)      979 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_bpf.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1234 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_connmark.py
--rw-r--r--   0 peet      (1001) peet      (1001)      709 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_gact.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1725 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_mirred.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1866 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_police.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3338 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_skbedit.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1465 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_vlan.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8478 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_basic.py
--rw-r--r--   0 peet      (1001) peet      (1001)     4613 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_flow.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1427 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_fw.py
--rw-r--r--   0 peet      (1001) peet      (1001)      986 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_matchall.py
--rw-r--r--   0 peet      (1001) peet      (1001)     8033 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_u32.py
--rw-r--r--   0 peet      (1001) peet      (1001)    10724 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/common.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2063 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/common_act.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3148 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/common_ematch.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2776 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/em_cmp.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1741 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/em_ipset.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5933 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/em_meta.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2571 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_bpf.py
--rw-r--r--   0 peet      (1001) peet      (1001)    12834 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_cake.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3431 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_choke.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1010 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_clsact.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1607 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_codel.py
--rw-r--r--   0 peet      (1001) peet      (1001)      754 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_drr.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2658 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_fq_codel.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2352 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_hfsc.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5738 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_htb.py
--rw-r--r--   0 peet      (1001) peet      (1001)      214 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_ingress.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5111 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_netem.py
--rw-r--r--   0 peet      (1001) peet      (1001)      196 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_pfifo.py
--rw-r--r--   0 peet      (1001) peet      (1001)      215 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_pfifo_fast.py
--rw-r--r--   0 peet      (1001) peet      (1001)      446 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_plug.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2717 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_sfq.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1087 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_tbf.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1249 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_template.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.957918 pyroute2.minimal-0.7.6/pyroute2/netlink/taskstats/
--rw-r--r--   0 peet      (1001) peet      (1001)     4920 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/taskstats/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.957918 pyroute2.minimal-0.7.6/pyroute2/netlink/uevent/
--rw-r--r--   0 peet      (1001) peet      (1001)     1096 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netlink/uevent/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.957918 pyroute2.minimal-0.7.6/pyroute2/netns/
--rw-r--r--   0 peet      (1001) peet      (1001)    10678 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netns/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3803 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/netns/manager.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.957918 pyroute2.minimal-0.7.6/pyroute2/protocols/
--rw-r--r--   0 peet      (1001) peet      (1001)     8716 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/protocols/__init__.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.958918 pyroute2.minimal-0.7.6/pyroute2/requests/
--rw-r--r--   0 peet      (1001) peet      (1001)        0 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/__init__.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3430 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/address.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5195 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/bridge.py
--rw-r--r--   0 peet      (1001) peet      (1001)     5083 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/common.py
--rw-r--r--   0 peet      (1001) peet      (1001)     9174 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/link.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2005 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/main.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1241 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/neighbour.py
--rw-r--r--   0 peet      (1001) peet      (1001)      107 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/netns.py
--rw-r--r--   0 peet      (1001) peet      (1001)    19591 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/route.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1229 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/requests/rule.py
--rw-r--r--   0 peet      (1001) peet      (1001)    19622 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/pyroute2/wiset.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.942918 pyroute2.minimal-0.7.6/pyroute2.minimal.egg-info/
--rw-r--r--   0 peet      (1001) peet      (1001)     1746 2023-03-19 16:57:39.000000 pyroute2.minimal-0.7.6/pyroute2.minimal.egg-info/PKG-INFO
--rw-r--r--   0 peet      (1001) peet      (1001)     7596 2023-03-19 16:57:39.000000 pyroute2.minimal-0.7.6/pyroute2.minimal.egg-info/SOURCES.txt
--rw-r--r--   0 peet      (1001) peet      (1001)        1 2023-03-19 16:57:39.000000 pyroute2.minimal-0.7.6/pyroute2.minimal.egg-info/dependency_links.txt
--rw-r--r--   0 peet      (1001) peet      (1001)       93 2023-03-19 16:57:39.000000 pyroute2.minimal-0.7.6/pyroute2.minimal.egg-info/requires.txt
--rw-r--r--   0 peet      (1001) peet      (1001)       20 2023-03-19 16:57:39.000000 pyroute2.minimal-0.7.6/pyroute2.minimal.egg-info/top_level.txt
--rw-r--r--   0 peet      (1001) peet      (1001)     1884 2023-03-19 16:57:39.961918 pyroute2.minimal-0.7.6/setup.cfg
--rw-r--r--   0 peet      (1001) peet      (1001)       38 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/setup.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.934918 pyroute2.minimal-0.7.6/tests/
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.959918 pyroute2.minimal-0.7.6/tests/test_unit/
--rw-r--r--   0 peet      (1001) peet      (1001)     2096 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_addr_pool.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1892 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_buffer.py
--rw-r--r--   0 peet      (1001) peet      (1001)      891 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_common.py
--rw-r--r--   0 peet      (1001) peet      (1001)      422 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_config.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.959918 pyroute2.minimal-0.7.6/tests/test_unit/test_entry_points/
--rw-r--r--   0 peet      (1001) peet      (1001)      379 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_entry_points/test_basic.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.959918 pyroute2.minimal-0.7.6/tests/test_unit/test_iproute_match/
--rw-r--r--   0 peet      (1001) peet      (1001)    50363 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_iproute_match/links.dump
--rw-r--r--   0 peet      (1001) peet      (1001)     2175 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_iproute_match/test_match.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.960918 pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/
--rw-r--r--   0 peet      (1001) peet      (1001)     1308 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/addrmsg_ipv4.dump
--rw-r--r--   0 peet      (1001) peet      (1001)     4287 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/gre_01.dump
--rw-r--r--   0 peet      (1001) peet      (1001)     1395 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/iw_info_rsp.dump
--rw-r--r--   0 peet      (1001) peet      (1001)    32910 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/iw_scan_rsp.dump
--rw-r--r--   0 peet      (1001) peet      (1001)      722 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/test_attr.py
--rw-r--r--   0 peet      (1001) peet      (1001)     1819 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/test_map_adapter.py
--rw-r--r--   0 peet      (1001) peet      (1001)     4154 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/test_marshal.py
-drwxr-xr-x   0 peet      (1001) peet      (1001)        0 2023-03-19 16:57:39.961918 pyroute2.minimal-0.7.6/tests/test_unit/test_requests/
--rw-r--r--   0 peet      (1001) peet      (1001)      375 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_requests/common.py
--rw-r--r--   0 peet      (1001) peet      (1001)     6431 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_requests/test_address.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2515 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_requests/test_link.py
--rw-r--r--   0 peet      (1001) peet      (1001)     2960 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_requests/test_neighbour.py
--rw-r--r--   0 peet      (1001) peet      (1001)     3938 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.6/tests/test_unit/test_requests/test_route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.299616 pyroute2.minimal-0.7.8/
+-rw-r--r--   0 root         (0) root         (0)    28688 2023-05-05 08:37:53.000000 pyroute2.minimal-0.7.8/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)       31 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/LICENSE.Apache-2.0
+-rw-r--r--   0 root         (0) root         (0)    18092 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/LICENSE.GPL-2.0-or-later
+-rw-r--r--   0 root         (0) root         (0)      237 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-05-05 08:51:26.299616 pyroute2.minimal-0.7.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/README.contribute.rst
+-rw-r--r--   0 root         (0) root         (0)      340 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/README.license.rst
+-rw-r--r--   0 root         (0) root         (0)      397 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/README.minimal.rst
+-rw-r--r--   0 root         (0) root         (0)      757 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/README.report.rst
+-rw-r--r--   0 root         (0) root         (0)     6853 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/README.rst
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-05 08:38:03.000000 pyroute2.minimal-0.7.8/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.227616 pyroute2.minimal-0.7.8/examples/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.229616 pyroute2.minimal-0.7.8/examples/devlink/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/devlink/devlink_list.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/devlink/devlink_monitor.py
+-rw-r--r--   0 root         (0) root         (0)      284 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/devlink/devlink_port_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.229616 pyroute2.minimal-0.7.8/examples/ethtool/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ethtool/ethtool-ioctl_get_infos.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ethtool/ethtool-netlink_get_infos.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ethtool/ethtool_get_infos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.230616 pyroute2.minimal-0.7.8/examples/generic/
+-rw-r--r--   0 root         (0) root         (0)      155 2022-05-21 16:48:21.000000 pyroute2.minimal-0.7.8/examples/generic/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3561 2022-05-21 16:48:21.000000 pyroute2.minimal-0.7.8/examples/generic/netl.c
+-rwxr-xr-x   0 root         (0) root         (0)     1179 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/generic/netl.py
+-rw-r--r--   0 root         (0) root         (0)      391 2022-05-21 16:48:21.000000 pyroute2.minimal-0.7.8/examples/ipq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.231616 pyroute2.minimal-0.7.8/examples/iproute/
+-rw-r--r--   0 root         (0) root         (0)      187 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/iproute/ip_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ipset.py
+-rw-r--r--   0 root         (0) root         (0)      127 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/kobject_uevent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.232616 pyroute2.minimal-0.7.8/examples/lab/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.234616 pyroute2.minimal-0.7.8/examples/lab/iproute_get_addr/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/iproute_get_addr/README.rst
+-rw-r--r--   0 root         (0) root         (0)      323 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/iproute_get_addr/check.py
+-rw-r--r--   0 root         (0) root         (0)       64 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/iproute_get_addr/setup.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/iproute_get_addr/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.235616 pyroute2.minimal-0.7.8/examples/lab/iproute_get_attr/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/iproute_get_attr/README.rst
+-rw-r--r--   0 root         (0) root         (0)      252 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/iproute_get_attr/check.py
+-rw-r--r--   0 root         (0) root         (0)       64 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/iproute_get_attr/setup.py
+-rw-r--r--   0 root         (0) root         (0)      308 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/lab/iproute_get_attr/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.237616 pyroute2.minimal-0.7.8/examples/ndb/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ndb/create_bond.py
+-rw-r--r--   0 root         (0) root         (0)      643 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ndb/create_interface.py
+-rw-r--r--   0 root         (0) root         (0)      684 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ndb/create_vlan.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ndb/keystone_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/ndb/radius_auth.py
+-rwxr-xr-x   0 root         (0) root         (0)      444 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/nftables.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/nftables_sets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.237616 pyroute2.minimal-0.7.8/examples/policy/
+-rwxr-xr-x   0 root         (0) root         (0)      536 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/policy/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.237616 pyroute2.minimal-0.7.8/examples/processes/
+-rw-r--r--   0 root         (0) root         (0)      414 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/processes/pmonitor.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/processes/taskstats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.238616 pyroute2.minimal-0.7.8/examples/pyroute2-cli/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/pyroute2-cli/comments
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/pyroute2-cli/create_bridge
+-rw-r--r--   0 root         (0) root         (0)      723 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/pyroute2-cli/create_dummy
+-rw-r--r--   0 root         (0) root         (0)       87 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/pyroute2-cli/dump_lo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.239616 pyroute2.minimal-0.7.8/examples/wifi/
+-rw-r--r--   0 root         (0) root         (0)      464 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/wifi/nl80211_interface_type.py
+-rw-r--r--   0 root         (0) root         (0)      422 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/wifi/nl80211_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/wifi/nl80211_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/examples/wifi/nl80211_scan_dump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.240616 pyroute2.minimal-0.7.8/pr2modules/
+-rw-r--r--   0 root         (0) root         (0)      568 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pr2modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       90 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.244616 pyroute2.minimal-0.7.8/pyroute2/
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-05-05 08:51:23.000000 pyroute2.minimal-0.7.8/pyroute2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/arp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.246616 pyroute2.minimal-0.7.8/pyroute2/bsd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-14 18:41:13.000000 pyroute2.minimal-0.7.8/pyroute2/bsd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.246616 pyroute2.minimal-0.7.8/pyroute2/bsd/pf_route/
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/bsd/pf_route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/bsd/pf_route/freebsd.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/bsd/pf_route/openbsd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.248616 pyroute2.minimal-0.7.8/pyroute2/bsd/rtmsocket/
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/bsd/rtmsocket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/bsd/rtmsocket/freebsd.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/bsd/rtmsocket/openbsd.py
+-rw-r--r--   0 root         (0) root         (0)     8136 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/bsd/util.py
+-rw-r--r--   0 root         (0) root         (0)    17833 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.250616 pyroute2.minimal-0.7.8/pyroute2/config/
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/config/asyncio.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/config/eventlet.py
+-rw-r--r--   0 root         (0) root         (0)      541 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/config/log.py
+-rw-r--r--   0 root         (0) root         (0)     8497 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/config/test_platform.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 19:19:05.000000 pyroute2.minimal-0.7.8/pyroute2/config/version.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/conntrack.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/devlink.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.251616 pyroute2.minimal-0.7.8/pyroute2/inotify/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/inotify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/inotify/inotify_fd.py
+-rw-r--r--   0 root         (0) root         (0)      539 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/inotify/inotify_msg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.254616 pyroute2.minimal-0.7.8/pyroute2/iproute/
+-rw-r--r--   0 root         (0) root         (0)     4920 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/iproute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10532 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/iproute/bsd.py
+-rw-r--r--   0 root         (0) root         (0)    23630 2023-04-05 11:12:44.000000 pyroute2.minimal-0.7.8/pyroute2/iproute/ipmock.py
+-rw-r--r--   0 root         (0) root         (0)    82477 2023-03-16 14:35:20.000000 pyroute2.minimal-0.7.8/pyroute2/iproute/linux.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/iproute/parsers.py
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/iproute/windows.py
+-rw-r--r--   0 root         (0) root         (0)    24131 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/ipset.py
+-rw-r--r--   0 root         (0) root         (0)    22019 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/iwutil.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/lab.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-05 11:12:40.000000 pyroute2.minimal-0.7.8/pyroute2/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-05 11:12:40.000000 pyroute2.minimal-0.7.8/pyroute2/minimal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.255616 pyroute2.minimal-0.7.8/pyroute2/netlink/
+-rw-r--r--   0 root         (0) root         (0)    72813 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.255616 pyroute2.minimal-0.7.8/pyroute2/netlink/devlink/
+-rw-r--r--   0 root         (0) root         (0)    23285 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/devlink/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.256616 pyroute2.minimal-0.7.8/pyroute2/netlink/diag/
+-rw-r--r--   0 root         (0) root         (0)    10423 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/diag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18781 2023-05-05 08:37:08.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/diag/ss2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.258616 pyroute2.minimal-0.7.8/pyroute2/netlink/event/
+-rw-r--r--   0 root         (0) root         (0)      714 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/event/acpi_event.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/event/dquot.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/event/thermal.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.259616 pyroute2.minimal-0.7.8/pyroute2/netlink/generic/
+-rw-r--r--   0 root         (0) root         (0)     3910 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/generic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/generic/ethtool.py
+-rw-r--r--   0 root         (0) root         (0)    19073 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/generic/l2tp.py
+-rw-r--r--   0 root         (0) root         (0)     3928 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/generic/mptcp.py
+-rw-r--r--   0 root         (0) root         (0)    12476 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/generic/wireguard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.259616 pyroute2.minimal-0.7.8/pyroute2/netlink/ipq/
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/ipq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.260616 pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7145 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/ipset.py
+-rw-r--r--   0 root         (0) root         (0)    27707 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/nfctsocket.py
+-rw-r--r--   0 root         (0) root         (0)    43123 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/nftsocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.260616 pyroute2.minimal-0.7.8/pyroute2/netlink/nl80211/
+-rw-r--r--   0 root         (0) root         (0)    61729 2023-04-05 11:25:50.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/nl80211/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49725 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/nlsocket.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.262616 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/
+-rw-r--r--   0 root         (0) root         (0)     5988 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/errmsg.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/fibmsg.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifaddrmsg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.267616 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/
+-rw-r--r--   0 root         (0) root         (0)    43260 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10801 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.273616 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-14 18:41:13.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/bond.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/geneve.py
+-rw-r--r--   0 root         (0) root         (0)      227 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/gtp.py
+-rwxr-xr-x   0 root         (0) root         (0)      376 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/ipoib.py
+-rw-r--r--   0 root         (0) root         (0)      291 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/ipvlan.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/team.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/tun.py
+-rw-r--r--   0 root         (0) root         (0)      569 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/tuntap.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vlan.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vrf.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vti.py
+-rw-r--r--   0 root         (0) root         (0)      357 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vti6.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vxlan.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/xfrm.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/sync.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/tuntap.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifstatsmsg.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/iprsocket.py
+-rw-r--r--   0 root         (0) root         (0)     3244 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/iw_event.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/marshal.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ndmsg.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ndtmsg.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/nsidmsg.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/nsinfmsg.py
+-rw-r--r--   0 root         (0) root         (0)      366 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/p2pmsg.py
+-rw-r--r--   0 root         (0) root         (0)      523 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/riprsocket.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/rtgenmsg.py
+-rw-r--r--   0 root         (0) root         (0)    26078 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/rtmsg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.285616 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_bpf.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_connmark.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_gact.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_mirred.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_police.py
+-rw-r--r--   0 root         (0) root         (0)     3338 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_skbedit.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_vlan.py
+-rw-r--r--   0 root         (0) root         (0)     8478 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_basic.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_flow.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_fw.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_matchall.py
+-rw-r--r--   0 root         (0) root         (0)     8033 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_u32.py
+-rw-r--r--   0 root         (0) root         (0)    10724 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/common.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/common_act.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/common_ematch.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_cmp.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_ipset.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_bpf.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_cake.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_choke.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_clsact.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_codel.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_drr.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_fq_codel.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_hfsc.py
+-rw-r--r--   0 root         (0) root         (0)     5738 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_htb.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_ingress.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_netem.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_pfifo.py
+-rw-r--r--   0 root         (0) root         (0)      215 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_pfifo_fast.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_plug.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_sfq.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_tbf.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.288616 pyroute2.minimal-0.7.8/pyroute2/netlink/taskstats/
+-rw-r--r--   0 root         (0) root         (0)     4920 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/taskstats/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.288616 pyroute2.minimal-0.7.8/pyroute2/netlink/uevent/
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netlink/uevent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.288616 pyroute2.minimal-0.7.8/pyroute2/netns/
+-rw-r--r--   0 root         (0) root         (0)    10678 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/netns/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.288616 pyroute2.minimal-0.7.8/pyroute2/protocols/
+-rw-r--r--   0 root         (0) root         (0)     8716 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.292616 pyroute2.minimal-0.7.8/pyroute2/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/address.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/bridge.py
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/common.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/link.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/main.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/neighbour.py
+-rw-r--r--   0 root         (0) root         (0)      107 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/netns.py
+-rw-r--r--   0 root         (0) root         (0)    19591 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/route.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/requests/rule.py
+-rw-r--r--   0 root         (0) root         (0)    19622 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/pyroute2/wiset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.245616 pyroute2.minimal-0.7.8/pyroute2.minimal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-05-05 08:51:26.000000 pyroute2.minimal-0.7.8/pyroute2.minimal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7596 2023-05-05 08:51:26.000000 pyroute2.minimal-0.7.8/pyroute2.minimal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 08:51:26.000000 pyroute2.minimal-0.7.8/pyroute2.minimal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-05 08:51:26.000000 pyroute2.minimal-0.7.8/pyroute2.minimal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-05 08:51:26.000000 pyroute2.minimal-0.7.8/pyroute2.minimal.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-05-05 08:51:26.299616 pyroute2.minimal-0.7.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.216616 pyroute2.minimal-0.7.8/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.292616 pyroute2.minimal-0.7.8/tests/test_unit/
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_addr_pool.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_buffer.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_common.py
+-rw-r--r--   0 root         (0) root         (0)      422 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.293616 pyroute2.minimal-0.7.8/tests/test_unit/test_entry_points/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_entry_points/test_basic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.293616 pyroute2.minimal-0.7.8/tests/test_unit/test_iproute_match/
+-rw-r--r--   0 root         (0) root         (0)    50363 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_iproute_match/links.dump
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_iproute_match/test_match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.296616 pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/addrmsg_ipv4.dump
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/gre_01.dump
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/iw_info_rsp.dump
+-rw-r--r--   0 root         (0) root         (0)    32910 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/iw_scan_rsp.dump
+-rw-r--r--   0 root         (0) root         (0)      722 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/test_attr.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/test_map_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/test_marshal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 08:51:26.299616 pyroute2.minimal-0.7.8/tests/test_unit/test_requests/
+-rw-r--r--   0 root         (0) root         (0)      375 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_requests/common.py
+-rw-r--r--   0 root         (0) root         (0)     6431 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_requests/test_address.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_requests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_requests/test_neighbour.py
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-03-15 10:10:02.000000 pyroute2.minimal-0.7.8/tests/test_unit/test_requests/test_route.py
```

### Comparing `pyroute2.minimal-0.7.6/CHANGELOG.rst` & `pyroute2.minimal-0.7.8/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+* 0.7.8
+    * ss2: more fixes <https://github.com/svinota/pyroute2/pull/1088>
+* 0.7.7
+    * ss2: user context patch <https://github.com/svinota/pyroute2/pull/1087>
+    * ndb: basic altname support
+    * nl80211: decoder improvements <https://github.com/svinota/pyroute2/pull/1086>
 * 0.7.6
     * setup: static loader <https://github.com/svinota/pyroute2/issues/1076>
     * iproute: support altname in link_lookup()
     * ethtool: fd leaks <https://github.com/svinota/pyroute2/pull/1081>
 * 0.7.5
     * nlsocket: fix marshal reference <https://github.com/svinota/pyroute2/issues/1068>
 * 0.7.4
```

### Comparing `pyroute2.minimal-0.7.6/LICENSE.Apache-2.0` & `pyroute2.minimal-0.7.8/LICENSE.Apache-2.0`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/LICENSE.GPL-2.0-or-later` & `pyroute2.minimal-0.7.8/LICENSE.GPL-2.0-or-later`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/PKG-INFO` & `pyroute2.minimal-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroute2.minimal
-Version: 0.7.6
+Version: 0.7.8
 Summary: Python Netlink library: minimal distribution
 Home-page: https://github.com/svinota/pyroute2
 Author: Peter Saveliev
 Author-email: peter@svinota.eu
 License: GPL-2.0-or-later OR Apache-2.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyroute2.minimal-0.7.6/README.contribute.rst` & `pyroute2.minimal-0.7.8/README.contribute.rst`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/README.report.rst` & `pyroute2.minimal-0.7.8/README.report.rst`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/README.rst` & `pyroute2.minimal-0.7.8/README.rst`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/ethtool/ethtool-ioctl_get_infos.py` & `pyroute2.minimal-0.7.8/examples/ethtool/ethtool-ioctl_get_infos.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/generic/netl.c` & `pyroute2.minimal-0.7.8/examples/generic/netl.c`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/generic/netl.py` & `pyroute2.minimal-0.7.8/examples/generic/netl.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/ipset.py` & `pyroute2.minimal-0.7.8/examples/ipset.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/ndb/create_bond.py` & `pyroute2.minimal-0.7.8/examples/ndb/create_bond.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/ndb/create_interface.py` & `pyroute2.minimal-0.7.8/examples/ndb/create_interface.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/ndb/create_vlan.py` & `pyroute2.minimal-0.7.8/examples/ndb/create_vlan.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/ndb/keystone_auth.py` & `pyroute2.minimal-0.7.8/examples/ndb/keystone_auth.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/ndb/radius_auth.py` & `pyroute2.minimal-0.7.8/examples/ndb/radius_auth.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/nftables_sets.py` & `pyroute2.minimal-0.7.8/examples/nftables_sets.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/policy/policy.py` & `pyroute2.minimal-0.7.8/examples/policy/policy.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/pyroute2-cli/create_bridge` & `pyroute2.minimal-0.7.8/examples/pyroute2-cli/create_bridge`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/pyroute2-cli/create_dummy` & `pyroute2.minimal-0.7.8/examples/pyroute2-cli/create_dummy`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/examples/wifi/nl80211_scan_dump.py` & `pyroute2.minimal-0.7.8/examples/wifi/nl80211_scan_dump.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pr2modules/__init__.py` & `pyroute2.minimal-0.7.8/pr2modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/arp.py` & `pyroute2.minimal-0.7.8/pyroute2/arp.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/bsd/pf_route/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/bsd/pf_route/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/bsd/pf_route/freebsd.py` & `pyroute2.minimal-0.7.8/pyroute2/bsd/pf_route/freebsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/bsd/pf_route/openbsd.py` & `pyroute2.minimal-0.7.8/pyroute2/bsd/pf_route/openbsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/bsd/rtmsocket/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/bsd/rtmsocket/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/bsd/rtmsocket/freebsd.py` & `pyroute2.minimal-0.7.8/pyroute2/bsd/rtmsocket/freebsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/bsd/rtmsocket/openbsd.py` & `pyroute2.minimal-0.7.8/pyroute2/bsd/rtmsocket/openbsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/bsd/util.py` & `pyroute2.minimal-0.7.8/pyroute2/bsd/util.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/common.py` & `pyroute2.minimal-0.7.8/pyroute2/common.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/config/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/config/asyncio.py` & `pyroute2.minimal-0.7.8/pyroute2/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/config/log.py` & `pyroute2.minimal-0.7.8/pyroute2/config/log.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/config/test_platform.py` & `pyroute2.minimal-0.7.8/pyroute2/config/test_platform.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/conntrack.py` & `pyroute2.minimal-0.7.8/pyroute2/conntrack.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/devlink.py` & `pyroute2.minimal-0.7.8/pyroute2/devlink.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/inotify/inotify_fd.py` & `pyroute2.minimal-0.7.8/pyroute2/inotify/inotify_fd.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/inotify/inotify_msg.py` & `pyroute2.minimal-0.7.8/pyroute2/inotify/inotify_msg.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/iproute/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/iproute/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/iproute/bsd.py` & `pyroute2.minimal-0.7.8/pyroute2/iproute/bsd.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/iproute/ipmock.py` & `pyroute2.minimal-0.7.8/pyroute2/iproute/ipmock.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         qdisc='noqueue',
         kind=None,
         link=None,
         vlan_id=None,
         master=0,
         br_max_age=0,
         br_forward_delay=0,
+        alt_ifname_list=None,
     ):
         self.index = index
         self.ifname = ifname
         self.flags = flags
         self.address = address
         self.broadcast = broadcast
         self.perm_address = perm_address
@@ -56,14 +57,15 @@
         self.qdisc = qdisc
         self.kind = kind
         self.link = link
         self.vlan_id = vlan_id
         self.master = master
         self.br_max_age = br_max_age
         self.br_forward_delay = br_forward_delay
+        self.alt_ifname_list = alt_ifname_list or []
 
     def export(self):
         ret = {
             'attrs': [
                 ['IFLA_IFNAME', self.ifname],
                 ['IFLA_TXQLEN', 1000],
                 ['IFLA_OPERSTATE', 'UNKNOWN'],
```

### Comparing `pyroute2.minimal-0.7.6/pyroute2/iproute/linux.py` & `pyroute2.minimal-0.7.8/pyroute2/iproute/linux.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/iproute/parsers.py` & `pyroute2.minimal-0.7.8/pyroute2/iproute/parsers.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/iproute/windows.py` & `pyroute2.minimal-0.7.8/pyroute2/iproute/windows.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/ipset.py` & `pyroute2.minimal-0.7.8/pyroute2/ipset.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/iwutil.py` & `pyroute2.minimal-0.7.8/pyroute2/iwutil.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/loader.py` & `pyroute2.minimal-0.7.8/pyroute2/loader.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/minimal.py` & `pyroute2.minimal-0.7.8/pyroute2/minimal.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/buffer.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/buffer.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/devlink/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/devlink/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/diag/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/diag/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/diag/ss2.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/diag/ss2.py`

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
@@ -137,20 +137,31 @@
             _pid=flow.pid,
             _ctxt=ctxt,
             _recurs_path=recurs_path,
         )
 
     def _build(self):
         for flow in psutil.net_connections(kind="all"):
-            proc = psutil.Process(flow.pid)
-            usr = proc.username()
-
-            ctxt = {"cmd": proc.exe(), "full_cmd": proc.cmdline(), "fds": []}
+            try:
+                proc = psutil.Process(flow.pid)
+                usr = proc.username()
 
-            self._enter_item(usr, flow, ctxt)
+                ctxt = {
+                    "cmd": proc.exe(),
+                    "full_cmd": proc.cmdline(),
+                    "fds": [],
+                }
+
+                self._enter_item(usr, flow, ctxt)
+            except (FileNotFoundError, AttributeError, psutil.NoSuchProcess):
+                # Handling edge case of race condition between build and parse
+                # time. That's for very volatile, shortlived flows that can
+                # exist during build but are gone once we want to parse the
+                # inode.
+                pass
 
     def __init__(self):
         self._build()
 
     def __getitem__(self, key):
         return self._data[key]
 
@@ -172,99 +183,99 @@
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
@@ -280,81 +291,81 @@
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
@@ -377,27 +388,27 @@
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
@@ -412,127 +423,127 @@
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
 
 
@@ -540,52 +551,52 @@
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
@@ -596,15 +607,15 @@
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

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/event/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/event/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/event/acpi_event.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/event/acpi_event.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/event/dquot.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/event/dquot.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/event/thermal.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/event/thermal.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/exceptions.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/generic/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/generic/ethtool.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/generic/ethtool.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/generic/l2tp.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/generic/l2tp.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/generic/mptcp.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/generic/mptcp.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/generic/wireguard.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/generic/wireguard.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/ipq/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/ipq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/ipset.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/ipset.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/nfctsocket.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/nfctsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/nfnetlink/nftsocket.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/nfnetlink/nftsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/nl80211/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/nl80211/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 import struct
 
 from pyroute2.common import map_namespace
 from pyroute2.netlink import genlmsg, nla, nla_base
 from pyroute2.netlink.generic import GenericNetlinkSocket
 from pyroute2.netlink.nlsocket import Marshal
 
+# Define from uapi/linux/nl80211.h
+NL80211_GENL_NAME = "nl80211"
+
 # nl80211 commands
 
 NL80211_CMD_UNSPEC = 0
 NL80211_CMD_GET_WIPHY = 1
 NL80211_CMD_SET_WIPHY = 2
 NL80211_CMD_NEW_WIPHY = 3
 NL80211_CMD_DEL_WIPHY = 4
@@ -221,14 +224,32 @@
 NL80211_STA_FLAG_AUTHENTICATED = 5
 NL80211_STA_FLAG_TDLS_PEER = 6
 NL80211_STA_FLAG_ASSOCIATED = 7
 (STA_FLAG_NAMES, STA_FLAG_VALUES) = map_namespace(
     'NL80211_STA_FLAG_', globals()
 )
 
+# Cipher suites
+WLAN_CIPHER_SUITE_USE_GROUP = 0x00FAC00
+WLAN_CIPHER_SUITE_WEP40 = 0x00FAC01
+WLAN_CIPHER_SUITE_TKIP = 0x00FAC02
+WLAN_CIPHER_SUITE_RESERVED = 0x00FAC03
+WLAN_CIPHER_SUITE_CCMP = 0x00FAC04
+WLAN_CIPHER_SUITE_WEP104 = 0x00FAC05
+WLAN_CIPHER_SUITE_AES_CMAC = 0x00FAC06
+WLAN_CIPHER_SUITE_GCMP = 0x00FAC08
+WLAN_CIPHER_SUITE_GCMP_256 = 0x00FAC09
+WLAN_CIPHER_SUITE_CCMP_256 = 0x00FAC0A
+WLAN_CIPHER_SUITE_BIP_GMAC_128 = 0x00FAC0B
+WLAN_CIPHER_SUITE_BIP_GMAC_256 = 0x00FAC0C
+WLAN_CIPHER_SUITE_BIP_CMAC_256 = 0x00FAC0D
+(WLAN_CIPHER_SUITE_NAMES, WLAN_CIPHER_SUITE_VALUES) = map_namespace(
+    'WLAN_CIPHER_SUITE_', globals()
+)
+
 
 class nl80211cmd(genlmsg):
     prefix = 'NL80211_ATTR_'
     nla_map = (
         ('NL80211_ATTR_UNSPEC', 'none'),
         ('NL80211_ATTR_WIPHY', 'uint32'),
         ('NL80211_ATTR_WIPHY_NAME', 'asciiz'),
@@ -257,15 +278,15 @@
         ('NL80211_ATTR_STA_PLINK_ACTION', 'hex'),
         ('NL80211_ATTR_MPATH_NEXT_HOP', 'hex'),
         ('NL80211_ATTR_MPATH_INFO', 'hex'),
         ('NL80211_ATTR_BSS_CTS_PROT', 'hex'),
         ('NL80211_ATTR_BSS_SHORT_PREAMBLE', 'hex'),
         ('NL80211_ATTR_BSS_SHORT_SLOT_TIME', 'hex'),
         ('NL80211_ATTR_HT_CAPABILITY', 'hex'),
-        ('NL80211_ATTR_SUPPORTED_IFTYPES', 'hex'),
+        ('NL80211_ATTR_SUPPORTED_IFTYPES', 'supported_iftypes'),
         ('NL80211_ATTR_REG_ALPHA2', 'asciiz'),
         ('NL80211_ATTR_REG_RULES', '*reg_rule'),
         ('NL80211_ATTR_MESH_CONFIG', 'hex'),
         ('NL80211_ATTR_BSS_BASIC_RATES', 'hex'),
         ('NL80211_ATTR_WIPHY_TXQ_PARAMS', 'hex'),
         ('NL80211_ATTR_WIPHY_FREQ', 'uint32'),
         ('NL80211_ATTR_WIPHY_CHANNEL_TYPE', 'hex'),
@@ -275,22 +296,22 @@
         ('NL80211_ATTR_MAX_NUM_SCAN_SSIDS', 'uint8'),
         ('NL80211_ATTR_SCAN_FREQUENCIES', 'hex'),
         ('NL80211_ATTR_SCAN_SSIDS', '*string'),
         ('NL80211_ATTR_GENERATION', 'uint32'),
         ('NL80211_ATTR_BSS', 'bss'),
         ('NL80211_ATTR_REG_INITIATOR', 'hex'),
         ('NL80211_ATTR_REG_TYPE', 'hex'),
-        ('NL80211_ATTR_SUPPORTED_COMMANDS', 'hex'),
+        ('NL80211_ATTR_SUPPORTED_COMMANDS', 'supported_commands'),
         ('NL80211_ATTR_FRAME', 'hex'),
         ('NL80211_ATTR_SSID', 'string'),
         ('NL80211_ATTR_AUTH_TYPE', 'uint32'),
         ('NL80211_ATTR_REASON_CODE', 'uint16'),
         ('NL80211_ATTR_KEY_TYPE', 'hex'),
         ('NL80211_ATTR_MAX_SCAN_IE_LEN', 'uint16'),
-        ('NL80211_ATTR_CIPHER_SUITES', 'hex'),
+        ('NL80211_ATTR_CIPHER_SUITES', 'cipher_suites'),
         ('NL80211_ATTR_FREQ_BEFORE', 'hex'),
         ('NL80211_ATTR_FREQ_AFTER', 'hex'),
         ('NL80211_ATTR_FREQ_FIXED', 'hex'),
         ('NL80211_ATTR_WIPHY_RETRY_SHORT', 'uint8'),
         ('NL80211_ATTR_WIPHY_RETRY_LONG', 'uint8'),
         ('NL80211_ATTR_WIPHY_FRAG_THRESHOLD', 'hex'),
         ('NL80211_ATTR_WIPHY_RTS_THRESHOLD', 'hex'),
@@ -330,16 +351,16 @@
         ('NL80211_ATTR_WIPHY_TX_POWER_LEVEL', 'uint32'),
         ('NL80211_ATTR_TX_FRAME_TYPES', 'hex'),
         ('NL80211_ATTR_RX_FRAME_TYPES', 'hex'),
         ('NL80211_ATTR_FRAME_TYPE', 'hex'),
         ('NL80211_ATTR_CONTROL_PORT_ETHERTYPE', 'hex'),
         ('NL80211_ATTR_CONTROL_PORT_NO_ENCRYPT', 'hex'),
         ('NL80211_ATTR_SUPPORT_IBSS_RSN', 'hex'),
-        ('NL80211_ATTR_WIPHY_ANTENNA_TX', 'hex'),
-        ('NL80211_ATTR_WIPHY_ANTENNA_RX', 'hex'),
+        ('NL80211_ATTR_WIPHY_ANTENNA_TX', 'uint32'),
+        ('NL80211_ATTR_WIPHY_ANTENNA_RX', 'uint32'),
         ('NL80211_ATTR_MCAST_RATE', 'hex'),
         ('NL80211_ATTR_OFFCHANNEL_TX_OK', 'hex'),
         ('NL80211_ATTR_BSS_HT_OPMODE', 'hex'),
         ('NL80211_ATTR_KEY_DEFAULT_TYPES', 'hex'),
         ('NL80211_ATTR_MAX_REMAIN_ON_CHANNEL_DURATION', 'hex'),
         ('NL80211_ATTR_MESH_SETUP', 'hex'),
         ('NL80211_ATTR_WIPHY_ANTENNA_AVAIL_TX', 'uint32'),
@@ -1269,14 +1290,121 @@
             ('NL80211_STA_INFO_BEACON_SIGNAL_AVG', 'uint8'),
             ('NL80211_STA_INFO_TID_STATS', 'hex'),
             ('NL80211_STA_INFO_RX_DURATION', 'uint64'),
             ('NL80211_STA_INFO_PAD', 'hex'),
             ('NL80211_STA_INFO_MAX', 'hex'),
         )
 
+    class supported_commands(nla_base):
+        '''
+        Supported commands format
+
+        NLA structure header::
+        +++++++++++++++++++++++
+        | uint16_t | uint16_t |
+        |  length  | NLA type |
+        +++++++++++++++++++++++
+
+        followed by multiple command entries::
+        ++++++++++++++++++++++++++++++++++
+        | uint16_t | uint16_t | uint32_t |
+        |   type   |  index   |   cmd    |
+        ++++++++++++++++++++++++++++++++++
+        '''
+
+        def decode(self):
+            nla_base.decode(self)
+            self.value = []
+
+            # Skip the first four bytes: NLA length and NLA type
+            length = self.length - 4
+            offset = self.offset + 4
+            while length > 0:
+                (msg_type, index, cmd_index) = struct.unpack_from(
+                    'HHI', self.data, offset
+                )
+                length -= 8
+                offset += 8
+
+                # Lookup for command name or assign a default name
+                name = NL80211_VALUES.get(
+                    cmd_index, 'NL80211_CMD_{}'.format(cmd_index)
+                )
+                self.value.append(name)
+
+    class cipher_suites(nla_base):
+        '''
+        Cipher suites format
+
+        NLA structure header::
+        +++++++++++++++++++++++
+        | uint16_t | uint16_t |
+        |  length  | NLA type |
+        +++++++++++++++++++++++
+
+        followed by multiple entries::
+        ++++++++++++
+        | uint32_t |
+        |  cipher  |
+        ++++++++++++
+        '''
+
+        def decode(self):
+            nla_base.decode(self)
+            self.value = []
+
+            # Skip the first four bytes: NLA length and NLA type
+            length = self.length - 4
+            offset = self.offset + 4
+            while length > 0:
+                (cipher,) = struct.unpack_from('<I', self.data, offset)
+                length -= 4
+                offset += 4
+
+                # Lookup for cipher name or assign a default name
+                name = WLAN_CIPHER_SUITE_VALUES.get(
+                    cipher, 'WLAN_CIPHER_SUITE_{:08X}'.format(cipher)
+                )
+                self.value.append(name)
+
+    class supported_iftypes(nla_base):
+        '''
+        Supported iftypes format
+
+        NLA structure header::
+        +++++++++++++++++++++++
+        | uint16_t | uint16_t |
+        |  length  | NLA type |
+        +++++++++++++++++++++++
+
+        followed by multiple iftype entries::
+        +++++++++++++++++++++++
+        | uint16_t | uint16_t |
+        |  length  |  iftype  |
+        +++++++++++++++++++++++
+        '''
+
+        def decode(self):
+            nla_base.decode(self)
+            self.value = []
+
+            # Skip the first four bytes: NLA length and NLA type
+            length = self.length - 4
+            offset = self.offset + 4
+            while length > 0:
+                (iflen, iftype) = struct.unpack_from('<HH', self.data, offset)
+                length -= 4
+                offset += 4
+
+                # Lookup for iftype name or assign a default name
+                name = IFTYPE_VALUES.get(
+                    iftype, 'NL80211_IFTYPE_{}'.format(iftype)
+                )
+                self.value.append(name)
+
 
 class MarshalNl80211(Marshal):
     msg_map = {
         NL80211_CMD_UNSPEC: nl80211cmd,
         NL80211_CMD_GET_WIPHY: nl80211cmd,
         NL80211_CMD_SET_WIPHY: nl80211cmd,
         NL80211_CMD_NEW_WIPHY: nl80211cmd,
@@ -1407,9 +1535,9 @@
 class NL80211(GenericNetlinkSocket):
     def __init__(self):
         GenericNetlinkSocket.__init__(self)
         self.marshal = MarshalNl80211()
 
     def bind(self, groups=0, **kwarg):
         GenericNetlinkSocket.bind(
-            self, 'nl80211', nl80211cmd, groups, None, **kwarg
+            self, NL80211_GENL_NAME, nl80211cmd, groups, None, **kwarg
         )
```

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/nlsocket.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/nlsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/proxy.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/proxy.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/fibmsg.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/fibmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifaddrmsg.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifaddrmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/compat.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/compat.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/bond.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/bond.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/geneve.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/geneve.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/tuntap.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/tuntap.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/vlan.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vlan.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/plugins/vxlan.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/plugins/vxlan.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/proxy.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/proxy.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/sync.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/sync.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifinfmsg/tuntap.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifinfmsg/tuntap.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ifstatsmsg.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ifstatsmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/iprsocket.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/iprsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/iw_event.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/iw_event.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/marshal.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/marshal.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ndmsg.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ndmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/ndtmsg.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/ndtmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/nsinfmsg.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/nsinfmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/riprsocket.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/riprsocket.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/rtmsg.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/rtmsg.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_bpf.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_bpf.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_connmark.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_connmark.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_gact.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_gact.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_mirred.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_mirred.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_police.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_police.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_skbedit.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_skbedit.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/act_vlan.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/act_vlan.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_basic.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_basic.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_flow.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_flow.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_fw.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_fw.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_matchall.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_matchall.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/cls_u32.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/cls_u32.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/common.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/common.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/common_act.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/common_act.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/common_ematch.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/common_ematch.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/em_cmp.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_cmp.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/em_ipset.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_ipset.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/em_meta.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/em_meta.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_bpf.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_bpf.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_cake.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_cake.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_choke.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_choke.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_clsact.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_clsact.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_codel.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_codel.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_drr.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_drr.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_fq_codel.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_fq_codel.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_hfsc.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_hfsc.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_htb.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_htb.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_netem.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_netem.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_sfq.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_sfq.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_tbf.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_tbf.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/rtnl/tcmsg/sched_template.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/rtnl/tcmsg/sched_template.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/taskstats/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/taskstats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netlink/uevent/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netlink/uevent/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netns/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/netns/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/netns/manager.py` & `pyroute2.minimal-0.7.8/pyroute2/netns/manager.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/protocols/__init__.py` & `pyroute2.minimal-0.7.8/pyroute2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/requests/address.py` & `pyroute2.minimal-0.7.8/pyroute2/requests/address.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/requests/bridge.py` & `pyroute2.minimal-0.7.8/pyroute2/requests/bridge.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/requests/common.py` & `pyroute2.minimal-0.7.8/pyroute2/requests/common.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/requests/link.py` & `pyroute2.minimal-0.7.8/pyroute2/requests/link.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/requests/main.py` & `pyroute2.minimal-0.7.8/pyroute2/requests/main.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/requests/neighbour.py` & `pyroute2.minimal-0.7.8/pyroute2/requests/neighbour.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/requests/route.py` & `pyroute2.minimal-0.7.8/pyroute2/requests/route.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/requests/rule.py` & `pyroute2.minimal-0.7.8/pyroute2/requests/rule.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2/wiset.py` & `pyroute2.minimal-0.7.8/pyroute2/wiset.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/pyroute2.minimal.egg-info/PKG-INFO` & `pyroute2.minimal-0.7.8/pyroute2.minimal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroute2.minimal
-Version: 0.7.6
+Version: 0.7.8
 Summary: Python Netlink library: minimal distribution
 Home-page: https://github.com/svinota/pyroute2
 Author: Peter Saveliev
 Author-email: peter@svinota.eu
 License: GPL-2.0-or-later OR Apache-2.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyroute2.minimal-0.7.6/pyroute2.minimal.egg-info/SOURCES.txt` & `pyroute2.minimal-0.7.8/pyroute2.minimal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/setup.cfg` & `pyroute2.minimal-0.7.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_addr_pool.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_addr_pool.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_buffer.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_buffer.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_common.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_common.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_iproute_match/links.dump` & `pyroute2.minimal-0.7.8/tests/test_unit/test_iproute_match/links.dump`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_iproute_match/test_match.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_iproute_match/test_match.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/addrmsg_ipv4.dump` & `pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/addrmsg_ipv4.dump`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/gre_01.dump` & `pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/gre_01.dump`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/iw_info_rsp.dump` & `pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/iw_info_rsp.dump`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/iw_scan_rsp.dump` & `pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/iw_scan_rsp.dump`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/test_attr.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/test_attr.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/test_map_adapter.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/test_map_adapter.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_nlmsg/test_marshal.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_nlmsg/test_marshal.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_requests/test_address.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_requests/test_address.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_requests/test_link.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_requests/test_link.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_requests/test_neighbour.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_requests/test_neighbour.py`

 * *Files identical despite different names*

### Comparing `pyroute2.minimal-0.7.6/tests/test_unit/test_requests/test_route.py` & `pyroute2.minimal-0.7.8/tests/test_unit/test_requests/test_route.py`

 * *Files identical despite different names*

