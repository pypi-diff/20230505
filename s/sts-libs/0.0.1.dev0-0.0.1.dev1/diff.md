# Comparing `tmp/sts_libs-0.0.1.dev0.tar.gz` & `tmp/sts_libs-0.0.1.dev1.tar.gz`

## Comparing `sts_libs-0.0.1.dev0.tar` & `sts_libs-0.0.1.dev1.tar`

### file list

```diff
@@ -1,232 +1,50 @@
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/requirements-stable.txt
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/__about__.data.json
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/__about__.meta.json
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/__init__.data.json
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/__init__.meta.json
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/noxfile.data.json
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/noxfile.meta.json
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/__init__.data.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/__init__.meta.json
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/__init__.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/__init__.meta.json
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/dm.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/dm.meta.json
--rw-r--r--   0        0        0    18158 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/dmpd.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/dmpd.meta.json
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/fc.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/fc.meta.json
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/fio.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/fio.meta.json
--rw-r--r--   0        0        0    34691 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/iscsi.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/iscsi.meta.json
--rw-r--r--   0        0        0    30934 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/linux.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/linux.meta.json
--rw-r--r--   0        0        0    32725 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/lio.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/lio.meta.json
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/loopdev.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/loopdev.meta.json
--rw-r--r--   0        0        0    51175 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/lsm.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/lsm.meta.json
--rw-r--r--   0        0        0    36542 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/lvm.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/lvm.meta.json
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/md.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/md.meta.json
--rw-r--r--   0        0        0    17228 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/mp.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/mp.meta.json
--rw-r--r--   0        0        0    13318 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/net.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/net.meta.json
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/qemu_img.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/qemu_img.meta.json
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/scsi.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/scsi.meta.json
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/scsi_debug.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/scsi_debug.meta.json
--rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/stratis.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/stratis.meta.json
--rw-r--r--   0        0        0    19904 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/vdo.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/vdo.meta.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/__init__.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/__init__.meta.json
--rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/atomic_run.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/atomic_run.meta.json
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/beaker.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/beaker.meta.json
--rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/cli_tools.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/cli_tools.meta.json
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/cmdline.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/cmdline.meta.json
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/logchecker.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/logchecker.meta.json
--rw-r--r--   0        0        0    19279 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/persistent_vars.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/persistent_vars.meta.json
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/restraint.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/restraint.meta.json
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/size.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/size.meta.json
--rw-r--r--   0        0        0    11096 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/tc.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/tc.meta.json
--rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/tmt.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/src/sts/utils/tmt.meta.json
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/__init__.data.json
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/__init__.meta.json
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/cmdline_test.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/cmdline_test.meta.json
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/fio_test.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/fio_test.meta.json
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/iscsi_test.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/iscsi_test.meta.json
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/linux_test.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/linux_test.meta.json
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/logchecker_test.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/logchecker_test.meta.json
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/loopdev_test.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/loopdev_test.meta.json
--rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/lvm_test.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/lvm_test.meta.json
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/md_test.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/md_test.meta.json
--rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/net_test.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/net_test.meta.json
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/persistent_vars_test.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/persistent_vars_test.meta.json
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/scsi_test.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.7/sts_libs/tests/scsi_test.meta.json
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/__about__.data.json
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/__about__.meta.json
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/__init__.data.json
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/__init__.meta.json
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/__init__.data.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/__init__.meta.json
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/__init__.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/__init__.meta.json
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/dm.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/dm.meta.json
--rw-r--r--   0        0        0    18160 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/dmpd.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/dmpd.meta.json
--rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/fc.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/fc.meta.json
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/fio.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/fio.meta.json
--rw-r--r--   0        0        0    34682 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/iscsi.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/iscsi.meta.json
--rw-r--r--   0        0        0    30923 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/linux.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/linux.meta.json
--rw-r--r--   0        0        0    32727 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/lio.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/lio.meta.json
--rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/loopdev.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/loopdev.meta.json
--rw-r--r--   0        0        0    51177 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/lsm.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/lsm.meta.json
--rw-r--r--   0        0        0    36544 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/lvm.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/lvm.meta.json
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/md.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/md.meta.json
--rw-r--r--   0        0        0    17230 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/mp.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/mp.meta.json
--rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/net.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/net.meta.json
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/qemu_img.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/qemu_img.meta.json
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/scsi.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/scsi.meta.json
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/scsi_debug.data.json
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/scsi_debug.meta.json
--rw-r--r--   0        0        0    19181 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/stratis.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/stratis.meta.json
--rw-r--r--   0        0        0    19906 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/vdo.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/vdo.meta.json
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/__init__.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/__init__.meta.json
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/atomic_run.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/atomic_run.meta.json
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/beaker.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/beaker.meta.json
--rw-r--r--   0        0        0    14260 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/cli_tools.data.json
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/cli_tools.meta.json
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/cmdline.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/cmdline.meta.json
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/logchecker.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/logchecker.meta.json
--rw-r--r--   0        0        0    19270 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/persistent_vars.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/persistent_vars.meta.json
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/restraint.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/restraint.meta.json
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/size.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/size.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/tc.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/tc.meta.json
--rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/tmt.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/src/sts/utils/tmt.meta.json
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/__init__.data.json
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/__init__.meta.json
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/cmdline_test.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/cmdline_test.meta.json
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/fio_test.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/fio_test.meta.json
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/iscsi_test.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/iscsi_test.meta.json
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/linux_test.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/linux_test.meta.json
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/logchecker_test.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/logchecker_test.meta.json
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/loopdev_test.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/loopdev_test.meta.json
--rw-r--r--   0        0        0     7992 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/lvm_test.data.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/lvm_test.meta.json
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/md_test.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/md_test.meta.json
--rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/net_test.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/net_test.meta.json
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/persistent_vars_test.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/persistent_vars_test.meta.json
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/scsi_test.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/.mypy_cache/3.8/sts_libs/tests/scsi_test.meta.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    40145 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    16943 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    48966 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    65812 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    35343 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    42046 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0    28673 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    22247 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/atomic_run.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/tc.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/LICENSE
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/sts_libs/README.md
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/requirements-stable.txt
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    40145 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    16943 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    48966 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    65812 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    35343 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    42046 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0    28673 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    22247 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/atomic_run.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/tc.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/LICENSE
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/sts_libs/README.md
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 sts_libs-0.0.1.dev1/PKG-INFO
```

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/dm.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/dm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/dmpd.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/dmpd.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/fc.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/fc.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/fio.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/fio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/iscsi.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/iscsi.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/linux.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/linux.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/lio.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/lio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/loopdev.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/loopdev.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/lsm.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/lsm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/lvm.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/lvm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/md.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/md.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/mp.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/mp.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/net.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/net.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/qemu_img.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/scsi.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/scsi.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/scsi_debug.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/stratis.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/stratis.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/vdo.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/vdo.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/__init__.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/atomic_run.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/atomic_run.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/beaker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/cmdline.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/logchecker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/restraint.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/size.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/size.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/tc.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/tc.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.0.1.dev1/sts_libs/src/sts/utils/tmt.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/cmdline_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/fio_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/iscsi_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/iscsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/linux_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/linux_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/logchecker_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/logchecker_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,28 +46,28 @@
         run_func.reset_mock()
 
         run_func.side_effect = _run_dmesg_segfault
         assert log_checker.dmesg_check() is False
         run_calls = [
             call("dmesg | grep -i ' segfault '", return_output=True),
             call("echo '\nINFO found  segfault   Saving it\n'>> dmesg.log"),
-            call("dmesg >> dmesg.log"),
+            call("dmesg >> ./dmesg.log"),
             call("dmesg | grep -i 'Call Trace:'", return_output=True),
         ]
         # print(run_func.call_args_list)
         run_func.assert_has_calls(run_calls)
         run_func.reset_mock()
 
         run_func.side_effect = _run_dmesg_calltrace
         assert log_checker.dmesg_check() is False
         run_calls = [
             call("dmesg | grep -i ' segfault '", return_output=True),
             call("dmesg | grep -i 'Call Trace:'", return_output=True),
             call("echo '\nINFO found Call Trace:  Saving it\n'>> dmesg.log"),
-            call("dmesg >> dmesg.log"),
+            call("dmesg >> ./dmesg.log"),
         ]
         # print(run_func.call_args_list)
         run_func.assert_has_calls(run_calls)
         run_func.reset_mock()
 
     @patch("sts.utils.logchecker.kernel_check")
     def test_check_all(self, check_func):
```

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/lvm_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/lvm_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/md_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/md_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/net_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/net_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/sts_libs/tests/scsi_test.py` & `sts_libs-0.0.1.dev1/sts_libs/tests/scsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/LICENSE` & `sts_libs-0.0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/pyproject.toml` & `sts_libs-0.0.1.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = ""
 readme = "sts_libs/README.md"
 requires-python = ">=3.8"
 dynamic = ["version", "optional-dependencies"]
 authors = [
   { name = "Bruno Goncalves", email = "bgoncalv@redhat.com" },
   { name = "Filip Suba", email = "fsuba@redhat.com" },
-  { name = "Jakub Krysl"},
+  { name = "Jakub Krysl", email = "jkrysl@redhat.com" },
   { name = "Martin Hoyer", email = "mhoyer@redhat.com" },
 ]
 maintainers = [
   { name = "Martin Hoyer", email = "mhoyer@redhat.com" },
   { name = "Filip Suba", email = "fsuba@redhat.com" },
   { name = "Bruno Goncalves", email = "bgoncalv@redhat.com" },
 ]
@@ -24,17 +24,19 @@
 classifiers = [
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Testing",
+  "Topic :: Software Development :: Quality Assurance",
   "Intended Audience :: Developers",
   "Operating System :: POSIX :: Linux",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+  "Framework :: Hatch",
 ]
 
 dependencies = [
   "configobj >=5.0.8",
   "netifaces2 >=0.0.15",
 ]
```

### Comparing `sts_libs-0.0.1.dev0/sts_libs/README.md` & `sts_libs-0.0.1.dev1/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.1.dev0/PKG-INFO` & `sts_libs-0.0.1.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: sts-libs
-Version: 0.0.1.dev0
+Version: 0.0.1.dev1
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
-Author: Jakub Krysl
-Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Martin Hoyer <mhoyer@redhat.com>
+Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
+Classifier: Framework :: Hatch
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Requires-Dist: configobj>=5.0.8
 Requires-Dist: netifaces2>=0.0.15
 Provides-Extra: stable
 Requires-Dist: configobj==5.0.8; extra == 'stable'
 Requires-Dist: netifaces2==0.0.15; extra == 'stable'
```

