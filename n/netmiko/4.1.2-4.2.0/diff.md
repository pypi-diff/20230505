# Comparing `tmp/netmiko-4.1.2.tar.gz` & `tmp/netmiko-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netmiko-4.1.2.tar", last modified: Tue Aug  9 21:24:58 2022, max compression
+gzip compressed data, was "netmiko-4.2.0.tar", max compression
```

## Comparing `netmiko-4.1.2.tar` & `netmiko-4.2.0.tar`

### file list

```diff
@@ -1,501 +1,193 @@
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.463442 netmiko-4.1.2/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2957 2022-03-15 19:38:09.000000 netmiko-4.1.2/COMMON_ISSUES.md
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    25739 2022-07-11 18:53:23.000000 netmiko-4.1.2/EXAMPLES.md
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1078 2022-03-15 19:38:09.000000 netmiko-4.1.2/LICENSE
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       82 2022-03-15 19:38:09.000000 netmiko-4.1.2/MANIFEST.in
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6991 2022-08-09 21:24:58.463442 netmiko-4.1.2/PKG-INFO
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4229 2022-07-11 18:53:23.000000 netmiko-4.1.2/PLATFORMS.md
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6360 2022-07-11 18:53:23.000000 netmiko-4.1.2/README.md
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      997 2022-03-15 19:38:09.000000 netmiko-4.1.2/TESTING.md
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2300 2022-03-15 19:38:09.000000 netmiko-4.1.2/VENDOR.md
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.423442 netmiko-4.1.2/netmiko/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2637 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/__init__.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/a10/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       61 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/a10/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      696 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/a10/a10_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/accedian/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       81 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/accedian/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1098 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/accedian/accedian_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/adtran/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      107 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/adtran/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2663 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/adtran/adtran.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/alcatel/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       87 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/alcatel/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      836 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/alcatel/alcatel_aos_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/allied_telesis/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      118 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/allied_telesis/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1607 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/allied_telesis/allied_telesis_awplus.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/apresia/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      126 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/apresia/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1409 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/apresia/apresia_aeos.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/arista/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      141 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/arista/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4926 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/arista/arista.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/aruba/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       69 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/aruba/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1674 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/aruba/aruba_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/audiocode/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      345 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/audiocode/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    15133 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/audiocode/audiocode_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    91815 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/base_connection.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/broadcom/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       99 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/broadcom/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1750 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/broadcom/broadcom_icos_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/brocade/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       87 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/brocade/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      563 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/brocade/brocade_fos_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/calix/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      104 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/calix/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3893 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/calix/calix_b6.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/cdot/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       78 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cdot/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4075 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/cdot/cdot_cros_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/centec/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      110 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/centec/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      723 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/centec/centec_os.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5619 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/channel.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/checkpoint/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      102 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/checkpoint/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      714 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/checkpoint/checkpoint_gaia_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.427442 netmiko-4.1.2/netmiko/ciena/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      179 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/ciena/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     7241 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ciena/ciena_saos.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/cisco/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1210 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cisco/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5957 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cisco/cisco_asa_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      849 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cisco/cisco_ftd_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9621 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cisco/cisco_ios.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6874 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cisco/cisco_nxos_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1190 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cisco/cisco_s300.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3214 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cisco/cisco_tp_tcce.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3143 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/cisco/cisco_viptela.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     8763 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/cisco/cisco_wlc_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9884 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/cisco/cisco_xr.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    10198 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cisco_base_connection.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/citrix/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       82 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/citrix/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1574 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/citrix/netscaler_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/cli_tools/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cli_tools/__init__.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     7508 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cli_tools/netmiko_cfg.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     7580 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cli_tools/netmiko_grep.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     7425 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/cli_tools/netmiko_show.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/cloudgenix/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       95 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/cloudgenix/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1889 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/cloudgenix/cloudgenix_ion.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/coriant/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       77 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/coriant/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1049 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/coriant/coriant_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/dell/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      693 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dell/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      938 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dell/dell_dnos6.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      530 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dell/dell_force10_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3811 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dell/dell_isilon_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4855 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dell/dell_os10_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4030 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dell/dell_powerconnect.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1362 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dell/dell_sonic_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/dlink/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      104 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dlink/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1407 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/dlink/dlink_ds.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/eltex/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      136 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/eltex/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4193 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/eltex/eltex_esr_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      543 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/eltex/eltex_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/endace/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       76 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/endace/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2126 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/endace/endace_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/enterasys/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       85 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/enterasys/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      543 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/enterasys/enterasys_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/ericsson/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       90 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ericsson/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5020 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/ericsson/ericsson_ipos.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1309 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/exceptions.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.431442 netmiko-4.1.2/netmiko/extreme/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      901 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/extreme/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2237 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/extreme/extreme_ers_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     8186 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/extreme/extreme_exos.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1063 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/extreme/extreme_netiron.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1013 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/extreme/extreme_nos_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1005 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/extreme/extreme_slx_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1060 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/extreme/extreme_tierraos_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      763 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/extreme/extreme_vsp_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      441 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/extreme/extreme_wing_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/f5/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      131 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/f5/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       84 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/f5/f5_linux_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1375 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/f5/f5_tmsh_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/flexvnf/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       77 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/flexvnf/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6996 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/flexvnf/flexvnf_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/fortinet/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       81 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/fortinet/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4218 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/fortinet/fortinet_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/hp/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      215 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/hp/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5346 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/hp/hp_comware.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     7903 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/hp/hp_procurve.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/huawei/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      245 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/huawei/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9032 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/huawei/huawei.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4200 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/huawei/huawei_smartax.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/ipinfusion/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      162 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/ipinfusion/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2789 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ipinfusion/ipinfusion_ocnos.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/juniper/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      235 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/juniper/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    10611 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/juniper/juniper.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1014 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/juniper/juniper_screenos.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/keymile/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      152 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/keymile/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1414 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/keymile/keymile_nos_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1453 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/keymile/keymile_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/linux/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      109 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/linux/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     7882 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/linux/linux_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/mellanox/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      100 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/mellanox/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3040 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/mellanox/mellanox_mlnxos_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/mikrotik/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      285 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/mikrotik/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    10963 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/mikrotik/mikrotik_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/mrv/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      133 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/mrv/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1473 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/mrv/mrv_lx.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1768 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/mrv/mrv_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/netapp/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       86 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/netapp/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1473 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/netapp/netapp_cdot_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/netgear/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       99 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/netgear/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1896 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/netgear/netgear_prosafe_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       43 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/netmiko_globals.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      844 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/no_config.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      953 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/no_enable.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/nokia/
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      243 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/nokia/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5814 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/nokia/nokia_srl.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    15209 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/nokia/nokia_sros.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.435442 netmiko-4.1.2/netmiko/oneaccess/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      143 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/oneaccess/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1265 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/oneaccess/oneaccess_oneos.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/ovs/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       77 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/ovs/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       85 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/ovs/ovs_linux_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/paloalto/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      137 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/paloalto/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     8668 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/paloalto/paloalto_panos.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/pluribus/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      106 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/pluribus/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      641 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/pluribus/pluribus_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/quanta/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       86 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/quanta/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      851 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/quanta/quanta_mesh_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/rad/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      128 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/rad/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3262 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/rad/rad_etx.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/raisecom/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      174 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/raisecom/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5851 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/raisecom/raisecom_roap.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/ruckus/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      182 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/ruckus/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3939 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ruckus/ruckus_fastiron.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/ruijie/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      110 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/ruijie/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1298 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ruijie/ruijie_os.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5336 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/scp_functions.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    16131 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/scp_handler.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2465 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/session_log.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/sixwind/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       80 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/sixwind/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3554 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/sixwind/sixwind_os.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    11701 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/snmp_autodetect.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/sophos/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       86 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/sophos/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1212 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/sophos/sophos_sfos_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      343 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ssh_auth.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    16682 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/ssh_autodetect.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)    18058 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/ssh_dispatcher.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/supermicro/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      138 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/supermicro/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1275 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/supermicro/smci_smis.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/terminal_server/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      200 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/terminal_server/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      927 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/terminal_server/terminal_server.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/tplink/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      145 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/tplink/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6926 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/tplink/tplink_jetstream.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/ubiquiti/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      285 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ubiquiti/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2868 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ubiquiti/edge_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1050 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ubiquiti/edgerouter_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1318 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/ubiquiti/unifiswitch_ssh.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    21298 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/utilities.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/vyos/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       65 2022-03-15 19:38:09.000000 netmiko-4.1.2/netmiko/vyos/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5106 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/vyos/vyos_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/watchguard/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      103 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/watchguard/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1430 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/watchguard/fireware_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/yamaha/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      139 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/yamaha/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3240 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/yamaha/yamaha.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/zte/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      144 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/zte/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2440 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/zte/zte_zxros.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.439442 netmiko-4.1.2/netmiko/zyxel/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       70 2022-07-11 18:53:23.000000 netmiko-4.1.2/netmiko/zyxel/__init__.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1028 2022-08-09 21:16:34.000000 netmiko-4.1.2/netmiko/zyxel/zyxel_ssh.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.423442 netmiko-4.1.2/netmiko.egg-info/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6991 2022-08-09 21:24:58.000000 netmiko-4.1.2/netmiko.egg-info/PKG-INFO
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    15282 2022-08-09 21:24:58.000000 netmiko-4.1.2/netmiko.egg-info/SOURCES.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        1 2022-08-09 21:24:58.000000 netmiko-4.1.2/netmiko.egg-info/dependency_links.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      179 2022-08-09 21:24:58.000000 netmiko-4.1.2/netmiko.egg-info/entry_points.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      113 2022-08-09 21:24:58.000000 netmiko-4.1.2/netmiko.egg-info/requires.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        8 2022-08-09 21:24:58.000000 netmiko-4.1.2/netmiko.egg-info/top_level.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       50 2022-03-15 19:38:09.000000 netmiko-4.1.2/requirements.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      917 2022-08-09 21:24:58.467442 netmiko-4.1.2/setup.cfg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     2103 2022-08-09 21:16:34.000000 netmiko-4.1.2/setup.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.447442 netmiko-4.1.2/tests/
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.447442 netmiko-4.1.2/tests/SLOG/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      722 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/SLOG/cisco881_slog.log
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1016 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/SLOG/cisco881_slog_append.log
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      721 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/SLOG/cisco881_slog_append_compare.log
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      722 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/SLOG/cisco881_slog_compare.log
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      186 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/SLOG/cisco881_slog_wr.log
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      880 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/SLOG/cisco881_slog_wr_compare.log
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3025 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/SLOG/netmiko.log
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.451442 netmiko-4.1.2/tests/__pycache__/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    11933 2022-06-02 20:51:29.000000 netmiko-4.1.2/tests/__pycache__/conftest.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    12366 2022-08-09 00:09:01.000000 netmiko-4.1.2/tests/__pycache__/conftest.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    11838 2022-03-17 02:14:10.000000 netmiko-4.1.2/tests/__pycache__/conftest.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    12418 2022-08-09 01:23:34.000000 netmiko-4.1.2/tests/__pycache__/conftest.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5588 2022-08-05 18:51:49.000000 netmiko-4.1.2/tests/__pycache__/network_utilities.cpython-310.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5617 2022-03-17 04:43:46.000000 netmiko-4.1.2/tests/__pycache__/network_utilities.cpython-37.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5706 2022-06-27 17:42:56.000000 netmiko-4.1.2/tests/__pycache__/network_utilities.cpython-39.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      548 2022-07-05 16:49:27.000000 netmiko-4.1.2/tests/__pycache__/test_import_netmiko.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      879 2022-04-14 21:03:12.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_autodetect.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      879 2022-06-27 17:53:03.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_autodetect.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      877 2022-06-24 20:28:43.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_autodetect.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3434 2022-04-25 21:54:13.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_cmd_verify.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3434 2022-08-08 21:37:55.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_cmd_verify.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    14123 2022-03-17 16:02:15.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_commit.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    14123 2022-08-05 19:24:50.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_commit.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    15716 2022-03-17 04:47:21.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_commit.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    14200 2022-06-27 17:44:25.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_commit.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     8538 2022-06-02 20:51:31.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_config.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    10082 2022-08-09 01:56:13.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_config.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     8882 2022-03-17 04:43:09.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_config.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    10182 2022-08-08 17:52:32.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_config.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3836 2022-03-17 02:00:54.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_config_acl.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3836 2022-08-05 18:51:49.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_config_acl.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3898 2022-03-17 04:43:46.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_config_acl.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3852 2022-06-27 17:42:56.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_config_acl.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4386 2022-03-17 02:01:07.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_exceptions.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4386 2022-08-05 19:20:58.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_exceptions.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4675 2022-03-17 04:43:58.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_exceptions.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1041 2022-04-25 21:53:37.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_save.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1041 2022-08-08 21:37:16.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_save.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1039 2022-06-27 17:42:47.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_save.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     8638 2022-03-22 21:05:37.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_scp.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9087 2022-08-05 18:46:08.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_scp.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9783 2022-03-17 02:14:12.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_scp.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9075 2022-08-05 18:41:05.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_scp.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     7683 2022-03-17 16:54:37.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_session_log.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     7683 2022-08-09 02:13:57.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_session_log.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     7673 2022-08-07 18:24:31.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_session_log.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    18282 2022-05-20 18:41:35.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_show.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19479 2022-08-09 01:55:26.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_show.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    20723 2022-03-17 02:14:37.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_show.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19576 2022-08-09 01:23:54.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_show.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3594 2022-03-17 16:05:23.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_tcl.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3594 2022-08-05 19:37:53.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_tcl.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3762 2022-03-17 04:50:27.000000 netmiko-4.1.2/tests/__pycache__/test_netmiko_tcl.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5410 2022-03-18 21:47:20.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_read_timing.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5414 2022-08-08 20:05:55.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_read_timing.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6306 2022-06-24 20:05:20.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_read_timing.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4717 2022-03-18 20:32:34.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_read_until_pattern.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4717 2022-08-08 18:35:44.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_read_until_pattern.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5740 2022-03-18 21:03:27.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_send_command.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5740 2022-08-08 19:06:15.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_send_command.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5402 2022-04-26 21:38:37.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_send_command_timing.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5402 2022-08-08 20:15:29.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_send_command_timing.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6298 2022-06-24 20:19:06.000000 netmiko-4.1.2/tests/__pycache__/test_timeout_send_command_timing.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      831 2022-03-17 01:53:04.000000 netmiko-4.1.2/tests/__pycache__/test_utils.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      831 2022-06-23 18:45:03.000000 netmiko-4.1.2/tests/__pycache__/test_utils.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      722 2022-05-19 16:54:39.000000 netmiko-4.1.2/tests/__pycache__/test_utils.cpython-310.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      797 2022-03-17 02:14:12.000000 netmiko-4.1.2/tests/__pycache__/test_utils.cpython-37-pytest-6.2.4.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      823 2022-06-24 16:53:37.000000 netmiko-4.1.2/tests/__pycache__/test_utils.cpython-39-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      566 2022-08-09 18:15:47.000000 netmiko-4.1.2/tests/arista9.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 18:16:00.000000 netmiko-4.1.2/tests/asa1.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       76 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/cisco_asa_commands.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       63 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/cisco_ios_commands.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)    18555 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/conftest.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.455442 netmiko-4.1.2/tests/etc/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      243 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/etc/.netmiko.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       66 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/etc/cisco_ios_show_version.template
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     7849 2022-08-08 18:09:50.000000 netmiko-4.1.2/tests/etc/commands.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    18805 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/etc/commands.yml.example
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      106 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/etc/index
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9394 2022-08-08 21:11:47.000000 netmiko-4.1.2/tests/etc/responses.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    12072 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/etc/responses.yml.example
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      180 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/etc/ssh_config
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      172 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/etc/ssh_config_proxyjump
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4087 2022-08-09 00:17:25.000000 netmiko-4.1.2/tests/etc/test_devices.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5146 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/etc/test_devices.yml.example
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      115 2022-03-17 02:26:49.000000 netmiko-4.1.2/tests/etc/test_devices_exc.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       52 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/etc/textfsm.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       65 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/etc/yaml_test.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    37626 2022-08-09 02:13:59.000000 netmiko-4.1.2/tests/foo.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9612 2022-08-09 18:18:07.000000 netmiko-4.1.2/tests/hpe.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      284 2022-06-24 17:33:49.000000 netmiko-4.1.2/tests/linux.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    22525 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/netmiko_audiocode_driver_test_results.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     7544 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/network_utilities.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.455442 netmiko-4.1.2/tests/performance/
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.455442 netmiko-4.1.2/tests/performance/__pycache__/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      524 2022-05-20 17:56:09.000000 netmiko-4.1.2/tests/performance/__pycache__/perf_utils.cpython-310.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5811 2022-03-24 03:52:19.000000 netmiko-4.1.2/tests/performance/__pycache__/test_netmiko.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      641 2022-03-23 21:35:27.000000 netmiko-4.1.2/tests/performance/asa1.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3390 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/gen_graph.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4439 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/gen_scrapli_graph.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.455442 netmiko-4.1.2/tests/performance/graphs/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    26951 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs/netmiko_arista_eos.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    26243 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs/netmiko_cisco_asa.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    26090 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs/netmiko_cisco_ios.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    27871 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs/netmiko_cisco_nxos.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    27592 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs/netmiko_cisco_xe.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    27725 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs/netmiko_cisco_xr.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    25233 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs/netmiko_hp_procurve.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    27532 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs/netmiko_juniper_junos.svg
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/performance/graphs_netmiko_scrapli/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19376 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs_netmiko_scrapli/netmiko_scrapli_arista_eos.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    18745 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs_netmiko_scrapli/netmiko_scrapli_cisco_ios.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19088 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs_netmiko_scrapli/netmiko_scrapli_cisco_nxos.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19086 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs_netmiko_scrapli/netmiko_scrapli_cisco_xe.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    18737 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/graphs_netmiko_scrapli/netmiko_scrapli_juniper_junos.svg
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5627 2022-03-24 03:54:06.000000 netmiko-4.1.2/tests/performance/hpe.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6748 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/netmiko_performance.csv
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1475 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/netmiko_scrapli_performance.csv
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      324 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/perf_utils.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      453 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/performance_netmiko_scrapli.md
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      300 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/performance_report.md
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/requirements.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       45 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/setup.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1685 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/test_devices.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1159 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/test_devices_scrapli.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6397 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/test_netmiko.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     1092 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/test_new_platform.sh
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      749 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/test_performance.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6445 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/performance/test_scrapli_new.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1576 2022-03-23 21:34:55.000000 netmiko-4.1.2/tests/performance/vmx1.out
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      113 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/remove_delay.sh
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      939 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/run_live_tests.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       66 2022-08-09 16:20:44.000000 netmiko-4.1.2/tests/show_run_interfaces.ttp
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    28801 2022-08-08 22:00:36.000000 netmiko-4.1.2/tests/test.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       42 2022-08-09 16:41:44.000000 netmiko-4.1.2/tests/test2_src.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-08-09 16:41:44.000000 netmiko-4.1.2/tests/test9.txt
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_arista_eos/
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      491 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_arista_eos/add_delay_cisco_xe.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_arista_eos/test9.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      548 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_arista_eos/test_arista_eos.sh
--rw-r--r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-08-09 16:24:47.000000 netmiko-4.1.2/tests/test_arista_eos/testx.txt
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_cisco_asa/
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      488 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_asa/add_delay_cisco_asa.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_asa/test9.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      628 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_asa/test_cisco_asa.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_asa/testx.txt
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_cisco_ios/
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      491 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_ios/add_delay_cisco881.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_ios/test9.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      810 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_ios/test_ios.sh
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_cisco_nxos/
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      489 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_nxos/add_delay_cisco_nxos.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_nxos/test9.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      455 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_nxos/test_cisco_nxos.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-08-09 16:40:26.000000 netmiko-4.1.2/tests/test_cisco_nxos/testx.txt
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_cisco_xe/
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      491 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_xe/add_delay_cisco_xe.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       42 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_xe/test2_src.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_xe/test9.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      462 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_xe/test_cisco_xe.sh
--rw-r--r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-08-09 01:23:53.000000 netmiko-4.1.2/tests/test_cisco_xe/testx.txt
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_cisco_xr/
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      433 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_xr/add_delay_iosxr_azure.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_xr/test9.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      558 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_xr/test_iosxr.sh
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      568 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_cisco_xr/test_iosxr_azure.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-08-09 16:35:52.000000 netmiko-4.1.2/tests/test_cisco_xr/testx.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      169 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_commit.sh
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_extreme_exos/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_extreme_exos/test9.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_extreme_exos/testx.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       85 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/test_import_netmiko.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_juniper_junos/
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      487 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_juniper_junos/add_delay_juniper_junos.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_juniper_junos/test9.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      564 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_juniper_junos/test_juniper_junos.sh
--rw-r--r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-08-09 16:26:12.000000 netmiko-4.1.2/tests/test_juniper_junos/testx.txt
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_linux/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_linux/test9.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-08-09 16:42:01.000000 netmiko-4.1.2/tests/test_linux/testx.txt
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.459442 netmiko-4.1.2/tests/test_mikrotik_routeros/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_mikrotik_routeros/test9.txt
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)       19 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_mikrotik_routeros/testx.txt
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      276 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/test_netmiko_autodetect.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     2075 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_netmiko_cmd_verify.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)    13705 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_netmiko_commit.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)    10070 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/test_netmiko_config.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     2918 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_netmiko_config_acl.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     1980 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_netmiko_exceptions.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      419 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_netmiko_save.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     8159 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_netmiko_scp.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6532 2022-08-07 18:24:13.000000 netmiko-4.1.2/tests/test_netmiko_session_log.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)    14077 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/test_netmiko_show.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     1314 2022-08-05 19:37:33.000000 netmiko-4.1.2/tests/test_netmiko_tcl.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.463442 netmiko-4.1.2/tests/test_nokia_srl/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      579 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_nokia_srl/README.md
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      117 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_nokia_srl/containerlabTest.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      264 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_nokia_srl/test_srl.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3891 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_nokia_srl/testoutput.txt
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.463442 netmiko-4.1.2/tests/test_out/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6113 2022-08-08 21:38:25.000000 netmiko-4.1.2/tests/test_out/test_arista_eos.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-08 21:36:43.000000 netmiko-4.1.2/tests/test_out/test_arista_eos.stderr
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_out/test_cisco_asa.stderr
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6622 2022-08-08 21:39:22.000000 netmiko-4.1.2/tests/test_out/test_cisco_ios.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-08 21:36:43.000000 netmiko-4.1.2/tests/test_out/test_cisco_ios.stderr
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5553 2022-08-08 21:39:37.000000 netmiko-4.1.2/tests/test_out/test_cisco_nxos.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-08 21:36:43.000000 netmiko-4.1.2/tests/test_out/test_cisco_nxos.stderr
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5078 2022-08-08 21:39:04.000000 netmiko-4.1.2/tests/test_out/test_cisco_xe.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-08 21:36:43.000000 netmiko-4.1.2/tests/test_out/test_cisco_xe.stderr
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5417 2022-08-08 21:41:02.000000 netmiko-4.1.2/tests/test_out/test_cisco_xr_azure.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-08 21:36:43.000000 netmiko-4.1.2/tests/test_out/test_cisco_xr_azure.stderr
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6867 2022-08-08 21:42:02.000000 netmiko-4.1.2/tests/test_out/test_cisco_xr_xrv.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-08 21:36:43.000000 netmiko-4.1.2/tests/test_out/test_cisco_xr_xrv.stderr
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     6913 2022-08-08 21:45:07.000000 netmiko-4.1.2/tests/test_out/test_juniper_junos.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-08 21:36:43.000000 netmiko-4.1.2/tests/test_out/test_juniper_junos.stderr
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     6229 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_suite_alt.sh
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3551 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_timeout_read_timing.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     4020 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_timeout_read_until_pattern.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     5672 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_timeout_send_command.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3082 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/test_timeout_send_command_timing.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      494 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/test_utils.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    10089 2022-04-27 02:47:46.000000 netmiko-4.1.2/tests/testx.out
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.463442 netmiko-4.1.2/tests/unit/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/unit/.netmiko.yml
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)        0 2022-03-15 19:38:09.000000 netmiko-4.1.2/tests/unit/__init__.py
-drwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)        0 2022-08-09 21:24:58.463442 netmiko-4.1.2/tests/unit/__pycache__/
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      137 2022-04-13 21:01:53.000000 netmiko-4.1.2/tests/unit/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19615 2022-04-13 21:01:53.000000 netmiko-4.1.2/tests/unit/__pycache__/test_base_connection.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19615 2022-08-08 23:45:21.000000 netmiko-4.1.2/tests/unit/__pycache__/test_base_connection.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3079 2022-04-13 21:01:53.000000 netmiko-4.1.2/tests/unit/__pycache__/test_connection.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     3079 2022-08-08 23:45:25.000000 netmiko-4.1.2/tests/unit/__pycache__/test_connection.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      853 2022-04-13 21:01:53.000000 netmiko-4.1.2/tests/unit/__pycache__/test_ssh_autodetect.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      853 2022-08-08 23:45:24.000000 netmiko-4.1.2/tests/unit/__pycache__/test_ssh_autodetect.cpython-310-pytest-7.1.2.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19115 2022-04-14 18:15:47.000000 netmiko-4.1.2/tests/unit/__pycache__/test_utilities.cpython-310-pytest-6.2.5.pyc
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)    19115 2022-08-08 23:47:09.000000 netmiko-4.1.2/tests/unit/__pycache__/test_utilities.cpython-310-pytest-7.1.2.pyc
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)    14493 2022-08-08 23:45:08.000000 netmiko-4.1.2/tests/unit/test_base_connection.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)     1502 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/unit/test_connection.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)      248 2022-07-11 18:53:23.000000 netmiko-4.1.2/tests/unit/test_ssh_autodetect.py
--rwxrwxr-x   0 ktbyers   (1002) ktbyers   (1002)    13969 2022-08-09 21:16:34.000000 netmiko-4.1.2/tests/unit/test_utilities.py
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)     9204 2022-08-09 02:00:05.000000 netmiko-4.1.2/tests/vmx1.out
--rw-rw-r--   0 ktbyers   (1002) ktbyers   (1002)      518 2022-08-09 18:17:23.000000 netmiko-4.1.2/tests/xr.out
+-rw-r--r--   0        0        0     1078 2022-03-15 19:38:09.010841 netmiko-4.2.0/LICENSE
+-rw-r--r--   0        0        0     6365 2023-05-05 16:30:15.008753 netmiko-4.2.0/README.md
+-rw-r--r--   0        0        0     2637 2023-05-05 16:30:15.060753 netmiko-4.2.0/netmiko/__init__.py
+-rw-r--r--   0        0        0       61 2022-03-15 19:38:09.086841 netmiko-4.2.0/netmiko/a10/__init__.py
+-rw-r--r--   0        0        0      696 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/a10/a10_ssh.py
+-rw-r--r--   0        0        0       81 2022-03-15 19:38:09.086841 netmiko-4.2.0/netmiko/accedian/__init__.py
+-rw-r--r--   0        0        0     1098 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/accedian/accedian_ssh.py
+-rw-r--r--   0        0        0      107 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/adtran/__init__.py
+-rw-r--r--   0        0        0     2921 2023-05-05 16:30:15.060753 netmiko-4.2.0/netmiko/adtran/adtran.py
+-rw-r--r--   0        0        0      221 2023-05-05 16:30:15.064753 netmiko-4.2.0/netmiko/adva/__init__.py
+-rw-r--r--   0        0        0     2067 2023-05-05 16:30:15.064753 netmiko-4.2.0/netmiko/adva/adva_aos_fsp_150_f2.py
+-rw-r--r--   0        0        0     4388 2023-05-05 16:30:15.064753 netmiko-4.2.0/netmiko/adva/adva_aos_fsp_150_f3.py
+-rw-r--r--   0        0        0       87 2022-03-15 19:38:09.086841 netmiko-4.2.0/netmiko/alcatel/__init__.py
+-rw-r--r--   0        0        0      836 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/alcatel/alcatel_aos_ssh.py
+-rw-r--r--   0        0        0      118 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/allied_telesis/__init__.py
+-rw-r--r--   0        0        0     1607 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/allied_telesis/allied_telesis_awplus.py
+-rw-r--r--   0        0        0      126 2022-03-15 19:38:09.086841 netmiko-4.2.0/netmiko/apresia/__init__.py
+-rw-r--r--   0        0        0     1409 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/apresia/apresia_aeos.py
+-rw-r--r--   0        0        0      141 2022-03-15 19:38:09.086841 netmiko-4.2.0/netmiko/arista/__init__.py
+-rw-r--r--   0        0        0     5584 2023-05-05 16:30:15.064753 netmiko-4.2.0/netmiko/arista/arista.py
+-rw-r--r--   0        0        0      105 2023-05-05 16:30:15.064753 netmiko-4.2.0/netmiko/arris/__init__.py
+-rw-r--r--   0        0        0      948 2023-05-05 16:30:15.064753 netmiko-4.2.0/netmiko/arris/arris_cer.py
+-rw-r--r--   0        0        0       69 2022-03-15 19:38:09.086841 netmiko-4.2.0/netmiko/aruba/__init__.py
+-rw-r--r--   0        0        0     1674 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/aruba/aruba_ssh.py
+-rw-r--r--   0        0        0      345 2022-08-09 21:16:34.346460 netmiko-4.2.0/netmiko/audiocode/__init__.py
+-rw-r--r--   0        0        0    16057 2023-05-05 16:30:15.068753 netmiko-4.2.0/netmiko/audiocode/audiocode_ssh.py
+-rw-r--r--   0        0        0    95124 2023-05-05 16:30:15.068753 netmiko-4.2.0/netmiko/base_connection.py
+-rw-r--r--   0        0        0       99 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/broadcom/__init__.py
+-rw-r--r--   0        0        0     1750 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/broadcom/broadcom_icos_ssh.py
+-rw-r--r--   0        0        0       87 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/brocade/__init__.py
+-rw-r--r--   0        0        0      563 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/brocade/brocade_fos_ssh.py
+-rw-r--r--   0        0        0      104 2022-03-15 19:38:09.086841 netmiko-4.2.0/netmiko/calix/__init__.py
+-rw-r--r--   0        0        0     3893 2022-07-11 18:53:23.699646 netmiko-4.2.0/netmiko/calix/calix_b6.py
+-rw-r--r--   0        0        0      104 2023-05-05 16:30:15.068753 netmiko-4.2.0/netmiko/casa/__init__.py
+-rw-r--r--   0        0        0     1963 2023-05-05 16:30:15.068753 netmiko-4.2.0/netmiko/casa/casa_cmts.py
+-rw-r--r--   0        0        0       78 2022-07-11 18:53:23.703646 netmiko-4.2.0/netmiko/cdot/__init__.py
+-rw-r--r--   0        0        0     4075 2022-08-09 21:16:34.350460 netmiko-4.2.0/netmiko/cdot/cdot_cros_ssh.py
+-rw-r--r--   0        0        0      110 2022-07-11 18:53:23.703646 netmiko-4.2.0/netmiko/centec/__init__.py
+-rw-r--r--   0        0        0      723 2022-07-11 18:53:23.703646 netmiko-4.2.0/netmiko/centec/centec_os.py
+-rw-r--r--   0        0        0     5619 2022-09-01 20:24:44.340067 netmiko-4.2.0/netmiko/channel.py
+-rw-r--r--   0        0        0      102 2022-03-15 19:38:09.086841 netmiko-4.2.0/netmiko/checkpoint/__init__.py
+-rw-r--r--   0        0        0      714 2022-07-11 18:53:23.703646 netmiko-4.2.0/netmiko/checkpoint/checkpoint_gaia_ssh.py
+-rw-r--r--   0        0        0      179 2022-03-15 19:38:09.090841 netmiko-4.2.0/netmiko/ciena/__init__.py
+-rw-r--r--   0        0        0     7927 2023-05-05 16:30:15.072753 netmiko-4.2.0/netmiko/ciena/ciena_saos.py
+-rw-r--r--   0        0        0     1356 2023-05-05 16:30:15.072753 netmiko-4.2.0/netmiko/cisco/__init__.py
+-rw-r--r--   0        0        0     6065 2023-05-05 16:30:15.072753 netmiko-4.2.0/netmiko/cisco/cisco_asa_ssh.py
+-rw-r--r--   0        0        0      849 2022-07-11 18:53:23.703646 netmiko-4.2.0/netmiko/cisco/cisco_ftd_ssh.py
+-rw-r--r--   0        0        0     9621 2022-07-11 18:53:23.703646 netmiko-4.2.0/netmiko/cisco/cisco_ios.py
+-rw-r--r--   0        0        0     6874 2022-07-11 18:53:23.703646 netmiko-4.2.0/netmiko/cisco/cisco_nxos_ssh.py
+-rw-r--r--   0        0        0     3186 2023-05-05 16:30:15.072753 netmiko-4.2.0/netmiko/cisco/cisco_s200.py
+-rw-r--r--   0        0        0     1190 2022-07-11 18:53:23.703646 netmiko-4.2.0/netmiko/cisco/cisco_s300.py
+-rw-r--r--   0        0        0     3214 2022-07-11 18:53:23.707646 netmiko-4.2.0/netmiko/cisco/cisco_tp_tcce.py
+-rw-r--r--   0        0        0     3143 2022-08-09 21:16:34.350460 netmiko-4.2.0/netmiko/cisco/cisco_viptela.py
+-rw-r--r--   0        0        0     8792 2023-05-05 16:30:15.072753 netmiko-4.2.0/netmiko/cisco/cisco_wlc_ssh.py
+-rw-r--r--   0        0        0     9936 2023-05-05 16:30:15.072753 netmiko-4.2.0/netmiko/cisco/cisco_xr.py
+-rw-r--r--   0        0        0    10259 2023-05-05 16:30:15.072753 netmiko-4.2.0/netmiko/cisco_base_connection.py
+-rw-r--r--   0        0        0       82 2022-03-15 19:38:09.094841 netmiko-4.2.0/netmiko/citrix/__init__.py
+-rw-r--r--   0        0        0     1574 2022-07-11 18:53:23.707646 netmiko-4.2.0/netmiko/citrix/netscaler_ssh.py
+-rw-r--r--   0        0        0        0 2022-07-11 18:53:23.707646 netmiko-4.2.0/netmiko/cli_tools/__init__.py
+-rwxr-xr-x   0        0        0     7508 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/cli_tools/netmiko_cfg.py
+-rwxr-xr-x   0        0        0     7580 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/cli_tools/netmiko_grep.py
+-rwxr-xr-x   0        0        0     7425 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/cli_tools/netmiko_show.py
+-rw-r--r--   0        0        0       95 2022-03-15 19:38:09.094841 netmiko-4.2.0/netmiko/cloudgenix/__init__.py
+-rw-r--r--   0        0        0     1889 2022-08-09 21:16:34.350460 netmiko-4.2.0/netmiko/cloudgenix/cloudgenix_ion.py
+-rw-r--r--   0        0        0       77 2022-03-15 19:38:09.094841 netmiko-4.2.0/netmiko/coriant/__init__.py
+-rw-r--r--   0        0        0     1049 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/coriant/coriant_ssh.py
+-rw-r--r--   0        0        0      693 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/dell/__init__.py
+-rw-r--r--   0        0        0      938 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/dell/dell_dnos6.py
+-rw-r--r--   0        0        0     1135 2023-05-05 16:30:15.076753 netmiko-4.2.0/netmiko/dell/dell_force10_ssh.py
+-rw-r--r--   0        0        0     3847 2023-05-05 16:30:15.076753 netmiko-4.2.0/netmiko/dell/dell_isilon_ssh.py
+-rw-r--r--   0        0        0     5496 2023-05-05 16:30:15.076753 netmiko-4.2.0/netmiko/dell/dell_os10_ssh.py
+-rw-r--r--   0        0        0     4030 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/dell/dell_powerconnect.py
+-rw-r--r--   0        0        0     1362 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/dell/dell_sonic_ssh.py
+-rw-r--r--   0        0        0      104 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/dlink/__init__.py
+-rw-r--r--   0        0        0     1407 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/dlink/dlink_ds.py
+-rw-r--r--   0        0        0      136 2022-03-15 19:38:09.094841 netmiko-4.2.0/netmiko/eltex/__init__.py
+-rw-r--r--   0        0        0     4193 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/eltex/eltex_esr_ssh.py
+-rw-r--r--   0        0        0      543 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/eltex/eltex_ssh.py
+-rw-r--r--   0        0        0       76 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/endace/__init__.py
+-rw-r--r--   0        0        0     2239 2023-05-05 16:30:15.076753 netmiko-4.2.0/netmiko/endace/endace_ssh.py
+-rw-r--r--   0        0        0       85 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/enterasys/__init__.py
+-rw-r--r--   0        0        0      543 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/enterasys/enterasys_ssh.py
+-rw-r--r--   0        0        0      228 2023-05-05 16:30:15.076753 netmiko-4.2.0/netmiko/ericsson/__init__.py
+-rw-r--r--   0        0        0     5128 2023-05-05 16:30:15.076753 netmiko-4.2.0/netmiko/ericsson/ericsson_ipos.py
+-rw-r--r--   0        0        0     5214 2023-05-05 16:30:15.076753 netmiko-4.2.0/netmiko/ericsson/ericsson_mltn.py
+-rw-r--r--   0        0        0     1309 2022-07-11 18:53:23.711646 netmiko-4.2.0/netmiko/exceptions.py
+-rw-r--r--   0        0        0      901 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/extreme/__init__.py
+-rw-r--r--   0        0        0     2512 2023-05-05 16:30:15.076753 netmiko-4.2.0/netmiko/extreme/extreme_ers_ssh.py
+-rw-r--r--   0        0        0     8186 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/extreme/extreme_exos.py
+-rw-r--r--   0        0        0     1063 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/extreme/extreme_netiron.py
+-rw-r--r--   0        0        0     1013 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/extreme/extreme_nos_ssh.py
+-rw-r--r--   0        0        0     1005 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/extreme/extreme_slx_ssh.py
+-rw-r--r--   0        0        0     1060 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/extreme/extreme_tierraos_ssh.py
+-rw-r--r--   0        0        0      763 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/extreme/extreme_vsp_ssh.py
+-rw-r--r--   0        0        0      441 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/extreme/extreme_wing_ssh.py
+-rw-r--r--   0        0        0      131 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/f5/__init__.py
+-rw-r--r--   0        0        0       84 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/f5/f5_linux_ssh.py
+-rw-r--r--   0        0        0     1375 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/f5/f5_tmsh_ssh.py
+-rw-r--r--   0        0        0       77 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/flexvnf/__init__.py
+-rw-r--r--   0        0        0     6996 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/flexvnf/flexvnf_ssh.py
+-rw-r--r--   0        0        0       81 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/fortinet/__init__.py
+-rw-r--r--   0        0        0     8045 2023-05-05 16:30:15.080753 netmiko-4.2.0/netmiko/fortinet/fortinet_ssh.py
+-rw-r--r--   0        0        0       95 2023-05-05 16:30:15.080753 netmiko-4.2.0/netmiko/hillstone/__init__.py
+-rw-r--r--   0        0        0     1423 2023-05-05 16:30:15.080753 netmiko-4.2.0/netmiko/hillstone/hillstone.py
+-rw-r--r--   0        0        0      215 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/hp/__init__.py
+-rw-r--r--   0        0        0     5380 2023-05-05 16:30:15.080753 netmiko-4.2.0/netmiko/hp/hp_comware.py
+-rw-r--r--   0        0        0     7954 2023-05-05 16:30:15.080753 netmiko-4.2.0/netmiko/hp/hp_procurve.py
+-rw-r--r--   0        0        0      245 2022-07-11 18:53:23.715646 netmiko-4.2.0/netmiko/huawei/__init__.py
+-rw-r--r--   0        0        0     9476 2023-05-05 16:30:15.080753 netmiko-4.2.0/netmiko/huawei/huawei.py
+-rw-r--r--   0        0        0     4610 2023-05-05 16:30:15.080753 netmiko-4.2.0/netmiko/huawei/huawei_smartax.py
+-rw-r--r--   0        0        0      162 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/ipinfusion/__init__.py
+-rw-r--r--   0        0        0     2789 2022-07-11 18:53:23.719646 netmiko-4.2.0/netmiko/ipinfusion/ipinfusion_ocnos.py
+-rw-r--r--   0        0        0      235 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/juniper/__init__.py
+-rw-r--r--   0        0        0    10722 2023-05-05 16:30:15.080753 netmiko-4.2.0/netmiko/juniper/juniper.py
+-rw-r--r--   0        0        0     1014 2022-07-11 18:53:23.719646 netmiko-4.2.0/netmiko/juniper/juniper_screenos.py
+-rw-r--r--   0        0        0      152 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/keymile/__init__.py
+-rw-r--r--   0        0        0     1414 2022-07-11 18:53:23.719646 netmiko-4.2.0/netmiko/keymile/keymile_nos_ssh.py
+-rw-r--r--   0        0        0     1453 2022-07-11 18:53:23.719646 netmiko-4.2.0/netmiko/keymile/keymile_ssh.py
+-rw-r--r--   0        0        0      109 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/linux/__init__.py
+-rw-r--r--   0        0        0     7896 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/linux/linux_ssh.py
+-rw-r--r--   0        0        0      100 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/mellanox/__init__.py
+-rw-r--r--   0        0        0     3090 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/mellanox/mellanox_mlnxos_ssh.py
+-rw-r--r--   0        0        0     1172 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/mikrotik/README.md
+-rw-r--r--   0        0        0      285 2022-07-11 18:53:23.719646 netmiko-4.2.0/netmiko/mikrotik/__init__.py
+-rw-r--r--   0        0        0    10708 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/mikrotik/mikrotik_ssh.py
+-rw-r--r--   0        0        0      133 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/mrv/__init__.py
+-rw-r--r--   0        0        0     1641 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/mrv/mrv_lx.py
+-rw-r--r--   0        0        0     1801 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/mrv/mrv_ssh.py
+-rw-r--r--   0        0        0       86 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/netapp/__init__.py
+-rw-r--r--   0        0        0     1473 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/netapp/netapp_cdot_ssh.py
+-rw-r--r--   0        0        0       99 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/netgear/__init__.py
+-rw-r--r--   0        0        0     1896 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/netgear/netgear_prosafe_ssh.py
+-rw-r--r--   0        0        0       43 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/netmiko_globals.py
+-rw-r--r--   0        0        0      844 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/no_config.py
+-rw-r--r--   0        0        0      987 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/no_enable.py
+-rwxr-xr-x   0        0        0      243 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/nokia/__init__.py
+-rw-r--r--   0        0        0     5814 2022-08-09 21:16:34.350460 netmiko-4.2.0/netmiko/nokia/nokia_srl.py
+-rw-r--r--   0        0        0    15328 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/nokia/nokia_sros.py
+-rw-r--r--   0        0        0      143 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/oneaccess/__init__.py
+-rw-r--r--   0        0        0     1542 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/oneaccess/oneaccess_oneos.py
+-rw-r--r--   0        0        0       77 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/ovs/__init__.py
+-rw-r--r--   0        0        0       85 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/ovs/ovs_linux_ssh.py
+-rw-r--r--   0        0        0      137 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/paloalto/__init__.py
+-rw-r--r--   0        0        0     8703 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/paloalto/paloalto_panos.py
+-rw-r--r--   0        0        0      106 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/pluribus/__init__.py
+-rw-r--r--   0        0        0      641 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/pluribus/pluribus_ssh.py
+-rw-r--r--   0        0        0       86 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/quanta/__init__.py
+-rw-r--r--   0        0        0      851 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/quanta/quanta_mesh_ssh.py
+-rw-r--r--   0        0        0      128 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/rad/__init__.py
+-rw-r--r--   0        0        0     3262 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/rad/rad_etx.py
+-rw-r--r--   0        0        0      174 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/raisecom/__init__.py
+-rw-r--r--   0        0        0     5851 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/raisecom/raisecom_roap.py
+-rw-r--r--   0        0        0      182 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/ruckus/__init__.py
+-rw-r--r--   0        0        0     3916 2023-05-05 16:30:15.084753 netmiko-4.2.0/netmiko/ruckus/ruckus_fastiron.py
+-rw-r--r--   0        0        0      110 2022-03-15 19:38:09.098841 netmiko-4.2.0/netmiko/ruijie/__init__.py
+-rw-r--r--   0        0        0     1298 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/ruijie/ruijie_os.py
+-rw-r--r--   0        0        0     5336 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/scp_functions.py
+-rw-r--r--   0        0        0    16161 2023-05-05 16:30:15.088753 netmiko-4.2.0/netmiko/scp_handler.py
+-rw-r--r--   0        0        0     2475 2023-05-05 16:30:15.088753 netmiko-4.2.0/netmiko/session_log.py
+-rw-r--r--   0        0        0       80 2022-07-11 18:53:23.723646 netmiko-4.2.0/netmiko/sixwind/__init__.py
+-rw-r--r--   0        0        0     3559 2023-05-05 16:30:15.088753 netmiko-4.2.0/netmiko/sixwind/sixwind_os.py
+-rw-r--r--   0        0        0    12105 2023-05-05 16:30:15.088753 netmiko-4.2.0/netmiko/snmp_autodetect.py
+-rw-r--r--   0        0        0       86 2022-07-11 18:53:23.727646 netmiko-4.2.0/netmiko/sophos/__init__.py
+-rw-r--r--   0        0        0     1212 2022-07-11 18:53:23.727646 netmiko-4.2.0/netmiko/sophos/sophos_sfos_ssh.py
+-rw-r--r--   0        0        0      343 2022-07-11 18:53:23.727646 netmiko-4.2.0/netmiko/ssh_auth.py
+-rw-r--r--   0        0        0    18323 2023-05-05 16:30:15.088753 netmiko-4.2.0/netmiko/ssh_autodetect.py
+-rwxr-xr-x   0        0        0    19082 2023-05-05 16:30:15.092754 netmiko-4.2.0/netmiko/ssh_dispatcher.py
+-rw-r--r--   0        0        0      138 2022-07-11 18:53:23.727646 netmiko-4.2.0/netmiko/supermicro/__init__.py
+-rw-r--r--   0        0        0     1275 2022-07-11 18:53:23.727646 netmiko-4.2.0/netmiko/supermicro/smci_smis.py
+-rw-r--r--   0        0        0      115 2023-05-05 16:30:15.092754 netmiko-4.2.0/netmiko/teldat/__init__.py
+-rw-r--r--   0        0        0     6799 2023-05-05 16:30:15.092754 netmiko-4.2.0/netmiko/teldat/teldat_cit.py
+-rw-r--r--   0        0        0      200 2022-03-15 19:38:09.102841 netmiko-4.2.0/netmiko/terminal_server/__init__.py
+-rw-r--r--   0        0        0      932 2023-05-05 16:30:15.092754 netmiko-4.2.0/netmiko/terminal_server/terminal_server.py
+-rw-r--r--   0        0        0      145 2022-07-11 18:53:23.727646 netmiko-4.2.0/netmiko/tplink/__init__.py
+-rw-r--r--   0        0        0     7111 2023-05-05 16:30:15.092754 netmiko-4.2.0/netmiko/tplink/tplink_jetstream.py
+-rw-r--r--   0        0        0      368 2023-05-05 16:30:15.092754 netmiko-4.2.0/netmiko/ubiquiti/__init__.py
+-rw-r--r--   0        0        0     2868 2022-07-11 18:53:23.727646 netmiko-4.2.0/netmiko/ubiquiti/edge_ssh.py
+-rw-r--r--   0        0        0     3214 2023-05-05 16:30:15.096753 netmiko-4.2.0/netmiko/ubiquiti/edgerouter_ssh.py
+-rw-r--r--   0        0        0     1318 2022-07-11 18:53:23.727646 netmiko-4.2.0/netmiko/ubiquiti/unifiswitch_ssh.py
+-rw-r--r--   0        0        0    21298 2022-08-09 21:16:34.350460 netmiko-4.2.0/netmiko/utilities.py
+-rw-r--r--   0        0        0       65 2022-03-15 19:38:09.102841 netmiko-4.2.0/netmiko/vyos/__init__.py
+-rw-r--r--   0        0        0     5106 2022-08-09 21:16:34.350460 netmiko-4.2.0/netmiko/vyos/vyos_ssh.py
+-rw-r--r--   0        0        0      103 2022-07-11 18:53:23.731646 netmiko-4.2.0/netmiko/watchguard/__init__.py
+-rw-r--r--   0        0        0     1435 2023-05-05 16:30:15.096753 netmiko-4.2.0/netmiko/watchguard/fireware_ssh.py
+-rw-r--r--   0        0        0      139 2022-07-11 18:53:23.731646 netmiko-4.2.0/netmiko/yamaha/__init__.py
+-rw-r--r--   0        0        0     3348 2023-05-05 16:30:15.096753 netmiko-4.2.0/netmiko/yamaha/yamaha.py
+-rw-r--r--   0        0        0      144 2022-07-11 18:53:23.731646 netmiko-4.2.0/netmiko/zte/__init__.py
+-rw-r--r--   0        0        0     2440 2022-07-11 18:53:23.731646 netmiko-4.2.0/netmiko/zte/zte_zxros.py
+-rw-r--r--   0        0        0       70 2022-07-11 18:53:23.731646 netmiko-4.2.0/netmiko/zyxel/__init__.py
+-rw-r--r--   0        0        0     1028 2022-08-09 21:16:34.350460 netmiko-4.2.0/netmiko/zyxel/zyxel_ssh.py
+-rw-r--r--   0        0        0     1445 2023-05-05 16:30:15.100753 netmiko-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8966 1970-01-01 00:00:00.000000 netmiko-4.2.0/setup.py
+-rw-r--r--   0        0        0     7544 1970-01-01 00:00:00.000000 netmiko-4.2.0/PKG-INFO
```

### Comparing `netmiko-4.1.2/LICENSE` & `netmiko-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/PKG-INFO` & `netmiko-4.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 Metadata-Version: 2.1
 Name: netmiko
-Version: 4.1.2
+Version: 4.2.0
 Summary: Multi-vendor library to simplify legacy CLI connections to network devices
 Home-page: https://github.com/ktbyers/netmiko
+License: MIT
 Author: Kirk Byers
 Author-email: ktbyers@twb-tech.com
-License: MIT
-Platform: UNKNOWN
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: ntc-templates (>=2.0.0)
+Requires-Dist: paramiko (>=2.9.5)
+Requires-Dist: pyserial (>=3.3)
+Requires-Dist: pyyaml (>=5.3)
+Requires-Dist: scp (>=0.13.6)
+Requires-Dist: textfsm (>=1.1.3)
+Project-URL: Repository, https://github.com/ktbyers/netmiko
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netmiko.svg)](https://img.shields.io/pypi/pyversions/netmiko)
 [![PyPI](https://img.shields.io/pypi/v/netmiko.svg)](https://pypi.python.org/pypi/netmiko)
 [![Downloads](https://pepy.tech/badge/netmiko)](https://pepy.tech/project/netmiko)
 [![GitHub contributors](https://img.shields.io/github/contributors/ktbyers/netmiko.svg)](https://GitHub.com/ktbyers/netmiko/graphs/contributors/)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
@@ -66,15 +78,15 @@
 $ pip install netmiko
 ```
 
 <br />
 
 ## API-Documentation
 
-[API-Documentation](https://ktbyers.github.io/netmiko/#api-documentation)
+[API-Documentation](https://ktbyers.github.io/netmiko/docs/netmiko/index.html)
 
 <br />
 
 ## Common Issues/FAQ
 
 Answers to some [common questions](COMMON_ISSUES.md)
 
@@ -184,8 +196,7 @@
 
 
 ---
 Kirk Byers  
 Python for Network Engineers  
 https://pynet.twb-tech.com  
 
-
```

### Comparing `netmiko-4.1.2/README.md` & `netmiko-4.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,306 +93,306 @@
 000005c0: 6060 600a 2420 7069 7020 696e 7374 616c  ```.$ pip instal
 000005d0: 6c20 6e65 746d 696b 6f0a 6060 600a 0a3c  l netmiko.```..<
 000005e0: 6272 202f 3e0a 0a23 2320 4150 492d 446f  br />..## API-Do
 000005f0: 6375 6d65 6e74 6174 696f 6e0a 0a5b 4150  cumentation..[AP
 00000600: 492d 446f 6375 6d65 6e74 6174 696f 6e5d  I-Documentation]
 00000610: 2868 7474 7073 3a2f 2f6b 7462 7965 7273  (https://ktbyers
 00000620: 2e67 6974 6875 622e 696f 2f6e 6574 6d69  .github.io/netmi
-00000630: 6b6f 2f23 6170 692d 646f 6375 6d65 6e74  ko/#api-document
-00000640: 6174 696f 6e29 0a0a 3c62 7220 2f3e 0a0a  ation)..<br />..
-00000650: 2323 2043 6f6d 6d6f 6e20 4973 7375 6573  ## Common Issues
-00000660: 2f46 4151 0a0a 416e 7377 6572 7320 746f  /FAQ..Answers to
-00000670: 2073 6f6d 6520 5b63 6f6d 6d6f 6e20 7175   some [common qu
-00000680: 6573 7469 6f6e 735d 2843 4f4d 4d4f 4e5f  estions](COMMON_
-00000690: 4953 5355 4553 2e6d 6429 0a0a 3c62 7220  ISSUES.md)..<br 
-000006a0: 2f3e 0a0a 2323 2320 5475 746f 7269 616c  />..### Tutorial
-000006b0: 730a 0a2d 205b 4e65 746d 696b 6f20 4f76  s..- [Netmiko Ov
-000006c0: 6572 7669 6577 5d28 6874 7470 733a 2f2f  erview](https://
-000006d0: 7079 6e65 742e 7477 622d 7465 6368 2e63  pynet.twb-tech.c
-000006e0: 6f6d 2f62 6c6f 672f 6175 746f 6d61 7469  om/blog/automati
-000006f0: 6f6e 2f6e 6574 6d69 6b6f 2e68 746d 6c29  on/netmiko.html)
-00000700: 0a2d 205b 5365 6375 7265 2043 6f70 795d  .- [Secure Copy]
-00000710: 2868 7474 7073 3a2f 2f70 796e 6574 2e74  (https://pynet.t
-00000720: 7762 2d74 6563 682e 636f 6d2f 626c 6f67  wb-tech.com/blog
-00000730: 2f61 7574 6f6d 6174 696f 6e2f 6e65 746d  /automation/netm
-00000740: 696b 6f2d 7363 702e 6874 6d6c 290a 2d20  iko-scp.html).- 
-00000750: 5b4e 6574 6d69 6b6f 2074 6872 6f75 6768  [Netmiko through
-00000760: 2053 5348 2050 726f 7879 5d28 6874 7470   SSH Proxy](http
-00000770: 733a 2f2f 7079 6e65 742e 7477 622d 7465  s://pynet.twb-te
-00000780: 6368 2e63 6f6d 2f62 6c6f 672f 6175 746f  ch.com/blog/auto
-00000790: 6d61 7469 6f6e 2f6e 6574 6d69 6b6f 2d70  mation/netmiko-p
-000007a0: 726f 7879 2e68 746d 6c29 0a2d 205b 4e65  roxy.html).- [Ne
-000007b0: 746d 696b 6f20 616e 6420 5465 7874 4653  tmiko and TextFS
-000007c0: 4d5d 2868 7474 7073 3a2f 2f70 796e 6574  M](https://pynet
-000007d0: 2e74 7762 2d74 6563 682e 636f 6d2f 626c  .twb-tech.com/bl
-000007e0: 6f67 2f61 7574 6f6d 6174 696f 6e2f 6e65  og/automation/ne
-000007f0: 746d 696b 6f2d 7465 7874 6673 6d2e 6874  tmiko-textfsm.ht
-00000800: 6d6c 290a 2d20 5b4e 6574 6d69 6b6f 2061  ml).- [Netmiko a
-00000810: 6e64 2077 6861 7420 636f 6e73 7469 7475  nd what constitu
-00000820: 7465 7320 646f 6e65 5d28 6874 7470 733a  tes done](https:
-00000830: 2f2f 7079 6e65 742e 7477 622d 7465 6368  //pynet.twb-tech
-00000840: 2e63 6f6d 2f62 6c6f 672f 6175 746f 6d61  .com/blog/automa
-00000850: 7469 6f6e 2f6e 6574 6d69 6b6f 2d77 6861  tion/netmiko-wha
-00000860: 742d 6973 2d64 6f6e 652e 6874 6d6c 290a  t-is-done.html).
-00000870: 0a3c 6272 202f 3e0a 0a23 2323 2047 6574  .<br />..### Get
-00000880: 7469 6e67 2053 7461 7274 6564 3a0a 0a23  ting Started:..#
-00000890: 2323 2320 4372 6561 7465 2061 2064 6963  ### Create a dic
-000008a0: 7469 6f6e 6172 7920 7265 7072 6573 656e  tionary represen
-000008b0: 7469 6e67 2074 6865 2064 6576 6963 652e  ting the device.
-000008c0: 0a0a 5375 7070 6f72 7465 6420 6465 7669  ..Supported devi
-000008d0: 6365 5f74 7970 6573 2063 616e 2062 6520  ce_types can be 
-000008e0: 666f 756e 6420 696e 205b 7373 685f 6469  found in [ssh_di
-000008f0: 7370 6174 6368 6572 2e70 795d 2868 7474  spatcher.py](htt
-00000900: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000910: 6b74 6279 6572 732f 6e65 746d 696b 6f2f  ktbyers/netmiko/
-00000920: 626c 6f62 2f6d 6173 7465 722f 6e65 746d  blob/master/netm
-00000930: 696b 6f2f 7373 685f 6469 7370 6174 6368  iko/ssh_dispatch
-00000940: 6572 2e70 7929 2c20 7365 6520 434c 4153  er.py), see CLAS
-00000950: 535f 4d41 5050 4552 206b 6579 732e 0a60  S_MAPPER keys..`
-00000960: 6060 7079 0a66 726f 6d20 6e65 746d 696b  ``py.from netmik
-00000970: 6f20 696d 706f 7274 2043 6f6e 6e65 6374  o import Connect
-00000980: 4861 6e64 6c65 720a 0a63 6973 636f 5f38  Handler..cisco_8
-00000990: 3831 203d 207b 0a20 2020 2027 6465 7669  81 = {.    'devi
-000009a0: 6365 5f74 7970 6527 3a20 2763 6973 636f  ce_type': 'cisco
-000009b0: 5f69 6f73 272c 0a20 2020 2027 686f 7374  _ios',.    'host
-000009c0: 273a 2020 2027 3130 2e31 302e 3130 2e31  ':   '10.10.10.1
-000009d0: 3027 2c0a 2020 2020 2775 7365 726e 616d  0',.    'usernam
-000009e0: 6527 3a20 2774 6573 7427 2c0a 2020 2020  e': 'test',.    
-000009f0: 2770 6173 7377 6f72 6427 3a20 2770 6173  'password': 'pas
-00000a00: 7377 6f72 6427 2c0a 2020 2020 2770 6f72  sword',.    'por
-00000a10: 7427 203a 2038 3032 322c 2020 2020 2020  t' : 8022,      
-00000a20: 2020 2020 2320 6f70 7469 6f6e 616c 2c20      # optional, 
-00000a30: 6465 6661 756c 7473 2074 6f20 3232 0a20  defaults to 22. 
-00000a40: 2020 2027 7365 6372 6574 273a 2027 7365     'secret': 'se
-00000a50: 6372 6574 272c 2020 2020 2023 206f 7074  cret',     # opt
-00000a60: 696f 6e61 6c2c 2064 6566 6175 6c74 7320  ional, defaults 
-00000a70: 746f 2027 270a 7d0a 0a60 6060 0a0a 2323  to ''.}..```..##
-00000a80: 2323 2045 7374 6162 6c69 7368 2061 6e20  ## Establish an 
-00000a90: 5353 4820 636f 6e6e 6563 7469 6f6e 2074  SSH connection t
-00000aa0: 6f20 7468 6520 6465 7669 6365 2062 7920  o the device by 
-00000ab0: 7061 7373 696e 6720 696e 2074 6865 2064  passing in the d
-00000ac0: 6576 6963 6520 6469 6374 696f 6e61 7279  evice dictionary
-00000ad0: 2e0a 0a60 6060 7079 0a6e 6574 5f63 6f6e  ...```py.net_con
-00000ae0: 6e65 6374 203d 2043 6f6e 6e65 6374 4861  nect = ConnectHa
-00000af0: 6e64 6c65 7228 2a2a 6369 7363 6f5f 3838  ndler(**cisco_88
-00000b00: 3129 0a60 6060 0a0a 2323 2323 2045 7865  1).```..#### Exe
-00000b10: 6375 7465 2073 686f 7720 636f 6d6d 616e  cute show comman
-00000b20: 6473 2e0a 0a60 6060 7079 0a6f 7574 7075  ds...```py.outpu
-00000b30: 7420 3d20 6e65 745f 636f 6e6e 6563 742e  t = net_connect.
-00000b40: 7365 6e64 5f63 6f6d 6d61 6e64 2827 7368  send_command('sh
-00000b50: 6f77 2069 7020 696e 7420 6272 6965 6627  ow ip int brief'
-00000b60: 290a 7072 696e 7428 6f75 7470 7574 290a  ).print(output).
-00000b70: 6060 600a 6060 600a 496e 7465 7266 6163  ```.```.Interfac
-00000b80: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-00000b90: 2020 2049 502d 4164 6472 6573 7320 2020     IP-Address   
-00000ba0: 2020 204f 4b3f 204d 6574 686f 6420 5374     OK? Method St
-00000bb0: 6174 7573 2020 2020 2020 2020 2020 2020  atus            
-00000bc0: 2020 2020 5072 6f74 6f63 6f6c 0a46 6173      Protocol.Fas
-00000bd0: 7445 7468 6572 6e65 7430 2020 2020 2020  tEthernet0      
-00000be0: 2020 2020 2020 2020 756e 6173 7369 676e          unassign
-00000bf0: 6564 2020 2020 2020 5945 5320 756e 7365  ed      YES unse
-00000c00: 7420 2064 6f77 6e20 2020 2020 2020 2020  t  down         
-00000c10: 2020 2020 2020 2020 2064 6f77 6e0a 4661           down.Fa
-00000c20: 7374 4574 6865 726e 6574 3120 2020 2020  stEthernet1     
-00000c30: 2020 2020 2020 2020 2075 6e61 7373 6967           unassig
-00000c40: 6e65 6420 2020 2020 2059 4553 2075 6e73  ned      YES uns
-00000c50: 6574 2020 646f 776e 2020 2020 2020 2020  et  down        
-00000c60: 2020 2020 2020 2020 2020 646f 776e 0a46            down.F
-00000c70: 6173 7445 7468 6572 6e65 7432 2020 2020  astEthernet2    
-00000c80: 2020 2020 2020 2020 2020 756e 6173 7369            unassi
-00000c90: 676e 6564 2020 2020 2020 5945 5320 756e  gned      YES un
-00000ca0: 7365 7420 2064 6f77 6e20 2020 2020 2020  set  down       
-00000cb0: 2020 2020 2020 2020 2020 2064 6f77 6e0a             down.
-00000cc0: 4661 7374 4574 6865 726e 6574 3320 2020  FastEthernet3   
-00000cd0: 2020 2020 2020 2020 2020 2075 6e61 7373             unass
-00000ce0: 6967 6e65 6420 2020 2020 2059 4553 2075  igned      YES u
-00000cf0: 6e73 6574 2020 646f 776e 2020 2020 2020  nset  down      
-00000d00: 2020 2020 2020 2020 2020 2020 646f 776e              down
-00000d10: 0a46 6173 7445 7468 6572 6e65 7434 2020  .FastEthernet4  
-00000d20: 2020 2020 2020 2020 2020 2020 3130 2e31              10.1
-00000d30: 302e 3130 2e31 3020 2020 2020 5945 5320  0.10.10     YES 
-00000d40: 6d61 6e75 616c 2075 7020 2020 2020 2020  manual up       
-00000d50: 2020 2020 2020 2020 2020 2020 2075 700a               up.
-00000d60: 566c 616e 3120 2020 2020 2020 2020 2020  Vlan1           
-00000d70: 2020 2020 2020 2020 2020 2075 6e61 7373             unass
-00000d80: 6967 6e65 6420 2020 2020 2059 4553 2075  igned      YES u
-00000d90: 6e73 6574 2020 646f 776e 2020 2020 2020  nset  down      
-00000da0: 2020 2020 2020 2020 2020 2020 646f 776e              down
-00000db0: 0a60 6060 0a0a 2323 2323 2045 7865 6375  .```..#### Execu
-00000dc0: 7465 2063 6f6e 6669 6775 7261 7469 6f6e  te configuration
-00000dd0: 2063 6861 6e67 6520 636f 6d6d 616e 6473   change commands
-00000de0: 2028 7769 6c6c 2061 7574 6f6d 6174 6963   (will automatic
-00000df0: 616c 6c79 2065 6e74 6572 2069 6e74 6f20  ally enter into 
-00000e00: 636f 6e66 6967 206d 6f64 6529 0a0a 6060  config mode)..``
-00000e10: 6070 790a 636f 6e66 6967 5f63 6f6d 6d61  `py.config_comma
-00000e20: 6e64 7320 3d20 5b20 276c 6f67 6769 6e67  nds = [ 'logging
-00000e30: 2062 7566 6665 7265 6420 3230 3030 3027   buffered 20000'
-00000e40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000e50: 2020 2020 2020 276c 6f67 6769 6e67 2062        'logging b
-00000e60: 7566 6665 7265 6420 3230 3031 3027 2c0a  uffered 20010',.
-00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e80: 2020 2020 276e 6f20 6c6f 6767 696e 6720      'no logging 
-00000e90: 636f 6e73 6f6c 6527 205d 0a6f 7574 7075  console' ].outpu
-00000ea0: 7420 3d20 6e65 745f 636f 6e6e 6563 742e  t = net_connect.
-00000eb0: 7365 6e64 5f63 6f6e 6669 675f 7365 7428  send_config_set(
-00000ec0: 636f 6e66 6967 5f63 6f6d 6d61 6e64 7329  config_commands)
-00000ed0: 0a70 7269 6e74 286f 7574 7075 7429 0a60  .print(output).`
-00000ee0: 6060 0a60 6060 0a70 796e 6574 2d72 7472  ``.```.pynet-rtr
-00000ef0: 3123 636f 6e66 6967 2074 6572 6d0a 456e  1#config term.En
-00000f00: 7465 7220 636f 6e66 6967 7572 6174 696f  ter configuratio
-00000f10: 6e20 636f 6d6d 616e 6473 2c20 6f6e 6520  n commands, one 
-00000f20: 7065 7220 6c69 6e65 2e20 2045 6e64 2077  per line.  End w
-00000f30: 6974 6820 434e 544c 2f5a 2e0a 7079 6e65  ith CNTL/Z..pyne
-00000f40: 742d 7274 7231 2863 6f6e 6669 6729 236c  t-rtr1(config)#l
-00000f50: 6f67 6769 6e67 2062 7566 6665 7265 6420  ogging buffered 
-00000f60: 3230 3030 300a 7079 6e65 742d 7274 7231  20000.pynet-rtr1
-00000f70: 2863 6f6e 6669 6729 236c 6f67 6769 6e67  (config)#logging
-00000f80: 2062 7566 6665 7265 6420 3230 3031 300a   buffered 20010.
-00000f90: 7079 6e65 742d 7274 7231 2863 6f6e 6669  pynet-rtr1(confi
-00000fa0: 6729 236e 6f20 6c6f 6767 696e 6720 636f  g)#no logging co
-00000fb0: 6e73 6f6c 650a 7079 6e65 742d 7274 7231  nsole.pynet-rtr1
-00000fc0: 2863 6f6e 6669 6729 2365 6e64 0a70 796e  (config)#end.pyn
-00000fd0: 6574 2d72 7472 3123 0a60 6060 0a0a 3c62  et-rtr1#.```..<b
-00000fe0: 7220 2f3e 0a0a 2323 2041 5049 2d44 6f63  r />..## API-Doc
-00000ff0: 756d 656e 7461 7469 6f6e 0a0a 3c61 2068  umentation..<a h
-00001000: 7265 663d 2268 7474 7073 3a2f 2f6b 7462  ref="https://ktb
-00001010: 7965 7273 2e67 6974 6875 622e 696f 2f6e  yers.github.io/n
-00001020: 6574 6d69 6b6f 2f64 6f63 732f 6e65 746d  etmiko/docs/netm
-00001030: 696b 6f2f 696e 6465 782e 6874 6d6c 2220  iko/index.html" 
-00001040: 7469 746c 653d 2244 6f63 7322 3e41 5049  title="Docs">API
-00001050: 2044 6f63 756d 656e 7461 7469 6f6e 3c2f   Documentation</
-00001060: 613e 0a0a 4265 6c6f 7720 6172 6520 736f  a>..Below are so
-00001070: 6d65 206f 6620 7468 6520 7061 7274 6963  me of the partic
-00001080: 756c 6172 6c79 2068 616e 6479 2043 6c61  ularly handy Cla
-00001090: 7373 6573 2f66 756e 6374 696f 6e73 2066  sses/functions f
-000010a0: 6f72 2065 6173 7920 7265 6665 7265 6e63  or easy referenc
-000010b0: 653a 0a2d 205b 4261 7365 2043 6f6e 6e65  e:.- [Base Conne
-000010c0: 6374 696f 6e20 4f62 6a65 6374 5d28 6874  ction Object](ht
-000010d0: 7470 733a 2f2f 6b74 6279 6572 732e 6769  tps://ktbyers.gi
-000010e0: 7468 7562 2e69 6f2f 6e65 746d 696b 6f2f  thub.io/netmiko/
-000010f0: 646f 6373 2f6e 6574 6d69 6b6f 2f62 6173  docs/netmiko/bas
-00001100: 655f 636f 6e6e 6563 7469 6f6e 2e68 746d  e_connection.htm
-00001110: 6c29 0a2d 205b 5353 4820 4175 746f 6465  l).- [SSH Autode
-00001120: 7465 6374 5d28 6874 7470 733a 2f2f 6b74  tect](https://kt
-00001130: 6279 6572 732e 6769 7468 7562 2e69 6f2f  byers.github.io/
-00001140: 6e65 746d 696b 6f2f 646f 6373 2f6e 6574  netmiko/docs/net
-00001150: 6d69 6b6f 2f69 6e64 6578 2e68 746d 6c23  miko/index.html#
-00001160: 6e65 746d 696b 6f2e 5353 4844 6574 6563  netmiko.SSHDetec
-00001170: 7429 0a2d 205b 5353 4820 4469 7370 6174  t).- [SSH Dispat
-00001180: 6368 6572 5d28 6874 7470 733a 2f2f 6b74  cher](https://kt
-00001190: 6279 6572 732e 6769 7468 7562 2e69 6f2f  byers.github.io/
-000011a0: 6e65 746d 696b 6f2f 646f 6373 2f6e 6574  netmiko/docs/net
-000011b0: 6d69 6b6f 2f69 6e64 6578 2e68 746d 6c23  miko/index.html#
-000011c0: 6e65 746d 696b 6f2e 7373 685f 6469 7370  netmiko.ssh_disp
-000011d0: 6174 6368 6572 290a 2d20 5b52 6564 6973  atcher).- [Redis
-000011e0: 7061 7463 685d 2868 7474 7073 3a2f 2f6b  patch](https://k
-000011f0: 7462 7965 7273 2e67 6974 6875 622e 696f  tbyers.github.io
-00001200: 2f6e 6574 6d69 6b6f 2f64 6f63 732f 6e65  /netmiko/docs/ne
-00001210: 746d 696b 6f2f 696e 6465 782e 6874 6d6c  tmiko/index.html
-00001220: 236e 6574 6d69 6b6f 2e72 6564 6973 7061  #netmiko.redispa
-00001230: 7463 6829 0a0a 3c62 7220 2f3e 0a0a 2323  tch)..<br />..##
-00001240: 2043 6f6e 7472 6962 7574 696e 670a 0a43   Contributing..C
-00001250: 6f6e 7472 6962 7574 6f72 7320 6172 6520  ontributors are 
-00001260: 7765 6c63 6f6d 652e 0a0a 596f 7520 6361  welcome...You ca
-00001270: 6e20 636f 6e74 7269 6275 7465 2074 6f20  n contribute to 
-00001280: 4e65 746d 696b 6f20 696e 2061 2076 6172  Netmiko in a var
-00001290: 6965 7479 206f 6620 7761 7973 3a20 616e  iety of ways: an
-000012a0: 7377 6572 696e 6720 7175 6573 7469 6f6e  swering question
-000012b0: 7320 6f6e 2053 6c61 636b 2028 7365 6520  s on Slack (see 
-000012c0: 6265 6c6f 7720 696e 2051 7565 7374 696f  below in Questio
-000012d0: 6e73 2f44 6973 6375 7373 696f 6e73 292c  ns/Discussions),
-000012e0: 2072 6573 706f 6e64 696e 6720 746f 2069   responding to i
-000012f0: 7373 7565 732c 2061 6464 696e 6720 746f  ssues, adding to
-00001300: 2074 6865 2063 6f6d 6d6f 6e20 6973 7375   the common issu
-00001310: 6573 2c20 7265 706f 7274 696e 672f 6669  es, reporting/fi
-00001320: 7869 6e67 2062 7567 732c 206f 7220 6576  xing bugs, or ev
-00001330: 656e 2061 6464 696e 6720 796f 7572 206f  en adding your o
-00001340: 776e 2064 6576 6963 6520 7479 7065 2e0a  wn device type..
-00001350: 0a42 6566 6f72 6520 636f 6e74 7269 6275  .Before contribu
-00001360: 7469 6e67 2061 206e 6577 2076 656e 646f  ting a new vendo
-00001370: 722f 706c 6174 666f 726d 2064 6576 6963  r/platform devic
-00001380: 6520 7479 7065 2c20 7265 6d65 6d62 6572  e type, remember
-00001390: 2074 6861 7420 616e 7920 636f 6465 2061   that any code a
-000013a0: 6464 6564 206e 6565 6473 2074 6f20 6265  dded needs to be
-000013b0: 2073 7570 706f 7274 6564 2069 6e20 736f   supported in so
-000013c0: 6d65 2066 6173 6869 6f6e 2e20 546f 2061  me fashion. To a
-000013d0: 6464 2061 2076 656e 646f 722f 706c 6174  dd a vendor/plat
-000013e0: 666f 726d 2079 6f75 2063 616e 2066 6f6c  form you can fol
-000013f0: 6c6f 7720 7468 6520 6f75 746c 696e 6520  low the outline 
-00001400: 5b68 6572 655d 2856 454e 444f 522e 6d64  [here](VENDOR.md
-00001410: 292e 204f 6e63 6520 796f 7527 7665 2077  ). Once you've w
-00001420: 6f72 6b65 6420 6f6e 2079 6f75 7220 6669  orked on your fi
-00001430: 7273 7420 7061 7373 206f 6620 796f 7572  rst pass of your
-00001440: 2064 7269 7665 7220 616e 6420 6861 7665   driver and have
-00001450: 2069 7420 6675 6e63 7469 6f6e 616c 2c20   it functional, 
-00001460: 796f 7527 6c6c 206e 6565 6420 746f 2069  you'll need to i
-00001470: 6e63 6c75 6465 2074 6573 7420 6461 7461  nclude test data
-00001480: 2069 6e20 6f72 6465 7220 666f 7220 6974   in order for it
-00001490: 2074 6f20 6265 206d 6572 6765 6420 696e   to be merged in
-000014a0: 746f 2064 6576 656c 6f70 2c20 796f 7520  to develop, you 
-000014b0: 6361 6e20 7365 6520 7468 6520 6765 6e65  can see the gene
-000014c0: 7261 6c20 666c 6f77 206f 6620 686f 7720  ral flow of how 
-000014d0: 746f 2064 6f20 7468 6174 205b 6865 7265  to do that [here
-000014e0: 5d28 5445 5354 494e 472e 6d64 292e 0a0a  ](TESTING.md)...
-000014f0: 466f 7220 616c 6c20 636f 6465 2063 6f6e  For all code con
-00001500: 7472 6962 7574 696f 6e73 2c20 706c 6561  tributions, plea
-00001510: 7365 2065 6e73 7572 6520 7468 6174 2079  se ensure that y
-00001520: 6f75 2068 6176 6520 7261 6e20 6062 6c61  ou have ran `bla
-00001530: 636b 6020 6167 6169 6e73 7420 7468 6520  ck` against the 
-00001540: 636f 6465 206f 7220 796f 7572 2063 6f64  code or your cod
-00001550: 6520 7769 6c6c 2066 6169 6c20 7468 6520  e will fail the 
-00001560: 5472 6176 6973 2043 4920 6275 696c 642e  Travis CI build.
-00001570: 0a0a 3c62 7220 2f3e 0a0a 2323 2051 7565  ..<br />..## Que
-00001580: 7374 696f 6e73 2f44 6973 6375 7373 696f  stions/Discussio
-00001590: 6e0a 0a49 6620 796f 7520 6669 6e64 2061  n..If you find a
-000015a0: 6e20 6973 7375 6520 7769 7468 204e 6574  n issue with Net
-000015b0: 6d69 6b6f 2c20 7468 656e 2079 6f75 2063  miko, then you c
-000015c0: 616e 206f 7065 6e20 616e 2069 7373 7565  an open an issue
-000015d0: 206f 6e20 7468 6973 2070 726f 6a65 6374   on this project
-000015e0: 7320 6973 7375 6520 7061 6765 2068 6572  s issue page her
-000015f0: 653a 205b 6874 7470 733a 2f2f 6769 7468  e: [https://gith
-00001600: 7562 2e63 6f6d 2f6b 7462 7965 7273 2f6e  ub.com/ktbyers/n
-00001610: 6574 6d69 6b6f 2f69 7373 7565 735d 2868  etmiko/issues](h
-00001620: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001630: 6d2f 6b74 6279 6572 732f 6e65 746d 696b  m/ktbyers/netmik
-00001640: 6f2f 6973 7375 6573 292e 2050 6c65 6173  o/issues). Pleas
-00001650: 6520 6d61 6b65 2073 7572 6520 796f 7527  e make sure you'
-00001660: 7665 2072 6561 6420 7468 726f 7567 6820  ve read through 
-00001670: 7468 6520 636f 6d6d 6f6e 2069 7373 7565  the common issue
-00001680: 7320 616e 6420 6578 616d 706c 6573 2070  s and examples p
-00001690: 7269 6f72 2074 6f20 6f70 656e 696e 6720  rior to opening 
-000016a0: 616e 2069 7373 7565 2e20 506c 6561 7365  an issue. Please
-000016b0: 206f 6e6c 7920 6f70 656e 2069 7373 7565   only open issue
-000016c0: 7320 666f 7220 6275 6773 2c20 6665 6174  s for bugs, feat
-000016d0: 7572 6520 7265 7175 6573 7473 2c20 6f72  ure requests, or
-000016e0: 206f 7468 6572 2074 6f70 6963 7320 7265   other topics re
-000016f0: 6c61 7465 6420 746f 2064 6576 656c 6f70  lated to develop
-00001700: 6d65 6e74 206f 6620 4e65 746d 696b 6f2e  ment of Netmiko.
-00001710: 2049 6620 796f 7520 7369 6d70 6c79 2068   If you simply h
-00001720: 6176 6520 6120 7175 6573 7469 6f6e 2c20  ave a question, 
-00001730: 6a6f 696e 2075 7320 6f6e 2053 6c61 636b  join us on Slack
-00001740: 2e2e 2e0a 0a49 6620 796f 7520 6861 7665  .....If you have
-00001750: 2071 7565 7374 696f 6e73 206f 7220 776f   questions or wo
-00001760: 756c 6420 6c69 6b65 2074 6f20 6469 7363  uld like to disc
-00001770: 7573 7320 4e65 746d 696b 6f2c 2061 2023  uss Netmiko, a #
-00001780: 6e65 746d 696b 6f20 6368 616e 6e65 6c20  netmiko channel 
-00001790: 6578 6973 7473 2069 6e20 5b74 6869 7320  exists in [this 
-000017a0: 536c 6163 6b5d 2868 7474 7073 3a2f 2f70  Slack](https://p
-000017b0: 796e 6574 2e73 6c61 636b 2e63 6f6d 2920  ynet.slack.com) 
-000017c0: 776f 726b 7370 6163 652e 2054 6f20 6a6f  workspace. To jo
-000017d0: 696e 2c20 7573 6520 5b74 6869 7320 696e  in, use [this in
-000017e0: 7669 7461 7469 6f6e 5d28 6874 7470 733a  vitation](https:
-000017f0: 2f2f 6a6f 696e 2e73 6c61 636b 2e63 6f6d  //join.slack.com
-00001800: 2f74 2f70 796e 6574 2f73 6861 7265 645f  /t/pynet/shared_
-00001810: 696e 7669 7465 2f7a 742d 6b6d 326b 3375  invite/zt-km2k3u
-00001820: 7066 2d41 6b57 4859 3459 4578 3373 4931  pf-AkWHY4YEx3sI1
-00001830: 5235 6972 4d6d 6337 5129 2e20 4f6e 6365  R5irMmc7Q). Once
-00001840: 2079 6f75 2068 6176 6520 656e 7465 7265   you have entere
-00001850: 6420 7468 6520 776f 726b 7370 6163 652c  d the workspace,
-00001860: 2074 6865 6e20 796f 7520 6361 6e20 6a6f   then you can jo
-00001870: 696e 2074 6865 2023 6e65 746d 696b 6f20  in the #netmiko 
-00001880: 6368 616e 6e65 6c2e 0a0a 0a2d 2d2d 0a4b  channel....---.K
-00001890: 6972 6b20 4279 6572 7320 200a 5079 7468  irk Byers  .Pyth
-000018a0: 6f6e 2066 6f72 204e 6574 776f 726b 2045  on for Network E
-000018b0: 6e67 696e 6565 7273 2020 0a68 7474 7073  ngineers  .https
-000018c0: 3a2f 2f70 796e 6574 2e74 7762 2d74 6563  ://pynet.twb-tec
-000018d0: 682e 636f 6d20 200a                      h.com  .
+00000630: 6b6f 2f64 6f63 732f 6e65 746d 696b 6f2f  ko/docs/netmiko/
+00000640: 696e 6465 782e 6874 6d6c 290a 0a3c 6272  index.html)..<br
+00000650: 202f 3e0a 0a23 2320 436f 6d6d 6f6e 2049   />..## Common I
+00000660: 7373 7565 732f 4641 510a 0a41 6e73 7765  ssues/FAQ..Answe
+00000670: 7273 2074 6f20 736f 6d65 205b 636f 6d6d  rs to some [comm
+00000680: 6f6e 2071 7565 7374 696f 6e73 5d28 434f  on questions](CO
+00000690: 4d4d 4f4e 5f49 5353 5545 532e 6d64 290a  MMON_ISSUES.md).
+000006a0: 0a3c 6272 202f 3e0a 0a23 2323 2054 7574  .<br />..### Tut
+000006b0: 6f72 6961 6c73 0a0a 2d20 5b4e 6574 6d69  orials..- [Netmi
+000006c0: 6b6f 204f 7665 7276 6965 775d 2868 7474  ko Overview](htt
+000006d0: 7073 3a2f 2f70 796e 6574 2e74 7762 2d74  ps://pynet.twb-t
+000006e0: 6563 682e 636f 6d2f 626c 6f67 2f61 7574  ech.com/blog/aut
+000006f0: 6f6d 6174 696f 6e2f 6e65 746d 696b 6f2e  omation/netmiko.
+00000700: 6874 6d6c 290a 2d20 5b53 6563 7572 6520  html).- [Secure 
+00000710: 436f 7079 5d28 6874 7470 733a 2f2f 7079  Copy](https://py
+00000720: 6e65 742e 7477 622d 7465 6368 2e63 6f6d  net.twb-tech.com
+00000730: 2f62 6c6f 672f 6175 746f 6d61 7469 6f6e  /blog/automation
+00000740: 2f6e 6574 6d69 6b6f 2d73 6370 2e68 746d  /netmiko-scp.htm
+00000750: 6c29 0a2d 205b 4e65 746d 696b 6f20 7468  l).- [Netmiko th
+00000760: 726f 7567 6820 5353 4820 5072 6f78 795d  rough SSH Proxy]
+00000770: 2868 7474 7073 3a2f 2f70 796e 6574 2e74  (https://pynet.t
+00000780: 7762 2d74 6563 682e 636f 6d2f 626c 6f67  wb-tech.com/blog
+00000790: 2f61 7574 6f6d 6174 696f 6e2f 6e65 746d  /automation/netm
+000007a0: 696b 6f2d 7072 6f78 792e 6874 6d6c 290a  iko-proxy.html).
+000007b0: 2d20 5b4e 6574 6d69 6b6f 2061 6e64 2054  - [Netmiko and T
+000007c0: 6578 7446 534d 5d28 6874 7470 733a 2f2f  extFSM](https://
+000007d0: 7079 6e65 742e 7477 622d 7465 6368 2e63  pynet.twb-tech.c
+000007e0: 6f6d 2f62 6c6f 672f 6175 746f 6d61 7469  om/blog/automati
+000007f0: 6f6e 2f6e 6574 6d69 6b6f 2d74 6578 7466  on/netmiko-textf
+00000800: 736d 2e68 746d 6c29 0a2d 205b 4e65 746d  sm.html).- [Netm
+00000810: 696b 6f20 616e 6420 7768 6174 2063 6f6e  iko and what con
+00000820: 7374 6974 7574 6573 2064 6f6e 655d 2868  stitutes done](h
+00000830: 7474 7073 3a2f 2f70 796e 6574 2e74 7762  ttps://pynet.twb
+00000840: 2d74 6563 682e 636f 6d2f 626c 6f67 2f61  -tech.com/blog/a
+00000850: 7574 6f6d 6174 696f 6e2f 6e65 746d 696b  utomation/netmik
+00000860: 6f2d 7768 6174 2d69 732d 646f 6e65 2e68  o-what-is-done.h
+00000870: 746d 6c29 0a0a 3c62 7220 2f3e 0a0a 2323  tml)..<br />..##
+00000880: 2320 4765 7474 696e 6720 5374 6172 7465  # Getting Starte
+00000890: 643a 0a0a 2323 2323 2043 7265 6174 6520  d:..#### Create 
+000008a0: 6120 6469 6374 696f 6e61 7279 2072 6570  a dictionary rep
+000008b0: 7265 7365 6e74 696e 6720 7468 6520 6465  resenting the de
+000008c0: 7669 6365 2e0a 0a53 7570 706f 7274 6564  vice...Supported
+000008d0: 2064 6576 6963 655f 7479 7065 7320 6361   device_types ca
+000008e0: 6e20 6265 2066 6f75 6e64 2069 6e20 5b73  n be found in [s
+000008f0: 7368 5f64 6973 7061 7463 6865 722e 7079  sh_dispatcher.py
+00000900: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000910: 2e63 6f6d 2f6b 7462 7965 7273 2f6e 6574  .com/ktbyers/net
+00000920: 6d69 6b6f 2f62 6c6f 622f 6d61 7374 6572  miko/blob/master
+00000930: 2f6e 6574 6d69 6b6f 2f73 7368 5f64 6973  /netmiko/ssh_dis
+00000940: 7061 7463 6865 722e 7079 292c 2073 6565  patcher.py), see
+00000950: 2043 4c41 5353 5f4d 4150 5045 5220 6b65   CLASS_MAPPER ke
+00000960: 7973 2e0a 6060 6070 790a 6672 6f6d 206e  ys..```py.from n
+00000970: 6574 6d69 6b6f 2069 6d70 6f72 7420 436f  etmiko import Co
+00000980: 6e6e 6563 7448 616e 646c 6572 0a0a 6369  nnectHandler..ci
+00000990: 7363 6f5f 3838 3120 3d20 7b0a 2020 2020  sco_881 = {.    
+000009a0: 2764 6576 6963 655f 7479 7065 273a 2027  'device_type': '
+000009b0: 6369 7363 6f5f 696f 7327 2c0a 2020 2020  cisco_ios',.    
+000009c0: 2768 6f73 7427 3a20 2020 2731 302e 3130  'host':   '10.10
+000009d0: 2e31 302e 3130 272c 0a20 2020 2027 7573  .10.10',.    'us
+000009e0: 6572 6e61 6d65 273a 2027 7465 7374 272c  ername': 'test',
+000009f0: 0a20 2020 2027 7061 7373 776f 7264 273a  .    'password':
+00000a00: 2027 7061 7373 776f 7264 272c 0a20 2020   'password',.   
+00000a10: 2027 706f 7274 2720 3a20 3830 3232 2c20   'port' : 8022, 
+00000a20: 2020 2020 2020 2020 2023 206f 7074 696f           # optio
+00000a30: 6e61 6c2c 2064 6566 6175 6c74 7320 746f  nal, defaults to
+00000a40: 2032 320a 2020 2020 2773 6563 7265 7427   22.    'secret'
+00000a50: 3a20 2773 6563 7265 7427 2c20 2020 2020  : 'secret',     
+00000a60: 2320 6f70 7469 6f6e 616c 2c20 6465 6661  # optional, defa
+00000a70: 756c 7473 2074 6f20 2727 0a7d 0a0a 6060  ults to ''.}..``
+00000a80: 600a 0a23 2323 2320 4573 7461 626c 6973  `..#### Establis
+00000a90: 6820 616e 2053 5348 2063 6f6e 6e65 6374  h an SSH connect
+00000aa0: 696f 6e20 746f 2074 6865 2064 6576 6963  ion to the devic
+00000ab0: 6520 6279 2070 6173 7369 6e67 2069 6e20  e by passing in 
+00000ac0: 7468 6520 6465 7669 6365 2064 6963 7469  the device dicti
+00000ad0: 6f6e 6172 792e 0a0a 6060 6070 790a 6e65  onary...```py.ne
+00000ae0: 745f 636f 6e6e 6563 7420 3d20 436f 6e6e  t_connect = Conn
+00000af0: 6563 7448 616e 646c 6572 282a 2a63 6973  ectHandler(**cis
+00000b00: 636f 5f38 3831 290a 6060 600a 0a23 2323  co_881).```..###
+00000b10: 2320 4578 6563 7574 6520 7368 6f77 2063  # Execute show c
+00000b20: 6f6d 6d61 6e64 732e 0a0a 6060 6070 790a  ommands...```py.
+00000b30: 6f75 7470 7574 203d 206e 6574 5f63 6f6e  output = net_con
+00000b40: 6e65 6374 2e73 656e 645f 636f 6d6d 616e  nect.send_comman
+00000b50: 6428 2773 686f 7720 6970 2069 6e74 2062  d('show ip int b
+00000b60: 7269 6566 2729 0a70 7269 6e74 286f 7574  rief').print(out
+00000b70: 7075 7429 0a60 6060 0a60 6060 0a49 6e74  put).```.```.Int
+00000b80: 6572 6661 6365 2020 2020 2020 2020 2020  erface          
+00000b90: 2020 2020 2020 2020 4950 2d41 6464 7265          IP-Addre
+00000ba0: 7373 2020 2020 2020 4f4b 3f20 4d65 7468  ss      OK? Meth
+00000bb0: 6f64 2053 7461 7475 7320 2020 2020 2020  od Status       
+00000bc0: 2020 2020 2020 2020 2050 726f 746f 636f           Protoco
+00000bd0: 6c0a 4661 7374 4574 6865 726e 6574 3020  l.FastEthernet0 
+00000be0: 2020 2020 2020 2020 2020 2020 2075 6e61               una
+00000bf0: 7373 6967 6e65 6420 2020 2020 2059 4553  ssigned      YES
+00000c00: 2075 6e73 6574 2020 646f 776e 2020 2020   unset  down    
+00000c10: 2020 2020 2020 2020 2020 2020 2020 646f                do
+00000c20: 776e 0a46 6173 7445 7468 6572 6e65 7431  wn.FastEthernet1
+00000c30: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00000c40: 6173 7369 676e 6564 2020 2020 2020 5945  assigned      YE
+00000c50: 5320 756e 7365 7420 2064 6f77 6e20 2020  S unset  down   
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00000c70: 6f77 6e0a 4661 7374 4574 6865 726e 6574  own.FastEthernet
+00000c80: 3220 2020 2020 2020 2020 2020 2020 2075  2              u
+00000c90: 6e61 7373 6967 6e65 6420 2020 2020 2059  nassigned      Y
+00000ca0: 4553 2075 6e73 6574 2020 646f 776e 2020  ES unset  down  
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 646f 776e 0a46 6173 7445 7468 6572 6e65  down.FastEtherne
+00000cd0: 7433 2020 2020 2020 2020 2020 2020 2020  t3              
+00000ce0: 756e 6173 7369 676e 6564 2020 2020 2020  unassigned      
+00000cf0: 5945 5320 756e 7365 7420 2064 6f77 6e20  YES unset  down 
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2064 6f77 6e0a 4661 7374 4574 6865 726e   down.FastEthern
+00000d20: 6574 3420 2020 2020 2020 2020 2020 2020  et4             
+00000d30: 2031 302e 3130 2e31 302e 3130 2020 2020   10.10.10.10    
+00000d40: 2059 4553 206d 616e 7561 6c20 7570 2020   YES manual up  
+00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d60: 2020 7570 0a56 6c61 6e31 2020 2020 2020    up.Vlan1      
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 756e 6173 7369 676e 6564 2020 2020 2020  unassigned      
+00000d90: 5945 5320 756e 7365 7420 2064 6f77 6e20  YES unset  down 
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2064 6f77 6e0a 6060 600a 0a23 2323 2320   down.```..#### 
+00000dc0: 4578 6563 7574 6520 636f 6e66 6967 7572  Execute configur
+00000dd0: 6174 696f 6e20 6368 616e 6765 2063 6f6d  ation change com
+00000de0: 6d61 6e64 7320 2877 696c 6c20 6175 746f  mands (will auto
+00000df0: 6d61 7469 6361 6c6c 7920 656e 7465 7220  matically enter 
+00000e00: 696e 746f 2063 6f6e 6669 6720 6d6f 6465  into config mode
+00000e10: 290a 0a60 6060 7079 0a63 6f6e 6669 675f  )..```py.config_
+00000e20: 636f 6d6d 616e 6473 203d 205b 2027 6c6f  commands = [ 'lo
+00000e30: 6767 696e 6720 6275 6666 6572 6564 2032  gging buffered 2
+00000e40: 3030 3030 272c 0a20 2020 2020 2020 2020  0000',.         
+00000e50: 2020 2020 2020 2020 2020 2027 6c6f 6767             'logg
+00000e60: 696e 6720 6275 6666 6572 6564 2032 3030  ing buffered 200
+00000e70: 3130 272c 0a20 2020 2020 2020 2020 2020  10',.           
+00000e80: 2020 2020 2020 2020 2027 6e6f 206c 6f67           'no log
+00000e90: 6769 6e67 2063 6f6e 736f 6c65 2720 5d0a  ging console' ].
+00000ea0: 6f75 7470 7574 203d 206e 6574 5f63 6f6e  output = net_con
+00000eb0: 6e65 6374 2e73 656e 645f 636f 6e66 6967  nect.send_config
+00000ec0: 5f73 6574 2863 6f6e 6669 675f 636f 6d6d  _set(config_comm
+00000ed0: 616e 6473 290a 7072 696e 7428 6f75 7470  ands).print(outp
+00000ee0: 7574 290a 6060 600a 6060 600a 7079 6e65  ut).```.```.pyne
+00000ef0: 742d 7274 7231 2363 6f6e 6669 6720 7465  t-rtr1#config te
+00000f00: 726d 0a45 6e74 6572 2063 6f6e 6669 6775  rm.Enter configu
+00000f10: 7261 7469 6f6e 2063 6f6d 6d61 6e64 732c  ration commands,
+00000f20: 206f 6e65 2070 6572 206c 696e 652e 2020   one per line.  
+00000f30: 456e 6420 7769 7468 2043 4e54 4c2f 5a2e  End with CNTL/Z.
+00000f40: 0a70 796e 6574 2d72 7472 3128 636f 6e66  .pynet-rtr1(conf
+00000f50: 6967 2923 6c6f 6767 696e 6720 6275 6666  ig)#logging buff
+00000f60: 6572 6564 2032 3030 3030 0a70 796e 6574  ered 20000.pynet
+00000f70: 2d72 7472 3128 636f 6e66 6967 2923 6c6f  -rtr1(config)#lo
+00000f80: 6767 696e 6720 6275 6666 6572 6564 2032  gging buffered 2
+00000f90: 3030 3130 0a70 796e 6574 2d72 7472 3128  0010.pynet-rtr1(
+00000fa0: 636f 6e66 6967 2923 6e6f 206c 6f67 6769  config)#no loggi
+00000fb0: 6e67 2063 6f6e 736f 6c65 0a70 796e 6574  ng console.pynet
+00000fc0: 2d72 7472 3128 636f 6e66 6967 2923 656e  -rtr1(config)#en
+00000fd0: 640a 7079 6e65 742d 7274 7231 230a 6060  d.pynet-rtr1#.``
+00000fe0: 600a 0a3c 6272 202f 3e0a 0a23 2320 4150  `..<br />..## AP
+00000ff0: 492d 446f 6375 6d65 6e74 6174 696f 6e0a  I-Documentation.
+00001000: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00001010: 2f2f 6b74 6279 6572 732e 6769 7468 7562  //ktbyers.github
+00001020: 2e69 6f2f 6e65 746d 696b 6f2f 646f 6373  .io/netmiko/docs
+00001030: 2f6e 6574 6d69 6b6f 2f69 6e64 6578 2e68  /netmiko/index.h
+00001040: 746d 6c22 2074 6974 6c65 3d22 446f 6373  tml" title="Docs
+00001050: 223e 4150 4920 446f 6375 6d65 6e74 6174  ">API Documentat
+00001060: 696f 6e3c 2f61 3e0a 0a42 656c 6f77 2061  ion</a>..Below a
+00001070: 7265 2073 6f6d 6520 6f66 2074 6865 2070  re some of the p
+00001080: 6172 7469 6375 6c61 726c 7920 6861 6e64  articularly hand
+00001090: 7920 436c 6173 7365 732f 6675 6e63 7469  y Classes/functi
+000010a0: 6f6e 7320 666f 7220 6561 7379 2072 6566  ons for easy ref
+000010b0: 6572 656e 6365 3a0a 2d20 5b42 6173 6520  erence:.- [Base 
+000010c0: 436f 6e6e 6563 7469 6f6e 204f 626a 6563  Connection Objec
+000010d0: 745d 2868 7474 7073 3a2f 2f6b 7462 7965  t](https://ktbye
+000010e0: 7273 2e67 6974 6875 622e 696f 2f6e 6574  rs.github.io/net
+000010f0: 6d69 6b6f 2f64 6f63 732f 6e65 746d 696b  miko/docs/netmik
+00001100: 6f2f 6261 7365 5f63 6f6e 6e65 6374 696f  o/base_connectio
+00001110: 6e2e 6874 6d6c 290a 2d20 5b53 5348 2041  n.html).- [SSH A
+00001120: 7574 6f64 6574 6563 745d 2868 7474 7073  utodetect](https
+00001130: 3a2f 2f6b 7462 7965 7273 2e67 6974 6875  ://ktbyers.githu
+00001140: 622e 696f 2f6e 6574 6d69 6b6f 2f64 6f63  b.io/netmiko/doc
+00001150: 732f 6e65 746d 696b 6f2f 696e 6465 782e  s/netmiko/index.
+00001160: 6874 6d6c 236e 6574 6d69 6b6f 2e53 5348  html#netmiko.SSH
+00001170: 4465 7465 6374 290a 2d20 5b53 5348 2044  Detect).- [SSH D
+00001180: 6973 7061 7463 6865 725d 2868 7474 7073  ispatcher](https
+00001190: 3a2f 2f6b 7462 7965 7273 2e67 6974 6875  ://ktbyers.githu
+000011a0: 622e 696f 2f6e 6574 6d69 6b6f 2f64 6f63  b.io/netmiko/doc
+000011b0: 732f 6e65 746d 696b 6f2f 696e 6465 782e  s/netmiko/index.
+000011c0: 6874 6d6c 236e 6574 6d69 6b6f 2e73 7368  html#netmiko.ssh
+000011d0: 5f64 6973 7061 7463 6865 7229 0a2d 205b  _dispatcher).- [
+000011e0: 5265 6469 7370 6174 6368 5d28 6874 7470  Redispatch](http
+000011f0: 733a 2f2f 6b74 6279 6572 732e 6769 7468  s://ktbyers.gith
+00001200: 7562 2e69 6f2f 6e65 746d 696b 6f2f 646f  ub.io/netmiko/do
+00001210: 6373 2f6e 6574 6d69 6b6f 2f69 6e64 6578  cs/netmiko/index
+00001220: 2e68 746d 6c23 6e65 746d 696b 6f2e 7265  .html#netmiko.re
+00001230: 6469 7370 6174 6368 290a 0a3c 6272 202f  dispatch)..<br /
+00001240: 3e0a 0a23 2320 436f 6e74 7269 6275 7469  >..## Contributi
+00001250: 6e67 0a0a 436f 6e74 7269 6275 746f 7273  ng..Contributors
+00001260: 2061 7265 2077 656c 636f 6d65 2e0a 0a59   are welcome...Y
+00001270: 6f75 2063 616e 2063 6f6e 7472 6962 7574  ou can contribut
+00001280: 6520 746f 204e 6574 6d69 6b6f 2069 6e20  e to Netmiko in 
+00001290: 6120 7661 7269 6574 7920 6f66 2077 6179  a variety of way
+000012a0: 733a 2061 6e73 7765 7269 6e67 2071 7565  s: answering que
+000012b0: 7374 696f 6e73 206f 6e20 536c 6163 6b20  stions on Slack 
+000012c0: 2873 6565 2062 656c 6f77 2069 6e20 5175  (see below in Qu
+000012d0: 6573 7469 6f6e 732f 4469 7363 7573 7369  estions/Discussi
+000012e0: 6f6e 7329 2c20 7265 7370 6f6e 6469 6e67  ons), responding
+000012f0: 2074 6f20 6973 7375 6573 2c20 6164 6469   to issues, addi
+00001300: 6e67 2074 6f20 7468 6520 636f 6d6d 6f6e  ng to the common
+00001310: 2069 7373 7565 732c 2072 6570 6f72 7469   issues, reporti
+00001320: 6e67 2f66 6978 696e 6720 6275 6773 2c20  ng/fixing bugs, 
+00001330: 6f72 2065 7665 6e20 6164 6469 6e67 2079  or even adding y
+00001340: 6f75 7220 6f77 6e20 6465 7669 6365 2074  our own device t
+00001350: 7970 652e 0a0a 4265 666f 7265 2063 6f6e  ype...Before con
+00001360: 7472 6962 7574 696e 6720 6120 6e65 7720  tributing a new 
+00001370: 7665 6e64 6f72 2f70 6c61 7466 6f72 6d20  vendor/platform 
+00001380: 6465 7669 6365 2074 7970 652c 2072 656d  device type, rem
+00001390: 656d 6265 7220 7468 6174 2061 6e79 2063  ember that any c
+000013a0: 6f64 6520 6164 6465 6420 6e65 6564 7320  ode added needs 
+000013b0: 746f 2062 6520 7375 7070 6f72 7465 6420  to be supported 
+000013c0: 696e 2073 6f6d 6520 6661 7368 696f 6e2e  in some fashion.
+000013d0: 2054 6f20 6164 6420 6120 7665 6e64 6f72   To add a vendor
+000013e0: 2f70 6c61 7466 6f72 6d20 796f 7520 6361  /platform you ca
+000013f0: 6e20 666f 6c6c 6f77 2074 6865 206f 7574  n follow the out
+00001400: 6c69 6e65 205b 6865 7265 5d28 5645 4e44  line [here](VEND
+00001410: 4f52 2e6d 6429 2e20 4f6e 6365 2079 6f75  OR.md). Once you
+00001420: 2776 6520 776f 726b 6564 206f 6e20 796f  've worked on yo
+00001430: 7572 2066 6972 7374 2070 6173 7320 6f66  ur first pass of
+00001440: 2079 6f75 7220 6472 6976 6572 2061 6e64   your driver and
+00001450: 2068 6176 6520 6974 2066 756e 6374 696f   have it functio
+00001460: 6e61 6c2c 2079 6f75 276c 6c20 6e65 6564  nal, you'll need
+00001470: 2074 6f20 696e 636c 7564 6520 7465 7374   to include test
+00001480: 2064 6174 6120 696e 206f 7264 6572 2066   data in order f
+00001490: 6f72 2069 7420 746f 2062 6520 6d65 7267  or it to be merg
+000014a0: 6564 2069 6e74 6f20 6465 7665 6c6f 702c  ed into develop,
+000014b0: 2079 6f75 2063 616e 2073 6565 2074 6865   you can see the
+000014c0: 2067 656e 6572 616c 2066 6c6f 7720 6f66   general flow of
+000014d0: 2068 6f77 2074 6f20 646f 2074 6861 7420   how to do that 
+000014e0: 5b68 6572 655d 2854 4553 5449 4e47 2e6d  [here](TESTING.m
+000014f0: 6429 2e0a 0a46 6f72 2061 6c6c 2063 6f64  d)...For all cod
+00001500: 6520 636f 6e74 7269 6275 7469 6f6e 732c  e contributions,
+00001510: 2070 6c65 6173 6520 656e 7375 7265 2074   please ensure t
+00001520: 6861 7420 796f 7520 6861 7665 2072 616e  hat you have ran
+00001530: 2060 626c 6163 6b60 2061 6761 696e 7374   `black` against
+00001540: 2074 6865 2063 6f64 6520 6f72 2079 6f75   the code or you
+00001550: 7220 636f 6465 2077 696c 6c20 6661 696c  r code will fail
+00001560: 2074 6865 2054 7261 7669 7320 4349 2062   the Travis CI b
+00001570: 7569 6c64 2e0a 0a3c 6272 202f 3e0a 0a23  uild...<br />..#
+00001580: 2320 5175 6573 7469 6f6e 732f 4469 7363  # Questions/Disc
+00001590: 7573 7369 6f6e 0a0a 4966 2079 6f75 2066  ussion..If you f
+000015a0: 696e 6420 616e 2069 7373 7565 2077 6974  ind an issue wit
+000015b0: 6820 4e65 746d 696b 6f2c 2074 6865 6e20  h Netmiko, then 
+000015c0: 796f 7520 6361 6e20 6f70 656e 2061 6e20  you can open an 
+000015d0: 6973 7375 6520 6f6e 2074 6869 7320 7072  issue on this pr
+000015e0: 6f6a 6563 7473 2069 7373 7565 2070 6167  ojects issue pag
+000015f0: 6520 6865 7265 3a20 5b68 7474 7073 3a2f  e here: [https:/
+00001600: 2f67 6974 6875 622e 636f 6d2f 6b74 6279  /github.com/ktby
+00001610: 6572 732f 6e65 746d 696b 6f2f 6973 7375  ers/netmiko/issu
+00001620: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00001630: 7562 2e63 6f6d 2f6b 7462 7965 7273 2f6e  ub.com/ktbyers/n
+00001640: 6574 6d69 6b6f 2f69 7373 7565 7329 2e20  etmiko/issues). 
+00001650: 506c 6561 7365 206d 616b 6520 7375 7265  Please make sure
+00001660: 2079 6f75 2776 6520 7265 6164 2074 6872   you've read thr
+00001670: 6f75 6768 2074 6865 2063 6f6d 6d6f 6e20  ough the common 
+00001680: 6973 7375 6573 2061 6e64 2065 7861 6d70  issues and examp
+00001690: 6c65 7320 7072 696f 7220 746f 206f 7065  les prior to ope
+000016a0: 6e69 6e67 2061 6e20 6973 7375 652e 2050  ning an issue. P
+000016b0: 6c65 6173 6520 6f6e 6c79 206f 7065 6e20  lease only open 
+000016c0: 6973 7375 6573 2066 6f72 2062 7567 732c  issues for bugs,
+000016d0: 2066 6561 7475 7265 2072 6571 7565 7374   feature request
+000016e0: 732c 206f 7220 6f74 6865 7220 746f 7069  s, or other topi
+000016f0: 6373 2072 656c 6174 6564 2074 6f20 6465  cs related to de
+00001700: 7665 6c6f 706d 656e 7420 6f66 204e 6574  velopment of Net
+00001710: 6d69 6b6f 2e20 4966 2079 6f75 2073 696d  miko. If you sim
+00001720: 706c 7920 6861 7665 2061 2071 7565 7374  ply have a quest
+00001730: 696f 6e2c 206a 6f69 6e20 7573 206f 6e20  ion, join us on 
+00001740: 536c 6163 6b2e 2e2e 0a0a 4966 2079 6f75  Slack.....If you
+00001750: 2068 6176 6520 7175 6573 7469 6f6e 7320   have questions 
+00001760: 6f72 2077 6f75 6c64 206c 696b 6520 746f  or would like to
+00001770: 2064 6973 6375 7373 204e 6574 6d69 6b6f   discuss Netmiko
+00001780: 2c20 6120 236e 6574 6d69 6b6f 2063 6861  , a #netmiko cha
+00001790: 6e6e 656c 2065 7869 7374 7320 696e 205b  nnel exists in [
+000017a0: 7468 6973 2053 6c61 636b 5d28 6874 7470  this Slack](http
+000017b0: 733a 2f2f 7079 6e65 742e 736c 6163 6b2e  s://pynet.slack.
+000017c0: 636f 6d29 2077 6f72 6b73 7061 6365 2e20  com) workspace. 
+000017d0: 546f 206a 6f69 6e2c 2075 7365 205b 7468  To join, use [th
+000017e0: 6973 2069 6e76 6974 6174 696f 6e5d 2868  is invitation](h
+000017f0: 7474 7073 3a2f 2f6a 6f69 6e2e 736c 6163  ttps://join.slac
+00001800: 6b2e 636f 6d2f 742f 7079 6e65 742f 7368  k.com/t/pynet/sh
+00001810: 6172 6564 5f69 6e76 6974 652f 7a74 2d6b  ared_invite/zt-k
+00001820: 6d32 6b33 7570 662d 416b 5748 5934 5945  m2k3upf-AkWHY4YE
+00001830: 7833 7349 3152 3569 724d 6d63 3751 292e  x3sI1R5irMmc7Q).
+00001840: 204f 6e63 6520 796f 7520 6861 7665 2065   Once you have e
+00001850: 6e74 6572 6564 2074 6865 2077 6f72 6b73  ntered the works
+00001860: 7061 6365 2c20 7468 656e 2079 6f75 2063  pace, then you c
+00001870: 616e 206a 6f69 6e20 7468 6520 236e 6574  an join the #net
+00001880: 6d69 6b6f 2063 6861 6e6e 656c 2e0a 0a0a  miko channel....
+00001890: 2d2d 2d0a 4b69 726b 2042 7965 7273 2020  ---.Kirk Byers  
+000018a0: 0a50 7974 686f 6e20 666f 7220 4e65 7477  .Python for Netw
+000018b0: 6f72 6b20 456e 6769 6e65 6572 7320 200a  ork Engineers  .
+000018c0: 6874 7470 733a 2f2f 7079 6e65 742e 7477  https://pynet.tw
+000018d0: 622d 7465 6368 2e63 6f6d 2020 0a         b-tech.com  .
```

### Comparing `netmiko-4.1.2/netmiko/__init__.py` & `netmiko-4.2.0/netmiko/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-__version__ = "4.1.2"
+__version__ = "4.2.0"
 PY_MAJ_VER = 3
 PY_MIN_VER = 7
 MIN_PYTHON_VER = "3.7"
 
 
 # Make sure user is using a valid Python version (for Netmiko)
 def check_python_version():  # type: ignore
```

### Comparing `netmiko-4.1.2/netmiko/a10/a10_ssh.py` & `netmiko-4.2.0/netmiko/a10/a10_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/accedian/accedian_ssh.py` & `netmiko-4.2.0/netmiko/accedian/accedian_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/adtran/adtran.py` & `netmiko-4.2.0/netmiko/adtran/adtran.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 from typing import Any, Optional
 import re
 from netmiko.cisco_base_connection import CiscoBaseConnection
 
 
 class AdtranOSBase(CiscoBaseConnection):
+    prompt_pattern = r"[>#]"
+
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         if kwargs.get("global_cmd_verify") is None:
             kwargs["global_cmd_verify"] = False
         return super().__init__(*args, **kwargs)
 
     def session_preparation(self) -> None:
         """Prepare the session after the connection has been established."""
         self.ansi_escape_codes = True
-        self._test_channel_read()
+        self._test_channel_read(pattern=self.prompt_pattern)
         self.set_base_prompt()
         self.disable_paging(command="terminal length 0")
+        cmd = "terminal width 132"
+        self.set_terminal_width(command=cmd, pattern=cmd)
 
     def check_enable_mode(self, check_string: str = "#") -> bool:
         return super().check_enable_mode(check_string=check_string)
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return super().enable(
-            cmd=cmd, pattern=pattern, enable_pattern=enable_pattern, re_flags=re_flags
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def exit_enable_mode(self, exit_command: str = "disable") -> str:
         return super().exit_enable_mode(exit_command=exit_command)
 
     def check_config_mode(
         self, check_string: str = ")#", pattern: str = "", force_regex: bool = False
```

### Comparing `netmiko-4.1.2/netmiko/alcatel/alcatel_aos_ssh.py` & `netmiko-4.2.0/netmiko/alcatel/alcatel_aos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/allied_telesis/allied_telesis_awplus.py` & `netmiko-4.2.0/netmiko/allied_telesis/allied_telesis_awplus.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/apresia/apresia_aeos.py` & `netmiko-4.2.0/netmiko/apresia/apresia_aeos.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/arista/arista.py` & `netmiko-4.2.0/netmiko/arista/arista.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,31 +5,55 @@
 from netmiko.cisco_base_connection import CiscoFileTransfer
 
 if TYPE_CHECKING:
     from netmiko.base_connection import BaseConnection
 
 
 class AristaBase(CiscoSSHConnection):
+    prompt_pattern = r"[$>#]"
+
     def session_preparation(self) -> None:
         """Prepare the session after the connection has been established."""
+        self._test_channel_read(pattern=self.prompt_pattern)
         cmd = "terminal width 511"
-        # Arista will echo immediately and then when the device really responds (like NX-OS)
         self.set_terminal_width(command=cmd, pattern=r"Width set to")
         self.disable_paging(cmd_verify=False, pattern=r"Pagination disabled")
         self.set_base_prompt()
 
+    def find_prompt(
+        self, delay_factor: float = 1.0, pattern: Optional[str] = None
+    ) -> str:
+        """
+        Arista's sometimes duplicate the command echo if they fall behind.
+
+        arista9-napalm#
+        show version | json
+        arista9-napalm#show version | json
+
+        Using the terminating pattern tries to ensure that it is less likely they
+        fall behind.
+        """
+        if not pattern:
+            pattern = self.prompt_pattern
+        return super().find_prompt(delay_factor=delay_factor, pattern=pattern)
+
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = r"\#",
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return super().enable(
-            cmd=cmd, pattern=pattern, enable_pattern=enable_pattern, re_flags=re_flags
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def check_config_mode(
         self,
         check_string: str = ")#",
         pattern: str = r"[>\#]",
         force_regex: bool = False,
```

### Comparing `netmiko-4.1.2/netmiko/aruba/aruba_ssh.py` & `netmiko-4.2.0/netmiko/aruba/aruba_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/audiocode/audiocode_ssh.py` & `netmiko-4.2.0/netmiko/audiocode/audiocode_ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,64 +4,86 @@
 from netmiko.base_connection import BaseConnection
 from netmiko.no_enable import NoEnable
 
 
 class AudiocodeBase(BaseConnection):
     """Common Methods for AudioCode Drivers."""
 
+    prompt_pattern = r"[>#]"
+
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         default_enter = kwargs.get("default_enter")
         kwargs["default_enter"] = "\r" if default_enter is None else default_enter
         super().__init__(*args, **kwargs)
 
     def session_preparation(self) -> None:
         """Prepare the session after the connection has been established."""
-        self._test_channel_read(pattern=r"[>#]")
+        self._test_channel_read(pattern=self.prompt_pattern)
         self.set_base_prompt()
         self.disable_paging()
         # Clear the read buffer
         self.clear_buffer()
 
     def set_base_prompt(
         self,
         pri_prompt_terminator: str = "#",
         alt_prompt_terminator: str = ">",
         delay_factor: float = 1.0,
-        pattern: Optional[str] = r"\*?(#|>)",
+        pattern: Optional[str] = None,
     ) -> str:
-        return super().set_base_prompt(
-            pri_prompt_terminator=pri_prompt_terminator,
-            alt_prompt_terminator=alt_prompt_terminator,
-            delay_factor=delay_factor,
-            pattern=pattern,
-        )
+
+        if pattern is None:
+            pattern = rf"\*?{self.prompt_pattern}"
+
+        if pattern:
+            prompt = self.find_prompt(delay_factor=delay_factor, pattern=pattern)
+        else:
+            prompt = self.find_prompt(delay_factor=delay_factor)
+
+        if not prompt[-1] in (pri_prompt_terminator, alt_prompt_terminator):
+            raise ValueError(f"Router prompt not found: {repr(prompt)}")
+
+        # If all we have is the 'terminator' just use that :-(
+        if len(prompt) == 1:
+            self.base_prompt = prompt
+        else:
+            # Audiocode will return a prompt with * in it in certain
+            # situations: 'MYDEVICE*#', strip this off.
+            if "*#" in prompt or "*>" in prompt:
+                self.base_prompt = prompt[:-2]
+            else:
+                # Strip off trailing terminator
+                self.base_prompt = prompt[:-1]
+        return self.base_prompt
 
     def find_prompt(
         self,
         delay_factor: float = 1.0,
-        pattern: Optional[str] = r"\*?(#|>)",
+        pattern: Optional[str] = None,
     ) -> str:
+
+        if pattern is None:
+            pattern = rf"\*?{self.prompt_pattern}"
         return super().find_prompt(
             delay_factor=delay_factor,
             pattern=pattern,
         )
 
     def _enable_paging(
         self,
         delay_factor: Optional[float] = 0.5,
     ) -> str:
         return ""
 
     def check_config_mode(
         self,
-        check_string: str = r"(\)#|\)\*#)",
+        check_string: str = r"(?:\)#|\)\*#)",
         pattern: str = r"..#",
         force_regex: bool = True,
     ) -> bool:
-
         return super().check_config_mode(
             check_string=check_string, pattern=pattern, force_regex=force_regex
         )
 
     def check_enable_mode(self, check_string: str = "#") -> bool:
         return super().check_enable_mode(check_string=check_string)
 
@@ -78,18 +100,23 @@
         self.write_channel(command + self.RETURN)
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = "#",
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return super().enable(
-            cmd=cmd, pattern=pattern, enable_pattern=enable_pattern, re_flags=re_flags
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def exit_config_mode(self, exit_config: str = "exit", pattern: str = r"#") -> str:
         output = ""
         max_exit_depth = 10
         if self.check_config_mode():
             # Keep "exitting" until out of config mode
@@ -368,15 +395,15 @@
         strip_prompt: bool = False,
         strip_command: bool = False,
         config_mode_command: Optional[str] = None,
         cmd_verify: bool = True,
         enter_config_mode: bool = True,
         error_pattern: str = "",
         terminator: str = r"/.*>",
-        bypass_commands: str = None,
+        bypass_commands: Optional[str] = None,
     ) -> str:
 
         return super().send_config_set(
             config_commands=config_commands,
             exit_config_mode=exit_config_mode,
             read_timeout=read_timeout,
             delay_factor=delay_factor,
@@ -443,15 +470,15 @@
         )
 
     def _enable_paging(
         self,
         delay_factor: Optional[float] = 0.5,
     ) -> str:
         """Not supported"""
-        pass
+        return ""
 
     def strip_command(self, command_string: str, output: str) -> str:
         # Support for Audiocode_Shell.
         pattern = r"^SIP.*[\s\S]?PING.*>?.*[\s\S]?.*>?$"
         output = re.sub(pattern, "", output, flags=re.M)
 
         cmd = command_string.strip()
```

### Comparing `netmiko-4.1.2/netmiko/base_connection.py` & `netmiko-4.2.0/netmiko/base_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 from threading import Lock
 import functools
 import logging
 import itertools
 
 import paramiko
 import serial
-from tenacity import retry, stop_after_attempt, wait_exponential
 import warnings
 
 from netmiko import log
 from netmiko.netmiko_globals import BACKSPACE_CHAR
 from netmiko.exceptions import (
     NetmikoTimeoutException,
     NetmikoAuthenticationException,
@@ -146,14 +145,15 @@
         global_delay_factor: float = 1.0,
         global_cmd_verify: Optional[bool] = None,
         use_keys: bool = False,
         key_file: Optional[str] = None,
         pkey: Optional[paramiko.PKey] = None,
         passphrase: Optional[str] = None,
         disabled_algorithms: Optional[Dict[str, Any]] = None,
+        disable_sha2_fix: bool = False,
         allow_agent: bool = False,
         ssh_strict: bool = False,
         system_host_keys: bool = False,
         alt_host_keys: bool = False,
         alt_key_file: str = "",
         ssh_config_file: Optional[str] = None,
         #
@@ -179,14 +179,15 @@
         session_log_record_writes: bool = False,
         session_log_file_mode: str = "write",
         allow_auto_change: bool = False,
         encoding: str = "utf-8",
         sock: Optional[socket.socket] = None,
         auto_connect: bool = True,
         delay_factor_compat: bool = False,
+        disable_lf_normalization: bool = False,
     ) -> None:
         """
         Initialize attributes for establishing connection to target device.
 
         :param ip: IP address of target device. Not required if `host` is
             provided.
 
@@ -218,45 +219,54 @@
 
         :param passphrase: Passphrase to use for encrypted key; password will be used for key
                 decryption if not specified.
 
         :param disabled_algorithms: Dictionary of SSH algorithms to disable. Refer to the Paramiko
                 documentation for a description of the expected format.
 
+        :param disable_sha2_fix: Boolean that fixes Paramiko issue with missing server-sig-algs
+            https://github.com/paramiko/paramiko/issues/1961 (default: False)
+
         :param allow_agent: Enable use of SSH key-agent.
 
         :param ssh_strict: Automatically reject unknown SSH host keys (default: False, which
                 means unknown SSH host keys will be accepted).
 
         :param system_host_keys: Load host keys from the users known_hosts file.
 
         :param alt_host_keys: If `True` host keys will be loaded from the file specified in
                 alt_key_file.
 
         :param alt_key_file: SSH host key file to use (if alt_host_keys=True).
 
         :param ssh_config_file: File name of OpenSSH configuration file.
 
-        :param timeout: Connection timeout.
+        :param conn_timeout: TCP connection timeout.
 
         :param session_timeout: Set a timeout for parallel requests.
 
         :param auth_timeout: Set a timeout (in seconds) to wait for an authentication response.
 
         :param banner_timeout: Set a timeout to wait for the SSH banner (pass to Paramiko).
 
+        :param read_timeout_override: Set a timeout that will override the default read_timeout
+                of both send_command and send_command_timing. This is useful for 3rd party
+                libraries where directly accessing method arguments might be impractical.
+
         :param keepalive: Send SSH keepalive packets at a specific interval, in seconds.
                 Currently defaults to 0, for backwards compatibility (it will not attempt
                 to keep the connection alive).
 
         :param default_enter: Character(s) to send to correspond to enter key (default: \n).
 
         :param response_return: Character(s) to use in normalized return data to represent
                 enter key (default: \n)
 
+        :param serial_settings: Dictionary of settings for use with serial port (pySerial).
+
         :param fast_cli: Provide a way to optimize for performance. Converts select_delay_factor
                 to select smallest of global and specific. Sets default global_delay_factor to .1
                 (default: True)
 
         :param session_log: File path or BufferedIOBase subclass object to write the session log to.
 
         :param session_log_record_writes: The session log generally only records channel reads due
@@ -281,14 +291,17 @@
 
         :param auto_connect: Control whether Netmiko automatically establishes the connection as
                 part of the object creation (default: True).
 
         :param delay_factor_compat: Set send_command and send_command_timing back to using Netmiko
                 3.x behavior for delay_factor/global_delay_factor/max_loops. This argument will be
                 eliminated in Netmiko 5.x (default: False).
+
+        :param disable_lf_normalization: Disable Netmiko's linefeed normalization behavior
+                (default: False)
         """
 
         self.remote_conn: Union[
             None, telnetlib.Telnet, paramiko.Channel, serial.Serial
         ] = None
         # Does the platform support a configuration mode
         self._config_mode = True
@@ -302,14 +315,16 @@
             else:
                 self.RETURN = self.TELNET_RETURN
         else:
             self.RETURN = default_enter
 
         # Line Separator in response lines
         self.RESPONSE_RETURN = "\n" if response_return is None else response_return
+        self.disable_lf_normalization = True if disable_lf_normalization else False
+
         if ip:
             self.host = ip.strip()
         elif host:
             self.host = host.strip()
         if not ip and not host and "serial" not in device_type:
             raise ValueError("Either ip or host must be set")
         if port is None:
@@ -425,15 +440,23 @@
                 self._key_check()
             self.pkey = pkey
             self.passphrase = passphrase
             self.allow_agent = allow_agent
             self.system_host_keys = system_host_keys
             self.alt_host_keys = alt_host_keys
             self.alt_key_file = alt_key_file
-            self.disabled_algorithms = disabled_algorithms or {}
+
+            if disabled_algorithms:
+                self.disabled_algorithms = disabled_algorithms
+            else:
+                self.disabled_algorithms = (
+                    {"pubkeys": ["rsa-sha2-256", "rsa-sha2-512"]}
+                    if disable_sha2_fix
+                    else {}
+                )
 
             # For SSH proxy support
             self.ssh_config_file = ssh_config_file
 
         # Establish the remote connection
         if auto_connect:
             self._open()
@@ -573,15 +596,28 @@
                 return False
         return False
 
     @lock_channel
     def read_channel(self) -> str:
         """Generic handler that will read all the data from given channel."""
         new_data = self.channel.read_channel()
-        new_data = self.normalize_linefeeds(new_data)
+
+        if self.disable_lf_normalization is False:
+            start = time.time()
+            # Data blocks shouldn't end in '\r' (can cause problems with normalize_linefeeds)
+            # Only do the extra read if '\n' exists in the output
+            # this avoids devices that only use \r.
+            while ("\n" in new_data) and (time.time() - start < 1.0):
+                if new_data[-1] == "\r":
+                    time.sleep(0.01)
+                    new_data += self.channel.read_channel()
+                else:
+                    break
+            new_data = self.normalize_linefeeds(new_data)
+
         if self.ansi_escape_codes:
             new_data = self.strip_ansi_escape_codes(new_data)
         log.debug(f"read_channel: {new_data}")
         if self.session_log:
             self.session_log.write(new_data)
 
         # If data had been previously saved to the buffer, the prepend it to output
@@ -627,16 +663,29 @@
             read_timeout = self.read_timeout_override
 
         output = ""
         loop_delay = 0.01
         start_time = time.time()
         # if read_timeout == 0 or 0.0 keep reading indefinitely
         while (time.time() - start_time < read_timeout) or (not read_timeout):
+
             output += self.read_channel()
+
             if re.search(pattern, output, flags=re_flags):
+                if "(" in pattern and "(?:" not in pattern:
+                    msg = f"""
+Parenthesis found in pattern.
+
+pattern: {pattern}\n
+
+This can be problemtic when used in read_until_pattern().
+
+You should ensure that you use either non-capture groups i.e. '(?:' or that the
+parenthesis completely wrap the pattern '(pattern)'"""
+                    log.debug(msg)
                 results = re.split(pattern, output, maxsplit=1, flags=re_flags)
 
                 # The string matched by pattern must be retained in the output string.
                 # re.split will do this if capturing parenthesis are used.
                 if len(results) == 2:
                     # no capturing parenthesis, convert and try again.
                     pattern = f"({pattern})"
@@ -677,24 +726,32 @@
         read_timeout: float = 120.0,
         delay_factor: Optional[float] = None,
         max_loops: Optional[int] = None,
     ) -> str:
         """Read data on the channel based on timing delays.
 
         General pattern is keep reading until no new data is read.
+
         Once no new data is read wait `last_read` amount of time (one last read).
         As long as no new data, then return data.
 
-        `read_timeout` is an absolute timer for how long to keep reading (which presupposes
-        we are still getting new data).
-
         Setting `read_timeout` to zero will cause read_channel_timing to never expire based
-        on an absolute timeout. It will only complete based on timeout based on their being
+        on an absolute timeout. It will only complete based on timeout based on there being
         no new data.
 
+        :param last_read: Amount of time to wait before performing one last read (under the
+            idea that we should be done reading at this point and there should be no new
+            data).
+
+        :param read_timeout: Absolute timer for how long Netmiko should keep reading data on
+            the channel (waiting for there to be no new data). Will raise ReadTimeout if this
+            timeout expires. A read_timeout value of 0 will cause the read-loop to never timeout
+            (i.e. Netmiko will keep reading indefinitely until there is no new data and last_read
+            passes).
+
         :param delay_factor: Deprecated in Netmiko 4.x. Will be eliminated in Netmiko 5.
 
         :param max_loops: Deprecated in Netmiko 4.x. Will be eliminated in Netmiko 5.
         """
 
         if delay_factor is not None or max_loops is not None:
             warnings.warn(DELAY_FACTOR_DEPR_SIMPLE_MSG, DeprecationWarning)
@@ -813,14 +870,16 @@
 
         :param pri_prompt_terminator: Primary trailing delimiter for identifying a device prompt
 
         :param alt_prompt_terminator: Alternate trailing delimiter for identifying a device prompt
 
         :param username_pattern: Pattern used to identify the username prompt
 
+        :param pwd_pattern: Pattern used to identify the pwd prompt
+
         :param delay_factor: See __init__: global_delay_factor
 
         :param max_loops: Controls the wait time in conjunction with the delay_factor
         """
         delay_factor = self.select_delay_factor(delay_factor)
 
         # Revert telnet_login back to old speeds/delays
@@ -1002,15 +1061,14 @@
         output: str,
         strip_command: bool = False,
         command_string: Optional[str] = None,
         strip_prompt: bool = False,
     ) -> str:
         """Strip out command echo and trailing router prompt."""
         if strip_command and command_string:
-            command_string = self.normalize_linefeeds(command_string)
             output = self.strip_command(command_string, output)
         if strip_prompt:
             output = self.strip_prompt(output)
         return output
 
     def establish_connection(self, width: int = 511, height: int = 1000) -> None:
         """Establish SSH connection to the network device
@@ -1204,14 +1262,18 @@
         pattern: Optional[str] = None,
     ) -> str:
         """Disable paging default to a Cisco CLI method.
 
         :param command: Device command to disable pagination of output
 
         :param delay_factor: Deprecated in Netmiko 4.x. Will be eliminated in Netmiko 5.
+
+        :param cmd_verify: Verify command echo before proceeding (default: True).
+
+        :param pattern: Pattern to terminate reading of channel
         """
         if delay_factor is not None:
             warnings.warn(DELAY_FACTOR_DEPR_SIMPLE_MSG, DeprecationWarning)
 
         command = self.normalize_cmd(command)
         log.debug("In disable_paging")
         log.debug(f"Command: {command}")
@@ -1258,20 +1320,14 @@
             output = self.read_until_pattern(pattern=re.escape(command.strip()))
         elif pattern:
             output = self.read_until_pattern(pattern=pattern)
         else:
             output = self.read_until_prompt()
         return output
 
-    # Retry by sleeping .33 and then double sleep until 5 attempts (.33, .66, 1.32, etc)
-    @retry(
-        wait=wait_exponential(multiplier=0.33, min=0, max=5),
-        stop=stop_after_attempt(5),
-        reraise=True,
-    )
     def set_base_prompt(
         self,
         pri_prompt_terminator: str = "#",
         alt_prompt_terminator: str = ">",
         delay_factor: float = 1.0,
         pattern: Optional[str] = None,
     ) -> str:
@@ -1427,14 +1483,22 @@
         cmd_verify: bool = False,
     ) -> Union[str, List[Any], Dict[str, Any]]:
         """Execute command_string on the SSH channel using a delay-based mechanism. Generally
         used for show commands.
 
         :param command_string: The command to be executed on the remote device.
 
+        :param last_read: Time waited after end of data
+
+        :param read_timeout: Absolute timer for how long Netmiko should keep reading data on
+            the channel (waiting for there to be no new data). Will raise ReadTimeout if this
+            timeout expires. A read_timeout value of 0 will cause the read-loop to never timeout
+            (i.e. Netmiko will keep reading indefinitely until there is no new data and last_read
+            passes).
+
         :param delay_factor: Deprecated in Netmiko 4.x. Will be eliminated in Netmiko 5.
 
         :param max_loops: Deprecated in Netmiko 4.x. Will be eliminated in Netmiko 5.
 
         :param strip_prompt: Remove the trailing router prompt from the output (default: True).
 
         :param strip_command: Remove the echo of the command from the output (default: True).
@@ -1573,18 +1637,23 @@
         automatically.
 
         :param command_string: The command to be executed on the remote device.
 
         :param expect_string: Regular expression pattern to use for determining end of output.
             If left blank will default to being based on router prompt.
 
+        :param read_timeout: Maximum time to wait looking for pattern. Will raise ReadTimeout
+            if timeout is exceeded.
+
         :param delay_factor: Deprecated in Netmiko 4.x. Will be eliminated in Netmiko 5.
 
         :param max_loops: Deprecated in Netmiko 4.x. Will be eliminated in Netmiko 5.
 
+        :param auto_find_prompt: Use find_prompt() to override base prompt
+
         :param strip_prompt: Remove the trailing router prompt from the output (default: True).
 
         :param strip_command: Remove the echo of the command from the output (default: True).
 
         :param normalize: Ensure the proper enter is sent at end of command (default: True).
 
         :param use_textfsm: Process command output through TextFSM template (default: False).
@@ -1891,61 +1960,67 @@
         return check_string in output
 
     def enable(
         self,
         cmd: str = "",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """Enter enable mode.
 
         :param cmd: Device command to enter enable mode
 
         :param pattern: pattern to search for indicating device is waiting for password
 
         :param enable_pattern: pattern indicating you have entered enable mode
 
+        :param check_state: Determine whether we are already in enable_mode using
+                check_enable_mode() before trying to elevate privileges (default: True)
+
         :param re_flags: Regular expression flags used in conjunction with pattern
         """
         output = ""
         msg = (
             "Failed to enter enable mode. Please ensure you pass "
             "the 'secret' argument to ConnectHandler."
         )
 
-        # Check if in enable mode
-        if not self.check_enable_mode():
-            # Send "enable" mode command
-            self.write_channel(self.normalize_cmd(cmd))
-            try:
-                # Read the command echo
-                end_data = ""
-                if self.global_cmd_verify is not False:
-                    output += self.read_until_pattern(pattern=re.escape(cmd.strip()))
-                    end_data = output.split(cmd.strip())[-1]
-
-                # Search for trailing prompt or password pattern
-                if pattern not in output and self.base_prompt not in end_data:
-                    output += self.read_until_prompt_or_pattern(
-                        pattern=pattern, re_flags=re_flags
-                    )
-                # Send the "secret" in response to password pattern
-                if re.search(pattern, output):
-                    self.write_channel(self.normalize_cmd(self.secret))
-                    output += self.read_until_prompt()
-
-                # Search for terminating pattern if defined
-                if enable_pattern and not re.search(enable_pattern, output):
-                    output += self.read_until_pattern(pattern=enable_pattern)
-                else:
-                    if not self.check_enable_mode():
-                        raise ValueError(msg)
-            except NetmikoTimeoutException:
-                raise ValueError(msg)
+        # Check if in enable mode already.
+        if check_state and self.check_enable_mode():
+            return output
+
+        # Send "enable" mode command
+        self.write_channel(self.normalize_cmd(cmd))
+        try:
+            # Read the command echo
+            if self.global_cmd_verify is not False:
+                output += self.read_until_pattern(pattern=re.escape(cmd.strip()))
+
+            # Search for trailing prompt or password pattern
+            output += self.read_until_prompt_or_pattern(
+                pattern=pattern, re_flags=re_flags
+            )
+
+            # Send the "secret" in response to password pattern
+            if re.search(pattern, output):
+                self.write_channel(self.normalize_cmd(self.secret))
+                output += self.read_until_prompt()
+
+            # Search for terminating pattern if defined
+            if enable_pattern and not re.search(enable_pattern, output):
+                output += self.read_until_pattern(pattern=enable_pattern)
+            else:
+                if not self.check_enable_mode():
+                    raise ValueError(msg)
+
+        except NetmikoTimeoutException:
+            raise ValueError(msg)
+
         return output
 
     def exit_enable_mode(self, exit_command: str = "") -> str:
         """Exit enable mode.
 
         :param exit_command: Command that exits the session from privileged mode
         :type exit_command: str
@@ -1964,14 +2039,18 @@
         """Checks if the device is in configuration mode or not.
 
         :param check_string: Identification of configuration mode from the device
         :type check_string: str
 
         :param pattern: Pattern to terminate reading of channel
         :type pattern: str
+
+        :param force_regex: Use regular expression pattern to find check_string in output
+        :type force_regex: bool
+
         """
         self.write_channel(self.RETURN)
         # You can encounter an issue here (on router name changes) prefer delay-based solution
         if not pattern:
             output = self.read_channel_timing(read_timeout=10.0)
         else:
             output = self.read_until_pattern(pattern=pattern)
@@ -2089,15 +2168,16 @@
 
         :param max_loops: Deprecated in Netmiko 4.x. Will be eliminated in Netmiko 5.
 
         :param strip_prompt: Determines whether or not to strip the prompt
 
         :param strip_command: Determines whether or not to strip the command
 
-        :param read_timeout: Absolute timer to send to read_channel_timing. Should be rarely needed.
+        :param read_timeout: Absolute timer to send to read_channel_timing. Also adjusts
+        read_timeout in read_until_pattern calls.
 
         :param config_mode_command: The command to enter into config mode
 
         :param cmd_verify: Whether or not to verify command echo for each command in config_set
 
         :param enter_config_mode: Do you enter config mode before sending config commands
 
@@ -2195,19 +2275,23 @@
                 output += self.read_channel_timing(read_timeout=read_timeout)
 
         else:
             for cmd in config_commands:
                 self.write_channel(self.normalize_cmd(cmd))
 
                 # Make sure command is echoed
-                output += self.read_until_pattern(pattern=re.escape(cmd.strip()))
+                output += self.read_until_pattern(
+                    pattern=re.escape(cmd.strip()), read_timeout=read_timeout
+                )
 
                 # Read until next prompt or terminator (#); the .*$ forces read of entire line
                 pattern = f"(?:{re.escape(self.base_prompt)}.*$|{terminator}.*$)"
-                output += self.read_until_pattern(pattern=pattern, re_flags=re.M)
+                output += self.read_until_pattern(
+                    pattern=pattern, read_timeout=read_timeout, re_flags=re.M
+                )
 
                 if error_pattern:
                     if re.search(error_pattern, output, flags=re.M):
                         msg = f"Invalid input detected at command: {cmd}"
                         raise ConfigInvalidException(msg)
 
         if exit_config_mode:
```

### Comparing `netmiko-4.1.2/netmiko/broadcom/broadcom_icos_ssh.py` & `netmiko-4.2.0/netmiko/broadcom/broadcom_icos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/brocade/brocade_fos_ssh.py` & `netmiko-4.2.0/netmiko/brocade/brocade_fos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/calix/calix_b6.py` & `netmiko-4.2.0/netmiko/calix/calix_b6.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cdot/cdot_cros_ssh.py` & `netmiko-4.2.0/netmiko/cdot/cdot_cros_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/centec/centec_os.py` & `netmiko-4.2.0/netmiko/centec/centec_os.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/channel.py` & `netmiko-4.2.0/netmiko/channel.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/checkpoint/checkpoint_gaia_ssh.py` & `netmiko-4.2.0/netmiko/checkpoint/checkpoint_gaia_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/ciena/ciena_saos.py` & `netmiko-4.2.0/netmiko/ciena/ciena_saos.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,41 @@
 class CienaSaosBase(NoEnable, NoConfig, BaseConnection):
     """
     Ciena SAOS support.
 
     Implements methods for interacting Ciena Saos devices.
     """
 
+    prompt_pattern = r"[>#$]"
+
+    def set_base_prompt(
+        self,
+        pri_prompt_terminator: str = "",
+        alt_prompt_terminator: str = "",
+        delay_factor: float = 1.0,
+        pattern: Optional[str] = None,
+    ) -> str:
+        """Ciena can use '>', '$', '#' for prompt terminator depending on the device."""
+        prompt = self.find_prompt(delay_factor=delay_factor)
+
+        pattern = rf"^.+{self.prompt_pattern}$"
+        if re.search(pattern, prompt):
+            raise ValueError(f"Router prompt not found: {repr(prompt)}")
+        # Strip off trailing terminator
+        self.base_prompt = prompt[:-1]
+        return self.base_prompt
+
     def session_preparation(self) -> None:
-        self._test_channel_read(pattern=r"[>#]")
+        self._test_channel_read(pattern=self.prompt_pattern)
         self.set_base_prompt()
         self.disable_paging(command="system shell session set more off")
 
     def _enter_shell(self) -> str:
         """Enter the Bourne Shell."""
-        output = self._send_command_str("diag shell", expect_string=r"[$#>]")
+        output = self._send_command_str("diag shell", expect_string=self.prompt_pattern)
         if "SHELL PARSER FAILURE" in output:
             msg = "SCP support on Ciena SAOS requires 'diag shell' permissions"
             raise ValueError(msg)
         return output
 
     def _return_cli(self) -> str:
         """Return to the Ciena SAOS CLI."""
```

### Comparing `netmiko-4.1.2/netmiko/cisco/__init__.py` & `netmiko-4.2.0/netmiko/cisco/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 from netmiko.cisco.cisco_ios import CiscoIosFileTransfer
 from netmiko.cisco.cisco_ios import InLineTransfer
 from netmiko.cisco.cisco_asa_ssh import CiscoAsaSSH, CiscoAsaFileTransfer
 from netmiko.cisco.cisco_ftd_ssh import CiscoFtdSSH
 from netmiko.cisco.cisco_nxos_ssh import CiscoNxosSSH, CiscoNxosFileTransfer
 from netmiko.cisco.cisco_xr import CiscoXrSSH, CiscoXrTelnet, CiscoXrFileTransfer
 from netmiko.cisco.cisco_wlc_ssh import CiscoWlcSSH
+from netmiko.cisco.cisco_s200 import CiscoS200SSH
+from netmiko.cisco.cisco_s200 import CiscoS200Telnet
 from netmiko.cisco.cisco_s300 import CiscoS300SSH
 from netmiko.cisco.cisco_s300 import CiscoS300Telnet
 from netmiko.cisco.cisco_tp_tcce import CiscoTpTcCeSSH
 from netmiko.cisco.cisco_viptela import CiscoViptelaSSH
 
 __all__ = [
     "CiscoIosSSH",
     "CiscoIosTelnet",
     "CiscoAsaSSH",
     "CiscoFtdSSH",
     "CiscoNxosSSH",
     "CiscoXrSSH",
     "CiscoXrTelnet",
     "CiscoWlcSSH",
+    "CiscoS200SSH",
+    "CiscoS200Telnet",
     "CiscoS300SSH",
     "CiscoS300Telnet",
     "CiscoTpTcCeSSH",
     "CiscoViptelaSSH",
     "CiscoIosBase",
     "CiscoIosFileTransfer",
     "InLineTransfer",
```

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_asa_ssh.py` & `netmiko-4.2.0/netmiko/cisco/cisco_asa_ssh.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,18 +50,23 @@
         return super().check_config_mode(check_string=check_string, pattern=pattern)
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = r"\#",
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return super().enable(
-            cmd=cmd, pattern=pattern, enable_pattern=enable_pattern, re_flags=re_flags
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def send_command_timing(
         self, *args: Any, **kwargs: Any
     ) -> Union[str, List[Any], Dict[str, Any]]:
         """
         If the ASA is in multi-context mode, then the base_prompt needs to be
```

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_ftd_ssh.py` & `netmiko-4.2.0/netmiko/cisco/cisco_ftd_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_ios.py` & `netmiko-4.2.0/netmiko/cisco/cisco_ios.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_nxos_ssh.py` & `netmiko-4.2.0/netmiko/cisco/cisco_nxos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_s300.py` & `netmiko-4.2.0/netmiko/cisco/cisco_s300.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_tp_tcce.py` & `netmiko-4.2.0/netmiko/cisco/cisco_tp_tcce.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_viptela.py` & `netmiko-4.2.0/netmiko/cisco/cisco_viptela.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_wlc_ssh.py` & `netmiko-4.2.0/netmiko/cisco/cisco_wlc_ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,16 @@
                 break
 
             # Don't automatically save the config (user's responsibility)
             if "Would you like to save them now" in output:
                 self._session_log_fin = True
                 self.write_channel("n" + self.RETURN)
 
+            time.sleep(0.5)
+
             try:
                 self.write_channel(self.RETURN)
             except socket.error:
                 break
             count += 1
 
     def check_config_mode(
```

### Comparing `netmiko-4.1.2/netmiko/cisco/cisco_xr.py` & `netmiko-4.2.0/netmiko/cisco/cisco_xr.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,22 +142,23 @@
             output += new_data
             new_data = self._send_command_str(
                 "y",
                 expect_string=r"#",
                 strip_prompt=False,
                 strip_command=False,
                 read_timeout=read_timeout,
+                cmd_verify=False,
             )
         output += new_data
         if error_marker in output:
             raise ValueError(f"Commit failed with the following errors:\n\n{output}")
         if alt_error_marker in output:
             # Other commits occurred, don't proceed with commit
             output += self._send_command_timing_str(
-                "no", strip_prompt=False, strip_command=False
+                "no", strip_prompt=False, strip_command=False, cmd_verify=False
             )
             raise ValueError(f"Commit failed with the following errors:\n\n{output}")
 
         return output
 
     def check_config_mode(
         self,
```

### Comparing `netmiko-4.1.2/netmiko/cisco_base_connection.py` & `netmiko-4.2.0/netmiko/cisco_base_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,34 +15,37 @@
         return super().check_enable_mode(check_string=check_string)
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """Enter enable mode."""
         return super().enable(
-            cmd=cmd, pattern=pattern, enable_pattern=enable_pattern, re_flags=re_flags
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def exit_enable_mode(self, exit_command: str = "disable") -> str:
         """Exits enable (privileged exec) mode."""
         return super().exit_enable_mode(exit_command=exit_command)
 
     def check_config_mode(
         self, check_string: str = ")#", pattern: str = "", force_regex: bool = False
     ) -> bool:
-        """
-        Checks if the device is in configuration mode or not.
-
-        Cisco IOS devices abbreviate the prompt at 20 chars in config mode
-        """
-        return super().check_config_mode(check_string=check_string, pattern=pattern)
+        """Checks if the device is in configuration mode or not."""
+        return super().check_config_mode(
+            check_string=check_string, pattern=pattern, force_regex=force_regex
+        )
 
     def config_mode(
         self,
         config_command: str = "configure terminal",
         pattern: str = "",
         re_flags: int = 0,
     ) -> str:
```

### Comparing `netmiko-4.1.2/netmiko/citrix/netscaler_ssh.py` & `netmiko-4.2.0/netmiko/citrix/netscaler_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cli_tools/netmiko_cfg.py` & `netmiko-4.2.0/netmiko/cli_tools/netmiko_cfg.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cli_tools/netmiko_grep.py` & `netmiko-4.2.0/netmiko/cli_tools/netmiko_grep.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cli_tools/netmiko_show.py` & `netmiko-4.2.0/netmiko/cli_tools/netmiko_show.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/cloudgenix/cloudgenix_ion.py` & `netmiko-4.2.0/netmiko/cloudgenix/cloudgenix_ion.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/coriant/coriant_ssh.py` & `netmiko-4.2.0/netmiko/coriant/coriant_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/dell/__init__.py` & `netmiko-4.2.0/netmiko/dell/__init__.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/dell/dell_dnos6.py` & `netmiko-4.2.0/netmiko/dell/dell_dnos6.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/dell/dell_isilon_ssh.py` & `netmiko-4.2.0/netmiko/dell/dell_isilon_ssh.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,29 +60,35 @@
         return super().check_enable_mode(check_string=check_string)
 
     def enable(
         self,
         cmd: str = "sudo su",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
+
         delay_factor = self.select_delay_factor(delay_factor=1)
         output = ""
+
+        if check_state and self.check_enable_mode():
+            return output
+
+        output += self._send_command_timing_str(
+            cmd, strip_prompt=False, strip_command=False
+        )
+        if re.search(pattern, output, flags=re_flags):
+            self.write_channel(self.normalize_cmd(self.secret))
+        output += self.read_until_pattern(pattern=r"#.*$")
+        time.sleep(1 * delay_factor)
+        self._set_prompt(prompt_terminator="#")
         if not self.check_enable_mode():
-            output += self._send_command_timing_str(
-                cmd, strip_prompt=False, strip_command=False
-            )
-            if re.search(pattern, output, flags=re_flags):
-                self.write_channel(self.normalize_cmd(self.secret))
-            output += self.read_until_pattern(pattern=r"#.*$")
-            time.sleep(1 * delay_factor)
-            self._set_prompt(prompt_terminator="#")
-            if not self.check_enable_mode():
-                raise ValueError("Failed to enter enable mode")
+            raise ValueError("Failed to enter enable mode")
+
         return output
 
     def exit_enable_mode(self, exit_command: str = "exit") -> str:
         return super().exit_enable_mode(exit_command=exit_command)
 
     def check_config_mode(
         self, check_string: str = "#", pattern: str = "", force_regex: bool = False
```

### Comparing `netmiko-4.1.2/netmiko/dell/dell_os10_ssh.py` & `netmiko-4.2.0/netmiko/dell/dell_os10_ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,34 @@
 import os
 import re
 
 
 class DellOS10SSH(CiscoSSHConnection):
     """Dell EMC Networking OS10 Driver - supports dellos10."""
 
+    def session_preparation(self) -> None:
+        """Prepare the session after the connection has been established."""
+        self._test_channel_read(pattern=r"[>#]")
+        self.set_base_prompt()
+        self.set_terminal_width()
+        self.disable_paging()
+
+    def check_config_mode(
+        self,
+        check_string: str = ")#",
+        pattern: str = r"[>#]",
+        force_regex: bool = False,
+    ) -> bool:
+        """
+        Checks if the device is in configuration mode or not.
+        """
+        return super().check_config_mode(
+            check_string=check_string, pattern=pattern, force_regex=force_regex
+        )
+
     def save_config(
         self,
         cmd: str = "copy running-configuration startup-configuration",
         confirm: bool = False,
         confirm_response: str = "",
     ) -> str:
         """Saves Config"""
```

### Comparing `netmiko-4.1.2/netmiko/dell/dell_powerconnect.py` & `netmiko-4.2.0/netmiko/dell/dell_powerconnect.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/dell/dell_sonic_ssh.py` & `netmiko-4.2.0/netmiko/dell/dell_sonic_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/dlink/dlink_ds.py` & `netmiko-4.2.0/netmiko/dlink/dlink_ds.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/eltex/eltex_esr_ssh.py` & `netmiko-4.2.0/netmiko/eltex/eltex_esr_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/eltex/eltex_ssh.py` & `netmiko-4.2.0/netmiko/eltex/eltex_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/endace/endace_ssh.py` & `netmiko-4.2.0/netmiko/endace/endace_ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,23 @@
         self.disable_paging(command="no cli session paging enable")
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return super().enable(
-            cmd=cmd, pattern=pattern, enable_pattern=enable_pattern, re_flags=re_flags
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def check_config_mode(
         self,
         check_string: str = "(config) #",
         pattern: str = "",
         force_regex: bool = False,
```

### Comparing `netmiko-4.1.2/netmiko/enterasys/enterasys_ssh.py` & `netmiko-4.2.0/netmiko/enterasys/enterasys_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/ericsson/ericsson_ipos.py` & `netmiko-4.2.0/netmiko/ericsson/ericsson_ipos.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,23 @@
         return super().check_enable_mode(check_string=check_string)
 
     def enable(
         self,
         cmd: str = "enable 15",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return super().enable(
-            cmd=cmd, pattern=pattern, enable_pattern=enable_pattern, re_flags=re_flags
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def exit_enable_mode(self, exit_command: str = "disable") -> str:
         return super().exit_enable_mode(exit_command=exit_command)
 
     def check_config_mode(
         self, check_string: str = ")#", pattern: str = "", force_regex: bool = False
```

### Comparing `netmiko-4.1.2/netmiko/exceptions.py` & `netmiko-4.2.0/netmiko/exceptions.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/extreme/__init__.py` & `netmiko-4.2.0/netmiko/extreme/__init__.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/extreme/extreme_ers_ssh.py` & `netmiko-4.2.0/netmiko/extreme/extreme_ers_ssh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Netmiko support for Extreme Ethernet Routing Switch."""
 import re
 from netmiko.cisco_base_connection import CiscoSSHConnection
 from netmiko.exceptions import NetmikoAuthenticationException
 
 # Extreme ERS presents Enter Ctrl-Y to begin.
 CTRL_Y = "\x19"
+CTRL_C = "\x63"
 
 
 class ExtremeErsSSH(CiscoSSHConnection):
     """Netmiko support for Extreme Ethernet Routing Switch."""
 
     prompt_pattern = r"(?m:[>#]\s*$)"  # force re.Multiline
 
@@ -29,29 +30,36 @@
         Newer devices this is after SSH-login.
         """
 
         output = ""
         uname = "sername"
         password = "ssword"
         cntl_y = "Ctrl-Y"
-        pattern = rf"(?:{uname}|{password}|{cntl_y}|{self.prompt_pattern})"
+        enter_msg = "Press ENTER to continue"
+        pattern = (
+            rf"(?:{uname}|{password}|{cntl_y}|{enter_msg}|{self.prompt_pattern}|Menu)"
+        )
         while True:
             new_data = self.read_until_pattern(pattern=pattern, read_timeout=25.0)
             output += new_data
             if re.search(self.prompt_pattern, new_data):
                 return
 
             if cntl_y in new_data:
                 self.write_channel(CTRL_Y)
+            elif "Press ENTER" in new_data:
+                self.write_channel(self.RETURN)
             elif uname in new_data:
                 assert isinstance(self.username, str)
                 self.write_channel(self.username + self.RETURN)
             elif password in new_data:
                 assert isinstance(self.password, str)
                 self.write_channel(self.password + self.RETURN)
+            elif "Menu" in new_data:
+                self.write_channel(CTRL_C)
             else:
                 msg = f"""
 
 Failed to login to Extreme ERS Device.
 
 Pattern not detected: {pattern}
 output:
```

### Comparing `netmiko-4.1.2/netmiko/extreme/extreme_exos.py` & `netmiko-4.2.0/netmiko/extreme/extreme_exos.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/extreme/extreme_netiron.py` & `netmiko-4.2.0/netmiko/extreme/extreme_netiron.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/extreme/extreme_nos_ssh.py` & `netmiko-4.2.0/netmiko/extreme/extreme_nos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/extreme/extreme_slx_ssh.py` & `netmiko-4.2.0/netmiko/extreme/extreme_slx_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/extreme/extreme_tierraos_ssh.py` & `netmiko-4.2.0/netmiko/extreme/extreme_tierraos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/extreme/extreme_vsp_ssh.py` & `netmiko-4.2.0/netmiko/extreme/extreme_vsp_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/f5/f5_tmsh_ssh.py` & `netmiko-4.2.0/netmiko/f5/f5_tmsh_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/flexvnf/flexvnf_ssh.py` & `netmiko-4.2.0/netmiko/flexvnf/flexvnf_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/hp/hp_comware.py` & `netmiko-4.2.0/netmiko/hp/hp_comware.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         return self.base_prompt
 
     def enable(
         self,
         cmd: str = "system-view",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """enable mode on Comware is system-view."""
         return self.config_mode(config_command=cmd)
 
     def exit_enable_mode(self, exit_command: str = "return") -> str:
         """enable mode on Comware is system-view."""
```

### Comparing `netmiko-4.1.2/netmiko/hp/hp_procurve.py` & `netmiko-4.2.0/netmiko/hp/hp_procurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,21 +76,23 @@
         return super().check_config_mode(check_string=check_string, pattern=pattern)
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "password",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
         default_username: str = "",
     ) -> str:
         """Enter enable mode"""
 
-        if self.check_enable_mode():
+        if check_state and self.check_enable_mode():
             return ""
+
         if not default_username:
             default_username = self.username
 
         output = ""
         username_pattern = r"(username|login|user name)"
         pwd_pattern = pattern
         prompt_pattern = r"[>#]"
```

### Comparing `netmiko-4.1.2/netmiko/huawei/huawei.py` & `netmiko-4.2.0/netmiko/huawei/huawei.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from typing import Optional, Any, Union, Sequence, Iterator, TextIO
-import time
 import re
 import warnings
 
 from netmiko.no_enable import NoEnable
 from netmiko.base_connection import DELAY_FACTOR_DEPR_SIMPLE_MSG
 from netmiko.cisco_base_connection import CiscoBaseConnection
 from netmiko.exceptions import NetmikoAuthenticationException
 from netmiko import log
 
 
 class HuaweiBase(NoEnable, CiscoBaseConnection):
+    prompt_pattern = r"[\]>]"
+    password_change_prompt = r"(?:Change now|Please choose)"
+    prompt_or_password_change = rf"(?:Change now|Please choose|{prompt_pattern})"
+
     def session_preparation(self) -> None:
         """Prepare the session after the connection has been established."""
         self.ansi_escape_codes = True
         # The _test_channel_read happens in special_login_handler()
         self.set_base_prompt()
         self.disable_paging(command="screen-length 0 temporary")
 
@@ -86,115 +89,121 @@
         self.base_prompt = prompt
         log.debug(f"prompt: {self.base_prompt}")
         return self.base_prompt
 
     def save_config(
         self, cmd: str = "save", confirm: bool = True, confirm_response: str = "y"
     ) -> str:
-        """Save Config for HuaweiSSH"""
-        return super().save_config(
-            cmd=cmd, confirm=confirm, confirm_response=confirm_response
-        )
+        """Save Config for HuaweiSSH
+
+        Expected behavior:
+
+        ######################################################################
+        Warning: The current configuration will be written to the device.
+        Are you sure to continue?[Y/N]:y
+         It will take several minutes to save configuration file, please wait.....................
+         Configuration file had been saved successfully
+         Note: The configuration file will take effect after being activated
+        ######################################################################
+        """
+
+        # Huawei devices might break if you try to use send_command_timing() so use send_command()
+        # instead.
+        if confirm:
+            pattern = rf"(?:Are you sure|{self.prompt_pattern})"
+            output = self._send_command_str(
+                command_string=cmd,
+                expect_string=pattern,
+                strip_prompt=False,
+                strip_command=False,
+                read_timeout=100.0,
+            )
+            if confirm_response and "Are you sure" in output:
+                output += self._send_command_str(
+                    command_string=confirm_response,
+                    expect_string=self.prompt_pattern,
+                    strip_prompt=False,
+                    strip_command=False,
+                    read_timeout=100.0,
+                )
+        # no confirm.
+        else:
+            # Some devices are slow so match on trailing-prompt if you can
+            output = self._send_command_str(
+                command_string=cmd,
+                strip_prompt=False,
+                strip_command=False,
+                read_timeout=100.0,
+            )
+        return output
 
     def cleanup(self, command: str = "quit") -> None:
         return super().cleanup(command=command)
 
 
 class HuaweiSSH(HuaweiBase):
     """Huawei SSH driver."""
 
     def special_login_handler(self, delay_factor: float = 1.0) -> None:
         # Huawei prompts for password change before displaying the initial base prompt.
         # Search for that password change prompt or for base prompt.
-        password_change_prompt = r"(Change now|Please choose)"
-        prompt_or_password_change = r"(?:Change now|Please choose|[>\]])"
-        data = self.read_until_pattern(pattern=prompt_or_password_change)
-        if re.search(password_change_prompt, data):
+        data = self.read_until_pattern(pattern=self.prompt_or_password_change)
+        if re.search(self.password_change_prompt, data):
             self.write_channel("N" + self.RETURN)
-            self.read_until_pattern(pattern=r"[>\]]")
+            self.read_until_pattern(pattern=self.prompt_pattern)
 
 
 class HuaweiTelnet(HuaweiBase):
     """Huawei Telnet driver."""
 
     def telnet_login(
         self,
-        pri_prompt_terminator: str = r"]\s*$",
-        alt_prompt_terminator: str = r">\s*$",
+        pri_prompt_terminator: str = r"",
+        alt_prompt_terminator: str = r"",
         username_pattern: str = r"(?:user:|username|login|user name)",
         pwd_pattern: str = r"assword",
         delay_factor: float = 1.0,
         max_loops: int = 20,
     ) -> str:
         """Telnet login for Huawei Devices"""
-
-        delay_factor = self.select_delay_factor(delay_factor)
-        password_change_prompt = r"(Change now|Please choose 'YES' or 'NO').+"
-        combined_pattern = r"({}|{}|{})".format(
-            pri_prompt_terminator, alt_prompt_terminator, password_change_prompt
-        )
-
         output = ""
         return_msg = ""
-        i = 1
-        while i <= max_loops:
-            try:
-                # Search for username pattern / send username
-                output = self.read_until_pattern(
-                    pattern=username_pattern, re_flags=re.I
-                )
-                return_msg += output
-                self.write_channel(self.username + self.TELNET_RETURN)
-
-                # Search for password pattern / send password
-                output = self.read_until_pattern(pattern=pwd_pattern, re_flags=re.I)
-                return_msg += output
-                assert self.password is not None
-                self.write_channel(self.password + self.TELNET_RETURN)
-
-                # Waiting for combined output
-                output = self.read_until_pattern(pattern=combined_pattern)
+        try:
+            # Search for username pattern / send username
+            output = self.read_until_pattern(pattern=username_pattern, re_flags=re.I)
+            return_msg += output
+            self.write_channel(self.username + self.TELNET_RETURN)
+
+            # Search for password pattern / send password
+            output = self.read_until_pattern(pattern=pwd_pattern, re_flags=re.I)
+            return_msg += output
+            assert self.password is not None
+            self.write_channel(self.password + self.TELNET_RETURN)
+
+            # Waiting for the prompt or password change message
+            output = self.read_until_pattern(pattern=self.prompt_or_password_change)
+            return_msg += output
+
+            # If password change prompt, send "N"
+            if re.search(self.password_change_prompt, output):
+                self.write_channel("N" + self.TELNET_RETURN)
+                output = self.read_until_pattern(pattern=self.prompt_pattern)
                 return_msg += output
-
-                # Search for password change prompt, send "N"
-                if re.search(password_change_prompt, output):
-                    self.write_channel("N" + self.TELNET_RETURN)
-                    output = self.read_until_pattern(pattern=combined_pattern)
-                    return_msg += output
-
-                # Check if proper data received
-                if re.search(pri_prompt_terminator, output, flags=re.M) or re.search(
-                    alt_prompt_terminator, output, flags=re.M
-                ):
-                    return return_msg
-
-                self.write_channel(self.TELNET_RETURN)
-                time.sleep(0.5 * delay_factor)
-                i += 1
-
-            except EOFError:
-                assert self.remote_conn is not None
-                self.remote_conn.close()
-                msg = f"Login failed: {self.host}"
-                raise NetmikoAuthenticationException(msg)
-
-        # Last try to see if we already logged in
-        self.write_channel(self.TELNET_RETURN)
-        time.sleep(0.5 * delay_factor)
-        output = self.read_channel()
-        return_msg += output
-        if re.search(pri_prompt_terminator, output, flags=re.M) or re.search(
-            alt_prompt_terminator, output, flags=re.M
-        ):
-            return return_msg
-
-        assert self.remote_conn is not None
-        self.remote_conn.close()
-        msg = f"Login failed: {self.host}"
-        raise NetmikoAuthenticationException(msg)
+                return return_msg
+            elif re.search(self.prompt_pattern, output):
+                return return_msg
+
+            # Should never be here
+            raise EOFError
+
+        except EOFError:
+            assert self.remote_conn is not None
+            self.remote_conn.close()
+            msg = f"Login failed: {self.host}"
+            raise NetmikoAuthenticationException(msg)
 
 
 class HuaweiVrpv8SSH(HuaweiSSH):
     def send_config_set(
         self,
         config_commands: Union[str, Sequence[str], Iterator[str], TextIO, None] = None,
         exit_config_mode: bool = False,
```

### Comparing `netmiko-4.1.2/netmiko/huawei/huawei_smartax.py` & `netmiko-4.2.0/netmiko/huawei/huawei_smartax.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,26 @@
 from netmiko.cisco_base_connection import CiscoBaseConnection
 from netmiko import log
 
 
 class HuaweiSmartAXSSH(CiscoBaseConnection):
     """Supports Huawei SmartAX and OLT."""
 
+    prompt_pattern = r"[>$]"
+
     def session_preparation(self) -> None:
         """Prepare the session after the connection has been established."""
         self.ansi_escape_codes = True
-        self._test_channel_read(pattern=r"[>#]")
+
+        data = self._test_channel_read(pattern=f"YES.NO|{self.prompt_pattern}")
+        # Huawei OLT might put a post-login banner that requires 'yes' to be sent.
+        if re.search(r"YES.NO", data):
+            self.write_channel(f"yes{self.RETURN}")
+            self._test_channel_read(pattern=self.prompt_pattern)
+
         self.set_base_prompt()
         self._disable_smart_interaction()
         self.disable_paging()
 
     def strip_ansi_escape_codes(self, string_buffer: str) -> str:
         """
         Huawei does a strange thing where they add a space and then add ESC[1D
@@ -87,18 +95,23 @@
         return super().check_enable_mode(check_string=check_string)
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return super().enable(
-            cmd=cmd, pattern=pattern, re_flags=re_flags, enable_pattern=enable_pattern
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def set_base_prompt(
         self,
         pri_prompt_terminator: str = ">",
         alt_prompt_terminator: str = "#",
         delay_factor: float = 1.0,
```

### Comparing `netmiko-4.1.2/netmiko/ipinfusion/ipinfusion_ocnos.py` & `netmiko-4.2.0/netmiko/ipinfusion/ipinfusion_ocnos.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/juniper/juniper.py` & `netmiko-4.2.0/netmiko/juniper/juniper.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,16 +189,17 @@
         if and_quit:
             command_string += " and-quit"
 
         # Enter config mode (if necessary)
         output = self.config_mode()
         # and_quit will get out of config mode on commit
 
-        expect_string = re.escape(self.base_prompt) if and_quit else None
-
+        # hostname might change on commit, and-quit might result in exiting config mode.
+        re_prompt = re.escape(self.base_prompt)
+        expect_string = rf"(?:{re_prompt}|[>#])"
         output += self._send_command_str(
             command_string,
             expect_string=expect_string,
             strip_prompt=False,
             strip_command=False,
             read_timeout=read_timeout,
         )
```

### Comparing `netmiko-4.1.2/netmiko/juniper/juniper_screenos.py` & `netmiko-4.2.0/netmiko/juniper/juniper_screenos.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/keymile/keymile_nos_ssh.py` & `netmiko-4.2.0/netmiko/keymile/keymile_nos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/keymile/keymile_ssh.py` & `netmiko-4.2.0/netmiko/keymile/keymile_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/linux/linux_ssh.py` & `netmiko-4.2.0/netmiko/linux/linux_ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,44 +111,48 @@
         return output
 
     def enable(
         self,
         cmd: str = "sudo -s",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """Attempt to become root."""
         msg = """
 
 Netmiko failed to elevate privileges.
 
 Please ensure you pass the sudo password into ConnectHandler
 using the 'secret' argument and that the user has sudo
 permissions.
 
 """
 
         output = ""
-        if not self.check_enable_mode():
-            self.write_channel(self.normalize_cmd(cmd))
-            # Failed "sudo -s" will put "#" in output so have to delineate further
-            root_prompt = rf"(?m:{LINUX_PROMPT_ROOT}\s*$)"
-            prompt_or_password = rf"({root_prompt}|{pattern})"
-            output += self.read_until_pattern(pattern=prompt_or_password)
-            if re.search(pattern, output, flags=re_flags):
-                self.write_channel(self.normalize_cmd(self.secret))
-                try:
-                    output += self.read_until_pattern(pattern=root_prompt)
-                except ReadTimeout:
-                    raise ValueError(msg)
-            # Nature of prompt might change with the privilege escalation
-            self.set_base_prompt(pattern=root_prompt)
-            if not self.check_enable_mode():
+        if check_state and self.check_enable_mode():
+            return output
+
+        self.write_channel(self.normalize_cmd(cmd))
+
+        # Failed "sudo -s" will put "#" in output so have to delineate further
+        root_prompt = rf"(?m:{LINUX_PROMPT_ROOT}\s*$)"
+        prompt_or_password = rf"({root_prompt}|{pattern})"
+        output += self.read_until_pattern(pattern=prompt_or_password)
+        if re.search(pattern, output, flags=re_flags):
+            self.write_channel(self.normalize_cmd(self.secret))
+            try:
+                output += self.read_until_pattern(pattern=root_prompt)
+            except ReadTimeout:
                 raise ValueError(msg)
+        # Nature of prompt might change with the privilege escalation
+        self.set_base_prompt(pattern=root_prompt)
+        if not self.check_enable_mode():
+            raise ValueError(msg)
         return output
 
     def cleanup(self, command: str = "exit") -> None:
         """Try to Gracefully exit the SSH session."""
         return super().cleanup(command=command)
 
     def save_config(self, *args: Any, **kwargs: Any) -> str:
```

### Comparing `netmiko-4.1.2/netmiko/mellanox/mellanox_mlnxos_ssh.py` & `netmiko-4.2.0/netmiko/mellanox/mellanox_mlnxos_ssh.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,29 @@
     """Mellanox MLNX-OS Switch support."""
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "#",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """Enter into enable mode."""
+
         output = ""
+        if check_state and self.check_enable_mode():
+            return output
+
+        self.write_channel(self.normalize_cmd(cmd))
+        output += self.read_until_prompt_or_pattern(
+            pattern=pattern, re_flags=re_flags, read_entire_line=True
+        )
         if not self.check_enable_mode():
-            self.write_channel(self.normalize_cmd(cmd))
-            output += self.read_until_prompt_or_pattern(
-                pattern=pattern, re_flags=re_flags, read_entire_line=True
-            )
-            if not self.check_enable_mode():
-                raise ValueError("Failed to enter enable mode.")
+            raise ValueError("Failed to enter enable mode.")
         return output
 
     def config_mode(
         self,
         config_command: str = "config term",
         pattern: str = r"\#",
         re_flags: int = 0,
```

### Comparing `netmiko-4.1.2/netmiko/mikrotik/mikrotik_ssh.py` & `netmiko-4.2.0/netmiko/mikrotik/mikrotik_ssh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from typing import Any, Union, List, Dict, Optional, Callable
 import re
 import os
 
 from netmiko.no_enable import NoEnable
+from netmiko.no_config import NoConfig
 from netmiko.cisco_base_connection import CiscoSSHConnection
 from netmiko.base_connection import BaseConnection
 from netmiko.scp_handler import BaseFileTransfer
 
 
-class MikrotikBase(NoEnable, CiscoSSHConnection):
+class MikrotikBase(NoEnable, NoConfig, CiscoSSHConnection):
     """Common Methods for Mikrotik RouterOS and SwitchOS"""
 
+    prompt_pattern = r"\].*>"
+
     def __init__(self, **kwargs: Any) -> None:
         if kwargs.get("default_enter") is None:
             kwargs["default_enter"] = "\r\n"
 
-        self._in_config_mode = False
-
         return super().__init__(**kwargs)
 
+    def special_login_handler(self, delay_factor: float = 1.0) -> None:
+        # Mikrotik might prompt to read software licenses before displaying the initial prompt.
+        license_prompt = "Do you want to see the software license"
+        combined_pattern = rf"(?:{self.prompt_pattern}|{license_prompt})"
+        data = self.read_until_pattern(pattern=combined_pattern, re_flags=re.I)
+        if license_prompt in data:
+            self.write_channel("n")
+            self.read_until_pattern(pattern=self.prompt_pattern)
+
     def session_preparation(self, *args: Any, **kwargs: Any) -> None:
         """Prepare the session after the connection has been established."""
         self.ansi_escape_codes = True
-        self._test_channel_read(pattern=r"\].*>")
         self.set_base_prompt()
 
     def _modify_connection_params(self) -> None:
         """Append login options to username
         c: disable console colors
         e: enable dumb terminal mode
         t: disable auto detect terminal capabilities
@@ -35,36 +44,14 @@
         """
         self.username += "+ctw511h4098"
 
     def disable_paging(self, *args: Any, **kwargs: Any) -> str:
         """Mikrotik does not have paging by default."""
         return ""
 
-    def save_config(self, *args: Any, **kwargs: Any) -> str:
-        """No save command, all configuration is atomic"""
-        return ""
-
-    def config_mode(
-        self, config_command: str = "", pattern: str = "", re_flags: int = 0
-    ) -> str:
-        """No configuration mode on Mikrotik"""
-        self._in_config_mode = True
-        return ""
-
-    def check_config_mode(
-        self, check_string: str = "", pattern: str = "", force_regex: bool = False
-    ) -> bool:
-        """Checks whether in configuration mode. Returns a boolean."""
-        return self._in_config_mode
-
-    def exit_config_mode(self, exit_config: str = ">", pattern: str = "") -> str:
-        """No configuration mode on Mikrotik"""
-        self._in_config_mode = False
-        return ""
-
     def strip_prompt(self, a_string: str) -> str:
         """Strip the trailing router prompt from the output.
 
         Mikrotik just does a lot of formatting/has ansi escape codes in output so
         we need a special handler here.
 
         There can be two trailing instances of the prompt probably due to
```

### Comparing `netmiko-4.1.2/netmiko/mrv/mrv_lx.py` & `netmiko-4.2.0/netmiko/mrv/mrv_lx.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,25 @@
         return super().check_enable_mode(check_string=check_string)
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "assword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """Enter enable mode."""
-        return super().enable(cmd=cmd, pattern=pattern, re_flags=re_flags)
+        return super().enable(
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
+        )
 
     def save_config(
         self,
         cmd: str = "save config flash",
         confirm: bool = False,
         confirm_response: str = "",
     ) -> str:
```

### Comparing `netmiko-4.1.2/netmiko/mrv/mrv_ssh.py` & `netmiko-4.2.0/netmiko/mrv/mrv_ssh.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,29 +21,32 @@
         self.clear_buffer()
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = r"#",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """Enable mode on MRV uses no password."""
         output = ""
+        if check_state and self.check_enable_mode():
+            return output
+
+        self.write_channel(self.normalize_cmd(cmd))
+        output += self.read_until_prompt_or_pattern(
+            pattern=pattern, re_flags=re_flags, read_entire_line=True
+        )
         if not self.check_enable_mode():
-            self.write_channel(self.normalize_cmd(cmd))
-            output += self.read_until_prompt_or_pattern(
-                pattern=pattern, re_flags=re_flags, read_entire_line=True
+            msg = (
+                "Failed to enter enable mode. Please ensure you pass "
+                "the 'secret' argument to ConnectHandler."
             )
-            if not self.check_enable_mode():
-                msg = (
-                    "Failed to enter enable mode. Please ensure you pass "
-                    "the 'secret' argument to ConnectHandler."
-                )
-                raise ValueError(msg)
+            raise ValueError(msg)
         return output
 
     def save_config(
         self,
         cmd: str = "save config flash",
         confirm: bool = False,
         confirm_response: str = "",
```

### Comparing `netmiko-4.1.2/netmiko/netapp/netapp_cdot_ssh.py` & `netmiko-4.2.0/netmiko/netapp/netapp_cdot_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/netgear/netgear_prosafe_ssh.py` & `netmiko-4.2.0/netmiko/netgear/netgear_prosafe_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/no_config.py` & `netmiko-4.2.0/netmiko/no_config.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/no_enable.py` & `netmiko-4.2.0/netmiko/no_enable.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,13 +21,14 @@
         return True
 
     def enable(
         self,
         cmd: str = "",
         pattern: str = "",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return ""
 
     def exit_enable_mode(self, exit_command: str = "") -> str:
         return ""
```

### Comparing `netmiko-4.1.2/netmiko/nokia/nokia_srl.py` & `netmiko-4.2.0/netmiko/nokia/nokia_srl.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/nokia/nokia_sros.py` & `netmiko-4.2.0/netmiko/nokia/nokia_sros.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,20 +87,27 @@
         return self.read_channel()
 
     def enable(
         self,
         cmd: str = "enable",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """Enable SR OS administrative mode"""
         if "@" not in self.base_prompt:
             cmd = "enable-admin"
-        return super().enable(cmd=cmd, pattern=pattern, re_flags=re_flags)
+        return super().enable(
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
+        )
 
     def check_enable_mode(self, check_string: str = "in admin mode") -> bool:
         """Check if in enable mode."""
         cmd = "enable"
         if "@" not in self.base_prompt:
             cmd = "enable-admin"
         self.write_channel(self.normalize_cmd(cmd))
@@ -171,21 +178,21 @@
     def save_config(self, *args: Any, **kwargs: Any) -> str:
         """Persist configuration to cflash for Nokia SR OS"""
         return self._send_command_str(command_string="/admin save", expect_string=r"#")
 
     def send_config_set(
         self,
         config_commands: Union[str, Sequence[str], Iterator[str], TextIO, None] = None,
-        exit_config_mode: bool = None,
+        exit_config_mode: bool = True,
         **kwargs: Any,
     ) -> str:
         """Model driven CLI requires you not exit from configuration mode."""
-        if exit_config_mode is None:
-            # Set to False if model-driven CLI
-            exit_config_mode = False if "@" in self.base_prompt else True
+        # Set to False if model-driven CLI
+        if "@" in self.base_prompt:
+            exit_config_mode = False
         return super().send_config_set(
             config_commands=config_commands, exit_config_mode=exit_config_mode, **kwargs
         )
 
     def commit(self, *args: Any, **kwargs: Any) -> str:
         """Activate changes from private candidate for Nokia SR OS"""
         output = self._exit_all()
```

### Comparing `netmiko-4.1.2/netmiko/oneaccess/oneaccess_oneos.py` & `netmiko-4.2.0/netmiko/oneaccess/oneaccess_oneos.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """Netmiko driver for OneAccess ONEOS"""
-import time
 from typing import Any
 
 from netmiko.cisco_base_connection import CiscoBaseConnection
 
 
 class OneaccessOneOSBase(CiscoBaseConnection):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Init connection - similar as Cisco"""
         default_enter = kwargs.get("default_enter")
         kwargs["default_enter"] = "\r\n" if default_enter is None else default_enter
         super().__init__(*args, **kwargs)
 
     def session_preparation(self) -> None:
         """Prepare connection - disable paging"""
-        self._test_channel_read()
-        self.set_base_prompt()
-        self.set_terminal_width(command="stty columns 255", pattern="stty")
+
+        self._test_channel_read(pattern=r"[>#]")
         self.disable_paging(command="term len 0")
-        # Clear the read buffer
-        time.sleep(0.3 * self.global_delay_factor)
-        self.clear_buffer()
+
+        # try ONEOS6 command first - fallback to ONEOS5 if it fails
+        self.set_terminal_width(command="screen-width 512", cmd_verify=True)
+        output = self._test_channel_read(pattern=r"[>#]")
+        if "error" in output.lower():
+            self.set_terminal_width(command="stty columns 255", cmd_verify=True)
+        else:
+            # ONEOS6 uses different enter
+            self.RETURN = "\n"
+
+        self._test_channel_read(pattern=r"[>#]")
+        self.set_base_prompt()
 
     def save_config(
         self, cmd: str = "write mem", confirm: bool = False, confirm_response: str = ""
     ) -> str:
         """Save config: write mem"""
         return super().save_config(
             cmd=cmd, confirm=confirm, confirm_response=confirm_response
```

### Comparing `netmiko-4.1.2/netmiko/paloalto/paloalto_panos.py` & `netmiko-4.2.0/netmiko/paloalto/paloalto_panos.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,17 @@
 
         Disable paging (the '--more--' prompts).
         Set the base prompt for interaction ('>').
         """
         self.ansi_escape_codes = True
         self._test_channel_read(pattern=r"[>#]")
         self.disable_paging(
-            command="set cli scripting-mode on", cmd_verify=False, pattern=r" on"
+            command="set cli scripting-mode on",
+            cmd_verify=False,
+            pattern=r"[>#].*mode on",
         )
         self.set_terminal_width(
             command="set cli terminal width 500", pattern=r"set cli terminal width 500"
         )
         self.disable_paging(command="set cli pager off")
         self.set_base_prompt()
```

### Comparing `netmiko-4.1.2/netmiko/pluribus/pluribus_ssh.py` & `netmiko-4.2.0/netmiko/pluribus/pluribus_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/quanta/quanta_mesh_ssh.py` & `netmiko-4.2.0/netmiko/quanta/quanta_mesh_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/rad/rad_etx.py` & `netmiko-4.2.0/netmiko/rad/rad_etx.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/raisecom/raisecom_roap.py` & `netmiko-4.2.0/netmiko/raisecom/raisecom_roap.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/ruckus/ruckus_fastiron.py` & `netmiko-4.2.0/netmiko/ruckus/ruckus_fastiron.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,52 +19,53 @@
         # Clear the read buffer
         time.sleep(0.3 * self.global_delay_factor)
         self.clear_buffer()
 
     def enable(
         self,
         cmd: str = "enable",
-        pattern: str = r"(ssword|User Name)",
+        pattern: str = r"(ssword|User Name|Login)",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """Enter enable mode.
-        With RADIUS can prompt for User Name
+        With RADIUS can prompt for User Name or Login
         SSH@Lab-ICX7250>en
         User Name:service_netmiko
         Password:
         SSH@Lab-ICX7250#
         """
         output = ""
-        if not self.check_enable_mode():
-            count = 4
-            i = 1
-            while i < count:
-                self.write_channel(self.normalize_cmd(cmd))
+        if check_state and self.check_enable_mode():
+            return output
+
+        count = 4
+        i = 1
+        while i < count:
+            self.write_channel(self.normalize_cmd(cmd))
+            new_data = self.read_until_prompt_or_pattern(
+                pattern=pattern, re_flags=re_flags, read_entire_line=True
+            )
+            output += new_data
+            if "User Name" in new_data or "Login" in new_data:
+                self.write_channel(self.normalize_cmd(self.username))
                 new_data = self.read_until_prompt_or_pattern(
                     pattern=pattern, re_flags=re_flags, read_entire_line=True
                 )
                 output += new_data
-                if "User Name" in new_data:
-                    self.write_channel(self.normalize_cmd(self.username))
-                    new_data = self.read_until_prompt_or_pattern(
-                        pattern=pattern, re_flags=re_flags, read_entire_line=True
-                    )
-                    output += new_data
-                if "ssword" in new_data:
-                    self.write_channel(self.normalize_cmd(self.secret))
-                    new_data = self.read_until_prompt(read_entire_line=True)
-                    output += new_data
-                    if not re.search(
-                        r"error.*incorrect.*password", new_data, flags=re.I
-                    ):
-                        break
+            if "ssword" in new_data:
+                self.write_channel(self.normalize_cmd(self.secret))
+                new_data = self.read_until_prompt(read_entire_line=True)
+                output += new_data
+                if not re.search(r"error.*incorrect.*password", new_data, flags=re.I):
+                    break
 
-                time.sleep(1)
-                i += 1
+            time.sleep(1)
+            i += 1
 
         if not self.check_enable_mode():
             msg = (
                 "Failed to enter enable mode. Please ensure you pass "
                 "the 'secret' argument to ConnectHandler."
             )
             raise ValueError(msg)
```

### Comparing `netmiko-4.1.2/netmiko/ruijie/ruijie_os.py` & `netmiko-4.2.0/netmiko/ruijie/ruijie_os.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/scp_functions.py` & `netmiko-4.2.0/netmiko/scp_functions.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/scp_handler.py` & `netmiko-4.2.0/netmiko/scp_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         else:
             raise ValueError("Unexpected value for self.direction")
 
     def _check_file_exists_unix(self, remote_cmd: str = "") -> bool:
         """Check if the dest_file already exists on the file system (return boolean)."""
         if self.direction == "put":
             self.ssh_ctl_chan._enter_shell()
-            remote_cmd = f"/bin/ls {self.file_system}"
+            remote_cmd = f"/bin/ls {self.file_system}/{self.dest_file} 2> /dev/null"
             remote_out = self.ssh_ctl_chan._send_command_str(
                 remote_cmd, expect_string=r"[\$#]"
             )
             self.ssh_ctl_chan._return_cli()
             return self.dest_file in remote_out
         elif self.direction == "get":
             return os.path.exists(self.dest_file)
```

### Comparing `netmiko-4.1.2/netmiko/session_log.py` & `netmiko-4.2.0/netmiko/session_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class SessionLog:
     def __init__(
         self,
         file_name: Optional[str] = None,
         buffered_io: Optional[io.BufferedIOBase] = None,
         file_mode: str = "write",
         file_encoding: str = "utf-8",
-        no_log: Dict[str, Any] = None,
+        no_log: Optional[Dict[str, Any]] = None,
         record_writes: bool = False,
     ) -> None:
         if no_log is None:
             self.no_log = {}
         else:
             self.no_log = no_log
         self.file_name = file_name
```

### Comparing `netmiko-4.1.2/netmiko/sixwind/sixwind_os.py` & `netmiko-4.2.0/netmiko/sixwind/sixwind_os.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.set_base_prompt()
         # Clear the read buffer
         time.sleep(0.3 * self.global_delay_factor)
         self.clear_buffer()
 
     def disable_paging(self, *args: Any, **kwargs: Any) -> str:
         """6WIND requires no-pager at the end of command, not implemented at this time."""
-        pass
+        return ""
 
     def set_base_prompt(
         self,
         pri_prompt_terminator: str = ">",
         alt_prompt_terminator: str = "#",
         delay_factor: float = 1.0,
         pattern: Optional[str] = None,
```

### Comparing `netmiko-4.1.2/netmiko/snmp_autodetect.py` & `netmiko-4.2.0/netmiko/snmp_autodetect.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 autodetect will return None if no match.
 
 SNMPDetect class defaults to SNMPv3
 
 Note, pysnmp is a required dependency for SNMPDetect and is intentionally not included in
 netmiko requirements. So installation of pysnmp might be required.
 """
+import ipaddress
 from typing import Optional, Dict
 from typing.re import Pattern
 import re
 
 try:
     from pysnmp.entity.rfc3413.oneliner import cmdgen
 except ImportError:
@@ -52,15 +53,15 @@
     "hp_procurve": {
         "oid": ".1.3.6.1.2.1.1.1.0",
         "expr": re.compile(r".ProCurve", re.IGNORECASE),
         "priority": 99,
     },
     "cisco_ios": {
         "oid": ".1.3.6.1.2.1.1.1.0",
-        "expr": re.compile(r".*Cisco IOS Software,.*", re.IGNORECASE),
+        "expr": re.compile(r".*Cisco IOS Software.*,.*", re.IGNORECASE),
         "priority": 60,
     },
     "cisco_xe": {
         "oid": ".1.3.6.1.2.1.1.1.0",
         "expr": re.compile(r".*IOS-XE Software,.*", re.IGNORECASE),
         "priority": 99,
     },
@@ -110,14 +111,19 @@
         "priority": 99,
     },
     "dell_powerconnect": {
         "oid": ".1.3.6.1.2.1.1.1.0",
         "expr": re.compile(r"PowerConnect.*", re.IGNORECASE),
         "priority": 50,
     },
+    "mikrotik_routeros": {
+        "oid": ".1.3.6.1.2.1.1.1.0",
+        "expr": re.compile(r".*RouterOS.*", re.IGNORECASE),
+        "priority": 60,
+    },
 }
 
 # Ensure all SNMP device types are supported by Netmiko
 SNMP_MAPPER = {}
 std_device_types = list(CLASS_MAPPER.keys())
 for device_type in std_device_types:
     if SNMP_MAPPER_BASE.get(device_type):
@@ -233,14 +239,24 @@
         self.community = community
         self.user = user
         self.auth_key = auth_key
         self.encrypt_key = encrypt_key
         self.auth_proto = self._snmp_v3_authentication[auth_proto]
         self.encryp_proto = self._snmp_v3_encryption[encrypt_proto]
         self._response_cache: Dict[str, str] = {}
+        self.snmp_target = (self.hostname, self.snmp_port)
+
+        if ipaddress.ip_address(self.hostname).version == 6:
+            self.udp_transport_target = cmdgen.Udp6TransportTarget(
+                self.snmp_target, timeout=1.5, retries=2
+            )
+        else:
+            self.udp_transport_target = cmdgen.UdpTransportTarget(
+                self.snmp_target, timeout=1.5, retries=2
+            )
 
     def _get_snmpv3(self, oid: str) -> str:
         """
         Try to send an SNMP GET operation using SNMPv3 for the specified OID.
 
         Parameters
         ----------
@@ -248,26 +264,25 @@
             The SNMP OID that you want to get.
 
         Returns
         -------
         string : str
             The string as part of the value from the OID you are trying to retrieve.
         """
-        snmp_target = (self.hostname, self.snmp_port)
         cmd_gen = cmdgen.CommandGenerator()
 
         (error_detected, error_status, error_index, snmp_data) = cmd_gen.getCmd(
             cmdgen.UsmUserData(
                 self.user,
                 self.auth_key,
                 self.encrypt_key,
                 authProtocol=self.auth_proto,
                 privProtocol=self.encryp_proto,
             ),
-            cmdgen.UdpTransportTarget(snmp_target, timeout=1.5, retries=2),
+            self.udp_transport_target,
             oid,
             lookupNames=True,
             lookupValues=True,
         )
 
         if not error_detected and snmp_data[0][1]:
             return str(snmp_data[0][1])
@@ -283,20 +298,19 @@
             The SNMP OID that you want to get.
 
         Returns
         -------
         string : str
             The string as part of the value from the OID you are trying to retrieve.
         """
-        snmp_target = (self.hostname, self.snmp_port)
         cmd_gen = cmdgen.CommandGenerator()
 
         (error_detected, error_status, error_index, snmp_data) = cmd_gen.getCmd(
             cmdgen.CommunityData(self.community),
-            cmdgen.UdpTransportTarget(snmp_target, timeout=1.5, retries=2),
+            self.udp_transport_target,
             oid,
             lookupNames=True,
             lookupValues=True,
         )
 
         if not error_detected and snmp_data[0][1]:
             return str(snmp_data[0][1])
```

### Comparing `netmiko-4.1.2/netmiko/sophos/sophos_sfos_ssh.py` & `netmiko-4.2.0/netmiko/sophos/sophos_sfos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/ssh_autodetect.py` & `netmiko-4.2.0/netmiko/ssh_autodetect.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,26 @@
     },
     "arista_eos": {
         "cmd": "show version",
         "search_patterns": [r"Arista"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
+    "arris_cer": {
+        "cmd": "show version",
+        "search_patterns": [r"CER"],
+        "priority": 99,
+        "dispatch": "_autodetect_std",
+    },
+    "casa_cmts": {
+        "cmd": "show version",
+        "search_patterns": [r"Casa"],
+        "priority": 99,
+        "dispatch": "_autodetect_std",
+    },
     "ciena_saos": {
         "cmd": "software show",
         "search_patterns": [r"saos"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
     "cisco_asa": {
@@ -93,26 +105,38 @@
         "search_patterns": [
             "Cisco IOS Software",
             "Cisco Internetwork Operating System Software",
         ],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
+    "cisco_xe": {
+        "cmd": "show version",
+        "search_patterns": [r"Cisco IOS XE Software"],
+        "priority": 99,
+        "dispatch": "_autodetect_std",
+    },
     "cisco_nxos": {
         "cmd": "show version",
         "search_patterns": [r"Cisco Nexus Operating System", r"NX-OS"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
     "cisco_xr": {
         "cmd": "show version",
         "search_patterns": [r"Cisco IOS XR"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
+    "cisco_xr_2": {
+        "cmd": "show version brief",
+        "search_patterns": [r"Cisco IOS XR"],
+        "priority": 99,
+        "dispatch": "_autodetect_std",
+    },
     "dell_force10": {
         "cmd": "show version",
         "search_patterns": [r"Real Time Operating System Software"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
     "dell_os9": {
@@ -150,14 +174,20 @@
     },
     "hp_comware": {
         "cmd": "display version",
         "search_patterns": ["HPE Comware", "HP Comware"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
+    "hp_procurve": {
+        "cmd": "show version",
+        "search_patterns": [r"Image stamp.*/code/build"],
+        "priority": 99,
+        "dispatch": "_autodetect_std",
+    },
     "huawei": {
         "cmd": "display version",
         "search_patterns": [
             r"Huawei Technologies",
             r"Huawei Versatile Routing Platform Software",
         ],
         "priority": 99,
@@ -176,14 +206,20 @@
     },
     "linux": {
         "cmd": "uname -a",
         "search_patterns": [r"Linux"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
+    "ericsson_ipos": {
+        "cmd": "show version",
+        "search_patterns": [r"Ericsson IPOS Version"],
+        "priority": 99,
+        "dispatch": "_autodetect_std",
+    },
     "extreme_exos": {
         "cmd": "show version",
         "search_patterns": [r"ExtremeXOS"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
     "extreme_netiron": {
@@ -215,15 +251,15 @@
         "dispatch": "_autodetect_remote_version",
         "search_patterns": [r"CISCO_WLC"],
         "priority": 99,
     },
     "cisco_wlc_85": {
         "cmd": "show inventory",
         "dispatch": "_autodetect_std",
-        "search_patterns": [r"Cisco Wireless Controller"],
+        "search_patterns": [r"Cisco.*Wireless.*Controller"],
         "priority": 99,
     },
     "mellanox_mlnxos": {
         "cmd": "show version",
         "search_patterns": [r"Onyx", r"SX_PPC_M460EX"],
         "priority": 99,
         "dispatch": "_autodetect_std",
@@ -254,14 +290,26 @@
     },
     "flexvnf": {
         "cmd": "show system package-info",
         "search_patterns": [r"Versa FlexVNF"],
         "priority": 99,
         "dispatch": "_autodetect_std",
     },
+    "cisco_viptela": {
+        "cmd": "show system status",
+        "search_patterns": [r"Viptela, Inc"],
+        "priority": 99,
+        "dispatch": "_autodetect_std",
+    },
+    "oneaccess_oneos": {
+        "cmd": "show version",
+        "search_patterns": [r"OneOS"],
+        "priority": 99,
+        "dispatch": "_autodetect_std",
+    },
 }
 
 # Sort SSH_MAPPER_DICT such that the most common commands are first
 cmd_count: Dict[str, int] = {}
 for k, v in SSH_MAPPER_DICT.items():
     my_cmd = v["cmd"]
     assert isinstance(my_cmd, str)
@@ -308,14 +356,18 @@
         Constructor of the SSHDetect class
         """
         if kwargs["device_type"] != "autodetect":
             raise ValueError("The connection device_type must be 'autodetect'")
         # Always set cmd_verify to False for autodetect
         kwargs["global_cmd_verify"] = False
         self.connection = ConnectHandler(*args, **kwargs)
+
+        # Add additional sleep to let the login complete.
+        time.sleep(3)
+
         # Call the _test_channel_read() in base to clear initial data
         output = BaseConnection._test_channel_read(self.connection)
         self.initial_buffer = output
         self.potential_matches: Dict[str, int] = {}
         self._results_cache: Dict[str, str] = {}
 
     def autodetect(self) -> Union[str, None]:
@@ -338,15 +390,17 @@
                 if accuracy >= 99:  # Stop the loop as we are sure of our match
                     best_match = sorted(
                         self.potential_matches.items(), key=lambda t: t[1], reverse=True
                     )
                     # WLC needs two different auto-dectect solutions
                     if "cisco_wlc_85" in best_match[0]:
                         best_match[0] = ("cisco_wlc", 99)
-
+                    # IOS XR needs two different auto-dectect solutions
+                    if "cisco_xr_2" in best_match[0]:
+                        best_match[0] = ("cisco_xr", 99)
                     self.connection.disconnect()
                     return best_match[0][0]
 
         if not self.potential_matches:
             self.connection.disconnect()
             return None
 
@@ -368,15 +422,15 @@
         Returns
         -------
         output : str
             The output from the command sent
         """
         self.connection.write_channel(cmd + "\n")
         time.sleep(1)
-        output = self.connection.read_channel_timing()
+        output = self.connection.read_channel_timing(last_read=6.0)
         output = self.connection.strip_backspaces(output)
         return output
 
     def _send_command_wrapper(self, cmd: str) -> str:
         """
         Send command to the remote device with a caching feature to avoid sending the same command
         twice based on the SSH_MAPPER_BASE dict cmd key.
```

### Comparing `netmiko-4.1.2/netmiko/ssh_dispatcher.py` & `netmiko-4.2.0/netmiko/ssh_dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,44 +2,48 @@
 from typing import Any, Type, Optional
 from typing import TYPE_CHECKING
 from netmiko.exceptions import ConnectionException
 from netmiko.exceptions import NetmikoTimeoutException, NetmikoAuthenticationException
 from netmiko.a10 import A10SSH
 from netmiko.accedian import AccedianSSH
 from netmiko.adtran import AdtranOSSSH, AdtranOSTelnet
+from netmiko.adva import AdvaAosFsp150F3SSH, AdvaAosFsp150F2SSH
 from netmiko.alcatel import AlcatelAosSSH
 from netmiko.allied_telesis import AlliedTelesisAwplusSSH
 from netmiko.arista import AristaSSH, AristaTelnet
 from netmiko.arista import AristaFileTransfer
+from netmiko.arris import ArrisCERSSH
 from netmiko.apresia import ApresiaAeosSSH, ApresiaAeosTelnet
 from netmiko.aruba import ArubaSSH
 from netmiko.audiocode import (
     Audiocode72SSH,
     Audiocode66SSH,
     AudiocodeShellSSH,
     Audiocode72Telnet,
     Audiocode66Telnet,
     AudiocodeShellTelnet,
 )
 from netmiko.brocade import BrocadeFOSSSH
 from netmiko.broadcom import BroadcomIcosSSH
 from netmiko.calix import CalixB6SSH, CalixB6Telnet
+from netmiko.casa import CasaCMTSSSH
 from netmiko.cdot import CdotCrosSSH
 from netmiko.centec import CentecOSSSH, CentecOSTelnet
 from netmiko.checkpoint import CheckPointGaiaSSH
 from netmiko.ciena import CienaSaosSSH, CienaSaosTelnet, CienaSaosFileTransfer
 from netmiko.cisco import CiscoAsaSSH, CiscoAsaFileTransfer
 from netmiko.cisco import CiscoFtdSSH
 from netmiko.cisco import (
     CiscoIosSSH,
     CiscoIosFileTransfer,
     CiscoIosTelnet,
     CiscoIosSerial,
 )
 from netmiko.cisco import CiscoNxosSSH, CiscoNxosFileTransfer
+from netmiko.cisco import CiscoS200SSH, CiscoS200Telnet
 from netmiko.cisco import CiscoS300SSH, CiscoS300Telnet
 from netmiko.cisco import CiscoTpTcCeSSH
 from netmiko.cisco import CiscoViptelaSSH
 from netmiko.cisco import CiscoWlcSSH
 from netmiko.cisco import CiscoXrSSH, CiscoXrTelnet, CiscoXrFileTransfer
 from netmiko.citrix import NetscalerSSH
 from netmiko.cloudgenix import CloudGenixIonSSH
@@ -52,15 +56,19 @@
 from netmiko.dell import DellPowerConnectSSH
 from netmiko.dell import DellPowerConnectTelnet
 from netmiko.dell import DellIsilonSSH
 from netmiko.dlink import DlinkDSTelnet, DlinkDSSSH
 from netmiko.eltex import EltexSSH, EltexEsrSSH
 from netmiko.endace import EndaceSSH
 from netmiko.enterasys import EnterasysSSH
-from netmiko.ericsson import EricssonIposSSH
+from netmiko.ericsson import (
+    EricssonIposSSH,
+    EricssonMinilink63SSH,
+    EricssonMinilink66SSH,
+)
 from netmiko.extreme import ExtremeErsSSH
 from netmiko.extreme import ExtremeExosSSH, ExtremeExosFileTransfer
 from netmiko.extreme import ExtremeExosTelnet
 from netmiko.extreme import ExtremeNetironSSH
 from netmiko.extreme import ExtremeNetironTelnet
 from netmiko.extreme import ExtremeNosSSH
 from netmiko.extreme import ExtremeSlxSSH
@@ -103,47 +111,52 @@
 from netmiko.raisecom import RaisecomRoapSSH
 from netmiko.raisecom import RaisecomRoapTelnet
 from netmiko.ruckus import RuckusFastironSSH
 from netmiko.ruckus import RuckusFastironTelnet
 from netmiko.ruijie import RuijieOSSSH, RuijieOSTelnet
 from netmiko.sixwind import SixwindOSSSH
 from netmiko.sophos import SophosSfosSSH
+from netmiko.teldat import TeldatCITSSH, TeldatCITTelnet
 from netmiko.terminal_server import TerminalServerSSH
 from netmiko.terminal_server import TerminalServerTelnet
 from netmiko.tplink import TPLinkJetStreamSSH, TPLinkJetStreamTelnet
-from netmiko.ubiquiti import UbiquitiEdgeRouterSSH
+from netmiko.ubiquiti import UbiquitiEdgeRouterSSH, UbiquitiEdgeRouterFileTransfer
 from netmiko.ubiquiti import UbiquitiEdgeSSH
 from netmiko.ubiquiti import UbiquitiUnifiSwitchSSH
 from netmiko.vyos import VyOSSSH
 from netmiko.watchguard import WatchguardFirewareSSH
 from netmiko.yamaha import YamahaSSH
 from netmiko.yamaha import YamahaTelnet
 from netmiko.zte import ZteZxrosSSH
 from netmiko.zte import ZteZxrosTelnet
 from netmiko.supermicro import SmciSwitchSmisSSH
 from netmiko.supermicro import SmciSwitchSmisTelnet
 from netmiko.zyxel import ZyxelSSH
+from netmiko.hillstone import HillstoneStoneosSSH
 
 if TYPE_CHECKING:
     from netmiko.base_connection import BaseConnection
     from netmiko.scp_handler import BaseFileTransfer
 
 GenericSSH = TerminalServerSSH
 GenericTelnet = TerminalServerTelnet
 
 # The keys of this dictionary are the supported device_types
 CLASS_MAPPER_BASE = {
     "a10": A10SSH,
     "accedian": AccedianSSH,
     "adtran_os": AdtranOSSSH,
+    "adva_fsp150f2": AdvaAosFsp150F2SSH,
+    "adva_fsp150f3": AdvaAosFsp150F3SSH,
     "alcatel_aos": AlcatelAosSSH,
     "alcatel_sros": NokiaSrosSSH,
     "allied_telesis_awplus": AlliedTelesisAwplusSSH,
     "apresia_aeos": ApresiaAeosSSH,
     "arista_eos": AristaSSH,
+    "arris_cer": ArrisCERSSH,
     "aruba_os": ArubaSSH,
     "aruba_osswitch": HPProcurveSSH,
     "aruba_procurve": HPProcurveSSH,
     "audiocode_72": Audiocode72SSH,
     "audiocode_66": Audiocode66SSH,
     "audiocode_shell": AudiocodeShellSSH,
     "avaya_ers": ExtremeErsSSH,
@@ -153,21 +166,23 @@
     "brocade_fastiron": RuckusFastironSSH,
     "brocade_netiron": ExtremeNetironSSH,
     "brocade_nos": ExtremeNosSSH,
     "brocade_vdx": ExtremeNosSSH,
     "brocade_vyos": VyOSSSH,
     "checkpoint_gaia": CheckPointGaiaSSH,
     "calix_b6": CalixB6SSH,
+    "casa_cmts": CasaCMTSSSH,
     "cdot_cros": CdotCrosSSH,
     "centec_os": CentecOSSSH,
     "ciena_saos": CienaSaosSSH,
     "cisco_asa": CiscoAsaSSH,
     "cisco_ftd": CiscoFtdSSH,
     "cisco_ios": CiscoIosSSH,
     "cisco_nxos": CiscoNxosSSH,
+    "cisco_s200": CiscoS200SSH,
     "cisco_s300": CiscoS300SSH,
     "cisco_tp": CiscoTpTcCeSSH,
     "cisco_viptela": CiscoViptelaSSH,
     "cisco_wlc": CiscoWlcSSH,
     "cisco_xe": CiscoIosSSH,
     "cisco_xr": CiscoXrSSH,
     "cloudgenix_ion": CloudGenixIonSSH,
@@ -182,14 +197,16 @@
     "dell_isilon": DellIsilonSSH,
     "dlink_ds": DlinkDSSSH,
     "endace": EndaceSSH,
     "eltex": EltexSSH,
     "eltex_esr": EltexEsrSSH,
     "enterasys": EnterasysSSH,
     "ericsson_ipos": EricssonIposSSH,
+    "ericsson_mltn63": EricssonMinilink63SSH,
+    "ericsson_mltn66": EricssonMinilink66SSH,
     "extreme": ExtremeExosSSH,
     "extreme_ers": ExtremeErsSSH,
     "extreme_exos": ExtremeExosSSH,
     "extreme_netiron": ExtremeNetironSSH,
     "extreme_nos": ExtremeNosSSH,
     "extreme_slx": ExtremeSlxSSH,
     "extreme_tierra": ExtremeTierraSSH,
@@ -199,19 +216,21 @@
     "f5_ltm": F5TmshSSH,
     "f5_tmsh": F5TmshSSH,
     "f5_linux": F5LinuxSSH,
     "flexvnf": FlexvnfSSH,
     "fortinet": FortinetSSH,
     "generic": GenericSSH,
     "generic_termserver": TerminalServerSSH,
+    "hillstone_stoneos": HillstoneStoneosSSH,
     "hp_comware": HPComwareSSH,
     "hp_procurve": HPProcurveSSH,
     "huawei": HuaweiSSH,
     "huawei_smartax": HuaweiSmartAXSSH,
     "huawei_olt": HuaweiSmartAXSSH,
+    "huawei_vrp": HuaweiSSH,
     "huawei_vrpv8": HuaweiVrpv8SSH,
     "ipinfusion_ocnos": IpInfusionOcNOSSSH,
     "juniper": JuniperSSH,
     "juniper_junos": JuniperSSH,
     "juniper_screenos": JuniperScreenOsSSH,
     "keymile": KeymileSSH,
     "keymile_nos": KeymileNOSSSH,
@@ -235,14 +254,15 @@
     "rad_etx": RadETXSSH,
     "raisecom_roap": RaisecomRoapSSH,
     "ruckus_fastiron": RuckusFastironSSH,
     "ruijie_os": RuijieOSSSH,
     "sixwind_os": SixwindOSSSH,
     "sophos_sfos": SophosSfosSSH,
     "supermicro_smis": SmciSwitchSmisSSH,
+    "teldat_cit": TeldatCITSSH,
     "tplink_jetstream": TPLinkJetStreamSSH,
     "ubiquiti_edge": UbiquitiEdgeSSH,
     "ubiquiti_edgerouter": UbiquitiEdgeRouterSSH,
     "ubiquiti_edgeswitch": UbiquitiEdgeSSH,
     "ubiquiti_unifiswitch": UbiquitiUnifiSwitchSSH,
     "vyatta_vyos": VyOSSSH,
     "vyos": VyOSSSH,
@@ -262,14 +282,15 @@
     "cisco_xr": CiscoXrFileTransfer,
     "dell_os10": DellOS10FileTransfer,
     "extreme_exos": ExtremeExosFileTransfer,
     "juniper_junos": JuniperFileTransfer,
     "linux": LinuxFileTransfer,
     "nokia_sros": NokiaSrosFileTransfer,
     "mikrotik_routeros": MikrotikRouterOsFileTransfer,
+    "ubiquiti_edgerouter": UbiquitiEdgeRouterFileTransfer,
 }
 
 # Also support keys that end in _ssh
 new_mapper = {}
 for k, v in CLASS_MAPPER_BASE.items():
     new_mapper[k] = v
     alt_key = k + "_ssh"
@@ -294,14 +315,15 @@
 CLASS_MAPPER["brocade_fastiron_telnet"] = RuckusFastironTelnet
 CLASS_MAPPER["brocade_netiron_telnet"] = ExtremeNetironTelnet
 CLASS_MAPPER["calix_b6_telnet"] = CalixB6Telnet
 CLASS_MAPPER["centec_os_telnet"] = CentecOSTelnet
 CLASS_MAPPER["ciena_saos_telnet"] = CienaSaosTelnet
 CLASS_MAPPER["cisco_ios_telnet"] = CiscoIosTelnet
 CLASS_MAPPER["cisco_xr_telnet"] = CiscoXrTelnet
+CLASS_MAPPER["cisco_s200_telnet"] = CiscoS200Telnet
 CLASS_MAPPER["cisco_s300_telnet"] = CiscoS300Telnet
 CLASS_MAPPER["dell_dnos6_telnet"] = DellDNOS6Telnet
 CLASS_MAPPER["dell_powerconnect_telnet"] = DellPowerConnectTelnet
 CLASS_MAPPER["dlink_ds_telnet"] = DlinkDSTelnet
 CLASS_MAPPER["extreme_telnet"] = ExtremeExosTelnet
 CLASS_MAPPER["extreme_exos_telnet"] = ExtremeExosTelnet
 CLASS_MAPPER["extreme_netiron_telnet"] = ExtremeNetironTelnet
@@ -317,14 +339,15 @@
 CLASS_MAPPER["oneaccess_oneos_telnet"] = OneaccessOneOSTelnet
 CLASS_MAPPER["paloalto_panos_telnet"] = PaloAltoPanosTelnet
 CLASS_MAPPER["rad_etx_telnet"] = RadETXTelnet
 CLASS_MAPPER["raisecom_telnet"] = RaisecomRoapTelnet
 CLASS_MAPPER["ruckus_fastiron_telnet"] = RuckusFastironTelnet
 CLASS_MAPPER["ruijie_os_telnet"] = RuijieOSTelnet
 CLASS_MAPPER["supermicro_smis_telnet"] = SmciSwitchSmisTelnet
+CLASS_MAPPER["teldat_cit_telnet"] = TeldatCITTelnet
 CLASS_MAPPER["tplink_jetstream_telnet"] = TPLinkJetStreamTelnet
 CLASS_MAPPER["yamaha_telnet"] = YamahaTelnet
 CLASS_MAPPER["zte_zxros_telnet"] = ZteZxrosTelnet
 
 # Add serial drivers
 CLASS_MAPPER["cisco_ios_serial"] = CiscoIosSerial
 
@@ -407,26 +430,27 @@
         return None
     except NetmikoTimeoutException as e:
         if "DNS failure" in str(e):
             msg = f"Device failed due to a DNS failure, hostname {hostname}"
         elif "TCP connection to device failed" in str(e):
             msg = f"Netmiko was unable to reach the provided host and port: {hostname}:{port}"
             msg += f"\n\n{str(e)}"
+        else:
+            msg = f"An unknown NetmikoTimeoutException occurred:\n\n{str(e)}"
         logger.error(msg)
         return None
     except Exception as e:
         msg = f"An unknown exception occurred during connection:\n\n{str(e)}"
         logger.error(msg)
         return None
 
 
 def ConnUnify(
     **kwargs: Any,
 ) -> "BaseConnection":
-
     try:
         kwargs["auto_connect"] = False
         net_connect = ConnectHandler(**kwargs)
         hostname = net_connect.host
         port = net_connect.port
         device_type = net_connect.device_type
         general_msg = f"Connection failure to {hostname}:{port} ({device_type})\n\n"
```

### Comparing `netmiko-4.1.2/netmiko/supermicro/smci_smis.py` & `netmiko-4.2.0/netmiko/supermicro/smci_smis.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/terminal_server/terminal_server.py` & `netmiko-4.2.0/netmiko/terminal_server/terminal_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,11 +23,11 @@
 
 
 class TerminalServerTelnet(TerminalServer):
     """Generic Terminal Server driver telnet."""
 
     def telnet_login(self, *args: Any, **kwargs: Any) -> str:
         # Disable automatic handling of username and password when using terminal server driver
-        pass
+        return ""
 
     def std_login(self, *args: Any, **kwargs: Any) -> str:
         return super().telnet_login(*args, **kwargs)
```

### Comparing `netmiko-4.1.2/netmiko/tplink/tplink_jetstream.py` & `netmiko-4.2.0/netmiko/tplink/tplink_jetstream.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Optional
 
 from cryptography.hazmat.primitives.asymmetric import dsa
 from cryptography.hazmat.primitives.asymmetric.dsa import DSAParameterNumbers
 
 from netmiko import log
 from netmiko.cisco_base_connection import CiscoSSHConnection
-from netmiko.exceptions import NetmikoTimeoutException
+from netmiko.exceptions import ReadTimeout
 
 
 class TPLinkJetStreamBase(CiscoSSHConnection):
     def __init__(self, **kwargs: Any) -> None:
         # TP-Link doesn't have a way to set terminal width which breaks cmd_verify
         if kwargs.get("global_cmd_verify") is None:
             kwargs["global_cmd_verify"] = False
@@ -36,48 +36,59 @@
         self.clear_buffer()
 
     def enable(
         self,
         cmd: str = "",
         pattern: str = "ssword",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         """
         TPLink JetStream requires you to first execute "enable" and then execute "enable-admin".
         This is necessary as "configure" is generally only available at "enable-admin" level
 
         If the user does not have the Admin role, he will need to execute enable-admin to really
         enable all functions.
         """
 
+        msg = """
+Failed to enter enable mode. Please ensure you pass
+the 'secret' argument to ConnectHandler.
+"""
+
         # If end-user passes in "cmd" execute that using normal process.
         if cmd:
-            return super().enable(cmd=cmd, pattern=pattern, re_flags=re_flags)
+            return super().enable(
+                cmd=cmd,
+                pattern=pattern,
+                enable_pattern=enable_pattern,
+                check_state=check_state,
+                re_flags=re_flags,
+            )
 
         output = ""
-        msg = (
-            "Failed to enter enable mode. Please ensure you pass "
-            "the 'secret' argument to ConnectHandler."
-        )
+        if check_state and self.check_enable_mode():
+            return output
 
-        cmds = ["enable", "enable-admin"]
-        if not self.check_enable_mode():
-            for cmd in cmds:
-                self.write_channel(self.normalize_cmd(cmd))
-                try:
-                    output += self.read_until_prompt_or_pattern(
-                        pattern=pattern, re_flags=re_flags, read_entire_line=True
-                    )
+        for cmd in ("enable", "enable-admin"):
+            self.write_channel(self.normalize_cmd(cmd))
+            try:
+                new_data = self.read_until_prompt_or_pattern(
+                    pattern=pattern, re_flags=re_flags, read_entire_line=True
+                )
+                output += new_data
+                if re.search(pattern, new_data):
                     self.write_channel(self.normalize_cmd(self.secret))
                     output += self.read_until_prompt(read_entire_line=True)
-                except NetmikoTimeoutException:
-                    raise ValueError(msg)
-                if not self.check_enable_mode():
-                    raise ValueError(msg)
+            except ReadTimeout:
+                raise ValueError(msg)
+
+        if not self.check_enable_mode():
+            raise ValueError(msg)
         return output
 
     def config_mode(
         self, config_command: str = "configure", pattern: str = "", re_flags: int = 0
     ) -> str:
         return super().config_mode(
             config_command=config_command, pattern=pattern, re_flags=re_flags
```

### Comparing `netmiko-4.1.2/netmiko/ubiquiti/edge_ssh.py` & `netmiko-4.2.0/netmiko/ubiquiti/edge_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/ubiquiti/edgerouter_ssh.py` & `netmiko-4.2.0/netmiko/dell/dell_force10_ssh.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,37 @@
-import time
-from netmiko.vyos.vyos_ssh import VyOSSSH
+"""Dell Force10 Driver - supports DNOS9."""
+from netmiko.cisco_base_connection import CiscoSSHConnection
 
 
-class UbiquitiEdgeRouterSSH(VyOSSSH):
-    """Implement methods for interacting with EdgeOS EdgeRouter network devices."""
+class DellForce10SSH(CiscoSSHConnection):
+    """Dell Force10 Driver - supports DNOS9."""
 
     def session_preparation(self) -> None:
         """Prepare the session after the connection has been established."""
-        self._test_channel_read()
+        self._test_channel_read(pattern=r"[>#]")
         self.set_base_prompt()
-        self.set_terminal_width(command="terminal width 512")
-        self.disable_paging(command="terminal length 0")
-        # Clear the read buffer
-        time.sleep(0.3 * self.global_delay_factor)
-        self.clear_buffer()
+        self.set_terminal_width()
+        self.disable_paging()
+
+    def check_config_mode(
+        self,
+        check_string: str = ")#",
+        pattern: str = r"[>#]",
+        force_regex: bool = False,
+    ) -> bool:
+        """
+        Checks if the device is in configuration mode or not.
+        """
+        return super().check_config_mode(
+            check_string=check_string, pattern=pattern, force_regex=force_regex
+        )
 
     def save_config(
-        self, cmd: str = "save", confirm: bool = False, confirm_response: str = ""
+        self,
+        cmd: str = "write memory",
+        confirm: bool = False,
+        confirm_response: str = "",
     ) -> str:
-        """Saves Config."""
-        if confirm is True:
-            raise ValueError("EdgeRouter does not support save_config confirmation.")
-        output = self._send_command_str(command_string=cmd)
-        if "Done" not in output:
-            raise ValueError(f"Save failed with following errors:\n\n{output}")
-        return output
+        """Saves Config"""
+        return super().save_config(
+            cmd=cmd, confirm=confirm, confirm_response=confirm_response
+        )
```

### Comparing `netmiko-4.1.2/netmiko/ubiquiti/unifiswitch_ssh.py` & `netmiko-4.2.0/netmiko/ubiquiti/unifiswitch_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/utilities.py` & `netmiko-4.2.0/netmiko/utilities.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/vyos/vyos_ssh.py` & `netmiko-4.2.0/netmiko/vyos/vyos_ssh.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/watchguard/fireware_ssh.py` & `netmiko-4.2.0/netmiko/watchguard/fireware_ssh.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,8 +37,8 @@
         )
 
     def exit_config_mode(self, exit_config: str = "exit", pattern: str = "#") -> str:
         return super().exit_config_mode(exit_config=exit_config, pattern=pattern)
 
     def save_config(self, *args: Any, **kwargs: Any) -> str:
         """No save config on Watchguard."""
-        pass
+        return ""
```

### Comparing `netmiko-4.1.2/netmiko/yamaha/yamaha.py` & `netmiko-4.2.0/netmiko/yamaha/yamaha.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,23 @@
         return super().check_enable_mode(check_string=check_string)
 
     def enable(
         self,
         cmd: str = "administrator",
         pattern: str = r"Password",
         enable_pattern: Optional[str] = None,
+        check_state: bool = True,
         re_flags: int = re.IGNORECASE,
     ) -> str:
         return super().enable(
-            cmd=cmd, pattern=pattern, enable_pattern=enable_pattern, re_flags=re_flags
+            cmd=cmd,
+            pattern=pattern,
+            enable_pattern=enable_pattern,
+            check_state=check_state,
+            re_flags=re_flags,
         )
 
     def exit_enable_mode(self, exit_command: str = "exit") -> str:
         """
         When any changes have been made, the prompt 'Save new configuration ? (Y/N)'
         appears before exiting. Ignore this by entering 'N'.
         """
```

### Comparing `netmiko-4.1.2/netmiko/zte/zte_zxros.py` & `netmiko-4.2.0/netmiko/zte/zte_zxros.py`

 * *Files identical despite different names*

### Comparing `netmiko-4.1.2/netmiko/zyxel/zyxel_ssh.py` & `netmiko-4.2.0/netmiko/zyxel/zyxel_ssh.py`

 * *Files identical despite different names*

