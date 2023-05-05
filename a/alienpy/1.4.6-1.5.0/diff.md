# Comparing `tmp/alienpy-1.4.6.tar.gz` & `tmp/alienpy-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alienpy-1.4.6.tar", last modified: Fri Nov  4 00:32:13 2022, max compression
+gzip compressed data, was "alienpy-1.5.0.tar", last modified: Fri May  5 05:26:56 2023, max compression
```

## Comparing `alienpy-1.4.6.tar` & `alienpy-1.5.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2022-11-04 00:32:13.544706 alienpy-1.4.6/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1538 2020-05-18 21:36:32.000000 alienpy-1.4.6/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2022-11-04 00:32:13.544706 alienpy-1.4.6/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     9570 2021-08-24 15:12:13.000000 alienpy-1.4.6/README.md
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2022-11-04 00:32:13.544706 alienpy-1.4.6/alienpy/
--rw-r--r--   0 adrian    (1000) adrian    (1000)        5 2022-11-04 00:31:49.000000 alienpy-1.4.6/alienpy/VERSION
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2022-11-03 18:03:32.000000 alienpy-1.4.6/alienpy/__init__.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)   241032 2022-11-04 00:32:07.000000 alienpy-1.4.6/alienpy/alien.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5540 2022-11-03 19:16:11.000000 alienpy-1.4.6/alienpy/cmds_client_local.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    35995 2022-11-03 19:15:35.000000 alienpy-1.4.6/alienpy/cmds_client_wb.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7533 2022-11-03 16:35:28.000000 alienpy-1.4.6/alienpy/data.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    81552 2022-11-03 17:12:20.000000 alienpy-1.4.6/alienpy/fs_grid.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13544 2022-11-03 17:09:30.000000 alienpy-1.4.6/alienpy/fs_local.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1256 2022-11-03 17:22:15.000000 alienpy-1.4.6/alienpy/http_tools.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    18385 2022-11-03 19:38:07.000000 alienpy-1.4.6/alienpy/jalien_talk.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      743 2022-11-03 17:08:55.000000 alienpy-1.4.6/alienpy/re_patt.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    11938 2022-11-03 17:26:13.000000 alienpy-1.4.6/alienpy/ssl_tools.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    17222 2022-11-03 17:24:22.000000 alienpy-1.4.6/alienpy/tools.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4939 2022-11-03 18:26:34.000000 alienpy-1.4.6/alienpy/wb_api.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    12254 2022-11-03 18:24:19.000000 alienpy-1.4.6/alienpy/wb_base.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2022-11-04 00:32:13.544706 alienpy-1.4.6/alienpy.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    10431 2022-11-04 00:32:13.000000 alienpy-1.4.6/alienpy.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      538 2022-11-04 00:32:13.000000 alienpy-1.4.6/alienpy.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2022-11-04 00:32:13.000000 alienpy-1.4.6/alienpy.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      761 2022-11-04 00:32:13.000000 alienpy-1.4.6/alienpy.egg-info/entry_points.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       56 2022-11-04 00:32:13.000000 alienpy-1.4.6/alienpy.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        8 2022-11-04 00:32:13.000000 alienpy-1.4.6/alienpy.egg-info/top_level.txt
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2022-11-04 00:32:13.544706 alienpy-1.4.6/examples/
--rwxrwxr-x   0 adrian    (1000) adrian    (1000)     2169 2022-09-23 15:55:55.000000 alienpy-1.4.6/examples/alien_wbtime
--rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2022-11-04 00:32:13.544706 alienpy-1.4.6/setup.cfg
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     3373 2022-09-23 15:22:14.000000 alienpy-1.4.6/setup.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-05 05:26:56.444389 alienpy-1.5.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1538 2020-05-18 21:36:32.000000 alienpy-1.5.0/LICENSE
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2023-05-05 05:26:56.443390 alienpy-1.5.0/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9570 2022-12-20 08:02:48.000000 alienpy-1.5.0/README.md
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-05 05:26:56.442389 alienpy-1.5.0/alienpy/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2022-11-03 18:03:32.000000 alienpy-1.5.0/alienpy/__init__.py
+-rwxr-xr-x   0 adrian    (1000) adrian    (1000)    93304 2023-05-04 21:21:13.000000 alienpy-1.5.0/alienpy/alien.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2821 2023-03-16 23:03:24.000000 alienpy-1.5.0/alienpy/async_tools.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    13461 2023-05-02 22:25:03.000000 alienpy-1.5.0/alienpy/connect_ssl.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6900 2023-03-17 15:40:29.000000 alienpy-1.5.0/alienpy/data_structs.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1903 2023-05-02 22:31:24.000000 alienpy-1.5.0/alienpy/global_vars.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1491 2023-03-17 15:53:13.000000 alienpy-1.5.0/alienpy/setup_cwd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2120 2023-05-02 22:41:20.000000 alienpy-1.5.0/alienpy/setup_logging.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    19706 2023-05-03 16:31:20.000000 alienpy-1.5.0/alienpy/tools_files.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    18022 2023-05-04 17:31:44.000000 alienpy-1.5.0/alienpy/tools_misc.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1719 2023-03-17 16:31:32.000000 alienpy-1.5.0/alienpy/tools_shell.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      851 2023-03-17 10:35:43.000000 alienpy-1.5.0/alienpy/tools_stackcmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      289 2023-05-04 21:26:56.000000 alienpy-1.5.0/alienpy/version.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    16919 2023-05-04 16:55:53.000000 alienpy-1.5.0/alienpy/wb_api.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8986 2023-03-17 15:01:28.000000 alienpy-1.5.0/alienpy/wb_async.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    56632 2023-05-04 21:10:51.000000 alienpy-1.5.0/alienpy/xrd_core.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    23884 2023-05-03 18:13:23.000000 alienpy-1.5.0/alienpy/xrd_tools.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-05 05:26:56.443390 alienpy-1.5.0/alienpy.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)    10431 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      604 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      761 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/entry_points.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       56 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        8 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/top_level.txt
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-05 05:26:56.443390 alienpy-1.5.0/examples/
+-rwxr-xr-x   0 adrian    (1000) adrian    (1000)     2169 2022-12-20 08:02:48.000000 alienpy-1.5.0/examples/alien_wbtime
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2023-05-05 05:26:56.444389 alienpy-1.5.0/setup.cfg
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3343 2023-03-17 11:15:21.000000 alienpy-1.5.0/setup.py
```

### Comparing `alienpy-1.4.6/LICENSE` & `alienpy-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alienpy-1.4.6/PKG-INFO` & `alienpy-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alienpy
-Version: 1.4.6
+Version: 1.5.0
 Summary: Websocket based cli interface for ALICE experiment GRID infrastructure
 Home-page: https://gitlab.cern.ch/jalien/xjalienfs
 Author: Adrian Sevcenco
 Author-email: adrian.sevcenco@cern.ch
 Project-URL: Dev git, https://github.com/adriansev/jalien_py
 Project-URL: Issues, https://github.com/adriansev/jalien_py/issues
 Project-URL: Changelog, https://github.com/adriansev/jalien_py/commits/master
```

### Comparing `alienpy-1.4.6/README.md` & `alienpy-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alienpy-1.4.6/alienpy/data.py` & `alienpy-1.5.0/alienpy/data_structs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+'''alienpy:: Definitions of data structures'''
+
+import os
+import sys
 from typing import NamedTuple
 from typing import Union
+# import shlex
+import json
+import logging
 
 
 ##############################################
-##   Start of data strucutures definitons
+##   Start of data structures definitons
 ##############################################
 
-class COLORS(NamedTuple):  # pylint: disable=inherit-non-class
+class COLORS_COLL(NamedTuple):  # pylint: disable=inherit-non-class
     """Collection of colors for terminal printing"""
     ColorReset = '\033[00m'     # Text Reset
     Black = '\033[0;30m'        # Black
     Red = '\033[0;31m'          # Red
     Green = '\033[0;32m'        # Green
     Yellow = '\033[0;33m'       # Yellow
     Blue = '\033[0;34m'         # Blue
@@ -65,85 +72,86 @@
     On_IPurple = '\033[0;105m'  # High Intensity backgrounds Purple
     On_ICyan = '\033[0;106m'    # High Intensity backgrounds Cyan
     On_IWhite = '\033[0;107m'   # High Intensity backgrounds White
 
 
 class XrdCpArgs(NamedTuple):  # pylint: disable=inherit-non-class
     """Structure to keep the set of xrootd flags used for xrootd copy process"""
-    overwrite: bool
-    batch: int
-    tpc: str
-    hashtype: str
-    cksum: bool
-    timeout: int
-    rate: int
+    overwrite: bool = True
+    batch: int = 8
+    tpc: str = ''
+    hashtype: str = ''
+    cksum: bool = True
+    timeout: int = 0
+    rate: int = 0
 
 
 class CopyFile(NamedTuple):  # pylint: disable=inherit-non-class
     """Structure to keep a generic copy task"""
-    src: str
-    dst: str
-    isUpload: bool
-    token_request: dict
-    lfn: str
+    src: str = ''
+    dst: str = ''
+    isUpload: bool = False
+    token_request: dict = {}
+    lfn: str = ''
 
 
 class CommitInfo(NamedTuple):  # pylint: disable=inherit-non-class
     """Structure for commit of succesful xrootd write to file catalogue"""
-    envelope: str
-    size: str
-    lfn: str
-    perm: str
-    expire: str
-    pfn: str
-    se: str
-    guid: str
-    md5: str
+    envelope: str = ''
+    size: str = ''
+    lfn: str = ''
+    perm: str = ''
+    expire: str = ''
+    pfn: str = ''
+    se: str = ''
+    guid: str = ''
+    md5: str = ''
 
 
 class lfn2file(NamedTuple):  # pylint: disable=inherit-non-class
     """Map a lfn to file (and reverse)"""
-    lfn: str
-    file: str
+    lfn: str = ''
+    file: str = ''
 
 
 class KV(NamedTuple):  # pylint: disable=inherit-non-class
     """Assign a value to a key"""
-    key: str
-    val: str
+    key: str = ''
+    val: str = ''
 
 
 class RET(NamedTuple):  # pylint: disable=inherit-non-class
     """Structure for POSIX like function return: exitcode, stdout, stderr, dictionary of server reply"""
     exitcode: int = -1
     out: str = ''
     err: str = ''
     ansdict: dict = {}
 
     def print(self, opts: str = '') -> None:
         """Print the in json format the content of ansdict, if existent"""
         if 'json' in opts:
             if self.ansdict:
                 json_out = json.dumps(self.ansdict, sort_keys = True, indent = 4)
-                print_out(json_out)
-                if _DEBUG: logging.debug(json_out)
+                print(json_out, flush = True)
+                DEBUG = os.getenv('ALIENPY_DEBUG', '')
+                if DEBUG: logging.debug(json_out)
             else:
-                print_err('This command did not return a json dictionary')
+                print('This command did not return a json dictionary', file = sys.stderr, flush = True)
             return
 
         if self.exitcode != 0:
             if 'info' in opts: logging.info(self.err)
             if 'warn' in opts: logging.warning(self.err)
             if 'err' in opts: logging.error(self.err)
             if 'debug' in opts: logging.debug(self.err)
             if self.err and not ('noerr' in opts or 'noprint' in opts):
-                print_err(f'{self.err.strip()}')
+                print(f'{self.err.strip()}', file = sys.stderr, flush = True)
         else:
             if self.out and not ('noout' in opts or 'noprint' in opts):
-                print_out(f'{self.out.strip()}')
+                print(f'{self.out.strip()}', flush = True)
 
     __call__ = print
 
     def __bool__(self) -> bool:
         return bool(self.exitcode == 0)
 
 
@@ -180,44 +188,12 @@
     ctime: str = ''
     mtime: str = ''
     guid: str = ''
     size: str = ''
     md5: str = ''
 
 
-class Msg:
-    """Class to create json messages to be sent to server"""
-    __slots__ = ('cmd', 'args', 'opts')
-
-    def __init__(self, cmd: str = '', args: Union[str, list, None] = None, opts: str = '') -> None:
-        self.cmd = cmd
-        self.opts = opts
-        if not args:
-            self.args = []
-        elif isinstance(args, str):
-            self.args = shlex.split(args)
-        elif isinstance(args, list):
-            self.args = args.copy()
-
-    def add_arg(self, arg: Union[str, list, None]) -> None:
-        if not arg: return
-        if isinstance(arg, str): self.args.extend(shlex.split(arg))
-        if isinstance(arg, list): self.args.extend(arg)
-
-    def msgdict(self) -> dict:
-        return CreateJsonCommand(self.cmd, self.args, self.opts, True)
-
-    def msgstr(self) -> str:
-        return CreateJsonCommand(self.cmd, self.args, self.opts)
-
-    def __call__(self) -> tuple:
-        return (self.cmd, self.args, self.opts)
-
-    def __bool__(self):
-        return bool(self.cmd)
-
-
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
```

### Comparing `alienpy-1.4.6/alienpy/fs_grid.py` & `alienpy-1.5.0/alienpy/xrd_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,51 @@
+'''alienpy:: XRootD mechanics'''
 
+import datetime
+import sys
+import xml.dom.minidom as MD  # nosec B408:blacklist
+import zipfile
+import traceback
+from urllib.parse import urlparse
+from .global_vars import *  # nosec PYL-W0614
+from .data_structs import *  # nosec PYL-W0614
+from .version import *  # nosec PYL-W0614
+from .tools_files import *  # nosec PYL-W0614
+from .xrd_tools import *  # nosec PYL-W0614
+from .tools_misc import *  # nosec PYL-W0614
+from .setup_logging import print_out, print_err
+from .tools_shell import runShellCMD
 
-_HAS_XROOTD = False
+HAS_XROOTD = False
 try:
-    from XRootD import client as xrd_client
-    _HAS_XROOTD = True
+    from XRootD import client as xrd_client  # type: ignore
+    HAS_XROOTD = True
 except Exception:
-    print("XRootD module could not be load", file = sys.stderr, flush = True)
+    print("XRootD module could not be imported! Not fatal, but XRootD transfers will not work (or any kind of file access)\n Make sure you can do:\npython3 -c 'from XRootD import client as xrd_client'", file = sys.stderr, flush = True)
 
 
 def _is_valid_xrootd() -> bool:
-    if not _HAS_XROOTD: return False
+    if not HAS_XROOTD: return False
     xrd_ver_arr = xrd_client.__version__.split(".")
-    if len(xrd_ver_arr) > 1:  # noqa: PLR1705
+    if len(xrd_ver_arr) > 1:
         _XRDVER_1 = xrd_ver_arr[0][1:] if xrd_ver_arr[0].startswith('v') else xrd_ver_arr[0]  # take out the v if present
         _XRDVER_2 = xrd_ver_arr[1]
         return int(_XRDVER_1) >= 5 and int(_XRDVER_2) > 2
 
     # version is not of x.y.z form, this is git based form
     xrdver_git = xrd_ver_arr[0].split("-")
     _XRDVER_1 = xrdver_git[0][1:] if xrdver_git[0].startswith('v') else xrdver_git[0]  # take out the v if present
     _XRDVER_2 = xrdver_git[1]
     return int(_XRDVER_1) > 20211113
 
 
 # use only 5.3 versions and up - reference point
-_HAS_XROOTD = _is_valid_xrootd()
-_HAS_XROOTD_GETDEFAULT = False
-if _HAS_XROOTD:
+HAS_XROOTD = _is_valid_xrootd()
+HAS_XROOTD_GETDEFAULT = False
+if HAS_XROOTD:
     def XRD_EnvPut(key, value):  # noqa: ANN001,ANN201
         """Sets the given key in the xrootd client environment to the given value.
         Returns false if there is already a shell-imported setting for this key, true otherwise
         """
         return xrd_client.EnvPutInt(key, value) if str(value).isdigit() else xrd_client.EnvPutString(key, value)
 
     def XRD_EnvGet(key):  # noqa: ANN001,ANN201
@@ -38,20 +53,21 @@
         val = xrd_client.EnvGetString(key)
         if not val:
             val = xrd_client.EnvGetInt(key)
         return val  # noqa: R504
 
     # Override the application name reported to the xrootd server.
     XRD_EnvPut('XRD_APPNAME', f'alien.py/{ALIENPY_VERSION_STR} xrootd/{xrd_client.__version__}')
-    _HAS_XROOTD_GETDEFAULT = hasattr(xrd_client, 'EnvGetDefault')
+    HAS_XROOTD_GETDEFAULT = hasattr(xrd_client, 'EnvGetDefault')
+
 
 
 def xrd_config_init():
     """Initialize generic XRootD client vars/timeouts"""
-    if not _HAS_XROOTD: return
+    if not HAS_XROOTD: return
     # xrdcp parameters (used by ALICE tests)
     # http://xrootd.org/doc/man/xrdcp.1.html
     # https://xrootd.slac.stanford.edu/doc/xrdcl-docs/www/xrdcldocs.html#x1-100004.2
     # xrootd defaults https://github.com/xrootd/xrootd/blob/master/src/XrdCl/XrdClConstants.hh
 
     # Resolution for the timeout events. Ie. timeout events will be processed only every XRD_TIMEOUTRESOLUTION seconds.
     if not os.getenv('XRD_TIMEOUTRESOLUTION'): XRD_EnvPut('TimeoutResolution', int(1))  # let's check the status every 1s; default 15
@@ -80,607 +96,34 @@
     # Time period after which an idle connection to a manager or a load balancer should be closed.
     if not os.getenv('XRD_LOADBALANCERTTL'): XRD_EnvPut('LoadBalancerTTL', int(30))  # we have no reasons to keep idle connections
 
     # If set the client tries first IPv4 address (turned off by default).
     if not os.getenv('XRD_PREFERIPV4'): XRD_EnvPut('PreferIPv4', int(1))
 
 
-
-def xrdcp_help() -> str:
-    return f'''Command format is of the form of (with the strict order of arguments):
-        cp <options> src dst
-        or
-        cp <options> -input input_file
-where src|dst are local files if prefixed with file:// or file: or grid files otherwise
-and -input argument is a file with >src dst< pairs
-after each src,dst can be added comma separated specifiers in the form of: @disk:N,SE1,SE2,!SE3
-where disk selects the number of replicas and the following specifiers add (or remove) storage endpoints from the received list
-options are the following :
--h : print help
--d | -dd | -ddd : enable XRootD log level to Info/Debug/Dump
--xrdlog : change the default filepath of XRootD logfile (default: xrdlog)
--f : replace destination file (if destination is local it will be replaced only if integrity check fails)
--cksum : check hash sum of the file; for downloads the central catalogue md5 will be verified
--S <aditional streams> : uses num additional parallel streams to do the transfer. (max = 15)
--chunks <nr chunks> : number of chunks that should be requested in parallel
--chunksz <bytes> : chunk size (bytes)
--T <nr_copy_jobs> : number of parralel copy jobs from a set (for recursive copy); defaults to 8 for downloads
--timeout <seconds> : the job will fail if did not finish in this nr of seconds
--retry <times> : retry N times the copy process if failed
--ratethreshold <bytes/s> : fail the job if the speed is lower than specified bytes/s
--noxrdzip: circumvent the XRootD mechanism of zip member copy and download the archive and locally extract the intended member.
-N.B.!!! for recursive copy (all files) the same archive will be downloaded for each member.
-If there are problems with native XRootD zip mechanism, download only the zip archive and locally extract the contents
-
-For the recursive copy of directories the following options (of the find command) can be used:
--glob <globbing pattern> : this is the usual AliEn globbing format; {PrintColor(COLORS.BIGreen)}N.B. this is NOT a REGEX!!!{PrintColor(COLORS.ColorReset)} defaults to all "*"
--select <pattern> : select only these files to be copied; {PrintColor(COLORS.BIGreen)}N.B. this is a REGEX applied to full path!!!{PrintColor(COLORS.ColorReset)}
--name <pattern> : select only these files to be copied; {PrintColor(COLORS.BIGreen)}N.B. this is a REGEX applied to a directory or file name!!!{PrintColor(COLORS.ColorReset)}
--name <verb>_string : where verb = begin|contain|ends|ext and string is the text selection criteria.
-verbs are aditive : -name begin_myf_contain_run1_ends_bla_ext_root
-{PrintColor(COLORS.BIRed)}N.B. the text to be filtered cannont have underline <_> within!!!{PrintColor(COLORS.ColorReset)}
--parent <parent depth> : in destination use this <parent depth> to add to destination ; defaults to 0
--a : copy also the hidden files .* (for recursive copy)
--j <queue_id> : select only the files created by the job with <queue_id>  (for recursive copy)
--l <count> : copy only <count> nr of files (for recursive copy)
--o <offset> : skip first <offset> files found in the src directory (for recursive copy)
-
-Further filtering of the files can be applied with the following options:
--mindepth/-maxdepth N : restrict results to N directories depth relative to the base/searched for directory.
-                        N.B. for in directory globbing (/path1/path2/*.sh : the base directory is /path1/path2)
--minsize/-maxsize N : restrict results to at least/at most N bytes in size
--min-ctime/-max-ctime UNIX_TIME: restrict results to at least/at most this UNIX_TIME (ms, 13 decimals integer)
--user/-group string_name : restrict results to specified user/group
-'''
-
-
-def _xrdcp_sysproc(cmdline: str, timeout: Union[str, int, None] = None) -> RET:
-    """xrdcp stanalone system command"""
-    if not cmdline: return RET(1, '', '_xrdcp_sysproc :: no cmdline')
-    if timeout is not None: timeout = int(timeout)
-    # --nopbar --posc
-    xrdcp_cmdline = f'xrdcp -N -P {cmdline}'
-    return runShellCMD(xrdcp_cmdline, captureout = True, do_shell = False, timeout = timeout)
-
-
-def _xrdcp_copyjob(copy_job: CopyFile, xrd_cp_args: XrdCpArgs) -> int:  # , printout: str = ''
-    """xrdcp based task that process a copyfile and it's arguments"""
-    if not copy_job: return int(2)
-    # overwrite = xrd_cp_args.overwrite
-    # batch = xrd_cp_args.batch
-    # tpc = xrd_cp_args.tpc
-    # hashtype = xrd_cp_args.hashtype
-    # cksum = xrd_cp_args.cksum
-    timeout = xrd_cp_args.timeout
-    # rate = xrd_cp_args.rate
-    cmdline = f'{copy_job.src} {copy_job.dst}'
-    return retf_print(_xrdcp_sysproc(cmdline, timeout))
-
-
-def XrdCopy_xrdcp(job_list: list, xrd_cp_args: XrdCpArgs) -> list:  # , printout: str = ''
-    """XRootD copy command :: the actual XRootD copy process"""
-    if not _HAS_XROOTD:
-        print_err("XRootD not found or lower version thant 5.3.3")
-        return []
-    if not xrd_cp_args:
-        print_err("cp arguments are not set, XrdCpArgs tuple missing")
-        return []
-    # overwrite = xrd_cp_args.overwrite
-    # batch = xrd_cp_args.batch
-    # makedir = xrd_cp_args.makedir
-
-    # ctx = mp.get_context('forkserver')
-    # q = ctx.JoinableQueue()
-    # p = ctx.Process(target=_xrdcp_copyjob, args=(q,))
-    # p.start()
-    # print(q.get())
-    # p.join()
-    for copy_job in job_list:
-        if _DEBUG: logging.debug('\nadd copy job with\nsrc: %s\ndst: %s\n', copy_job.src, copy_job.dst)
-        # xrdcp_cmd = f' {copy_job.src} {copy_job.dst}'
-        if _DEBUG: print_out(copy_job)
-    return []
-
-
-def lfnAccessUrl(wb, lfn: str, local_file: str = '', specs: Union[None, list, str] = None, isWrite: bool = False, strictspec: bool = False, httpurl: bool = False) -> dict:
-    """Query central services for the access envelope of a lfn, it will return a lfn:server answer with envelope pairs"""
-    if not wb: return {}
-    if not lfn: return {}
-    if not specs: specs = []
-    if specs and isinstance(specs, str): specs = specs_split.split(specs)
-    if isWrite:
-        if not local_file or not os.path.exists(local_file):
-            print_err(f'lfnAccessUrl/write token:: invalid local file: {local_file}')
-            return {}
-        access_type = 'write'
-        size = int(os.stat(local_file).st_size)
-        md5sum = md5(local_file)
-        files_with_default_replicas = ['.sh', '.C', '.jdl', '.xml']
-        if any(lfn.endswith(ext) for ext in files_with_default_replicas) and size < 1048576 and not specs:  # we have a special lfn
-            specs.append('disk:4')  # and no specs defined then default to disk:4
-        get_envelope_arg_list = ['-s', size, '-m', md5sum, access_type, lfn]
-        if not specs: specs.append('disk:2')  # hard default if nothing is specified
-    else:
-        access_type = 'read'
-        get_envelope_arg_list = [access_type, lfn]
-
-    if specs: get_envelope_arg_list.append(",".join(specs))
-    if httpurl: get_envelope_arg_list.insert(0, '-u')
-    if strictspec: get_envelope_arg_list.insert(0, '-f')
-    ret_obj = SendMsg(wb, 'access', get_envelope_arg_list, opts = 'nomsg')
-    if ret_obj.exitcode != 0 or 'results' not in ret_obj.ansdict:
-        ret_obj = ret_obj._replace(err = f'No token for {lfn} :: errno {ret_obj.exitcode} -> {ret_obj.err}')
-        retf_print(ret_obj, opts = 'err noprint')
-        return {}
-    return ret_obj.ansdict
-
-
-def lfn2uri(wb, lfn: str, local_file: str = '', specs: Union[None, list, str] = None, isWrite: bool = False, strictspec: bool = False, httpurl: bool = False) -> str:
-    """Return the list of access URIs for all replica of an ALICE lfn - can be used directly with xrdcp"""
-    result = lfnAccessUrl(wb, lfn, local_file, specs, isWrite, strictspec, httpurl)
-    if not result: return ''
-    output_list = []
-    for replica in result['results']:
-        output_list.append(repr(f"{replica['url']}?xrd.wantprot=unix&authz={replica['envelope']}"))
-    return '\n'.join(output_list)
-
-
-def lfn2meta(wb, lfn: str, local_file: str = '', specs: Union[None, list, str] = None, isWrite: bool = False, strictspec: bool = False, httpurl: bool = False) -> str:
-    """Create metafile for download of an ALICE lfn and return it's location - can be used directly with xrdcp"""
-    if isWrite:
-        print_err('Metafile creation possible only for download')
-        return ''
-    result = lfnAccessUrl(wb, lfn, local_file, specs, isWrite, strictspec, httpurl)
-    if not result: return ''
-    size_4meta = result['results'][0]['size']  # size SHOULD be the same for all replicas
-    md5_4meta = result['results'][0]['md5']  # the md5 hash SHOULD be the same for all replicas
-    file_in_zip = None
-    url_list_4meta = []
-    for replica in result['results']:
-        url_components = replica['url'].rsplit('#', maxsplit = 1)
-        if len(url_components) > 1: file_in_zip = url_components[1]
-        # if is_pfn_readable(url_components[0]):  # it is a lot cheaper to check readability of replica than to try and fail a non-working replica
-        url_list_4meta.append(f'{url_components[0]}?xrd.wantprot=unix&authz={replica["envelope"]}')
-
-    # Create the metafile as a temporary uuid5 named file (the lfn can be retrieved from meta if needed)
-    metafile = create_metafile(make_tmp_fn(lfn, '.meta4', uuid5 = True), lfn, local_file, size_4meta, md5_4meta, url_list_4meta)
-    if not metafile:
-        print_err(f"Could not create the download metafile for {lfn}")
-        return ''
-    subprocess.run(shlex.split(f'mv {metafile} {os.getcwd()}/'), check = False)  # keep it in local directory
-    metafile = os.path.realpath(os.path.basename(metafile))
-    return f'{metafile}?xrdcl.unzip={file_in_zip}' if (file_in_zip and 'ALIENPY_NOXRDZIP' not in os.environ) else f'{metafile}'
-
-
-def lfn2fileTokens(wb, arg_lfn2file: lfn2file, specs: Union[None, list, str] = None, isWrite: bool = False, strictspec: bool = False, httpurl: bool = False) -> dict:
-    """Query central services for the access envelope of a lfn, it will return a lfn:server answer with envelope pairs"""
-    if not wb: return {}
-    if not arg_lfn2file: return {}
-    lfn = arg_lfn2file.lfn
-    file = arg_lfn2file.file
-    if not specs: specs = []
-    if specs and isinstance(specs, str): specs = specs_split.split(specs)
-    result = lfnAccessUrl(wb, lfn, file, specs, isWrite, strictspec, httpurl)
-    if not result:
-        return {"lfn": lfn, "answer": {}}
-    qos_tags = [el for el in specs if 'ALICE::' not in el]  # for element in specs, if not ALICE:: then is qos tag
-    SEs_list_specs = [el for el in specs if 'ALICE::' in el]  # explicit requests of SEs
-    SEs_list_total = [replica["se"] for replica in result["results"]]
-    # let's save for each replica the orginal request info
-    for replica in result["results"]:
-        replica["qos_specs"] = qos_tags  # qos tags from specs
-        replica["SElist_specs"] = SEs_list_specs  # SE from specs
-        replica["SElist"] = SEs_list_total  # list of SEs that were used
-        replica["file"] = file
-        replica["lfn"] = lfn
-    return {"lfn": lfn, "answer": result}
-
-
-def lfn2fileTokens_list(wb, input_lfn_list: list, specs: Union[None, list, str] = None, isWrite: bool = False, strictspec: bool = False, httpurl: bool = False) -> list:
-    """Query central services for the access envelope of the list of lfns, it will return a list of lfn:server answer with envelope pairs"""
-    if not wb: return []
-    access_list = []
-    if not input_lfn_list: return access_list
-    if specs is None: specs = []
-    for l2f in input_lfn_list: access_list.append(lfn2fileTokens(wb, l2f, specs, isWrite, strictspec, httpurl))
-    return access_list
-
-
-
-def path_grid_stat(wb, path: str) -> STAT_FILEPATH:
-    """Get full information on a GRID path/lfn"""
-    norm_path = expand_path_grid(path)
-    ret_obj = SendMsg(wb, 'stat', [norm_path], opts = 'nomsg log')
-    if ret_obj.exitcode != 0: return STAT_FILEPATH(norm_path)
-    file_stat = ret_obj.ansdict["results"][0]  # stat can query and return multiple results, but we are using only one
-    mtime = file_stat.get('mtime', '')
-    guid = file_stat.get('guid', '')
-    size = file_stat.get('size', '')
-    md5hash = file_stat.get('md5', '')
-    return STAT_FILEPATH(file_stat['lfn'], file_stat['type'], file_stat['perm'], file_stat['owner'], file_stat['gowner'], file_stat['ctime'],
-                         mtime, guid, size, md5hash)
-
-
-def path_grid_writable(file_stat: STAT_FILEPATH) -> bool:
-    p_user = int(file_stat['perm'][0])
-    p_group = int(file_stat['perm'][1])
-    p_others = int(file_stat['perm'][2])
-    writable_user = writable_group = writable_others = False
-    write_perm = {2, 6, 7}
-    if AlienSessionInfo['user'] == file_stat['uid'] and p_user in write_perm: writable_user = True
-    if AlienSessionInfo['user'] == file_stat['gid'] and p_group in write_perm: writable_group = True
-    if p_others in write_perm: writable_others = True
-    return writable_user or writable_group or writable_others
-
-
-def expand_path_grid(path_arg: str) -> str:
-    """Given a string representing a GRID file (lfn), return a full path after interpretation of AliEn HOME location, current directory, . and .. and making sure there are only single /"""
-    global AlienSessionInfo
-    is_dir = path_arg.endswith('/')
-    exp_path = lfn_prefix_re.sub('', path_arg)  # lets remove any prefixes
-    exp_path = re.sub(r"^\/*\%ALIEN[\/\s]*", AlienSessionInfo['alienHome'], exp_path)  # replace %ALIEN token with user grid home directory
-    if exp_path == '.': exp_path = AlienSessionInfo['currentdir']
-    if exp_path == '~': exp_path = AlienSessionInfo['alienHome']
-    if exp_path.startswith('./'): exp_path = exp_path.replace('.', AlienSessionInfo['currentdir'], 1)
-    if exp_path.startswith('~/'): exp_path = exp_path.replace('~', AlienSessionInfo['alienHome'], 1)  # replace ~ for the usual meaning
-    if not exp_path.startswith('/'): exp_path = f'{AlienSessionInfo["currentdir"]}/{exp_path}'  # if not full path add current directory to the referenced path
-    exp_path = os.path.normpath(exp_path)
-    if is_dir: exp_path = f'{exp_path}/'
-    return exp_path  # noqa: R504
-
-
-def pathtype_grid(wb, path: str) -> str:
-    """Query if a lfn is a file or directory, return f, d or empty"""
-    if not wb: return ''
-    if not path: return ''
-    ret_obj = SendMsg(wb, 'type', [path], opts = 'nomsg log')
-    if ret_obj.exitcode != 0: return ''
-    return str(ret_obj.ansdict['results'][0]["type"])[0]
-
-
-
-def create_metafile(meta_filename: str, lfn: str, local_filename: str, size: Union[str, int], md5in: str, replica_list: Union[None, list] = None) -> str:
-    """Generate a meta4 xrootd virtual redirector with the specified location and using the rest of arguments"""
-    if not (meta_filename and replica_list): return ''
-    try:
-        with open(meta_filename, 'w', encoding="ascii", errors="replace") as f:
-            published = str(datetime.datetime.now().replace(microsecond=0).isoformat())
-            f.write('<?xml version="1.0" encoding="UTF-8"?>\n')
-            f.write(' <metalink xmlns="urn:ietf:params:xml:ns:metalink">\n')
-            f.write(f'   <published>{published}</published>\n')
-            f.write(f'   <file name="{local_filename}">\n')
-            f.write(f'     <lfn>{lfn}</lfn>\n')
-            f.write(f'     <size>{size}</size>\n')
-            if md5in: f.write(f'     <hash type="md5">{md5in}</hash>\n')
-            for url in replica_list:
-                f.write(f'     <url><![CDATA[{url}]]></url>\n')
-            f.write('   </file>\n')
-            f.write(' </metalink>\n')
-        return meta_filename
-    except Exception:
-        logging.error(traceback.format_exc())
-        return ''
-
-
-def format_dst_fn(src_dir, src_file, dst, parent):
-    """Return the destination filename given the source dir/name, destination directory and number of parents to keep"""
-    # let's get destination file name (relative path with parent value)
-    if src_dir != src_file:  # recursive operation
-        total_relative_path = src_file.replace(src_dir, '', 1)
-        src_dir_path = Path(src_dir)
-        src_dir_parts = src_dir_path.parts
-        if not src_dir.endswith('/'): src_dir_parts = src_dir_parts[:-1]
-        src_dir = '/'.join(map(lambda x: str(x or ''), src_dir_parts))
-        src_dir = src_dir.replace('//', '/')
-        components_list = src_dir.split('/')
-        components_list[0] = '/'  # first slash is lost in split
-        file_components = len(components_list)  # it's directory'
-        parent = min(parent, file_components)  # make sure maximum parent var point to first dir in path
-        parent_selection = components_list[(file_components - parent):]
-        rootdir_src_dir = '/'.join(parent_selection)
-        file_relative_name = f'{rootdir_src_dir}/{total_relative_path}'
-    else:
-        src_file_path = Path(src_file)
-        file_components = len(src_file_path.parts) - 1 - 1  # without the file and up to slash
-        parent = min(parent, file_components)  # make sure maximum parent var point to first dir in path
-        rootdir_src_file = src_file_path.parents[parent].as_posix()
-        file_relative_name = src_file.replace(rootdir_src_file, '', 1)
-
-    dst_file = f'{dst}/{file_relative_name}' if dst.endswith('/') else dst
-    return os.path.normpath(dst_file)
-
-
-def setDst(file: str = '', parent: int = 0) -> str:
-    """For a given file path return the file path keeping the <parent> number of components"""
-    p = Path(file)
-    path_components = len(p.parts)
-    if parent >= (path_components - 1): parent = path_components - 1 - 1  # IF parent >= number of components without filename THEN make parent = number of component without / and filename
-    basedir = p.parents[parent].as_posix()
-    if basedir == '/': return file
-    return p.as_posix().replace(basedir, '', 1)
-
-
-def name2regex(pattern_regex: str = '') -> str:
-    if not pattern_regex: return ''
-    translated_pattern_regex = ''
-    re_all = '.*'
-    re_all_end = '[^/]*'
-    verbs = ('begin', 'contain', 'ends', 'ext')
-    pattern_list = pattern_regex.split('_')
-    if any(verb in pattern_regex for verb in verbs):
-        if pattern_list.count('begin') > 1 or pattern_list.count('end') > 1 or pattern_list.count('ext') > 1:
-            print_out('<begin>, <end>, <ext> verbs cannot appear more than once in the name selection')
-            return ''
-
-        list_begin = []
-        list_contain = []
-        list_ends = []
-        list_ext = []
-        for idx, tokenstr in enumerate(pattern_list):
-            if tokenstr == 'begin': list_begin.append(KV(tokenstr, pattern_list[idx + 1]))
-            if tokenstr == 'contain': list_contain.append(KV(tokenstr, pattern_list[idx + 1]))
-            if tokenstr == 'ends': list_ends.append(KV(tokenstr, pattern_list[idx + 1]))
-            if tokenstr == 'ext': list_ext.append(KV(tokenstr, pattern_list[idx + 1]))
-
-        if list_begin:
-            translated_pattern_regex = re_all + '/' + f'{list_begin[0].val}{re_all_end}'  # first string after the last slash (last match exclude /)
-        for patt in list_contain:
-            if not list_begin: translated_pattern_regex = f'{re_all}'
-            translated_pattern_regex = f'{translated_pattern_regex}{patt.val}{re_all_end}'
-        if list_ends:
-            translated_pattern_regex = f'{translated_pattern_regex}{list_ends[0].val}{re_all_end}'
-        if list_ext:
-            translated_pattern_regex = translated_pattern_regex + "\\." + list_ext[0].val
-        if translated_pattern_regex:
-            if list_ext:
-                translated_pattern_regex = f'{translated_pattern_regex}' + '$'
-            else:
-                translated_pattern_regex = f'{translated_pattern_regex}{re_all_end}' + '$'
-    return translated_pattern_regex  # noqa: R504
-
-
-def extract_glob_pattern(path_arg: str) -> tuple:
-    """Extract glob pattern from a path"""
-    if not path_arg: return None, None
-    base_path = pattern = None
-    if '*' in path_arg:  # we have globbing in src path
-        path_components = path_arg.split("/")
-        base_path_arr = []  # let's establish the base path
-        for el in path_components:
-            if '*' not in el: base_path_arr.append(el)
-            else: break
-
-        for el in base_path_arr: path_components.remove(el)  # remove the base path components (those without *) from full path components
-        base_path = f'{"/".join(base_path_arr)}{"/" if base_path_arr else ""}'  # rewrite the source path without the globbing part
-        pattern = '/'.join(path_components)  # the globbing part is the rest of element that contain *
-    else:
-        base_path = path_arg
-    return (base_path, pattern)
-
-
-def path_type(path_arg: str) -> tuple:
-    """Check if path is local or grid; default is grid and local must have file: prefix"""
-    location = 'local' if path_arg.startswith('file:') else 'grid'
-    return (path_arg, location)
-
-
-def commit(wb, tokenstr: str, size: int, lfn: str, perm: str, expire: str, pfn: str, se: str, guid: str, md5sum: str) -> RET:
-    """Upon succesful xrootd upload to server, commit the guid name into central catalogue"""
-    if not wb: return RET()
-    return SendMsg(wb, 'commit', [tokenstr, int(size), lfn, perm, expire, pfn, se, guid, md5sum], opts = 'log')
-
-
-def commitFile(wb, lfnInfo: CommitInfo) -> RET:
-    """Upon succesful xrootd upload to server, commit the guid name into central catalogue"""
-    if not wb or not lfnInfo: return RET()
-    return SendMsg(wb, 'commit', [lfnInfo.envelope, int(lfnInfo.size), lfnInfo.lfn, lfnInfo.perm, lfnInfo.expire, lfnInfo.pfn, lfnInfo.se, lfnInfo.guid, lfnInfo.md5], opts = 'log')
-
-
-def commitFileList(wb, lfnInfo_list: list) -> list:  # returns list of RET
-    """Upon succesful xrootd upload to server, commit the guid name into central catalogue for a list of pfns"""
-    if not wb or not lfnInfo_list: return []
-    batch_size = 30
-    batches_list = [lfnInfo_list[x: x + batch_size] for x in range(0, len(lfnInfo_list), batch_size)]
-    commit_results = []
-    for batch in batches_list:
-        commit_list = []
-        for file_commit in batch:
-            jsoncmd = CreateJsonCommand('commit', [file_commit.envelope, int(file_commit.size), file_commit.lfn,
-                                                   file_commit.perm, file_commit.expire, file_commit.pfn, file_commit.se,
-                                                   file_commit.guid, file_commit.md5],
-                                        'nokeys')
-            commit_list.append(jsoncmd)
-        commit_results.extend(SendMsgMulti(wb, commit_list, 'log'))
-    return commit_results
-
-
-def list_files_grid(wb, search_dir: str, pattern: Union[None, REGEX_PATTERN_TYPE, str] = None, is_regex: bool = False, find_args: Union[str, list, None] = None) -> RET:
-    """Return a list of files(lfn/grid files) that match pattern found in dir
-    Returns a RET object (from find), and takes: wb, directory, pattern, is_regex, find_args
-    """
-    if not search_dir: return RET(-1, "", "No search directory specified")
-
-    if find_args is None: find_args = []
-    find_args_list = find_args.split() if isinstance(find_args, str) else find_args.copy()
-
-    # lets process the pattern: extract it from src if is in the path globbing form
-    is_single_file = False  # dir actually point to a file
-
-    dir_arg_list = search_dir.split()
-    if len(dir_arg_list) > 1:  # dir is actually a list of arguments
-        if not pattern: pattern = dir_arg_list.pop(-1)
-        search_dir = dir_arg_list.pop(-1)
-        if dir_arg_list: find_args = ' '.join(dir_arg_list)
-
-    if '*' in search_dir:  # we have globbing in src path
-        is_regex = False
-        src_arr = search_dir.split("/")
-        base_path_arr = []  # let's establish the base path
-        for el in src_arr:
-            if '*' not in el:
-                base_path_arr.append(el)
-            else:
-                break
-        for el in base_path_arr: src_arr.remove(el)  # remove the base path
-        search_dir = '/'.join(base_path_arr) + '/'  # rewrite the source path without the globbing part
-        pattern = '/'.join(src_arr)  # the globbing part is the rest of element that contain *
-    else:  # pattern is specified by argument
-        if pattern is None:
-            if not search_dir.endswith('/'):  # this is a single file
-                is_single_file = True
-            else:
-                pattern = '*'  # prefer globbing as default
-        elif type(pattern) is REGEX_PATTERN_TYPE:  # unlikely but supported to match signatures # noqa: PIE789,PLC0123
-            pattern = pattern.pattern  # We pass the regex pattern into command as string
-            is_regex = True
-
-        # it was explictly requested that pattern is regex
-        if is_regex and isinstance(pattern, str) and valid_regex(pattern) is None:
-            msg = f'list_files_grid:: {pattern} failed to re.compile'
-            logging.error(msg)
-            return RET(-1, '', msg)
-
-    # remove default from additional args
-    filter_args_list = []
-    get_arg(find_args_list, '-a')
-    get_arg(find_args_list, '-s')
-    get_arg(find_args_list, '-f')
-    get_arg(find_args_list, '-d')
-    get_arg(find_args_list, '-w')
-    get_arg(find_args_list, '-wh')
-
-    exclude_string = get_arg_value(find_args_list, '-exclude')
-    if exclude_string:
-        filter_args_list.extend(['-exclude', exclude_string])
-
-    exclude_regex = get_arg_value(find_args_list, '-exclude_re')
-    if exclude_regex:
-        filter_args_list.extend(['-exclude_re', exclude_regex])
-
-    min_depth = get_arg_value(find_args_list, '-mindepth')
-    if min_depth:
-        if not min_depth.isdigit() or min_depth.startswith("-"):
-            print_err(f'list_files_grid::mindepth arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-mindepth', min_depth])
-
-    max_depth = get_arg_value(find_args_list, '-maxdepth')
-    if max_depth:
-        if not max_depth.isdigit() or max_depth.startswith("-"):
-            print_err(f'list_files_grid::maxdepth arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-maxdepth', max_depth])
-
-    min_size = get_arg_value(find_args_list, '-minsize')
-    if min_size:
-        if not min_size.isdigit() or min_size.startswith("-"):
-            print_err(f'list_files_grid::minsize arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-minsize', min_size])
-
-    max_size = get_arg_value(find_args_list, '-maxsize')
-    if max_size:
-        if not max_size.isdigit() or max_size.startswith("-"):
-            print_err(f'list_files_grid::maxsize arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-maxsize', max_size])
-
-    min_ctime = get_arg_value(find_args_list, '-min-ctime')
-    if min_ctime:
-        if min_ctime.startswith("-"):
-            print_err(f'list_files_grid::min-ctime arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-min-ctime', min_ctime])
-
-    max_ctime = get_arg_value(find_args_list, '-max-ctime')
-    if max_ctime:
-        if max_ctime.startswith("-"):
-            print_err(f'list_files_grid::max-ctime arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-max-ctime', max_ctime])
-
-    jobid = get_arg_value(find_args_list, '-jobid')
-    if jobid:
-        if not jobid.isdigit() or jobid.startswith("-"):
-            print_err(f'list_files_grid::jobid arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-jobid', jobid])
-
-    user = get_arg_value(find_args_list, '-user')
-    if user:
-        if not user.isalpha() or user.startswith("-"):
-            print_err(f'list_files_grid::user arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-user', user])
-
-    group = get_arg_value(find_args_list, '-group')
-    if group:
-        if not group.isalpha() or group.startswith("-"):
-            print_err(f'list_files_grid::group arg not recognized: {" ".join(find_args_list)}')
-        else:
-            filter_args_list.extend(['-group', group])
-
-    # create and return the list object just for a single file
-    if is_single_file:
-        send_opts = 'nomsg' if not _DEBUG else ''
-        ret_obj = SendMsg(wb, 'stat', [search_dir], opts = send_opts)
-    else:
-        find_args_default = ['-f', '-a', '-s']
-        if is_regex: find_args_default.insert(0, '-r')
-        if find_args_list: find_args_default.extend(find_args_list)  # insert any other additional find arguments
-        find_args_default.append(search_dir)
-        find_args_default.append(pattern)
-        send_opts = 'nomsg' if not _DEBUG else ''
-        ret_obj = SendMsg(wb, 'find', find_args_default, opts = send_opts)
-
-    if ret_obj.exitcode != 0:
-        logging.error('list_files_grid error:: %s %s %s', search_dir, pattern, find_args)
-        return ret_obj
-    if 'results' not in ret_obj.ansdict or not ret_obj.ansdict["results"]:
-        logging.error('list_files_grid exitcode==0 but no results(!!!):: %s /pattern: %s /find_args: %s', search_dir, pattern, find_args)
-        return RET(2, '', f'No files found in :: {search_dir} /pattern: {pattern} /find_args: {find_args}')
-
-    exitcode = ret_obj.exitcode
-    stderr = ret_obj.err
-    results_list = ret_obj.ansdict["results"]
-    results_list_filtered = []
-    # items that pass the conditions are the actual/final results
-
-    compiled_regex = None
-    if exclude_regex: compiled_regex = re.compile(exclude_regex)   # precompile the regex for exclusion
-
-    for found_lfn_dict in results_list:  # parse results to apply filters
-        if not filter_file_prop(found_lfn_dict, search_dir, filter_args_list, compiled_regex): continue
-        results_list_filtered.append(found_lfn_dict)  # at this point all filters were passed
-
-    if not results_list_filtered:
-        return RET(2, "", f"No files passed the filters :: {search_dir} /pattern: {pattern} /find_args: {find_args}")
-
-    ansdict = {"results": results_list_filtered}
-    lfn_list = [get_lfn_key(lfn_obj) for lfn_obj in results_list_filtered]
-    stdout = '\n'.join(lfn_list)
-    return RET(exitcode, stdout, stderr, ansdict)
-
-
-
-
-
-def makelist_lfn(wb, arg_source, arg_target, find_args: list, parent: int, overwrite: bool, pattern: Union[None, REGEX_PATTERN_TYPE, str], is_regex: bool, copy_list: list, strictspec: bool = False, httpurl: bool = False) -> RET:  # pylint: disable=unused-argument
+def makelist_lfn(wb, arg_source, arg_target, find_args: Union[None, list] = None, copy_list: Union[None, list] = None, pattern: Union[None, REGEX_PATTERN_TYPE, str] = None, parent: int = 999, overwrite: bool = False, is_regex: bool = False, strictspec: bool = False, httpurl: bool = False) -> RET:  # pylint: disable=unused-argument
     """Process a source and destination copy arguments and make a list of individual lfns to be copied"""
     isSrcDir = isSrcLocal = isDownload = specs = None  # make sure we set these to valid values later
+    if find_args is None: find_args = []
+    if copy_list is None or not isinstance(copy_list, list):
+        print_out('makelist_lfn:: copy_list arguments is not a list!!')
+        return RET()
 
     # lets extract the specs from both src and dst if any (to clean up the file-paths) and record specifications like disk=3,SE1,!SE2
     src_specs_remotes = specs_split.split(arg_source, maxsplit = 1)  # NO comma allowed in names (hopefully)
     arg_src = src_specs_remotes.pop(0)  # first item is the file path, let's remove it; it remains disk specifications
     src_specs = src_specs_remotes.pop(0) if src_specs_remotes else None  # whatever remains is the specifications
 
     dst_specs_remotes = specs_split.split(arg_target, maxsplit = 1)
     arg_dst = dst_specs_remotes.pop(0)
     dst_specs = dst_specs_remotes.pop(0) if dst_specs_remotes else None
 
+    arg_src = re.sub(r"^\/*\%ALIEN[\/\s]*", AlienSessionInfo['alienHome'], arg_src)  # replace %ALIEN token with user grid home directory
+    arg_dst = re.sub(r"^\/*\%ALIEN[\/\s]*", AlienSessionInfo['alienHome'], arg_dst)  # replace %ALIEN token with user grid home directory
+
     # lets process the pattern: extract it from src if is in the path globbing form
     src_glob = False
     if '*' in arg_src:  # we have globbing in src path
         src_glob = True
         arg_src, pattern = extract_glob_pattern(arg_src)
     else:  # pattern is specified by argument
         if type(pattern) is REGEX_PATTERN_TYPE:  # unlikely but supported to match signatures
@@ -695,30 +138,30 @@
 
     slashend_src = arg_src.endswith('/')  # after extracting the globbing if present we record the slash
     # N.B.!!! the check will be wrong when the same relative path is present local and on grid
     # first let's check only prefixes
     src, src_type = path_type(arg_src)
     dst, dst_type = path_type(arg_dst)
 
-    if src_type == dst_type == 'grid':
-        return RET(1, '', 'grid to grid copy is WIP; for the moment use two steps: download file and upload it; local src,dst should be ALWAYS prefixed with file:')
-    if src_type == dst_type == 'local':
-        return RET(1, '', 'for local copy use system command; within interactiv shell start a system command with "!"')
-
     isSrcLocal = (src_type == 'local')
     isDownload = not isSrcLocal
     if isSrcLocal:  # UPLOAD
         src_stat = path_local_stat(src)
         dst_stat = path_grid_stat(wb, dst)
     else:           # DOWNLOAD
         src_stat = path_grid_stat(wb, src)
         dst_stat = path_local_stat(dst)
-        if not path_writable_any(dst_stat.path):
+        if not path_writable_any(dst_stat.path) and not parent > 1:
             return RET(2, '', f'no write permission/or missing in any component of {dst_stat.path}')
 
+    if src_type == dst_type == 'grid':
+        return RET(1, '', 'grid to grid copy is WIP; for the moment use two steps: download file and upload it; local src,dst should be ALWAYS prefixed with file:')
+    if src_type == dst_type == 'local':
+        return RET(1, '', 'for local copy use system command; within interactiv shell start a system command with "!"')
+
     if not src_stat.type: return RET(2, '', f'Specified source {src_stat.path} not found!')
 
     src = src_stat.path
     dst = dst_stat.path
 
     if not src: return RET(2, '', f'{arg_src} => {src} does not exist (or not accessible) on {src_type}')  # ENOENT /* No such file or directory */
 
@@ -732,15 +175,15 @@
     # prepare destination locations
     if isDownload:
         try:  # we can try anyway, this is like mkdir -p
             mk_path = Path(dst) if dst.endswith('/') else Path(dst).parent  # if destination is file create it dir parent
             mk_path.mkdir(parents=True, exist_ok=True)
         except Exception:
             logging.error(traceback.format_exc())
-            msg = f"Could not create local destination directory: {mk_path.as_posix()}\ncheck log file {_DEBUG_FILE}"
+            msg = f"Could not create local destination directory: {mk_path.as_posix()}\ncheck log file {DEBUG_FILE}"
             return RET(42, '', msg)  # ENOMSG /* No message of desired type */
     else:  # this is upload to GRID
         mk_path = dst if dst.endswith('/') else Path(dst).parent.as_posix()
         if not dst_stat.type:  # dst does not exists
             ret_obj = SendMsg(wb, 'mkdir', ['-p', mk_path], opts = 'nomsg')  # do it anyway, there is not point in checking before
             if retf_print(ret_obj, opts = 'noprint err') != 0: return ret_obj  # just return the mkdir result  # noqa: R504
 
@@ -764,15 +207,15 @@
             if not skip_file:
                 tokens = lfn2fileTokens(wb, lfn2file(src, dst_filename), specs_list, isWrite, strictspec, httpurl)
                 if tokens and 'answer' in tokens:
                     copy_list.append(CopyFile(src, dst_filename, isWrite, tokens['answer'], src))
         else:  # directory to be listed
             results_list = list_files_grid(wb, src, pattern, is_regex, " ".join(find_args))
             if "results" not in results_list.ansdict or len(results_list.ansdict["results"]) < 1:
-                msg = f"No files found with: find {' '.join(find_args) if find_args else ''}{' -r ' if is_regex else ''}-a -s {src} {pattern}"
+                msg = f"No files found with: find {' '.join(find_args) if find_args else ''}{' -r ' if is_regex else ''} -a -s {src} {pattern}"
                 return RET(42, '', msg)  # ENOMSG /* No message of desired type */
 
             for lfn_obj in results_list.ansdict["results"]:  # make CopyFile objs for each lfn
                 lfn = get_lfn_key(lfn_obj)
                 dst_filename = format_dst_fn(src, lfn, dst, parent)
                 # if overwrite the file validity checking will do md5
                 skip_file = (retf_print(fileIsValid(dst_filename, lfn_obj['size'], lfn_obj['md5'], shallow_check = not overwrite), opts = 'noerr') == 0)
@@ -786,15 +229,14 @@
         results_list = list_files_local(src, pattern, is_regex, " ".join(find_args))
         if "results" not in results_list.ansdict or len(results_list.ansdict["results"]) < 1:
             msg = f"No files found in: {src} /pattern: {pattern} /find_args: {' '.join(find_args)}"
             return RET(42, '', msg)  # ENOMSG /* No message of desired type */
 
         for file in results_list.ansdict["results"]:
             file_path = get_lfn_key(file)
-            print(file_path)
             lfn = format_dst_fn(src, file_path, dst, parent)
             lfn_dst_stat = path_grid_stat(wb, lfn)  # check each destination lfn
             if lfn_dst_stat.type == 'f':  # lfn exists
                 if not overwrite:
                     print_out(f'{lfn} exists, skipping..')
                     continue
                 md5sum = md5(file_path)
@@ -837,33 +279,40 @@
 
             # Create the metafile as a temporary uuid5 named file (the lfn can be retrieved from meta if needed)
             metafile = create_metafile(make_tmp_fn(cpfile.src, '.meta4', uuid5 = True), cpfile.src, cpfile.dst, size_4meta, md5_4meta, url_list_4meta)
             if not metafile:
                 print_err(f"Could not create the download metafile for {cpfile.src}")
                 continue
             if file_in_zip and 'ALIENPY_NOXRDZIP' not in os.environ: metafile = f'{metafile}?xrdcl.unzip={file_in_zip}'
-            if _DEBUG: print_out(f'makelist_xrdjobs:: {metafile}')
+            if DEBUG: print_out(f'makelist_xrdjobs:: {metafile}')
             copylist_xrd.append(CopyFile(metafile, cpfile.dst, cpfile.isUpload, {}, cpfile.src))  # we do not need the tokens in job list when downloading
 
 
+def DO_XrootdCp(wb, xrd_copy_command: Union[None, list] = None, printout: str = '', api_src: Union[None, list] = None, api_dst: Union[None, list] = None) -> RET:
+    """XRootD cp function :: process list of arguments for a xrootd copy command"""
+    if not HAS_XROOTD: return RET(1, "", 'DO_XrootdCp:: python XRootD module not found or lower than 5.3.3, the copy process cannot continue')
 
+    if xrd_copy_command is None: xrd_copy_command = []
+    if api_src is None: api_src =[]
+    if api_dst is None: api_dst =[]
 
+    if bool(api_src) ^ bool(api_dst): return RET(1, '', 'API _src,_dst used but only one is defined')
+    if len(api_src) != len(api_dst): return RET(1, '', 'API _src,_dst used but not of equal lenght')
 
-
-def DO_XrootdCp(wb, xrd_copy_command: Union[None, list] = None, printout: str = '') -> RET:
-    """XRootD cp function :: process list of arguments for a xrootd copy command"""
-    if not _HAS_XROOTD: return RET(1, "", 'DO_XrootdCp:: python XRootD module not found or lower than 5.3.3, the copy process cannot continue')
-    if xrd_copy_command is None: xrd_copy_command = []
-    global AlienSessionInfo
     if not wb: return RET(107, "", 'DO_XrootdCp:: websocket not found')  # ENOTCONN /* Transport endpoint is not connected */
 
-    if not xrd_copy_command or len(xrd_copy_command) < 2 or is_help(xrd_copy_command):
+    if is_help(xrd_copy_command):
+        help_msg = xrdcp_help()
+        return RET(0, help_msg)
+
+    if (not api_src) and (len(xrd_copy_command) < 2):
         help_msg = xrdcp_help()
-        return RET(0, help_msg)  # EX_USAGE /* command line usage error */
+        return RET(22, '', f'\n{help_msg}')  # 22 /* Invalid argument */
 
+    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     xrd_config_init()  # reset XRootD preferences to cp oriented settings
 
     # XRootD copy parameters
     # inittimeout: copy initialization timeout(int)
     # tpctimeout: timeout for a third-party copy to finish(int)
     # coerce: ignore file usage rules, i.e. apply `FORCE` flag to open() (bool)
     # :param checksummode: checksum mode to be used #:type    checksummode: string
@@ -875,31 +324,14 @@
     chunks = int(4)  # number of chunks that should be requested in parallel; use defaults from XrdCl/XrdClConstants.hh
     chunksize = int(8388608)  # chunk size for remote transfers; use defaults from XrdCl/XrdClConstants.hh
     overwrite = bool(False)  # overwrite target if it exists
     cksum = bool(False)
     timeout = int(0)
     rate = int(0)
 
-    if get_arg(xrd_copy_command, '-d'):
-        if os.getenv('XRD_LOGLEVEL'): print_out('XRD_LOGLEVEL already set, it will be overwritten with Info')
-        XRD_EnvPut('XRD_LOGLEVEL', 'Info')
-    if get_arg(xrd_copy_command, '-dd'):
-        if os.getenv('XRD_LOGLEVEL'): print_out('XRD_LOGLEVEL already set, it will be overwritten with Debug')
-        XRD_EnvPut('XRD_LOGLEVEL', 'Debug')
-    if get_arg(xrd_copy_command, '-ddd'):
-        if os.getenv('XRD_LOGLEVEL'): print_out('XRD_LOGLEVEL already set, it will be overwritten with Dump')
-        XRD_EnvPut('XRD_LOGLEVEL', 'Dump')
-
-    XRD_LOG = 'xrdlog.txt'
-    xrd_logfile_arg = get_arg_value(xrd_copy_command, '-xrdlog')
-    if xrd_logfile_arg:
-        if os.getenv('XRD_LOGFILE'): print_out(f'XRD_LOGFILE already set, it will be overwritten with {xrd_logfile_arg}')
-        XRD_LOG = xrd_logfile_arg
-    XRD_EnvPut('XRD_LOGFILE', XRD_LOG)
-
     streams_arg = get_arg_value(xrd_copy_command, '-S')
     if streams_arg:
         if is_int(streams_arg):
             streams = min(abs(int(streams)), 15)
             if os.getenv('XRD_SUBSTREAMSPERCHANNEL'):
                 print_out(f'Warning! env var XRD_SUBSTREAMSPERCHANNEL is set and will be overwritten with value: {streams}')
             XRD_EnvPut('SubStreamsPerChannel', streams)
@@ -936,22 +368,31 @@
     rate_arg = get_arg_value(xrd_copy_command, '-ratethreshold')
     if rate_arg:
         rate = abs(int(rate_arg))
         XRD_EnvPut('XRateThreshold', rate)
 
     XRD_EnvPut('CpRetryPolicy', 'force')
     retry_arg = get_arg_value(xrd_copy_command, '-retry')
-    if rate_arg:
+    if retry_arg:
         retry = abs(int(retry_arg))
         XRD_EnvPut('CpRetry', retry)
 
     _use_system_xrdcp = get_arg(xrd_copy_command, '-xrdcp')
-    overwrite = get_arg(xrd_copy_command, '-f')
-    cksum = get_arg(xrd_copy_command, '-cksum')
-
+    f_arg = get_arg(xrd_copy_command, '-f')
+    if f_arg:
+        print_out('No longer used flag! md5 verification of present destination is default; disable with -fastcheck')
+    
+    fastcheck = get_arg(xrd_copy_command, '-fastcheck')
+    overwrite = not fastcheck 
+    
+    get_arg(xrd_copy_command, '-cksum')
+    cksum = True
+ 
+    dryrun = get_arg(xrd_copy_command, '-dryrun')
+ 
     tpc = 'none'
     if get_arg(xrd_copy_command, '-tpc'): tpc = 'first'
     if tpc != 'none': return RET(1, "", 'DO_XrootdCp:: TPC is not allowed!!')
 
     y_arg_val = get_arg_value(xrd_copy_command, '-y')
     # sources = int(y_arg_val)
     if y_arg_val: print_out("Ignored option! multiple source usage is known to break the files stored in zip files, so better to be ignored")
@@ -965,39 +406,77 @@
     httpurl = get_arg(xrd_copy_command, '-http')
 
     # keep this many path components into destination filepath
     parent = int(0)
     parent_arg = get_arg_value(xrd_copy_command, '-parent')
     if parent_arg: parent = int(parent_arg)
 
+    # explicit specify a destination, the rest of arguments are source files
+    dst_arg_specified = get_arg_value(xrd_copy_command, '-dst')
+
     # find options for recursive copy of directories
     find_args = []
     if get_arg(xrd_copy_command, '-v'): print_out("Verbose mode not implemented, ignored; enable debugging with ALIENPY_DEBUG=1")
-    if get_arg(xrd_copy_command, '-a'): print_out("-a is enabled as default")
-    if get_arg(xrd_copy_command, '-s'): print_out("-s is enabled as default")
-    if get_arg(xrd_copy_command, '-f'): print_out("-f API flag not usefull for copy operations")
-    if get_arg(xrd_copy_command, '-w'): print_out("-w flag not usefull for copy operations")
-    if get_arg(xrd_copy_command, '-wh'): print_out("-wh flag not usefull for copy operations")
-    if get_arg(xrd_copy_command, '-d'): print_out("-d flag not usefull for copy operations")
+
+    # find options not used or controlled
+    get_arg(xrd_copy_command, '-a')
+    get_arg(xrd_copy_command, '-s')
+    get_arg(xrd_copy_command, '-c')
+    get_arg(xrd_copy_command, '-w')
+    get_arg(xrd_copy_command, '-wh')
+    get_arg(xrd_copy_command, '-d')
 
     mindepth_arg = get_arg_value(xrd_copy_command, '-mindepth')
     if mindepth_arg: find_args.extend(['-mindepth', mindepth_arg])
 
     maxdepth_arg = get_arg_value(xrd_copy_command, '-maxdepth')
     if maxdepth_arg: find_args.extend(['-maxdepth', maxdepth_arg])
 
+    minsize_arg = get_arg_value(xrd_copy_command, '-minsize')
+    if minsize_arg: find_args.extend(['-minsize', minsize_arg])
+
+    maxsize_arg = get_arg_value(xrd_copy_command, '-maxsize')
+    if maxsize_arg: find_args.extend(['-maxsize', maxsize_arg])
+
+    minctime_arg = get_arg_value(xrd_copy_command, '-min-ctime')
+    if minctime_arg: find_args.extend(['-min-ctime', minctime_arg])
+
+    maxctime_arg = get_arg_value(xrd_copy_command, '-max-ctime')
+    if maxctime_arg: find_args.extend(['-max-ctime', maxctime_arg])
+
+    exclude_str_arg = get_arg_value(xrd_copy_command, '-exclude')
+    if exclude_str_arg: find_args.extend(['-exclude', exclude_str_arg])
+
+    exclude_re_arg = get_arg_value(xrd_copy_command, '-exclude_re')
+    if exclude_re_arg: find_args.extend(['-exclude_re', exclude_re_arg])
+
+    user_arg = get_arg_value(xrd_copy_command, '-user')
+    if user_arg: find_args.extend(['-user', user_arg])
+
+    group_arg = get_arg_value(xrd_copy_command, '-group')
+    if group_arg: find_args.extend(['-group', group_arg])
+
+    jobid_arg = get_arg_value(xrd_copy_command, '-jobid')
+    if jobid_arg: find_args.extend(['-jobid', jobid_arg])
+
     qid = get_arg_value(xrd_copy_command, '-j')
     if qid: find_args.extend(['-j', qid])
 
     files_limit = get_arg_value(xrd_copy_command, '-l')
     if files_limit: find_args.extend(['-l', files_limit])
 
     offset = get_arg_value(xrd_copy_command, '-o')
     if offset: find_args.extend(['-o', offset])
 
+    ref_site = get_arg_value(xrd_copy_command, '-site')
+    if ref_site: find_args.extend(['-S', ref_site])
+
+    exclude_pattern = get_arg_value(xrd_copy_command, '-e')
+    if exclude_pattern: find_args.extend(['-e', exclude_pattern])
+
     use_regex = False
     filtering_enabled = False
     pattern = get_arg_value(xrd_copy_command, '-glob')
     if pattern:
         use_regex = False
         filtering_enabled = True
 
@@ -1022,50 +501,74 @@
         if use_regex and not pattern_regex:
             msg = ("-name :: No selection verbs were recognized!"
                    "usage format is -name <attribute>_<string> where attribute is one of: begin, contain, ends, ext"
                    f"The invalid pattern was: {pattern_regex}")
             return RET(22, '', msg)  # EINVAL /* Invalid argument */
 
     if use_regex: pattern = pattern_regex
-    copy_lfnlist = []  # list of lfn copy tasks
 
     inputfile_arg = get_arg_value(xrd_copy_command, '-input')  # input file with <source, destination> pairs
-    if inputfile_arg:
+
+    # Start of resolving src to dst pairs
+    copy_lfnlist = []  # list of lfn copy tasks
+
+    if api_src and api_dst:
+        for src,dst in zip(api_src, api_dst):
+            retobj = makelist_lfn(wb, src, dst, find_args = find_args, parent = parent, overwrite = overwrite, pattern = pattern, is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
+            if retobj.exitcode != 0: print_err(retobj.err)  # if any error let's just return what we got  # noqa: R504
+    elif inputfile_arg:
         cp_arg_list = fileline2list(inputfile_arg)
         if not cp_arg_list: return RET(1, '', f'Input file {inputfile_arg} not found or invalid content')
         for cp_line in cp_arg_list:
             cp_line_items = cp_line.strip().split()
             if len(cp_line_items) > 2:
                 print_out(f'Line skipped, it has more than 2 arguments => f{cp_line.strip()}')
                 continue
             retobj = makelist_lfn(wb, cp_line_items[0], cp_line_items[1], find_args, parent, overwrite, pattern, use_regex, copy_lfnlist, strictspec, httpurl)
             retf_print(retobj, "noout err")  # print error and continue with the other files
+    elif dst_arg_specified:
+            # the assumption is that every argument from arg list was removed and what remain is a list of sources
+            common_root_path = common_path(xrd_copy_command)
+            for src in xrd_copy_command:
+                retobj = makelist_lfn(wb, src, f'{dst_arg_specified}/{src.replace(common_root_path, "")}', find_args = find_args, parent = parent, overwrite = overwrite, pattern = pattern, is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
+                if retobj.exitcode != 0: print_err(retobj.err)  # if any error let's just return what we got  # noqa: R504
     else:
-        retobj = makelist_lfn(wb, xrd_copy_command[-2], xrd_copy_command[-1], find_args, parent, overwrite, pattern, use_regex, copy_lfnlist, strictspec, httpurl)
+        if len(xrd_copy_command) < 2:
+            return RET(1, '', 'Argument list invalid (less then 2 arguments)')    
+        src = xrd_copy_command[-2]
+        dst = xrd_copy_command[-1]
+        retobj = makelist_lfn(wb, src, dst, find_args = find_args, parent = parent, overwrite = overwrite, pattern = pattern, is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
         if retobj.exitcode != 0: return retobj  # if any error let's just return what we got  # noqa: R504
 
-    if not copy_lfnlist:  # at this point if any errors, the processing was already stopped
-        return RET(0)
+    # at this point if any errors, the processing was already stopped
+    if not copy_lfnlist: return RET(0, 'No copy jobs to be done!')
 
-    if _DEBUG:
+    if DEBUG:
         logging.debug("We are going to copy these files:")
-        for file in copy_lfnlist: logging.debug(file)
+        for f in copy_lfnlist: logging.debug(f)
 
     # create a list of copy jobs to be passed to XRootD mechanism
     xrdcopy_job_list = []
     makelist_xrdjobs(copy_lfnlist, xrdcopy_job_list)
 
     if not xrdcopy_job_list:
         msg = "No XRootD operations in list! enable the DEBUG mode for more info"
         logging.info(msg)
         return RET(2, '', msg)  # ENOENT /* No such file or directory */
 
-    if _DEBUG:
+    if DEBUG:
         logging.debug("XRootD copy jobs:")
-        for file in xrdcopy_job_list: logging.debug(file)
+        for f in xrdcopy_job_list: logging.debug(f)
+
+    if dryrun:
+        msg = ''
+        for f in xrdcopy_job_list:
+            c_msg = f'{f.src} -> {f.lfn} ({f.token_request["se"]})' if f.isUpload else f'{f.lfn} -> {f.dst}'
+            msg = f'{msg}{c_msg}\n'
+        return RET(0, msg)
 
     msg1 = msg2 = msg3 = msg_sum = ''
     copy_jobs_nr = copy_jobs_nr1 = copy_jobs_nr2 = 0
     copy_jobs_failed_nr = copy_jobs_failed_nr1 = copy_jobs_failed_nr2 = 0
     copy_jobs_success_nr = copy_jobs_success_nr1 = copy_jobs_success_nr2 = 0
 
     my_cp_args = XrdCpArgs(overwrite, batch, tpc, hashtype, cksum, timeout, rate)
@@ -1146,15 +649,15 @@
         msg_sum = f"Succesful jobs (total): {copy_jobs_success_nr_total}/{copy_jobs_nr_total}" if not ('quiet' in printout or 'silent' in printout) else ''
         msg_list.append(msg_sum)
     msg_all = '\n'.join(x.strip() for x in msg_list if x.strip())
     if 'ALIENPY_NOXRDZIP' in os.environ: os.environ.pop("ALIENPY_NOXRDZIP")
     return RET(0, msg_all) if copy_jobs_success_nr_total > 0 else RET(1, '', msg_all)
 
 
-if _HAS_XROOTD:
+if HAS_XROOTD:
     class MyCopyProgressHandler(xrd_client.utils.CopyProgressHandler):
         """Custom ProgressHandler for XRootD copy process"""
         __slots__ = ('wb', 'copy_failed_list', 'jobs', 'job_list', 'xrdjob_list', 'succesful_writes', 'printout', 'debug')
 
         def __init__(self):
             self.wb = None
             self.copy_failed_list = []  # record the failed jobs
@@ -1182,30 +685,34 @@
                 status = f'{PrintColor(COLORS.Green)}OK{PrintColor(COLORS.ColorReset)}'
             elif results['status'].error:
                 status = f'{PrintColor(COLORS.BRed)}ERROR{PrintColor(COLORS.ColorReset)}'
             elif results['status'].fatal:
                 status = f'{PrintColor(COLORS.BIRed)}FATAL{PrintColor(COLORS.ColorReset)}'
             else:
                 status = f'{PrintColor(COLORS.BIRed)}UNKNOWN{PrintColor(COLORS.ColorReset)}'
+
             job_info = self.job_list[jobId - 1]
             xrdjob = self.xrdjob_list[jobId - 1]  # joblist initilized when starting; we use the internal index to locate the job
             replica_dict = xrdjob.token_request
             job_status_info = f"jobID: {jobId}/{self.jobs} >>> STATUS {status}"
 
             deltaT = datetime.datetime.now().timestamp() - float(job_info['start'])
-            if os.getenv('XRD_LOGLEVEL'): logging.debug('XRD copy job time:: %s -> %s', xrdjob.lfn, deltaT)
+            if os.getenv('XRD_LOGLEVEL'):
+                logging.debug('XRD copy job time:: %s -> %s', xrdjob.lfn, deltaT)
+                logging.debug(results)
 
             if results['status'].ok:
                 speed = float(job_info['bytes_total']) / deltaT
-                speed_str = f'{GetHumanReadable(speed)}/s'
+                speed_str = f'{GetHumanReadableSize(speed)}/s'
 
                 if xrdjob.isUpload:  # isUpload
+                    md5 = results['sourceCheckSum'].replace('md5:','',1)
                     perm = '644'
                     expire = '0'
-                    self.succesful_writes.append(CommitInfo(replica_dict['envelope'], replica_dict['size'], xrdjob.lfn, perm, expire, replica_dict['url'], replica_dict['se'], replica_dict['guid'], replica_dict['md5']))
+                    self.succesful_writes.append(CommitInfo(replica_dict['envelope'], replica_dict['size'], xrdjob.lfn, perm, expire, replica_dict['url'], replica_dict['se'], replica_dict['guid'], md5))
                 else:  # isDownload
                     # NOXRDZIP was requested
                     if 'ALIENPY_NOXRDZIP' in os.environ and os.path.isfile(xrdjob.dst) and zipfile.is_zipfile(xrdjob.dst):
                         src_file_name = os.path.basename(xrdjob.lfn)
                         dst_file_name = os.path.basename(xrdjob.dst)
                         dst_file_path = os.path.dirname(xrdjob.dst)
                         zip_name = f'{xrdjob.dst}_{uuid.uuid4()}.zip'
@@ -1225,25 +732,25 @@
                 codes_info = f">>> ERRNO/CODE/XRDSTAT {results['status'].errno}/{results['status'].code}/{results['status'].status}"
                 xrd_resp_msg = results['status'].message
                 failed_after = f'Failed after {deltaT}'
                 if xrdjob.isUpload:
                     msg = f"{job_status_info} : {xrdjob.token_request['file']} to {xrdjob.token_request['se']}, {xrdjob.token_request['nSEs']} replicas\n{xrd_resp_msg}"
                 else:
                     msg = f"{job_status_info} : {xrdjob.lfn}\n{xrd_resp_msg}"
-                if _DEBUG: msg = f'{msg}\n{failed_after}'
+                if DEBUG: msg = f'{msg}\n{failed_after}'
                 logging.error('\n%s\n%s', codes_info, msg)
                 print_err(msg)
                 defined_reqtimeout = float(XRD_EnvGet('RequestTimeout'))
                 if deltaT >= defined_reqtimeout:
                     print_err(f'Copy job duration >= RequestTimeout default setting ({defined_reqtimeout}); Contact developer for support.')
 
             if not xrdjob.isUpload:
                 meta_path = str(xrdjob.src).partition("?")[0]
                 if os.getenv('ALIENPY_KEEP_META'):
-                    subprocess.run(shlex.split(f'mv {meta_path} {os.getcwd()}/'), check = False)
+                    subprocess.run(shlex.split(f'mv {meta_path} {os.getcwd()}/'), check = False)  # nosec
                 else:
                     os.remove(meta_path)  # remove the created metalink
 
         def update(self, jobId, processed, total):
             # self.job_list[jobId - 1]['bytes_total'] = total
             # self.job_list[jobId - 1]['bytes_processed'] = processed
             pass
@@ -1251,15 +758,15 @@
         @staticmethod
         def should_cancel():  # self, jobId
             return False
 
 
 def XrdCopy(wb, job_list: list, xrd_cp_args: XrdCpArgs, printout: str = '') -> list:
     """XRootD copy command :: the actual XRootD copy process"""
-    if not _HAS_XROOTD:
+    if not HAS_XROOTD:
         print_err("XRootD not found or lower than 5.3.3")
         return []
     if not xrd_cp_args:
         print_err("cp arguments are not set, XrdCpArgs tuple missing")
         return []
 
     # MANDATORY DEFAULTS, always used
@@ -1268,67 +775,127 @@
     sources = int(1)  # max number of download sources; we (ALICE) do not rely on parallel multi-source downloads
 
     # passed arguments
     overwrite = xrd_cp_args.overwrite
     batch = xrd_cp_args.batch
     tpc = xrd_cp_args.tpc
     # hashtype = xrd_cp_args.hashtype
-    cksum = xrd_cp_args.cksum
     # timeout = xrd_cp_args.timeout
     # rate = xrd_cp_args.rate
 
-    cksum_mode = 'none'  # none | source | target | end2end
-    cksum_type = ''
-    cksum_preset = ''
-    delete_invalid_chk = False
-    if cksum:  # checksumming defaults good enough also for uploads
-        xrd_client.EnvPutInt('ZipMtlnCksum', 1)
-        cksum_mode = 'end2end'
-        cksum_type = 'auto'
-        delete_invalid_chk = True
+    xrd_client.EnvPutInt('ZipMtlnCksum', 1)
 
     handler = MyCopyProgressHandler()
     handler.wb = wb
     handler.xrdjob_list = job_list
     handler.printout = printout
     handler.succesful_writes = []
-    if _DEBUG: handler.debug = True
+    if DEBUG: handler.debug = True
 
     process = xrd_client.CopyProcess()
     process.parallel(int(batch))
     for copy_job in job_list:
-        if _DEBUG: logging.debug('\nadd copy job with\nsrc: %s\ndst: %s\n', copy_job.src, copy_job.dst)
-        if cksum:
-            if copy_job.isUpload:
-                # WIP: checksumming with md5 for uploading breaks, keep it on auto
-                # cksum_type = 'md5'
-                # cksum_preset = copy_job.token_request['md5']
-                pass
-            else:  # for downloads we already have the md5 value, lets use that
-                cksum_type, cksum_preset = get_hash_meta(copy_job.src)
-                if not cksum_type or not cksum_preset:
-                    cksum_type = ''
-                    cksum_preset = ''
-                    cksum_mode = 'none'
-        process.add_job(copy_job.src, copy_job.dst,
-                        sourcelimit = sources, posc = posc, mkdir = makedir,
-                        force = overwrite, thirdparty = tpc,
-                        checksummode = cksum_mode, checksumtype = cksum_type, checksumpreset = cksum_preset, rmBadCksum = delete_invalid_chk)
+        if DEBUG: logging.debug('\nadd copy job with\nsrc: %s\ndst: %s\n', copy_job.src, copy_job.dst)
+        if copy_job.isUpload:
+            cksum_mode = 'source'; cksum_type = 'md5' ; cksum_preset = ''; # copy_job.token_request['md5']
+        else:  # for downloads we already have the md5 value, lets use that
+            cksum_mode = 'target';
+            cksum_type, cksum_preset = get_hash_meta(copy_job.src)
+            # If the remote file had no hash registered
+            if not cksum_type or not cksum_preset:
+                logging.error(f'COPY:: MD5 missing for {copy_job.lfn}')
+                cksum_mode = 'none'; cksum_type = cksum_preset = '';
+
+        delete_invalid_cksum = (not cksum_mode == 'none')  # if no checksumming mode, disable rmBadCksum
+        if 'xrateThreshold' in process.add_job.__code__.co_varnames:
+            process.add_job(copy_job.src, copy_job.dst, sourcelimit = sources, posc = posc, mkdir = makedir, force = overwrite, thirdparty = tpc,
+                            checksummode = cksum_mode, checksumtype = cksum_type, checksumpreset = cksum_preset, rmBadCksum = delete_invalid_cksum,
+                            retry = xrd_client.EnvGetInt('CpRetry'), cptimeout = xrd_client.EnvGetInt('CPTimeout'), xrateThreshold = xrd_client.EnvGetInt('XRateThreshold') )
+        else:
+            process.add_job(copy_job.src, copy_job.dst, sourcelimit = sources, posc = posc, mkdir = makedir, force = overwrite, thirdparty = tpc,
+                            checksummode = cksum_mode, checksumtype = cksum_type, checksumpreset = cksum_preset, rmBadCksum = delete_invalid_cksum,
+                            retry = xrd_client.EnvGetInt('CpRetry'), cptimeout = xrd_client.EnvGetInt('CPTimeout'), xrateThreashold = xrd_client.EnvGetInt('XRateThreshold') )
 
     process.prepare()
+
+    #faulthandler.disable()
+    #faulthandler.enable(file = sys.__stderr__, all_threads = True)
     process.run(handler)
+    #faulthandler.disable()
+
     if handler.succesful_writes:  # if there were succesful uploads/remote writes, let's commit them to file catalogue
         ret_list = commitFileList(wb, handler.succesful_writes)
         for ret in ret_list: retf_print(ret, 'noout err')
     return handler.copy_failed_list  # lets see what failed and try to recover
 
 
+def _xrdcp_sysproc(cmdline: str, timeout: Union[str, int, None] = None) -> RET:
+    """xrdcp stanalone system command"""
+    if not cmdline: return RET(1, '', '_xrdcp_sysproc :: no cmdline')  # type: ignore [call-arg]
+    if timeout is not None: timeout = int(timeout)
+    # --nopbar --posc
+    xrdcp_cmdline = f'xrdcp -N -P {cmdline}'
+    return runShellCMD(xrdcp_cmdline, captureout = True, do_shell = False, timeout = timeout)
+
+
+def _xrdcp_copyjob(copy_job: CopyFile, xrd_cp_args: XrdCpArgs) -> int:  # , printout: str = ''
+    """xrdcp based task that process a copyfile and it's arguments"""
+    if not copy_job: return int(2)
+    # overwrite = xrd_cp_args.overwrite
+    # batch = xrd_cp_args.batch
+    # tpc = xrd_cp_args.tpc
+    # hashtype = xrd_cp_args.hashtype
+    # cksum = xrd_cp_args.cksum
+    timeout = xrd_cp_args.timeout
+    # rate = xrd_cp_args.rate
+    cmdline = f'{copy_job.src} {copy_job.dst}'
+    return retf_print(_xrdcp_sysproc(cmdline, timeout))
+
+
+def XrdCopy_xrdcp(job_list: list, xrd_cp_args: XrdCpArgs) -> list:  # , printout: str = ''
+    """XRootD copy command :: the actual XRootD copy process"""
+    if not HAS_XROOTD:
+        print_err("XRootD not found or lower version thant 5.3.3")
+        return []
+    if not xrd_cp_args:
+        print_err("cp arguments are not set, XrdCpArgs tuple missing")
+        return []
+    # overwrite = xrd_cp_args.overwrite
+    # batch = xrd_cp_args.batch
+    # makedir = xrd_cp_args.makedir
+
+    # ctx = mp.get_context('forkserver')
+    # q = ctx.JoinableQueue()
+    # p = ctx.Process(target=_xrdcp_copyjob, args=(q,))
+    # p.start()
+    # print(q.get())
+    # p.join()
+    for copy_job in job_list:
+        if DEBUG: logging.debug('\nadd copy job with\nsrc: %s\ndst: %s\n', copy_job.src, copy_job.dst)
+        # xrdcp_cmd = f' {copy_job.src} {copy_job.dst}'
+        if DEBUG: print_out(copy_job)
+    return []
+
+
+def xrd_response2dict(response_status) -> dict:
+    """Convert a XRootD response status answer to a dict"""
+    if not response_status: return {}
+    if not HAS_XROOTD:
+        print_err('XRootD not present')
+        return {}
+    if not isinstance(response_status, xrd_client.responses.XRootDStatus):
+        print_err('Invalid argument type passed to xrd_response2dict')
+        return {}
+    return {'status': response_status.status, 'code': response_status.code, 'errno': response_status.errno, 'message': response_status.message.strip(),
+            'shellcode': response_status.shellcode, 'error': response_status.error, 'fatal': response_status.fatal, 'ok': response_status.ok}
+
+
 def xrdfs_q_config(fqdn_port: str) -> dict:
     """Return a dictionary of xrdfs query config"""
-    if not _HAS_XROOTD:
+    if not HAS_XROOTD:
         print_err('python XRootD module not found')
         return None
     endpoint = xrd_client.FileSystem(f'{fqdn_port}/?xrd.wantprot=unix')
 
     config_args_list = ['bind_max', 'chksum', 'pio_max', 'readv_ior_max', 'readv_iov_max', 'tpc', 'wan_port', 'wan_window', 'window', 'cms', 'role', 'sitename', 'version']
     config_dict = {}
     for cfg in config_args_list:
@@ -1342,15 +909,15 @@
             print_err(f'Query error for {fqdn_port} : {status["message"]}')
             break
     return config_dict
 
 
 def xrdfs_ping(fqdn_port: str):
     """Return a dictionary of xrdfs ping, it will contain ping_time_ms key"""
-    if not _HAS_XROOTD:
+    if not HAS_XROOTD:
         print_err('python XRootD module not found')
         return None
     endpoint = xrd_client.FileSystem(f'{fqdn_port}/?xrd.wantprot=unix')
     result, _ = endpoint.ping(timeout = 2)  # ping the server 1st time to eliminate strange 1st time behaviour
 
     time_begin = time.perf_counter()
     result, _ = endpoint.ping(timeout = 2)  # ping the server
@@ -1358,15 +925,15 @@
 
     response_dict = xrd_response2dict(result)
     response_dict['ping_time_ms'] = float(ping_ms)
     return response_dict
 
 
 def xrdfs_q_stats(fqdn_port: str, xml: bool = False, xml_raw: bool = False, compact: bool = False):
-    if not _HAS_XROOTD:
+    if not HAS_XROOTD:
         print_err('python XRootD module not found')
         return None
     endpoint = xrd_client.FileSystem(f'{fqdn_port}/?xrd.wantprot=unix')
     q_status, response = endpoint.query(1, 'a')  # get the stats (ALL)
     status = xrd_response2dict(q_status)
     if not status['ok']:
         print_err(f'xrdfs_q_stats:: query error to {fqdn_port} : {status["message"]}')
@@ -1374,15 +941,15 @@
 
     response = response.decode('ascii').strip().strip('\x00')
     # if xml is requested or xmltodict missing
     if xml:
         if xml_raw: return response
         # xml_stats = ET.fromstring(response)
         # return ET.dump(xml_stats)
-        xml_stats = MD.parseString(response)
+        xml_stats = MD.parseString(response)  # nosec B318:blacklist
         indent = '  '
         newl = '\n'
         if compact: indent = newl = ''
         return xml_stats.toprettyxml(indent = indent, newl = newl).replace('&quot;', '"')
 
     try:
         import xmltodict
@@ -1408,42 +975,40 @@
     # to search for a recursive solution
     for i in old_stats:
         if 'oss' in i: convert_dict(i['oss']['paths']['stats'])
 
     merged_stats = {}
     for i in old_stats: merged_stats.update(i)
     q_stats_dict['stats'] = merged_stats
-
     return q_stats_dict
 
 
-def xrd_response2dict(response_status: xrd_client.responses.XRootDStatus) -> dict:
-    """Convert a XRootD response status answer to a dict"""
-    if not response_status: return {}
-    return {'status': response_status.status, 'code': response_status.code, 'errno': response_status.errno, 'message': response_status.message.strip(),
-            'shellcode': response_status.shellcode, 'error': response_status.error, 'fatal': response_status.fatal, 'ok': response_status.ok}
-
-
-def xrd_statinfo2dict(response_statinfo: xrd_client.responses.StatInfo) -> dict:
+def xrd_statinfo2dict(response_statinfo) -> dict:
     """Convert a XRootD StatInfo answer to a dict"""
     if not response_statinfo: return {}
+    if not HAS_XROOTD:
+        print_err('XRootD not present')
+        return {}
+    if not isinstance(response_statinfo, xrd_client.responses.StatInfo):
+        print_err('Invalid argument type passed to xrd_statinfo2dict')
+        return {}
     return {'size': response_statinfo.size, 'flags': response_statinfo.flags, 'modtime': response_statinfo.modtime, 'modtimestr': response_statinfo.modtimestr}
 
 
 def xrdstat2dict(xrdstat: tuple) -> dict:
     """Convert a XRootD status answer to a dict"""
     if not xrdstat: return {}
     xrd_stat, xrd_info = xrdstat
     xrdstat_dict = xrd_response2dict(xrd_stat)
     xrdinfo_dict = xrd_statinfo2dict(xrd_info)
     return {**xrdstat_dict, **xrdinfo_dict}
 
 
 def xrdfs_stat(pfn: str):
-    if not _HAS_XROOTD:
+    if not HAS_XROOTD:
         print_err('python XRootD module not found')
         return None
     url_components = urlparse(pfn)
     endpoint = xrd_client.FileSystem(url_components.netloc)
     return endpoint.stat(f'{url_components.path}?xrd.wantprot=unix')
 
 
@@ -1463,79 +1028,37 @@
     get_pfn_info = xrdstat2dict(xrdfs_stat(pfn))
     if 'flags' in get_pfn_info:
         pfn_flags = xrdstat_flags2dict(get_pfn_info['flags'])
         return pfn_flags['is_readable']
     return False
 
 
-
 def get_pfn_list(wb, lfn: str) -> list:
     if not wb: return []
     if not lfn: return []
     if pathtype_grid(wb, lfn) != 'f': return []
     ret_obj = SendMsg(wb, 'whereis', [lfn], opts = 'nomsg')
     retf_print(ret_obj, 'debug')
     return [str(item['pfn']) for item in ret_obj.ansdict['results']]
 
 
-
-
-def get_lfn_meta(meta_fn: str) -> str:
-    if 'meta4?' in meta_fn: meta_fn = meta_fn.partition('?')[0]
-    if not os.path.isfile(meta_fn): return ''
-    return MD.parse(meta_fn).documentElement.getElementsByTagName('lfn')[0].firstChild.nodeValue
-
-
-def get_size_meta(meta_fn: str) -> int:
-    if 'meta4?' in meta_fn: meta_fn = meta_fn.partition('?')[0]
-    if not os.path.isfile(meta_fn): return int(0)
-    return int(MD.parse(meta_fn).documentElement.getElementsByTagName('size')[0].firstChild.nodeValue)
-
-
-def get_hash_meta(meta_fn: str) -> tuple:
-    if 'meta4?' in meta_fn: meta_fn = meta_fn.partition('?')[0]
-    if not os.path.isfile(meta_fn): return ('', '')
-    content = MD.parse(meta_fn).documentElement.getElementsByTagName('hash')[0]
-    return (content.getAttribute('type'), content.firstChild.nodeValue)
-
-
-def lfn2tmp_fn(lfn: str = '', uuid5: bool = False) -> str:
-    """make temporary file name that can be reconstructed back to the lfn"""
-    if not lfn: return str(uuid.uuid4())
-    if uuid5:
-        return str(uuid.uuid5(uuid.NAMESPACE_URL, lfn))
-    return lfn.replace("/", '%%')
-
-
-def make_tmp_fn(lfn: str = '', ext: str = '', uuid5: bool = False) -> str:
-    """make temporary file path string either random or based on grid lfn string"""
-    if not ext: ext = f'_{str(os.getuid())}.alienpy_tmp'
-    return f'{__TMPDIR}/{lfn2tmp_fn(lfn, uuid5)}{ext}'
-
-
-def get_lfn_name(tmp_name: str = '', ext: str = '') -> str:
-    lfn = tmp_name.replace(ext, '') if ext else tmp_name.replace(f'_{str(os.getuid())}.alienpy_tmp', '')
-    return lfn.replace(f'{__TMPDIR}/', '').replace("%%", "/")
-
-
 def download_tmp(wb, lfn: str, overwrite: bool = False, verbose: bool = False) -> str:
     """Download a lfn to a temporary file, it will return the file path of temporary"""
-    global AlienSessionInfo
     tmpfile = make_tmp_fn(expand_path_grid(lfn))
     if os.path.isfile(tmpfile):
         if overwrite:
             os.remove(tmpfile)
             if tmpfile in AlienSessionInfo['templist']: AlienSessionInfo['templist'].remove(tmpfile)
         else:
             if tmpfile not in AlienSessionInfo['templist']: AlienSessionInfo['templist'].append(tmpfile)
             return tmpfile
 
     if tmpfile in AlienSessionInfo['templist']: AlienSessionInfo['templist'].remove(tmpfile)  # just in case it is still in list
-    copycmd = f"-f {lfn} file:{tmpfile}"
-    ret_obj = DO_XrootdCp(wb, copycmd.split(), printout = 'silent')  # print only errors for temporary downloads
+    ret_obj = DO_XrootdCp(wb, xrd_copy_command = ['-fastcheck'], api_src = [f'{lfn}'], api_dst = [f'file:{tmpfile}'], printout = 'silent')  # print only errors for temporary downloads
+
     if ret_obj.exitcode == 0 and os.path.isfile(tmpfile):
         AlienSessionInfo['templist'].append(tmpfile)
         return tmpfile
     if verbose: print_err(f'{ret_obj.err}')
     return ''
 
 
@@ -1548,31 +1071,19 @@
     ret_obj = SendMsg(wb, 'mv', [lfn, lfn_backup])  # let's create a backup of old lfn
     if retf_print(ret_obj, 'debug') != 0: return ''
     tokens = lfn2fileTokens(wb, lfn2file(lfn, temp_file_name), [upload_specs], isWrite = True)
     access_request = tokens['answer']
     replicas = access_request["results"][0]["nSEs"]
     if "disk:" not in upload_specs: upload_specs = f'disk:{replicas}'
     if upload_specs: upload_specs = f'@{upload_specs}'
-    copycmd = f'-f file:{temp_file_name} {lfn}{upload_specs}'
-    ret_obj = DO_XrootdCp(wb, copycmd.split())
+
+    ret_obj = DO_XrootdCp(wb, xrd_copy_command = ['-fastcheck'], api_src = [f'file:{temp_file_name}'], api_dst = [f'{lfn}{upload_specs}'])
     if ret_obj.exitcode == 0: return lfn
     ret_obj = SendMsg(wb, 'mv', [lfn_backup, lfn])  # if the upload failed let's move back the backup to original lfn name'
     retf_print(ret_obj, 'debug')
     return ''
 
 
-
-
-
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
-    
-    
-
-
-
-
-
-
-
```

### Comparing `alienpy-1.4.6/alienpy/fs_local.py` & `alienpy-1.5.0/alienpy/tools_files.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,162 @@
-import sys
-import re
+'''alienpy:: file and path manipulation tools/helpers - not-networked'''
+
+
+import uuid
 from pathlib import Path
+import xml.dom.minidom as MD  # nosec B408:blacklist
+from .data_structs import *  # nosec PYL-W0614
+from .tools_misc import *  # nosec PYL-W0614
+import multiprocessing as mp
+import traceback
+
+NCPU = int(mp.cpu_count() * 0.8)  # use at most 80% of host CPUs
+
+
+def common_path(path_list: list) -> str:
+    """Return common path of a list of paths"""
+    if not path_list: return ''
+    if not isinstance(path_list, list): return ''
+    common = ''
+    try:
+        common = os.path.commonpath(path_list)
+    except:
+        pass
+    return common
 
-from data import *
-from re_patt import *
+
+def format_dst_fn(src_dir, src_file, dst, parent):
+    """Return the destination filename given the source dir/name, destination directory and number of parents to keep"""
+    # let's get destination file name (relative path with parent value)
+    if src_dir != src_file:  # recursive operation
+        total_relative_path = src_file.replace(src_dir, '', 1)
+        src_dir_path = Path(src_dir)
+        src_dir_parts = src_dir_path.parts
+        if not src_dir.endswith('/'): src_dir_parts = src_dir_parts[:-1]
+        src_dir = '/'.join(map(lambda x: str(x or ''), src_dir_parts))
+        src_dir = src_dir.replace('//', '/')
+        components_list = src_dir.split('/')
+        components_list[0] = '/'  # first slash is lost in split
+        file_components = len(components_list)  # it's directory'
+        parent = min(parent, file_components)  # make sure maximum parent var point to first dir in path
+        parent_selection = components_list[(file_components - parent):]
+        rootdir_src_dir = '/'.join(parent_selection)
+        file_relative_name = f'{rootdir_src_dir}/{total_relative_path}'
+    else:
+        src_file_path = Path(src_file)
+        file_components = len(src_file_path.parts) - 1 - 1  # without the file and up to slash
+        parent = min(parent, file_components)  # make sure maximum parent var point to first dir in path
+        rootdir_src_file = src_file_path.parents[parent].as_posix()
+        file_relative_name = src_file.replace(rootdir_src_file, '', 1)
+
+    dst_file = f'{dst}/{file_relative_name}' if dst.endswith('/') else dst
+    return os.path.normpath(dst_file)
+
+
+def setDst(file: str = '', parent: int = 0) -> str:
+    """For a given file path return the file path keeping the <parent> number of components"""
+    p = Path(file)
+    path_components = len(p.parts)
+    if parent >= (path_components - 1): parent = path_components - 1 - 1  # IF parent >= number of components without filename THEN make parent = number of component without / and filename
+    basedir = p.parents[parent].as_posix()
+    if basedir == '/': return file
+    return p.as_posix().replace(basedir, '', 1)
 
 
+def pathtype_local(path: str) -> str:
+    """Query if a local path is a file or directory, return f, d or empty"""
+    if not path: return ''
+    p = Path(path)
+    if p.is_dir(): return str('d')
+    if p.is_file(): return str('f')
+    return ''
+
+
+def fileIsValid(filename: str, size: Union[str, int], reported_md5: str, shallow_check: bool = False) -> RET:
+    """Check if the file path is consistent with the size and md5 argument. N.B.! the local file will be deleted with size,md5 not match"""
+    if os.path.isfile(filename):  # first check
+        if int(os.stat(filename).st_size) != int(size):
+            os.remove(filename)
+            return RET(9, '', f'{filename} : Removed (invalid size)')
+        if shallow_check:
+            return RET(0, f'{filename} --> TARGET VALID (size match)')
+        if md5(filename) != reported_md5:
+            os.remove(filename)
+            return RET(9, '', f'{filename} : Removed (invalid md5)')
+        return RET(0, f'{filename} --> TARGET VALID (md5 match)')
+    return RET(2, '', f'{filename} : No such file')  # ENOENT
+
+
+def create_metafile(meta_filename: str, lfn: str, local_filename: str, size: Union[str, int], md5in: str, replica_list: Union[None, list] = None) -> str:
+    """Generate a meta4 xrootd virtual redirector with the specified location and using the rest of arguments"""
+    if not (meta_filename and replica_list): return ''
+    try:
+        with open(meta_filename, 'w', encoding="ascii", errors="replace") as f:
+            published = str(datetime.datetime.now().replace(microsecond=0).isoformat())
+            f.write('<?xml version="1.0" encoding="UTF-8"?>\n')
+            f.write(' <metalink xmlns="urn:ietf:params:xml:ns:metalink">\n')
+            f.write(f'   <published>{published}</published>\n')
+            f.write(f'   <file name="{local_filename}">\n')
+            f.write(f'     <lfn>{lfn}</lfn>\n')
+            f.write(f'     <size>{size}</size>\n')
+            if md5in: f.write(f'     <hash type="md5">{md5in}</hash>\n')
+            for url in replica_list:
+                f.write(f'     <url><![CDATA[{url}]]></url>\n')
+            f.write('   </file>\n')
+            f.write(' </metalink>\n')
+        return meta_filename
+    except Exception:
+        logging.error(traceback.format_exc())
+        return ''
+
+
+def get_lfn_meta(meta_fn: str) -> str:
+    """Extract lfn value from metafile"""
+    if 'meta4?' in meta_fn: meta_fn = meta_fn.partition('?')[0]
+    if not os.path.isfile(meta_fn): return ''
+    return MD.parse(meta_fn).documentElement.getElementsByTagName('lfn')[0].firstChild.nodeValue  # nosec B318:blacklist
+
+
+def get_size_meta(meta_fn: str) -> int:
+    """Extract size value from metafile"""
+    if 'meta4?' in meta_fn: meta_fn = meta_fn.partition('?')[0]
+    if not os.path.isfile(meta_fn): return int(0)
+    return int(MD.parse(meta_fn).documentElement.getElementsByTagName('size')[0].firstChild.nodeValue)  # nosec B318:blacklist
+
+
+def get_hash_meta(meta_fn: str) -> tuple:
+    """Extract hash value from metafile"""
+    if 'meta4?' in meta_fn: meta_fn = meta_fn.partition('?')[0]
+    if not os.path.isfile(meta_fn): return ('', '')
+    content = MD.parse(meta_fn).documentElement.getElementsByTagName('hash')[0]  # nosec B318:blacklist
+    return (content.getAttribute('type'), content.firstChild.nodeValue)
+
+
+def md5(input_file: str) -> str:
+    """Compute the md5 digest of the specified file"""
+    if not path_readable(input_file): return '-1'
+    from hashlib import md5 as hash_md5
+    BLOCKSIZE = 65536
+    
+    if hash_md5.__text_signature__ and 'usedforsecurity' in hash_md5.__text_signature__:
+        hasher = hash_md5(usedforsecurity = False)
+    else:
+        hasher = hash_md5()  # nosec
+
+    with open(input_file, 'rb', buffering = 0) as f:
+        for chunk in iter(lambda: f.read(BLOCKSIZE), b''): hasher.update(chunk)
+    return hasher.hexdigest()
+
+
+def md5_mp(list_of_files: Union[None, list] = None) -> list:
+    """Compute md5 hashes in parallel; the results are guaranteed (by documentation) to be in the order of input list"""
+    if not list_of_files: return []
+    hash_list = []
+    with mp.Pool(processes = NCPU) as pool: hash_list = pool.map(md5, list_of_files)
+    return hash_list
 
 
 def expand_path_local(path_arg: str, strict: bool = False) -> str:
     """Given a string representing a local file, return a full path after interpretation of HOME location, current directory, . and .. and making sure there are only single /"""
     if not path_arg: return ''
     exp_path = None
     path_arg = lfn_prefix_re.sub('', path_arg)  # lets remove any prefixes
@@ -22,20 +169,15 @@
 
 
 def check_path_perm(filepath: str, mode) -> bool:
     """Resolve a file/path and check if mode is valid"""
     filepath = expand_path_local(filepath, True)
     if not filepath: return False
     if not mode: mode = os.F_OK
-    have_access = False
-    try:
-        have_access = os.access(filepath, mode, follow_symlinks = True)
-    except Exception:
-        pass
-    return have_access  # noqa: R504
+    return os.access(filepath, mode, follow_symlinks = True)
 
 
 def path_readable(filepath: str = '') -> bool:
     """Resolve a file/path and check if it is readable"""
     return check_path_perm(filepath, os.R_OK)
 
 
@@ -67,61 +209,97 @@
     guid = ''
     size = str(statinfo.st_size)
     md5hash = ''
     if do_md5 and filetype == 'f': md5hash = md5(norm_path)
     return STAT_FILEPATH(norm_path, filetype, perm, uid, gid, ctime, mtime, guid, size, md5hash)
 
 
-def pathtype_local(path: str) -> str:
-    """Query if a local path is a file or directory, return f, d or empty"""
-    if not path: return ''
-    p = Path(path)
-    if p.is_dir(): return str('d')
-    if p.is_file(): return str('f')
-    return ''
+def list_files_local(search_dir: str, pattern: Union[None, REGEX_PATTERN_TYPE, str] = None, is_regex: bool = False, find_args: str = '') -> RET:
+    """Return a list of files(local)(N.B! ONLY FILES) that match pattern found in dir"""
+    if not search_dir: return RET(2, "", "No search directory specified")
 
+    # let's process the pattern: extract it from src if is in the path globbing form
+    regex = None
+    is_single_file = False  # dir actually point to a file
+    if '*' in search_dir:  # we have globbing in src path
+        is_regex = False
+        src_arr = search_dir.split("/")
+        base_path_arr = []  # let's establish the base path
+        for el in src_arr:
+            if '*' not in el:
+                base_path_arr.append(el)
+            else:
+                break
+        for el in base_path_arr: src_arr.remove(el)  # remove the base path
+        search_dir = '/'.join(base_path_arr) + '/'  # rewrite the source path without the globbing part
+        pattern = '/'.join(src_arr)  # the globbing part is the rest of element that contain *
+    else:  # pattern is specified by argument or not specified
+        if pattern is None:
+            if not search_dir.endswith('/'):  # this is a single file
+                is_single_file = True
+            else:
+                pattern = '*'  # prefer globbing as default
+        elif type(pattern) is REGEX_PATTERN_TYPE:  # unlikely but supported to match signatures
+            regex = pattern
+            is_regex = True
+        elif is_regex and isinstance(pattern, str):  # it was explictly requested that pattern is regex
+            regex = valid_regex(pattern)
+            if regex is None:
+                msg = f'list_files_grid:: {pattern} failed to re.compile'
+                logging.error(msg)
+                return RET(-1, '', msg)
 
-def md5(filename: str) -> str:
-    """Compute the md5 digest of the specified file"""
-    import hashlib
-    BLOCKSIZE = 65536
-    hasher = hashlib.md5()
-    with open(filename, 'rb') as f:
-        buf = f.read(BLOCKSIZE)
-        while len(buf) > 0:
-            hasher.update(buf)
-            buf = f.read(BLOCKSIZE)
-    return hasher.hexdigest()
+    directory = None  # resolve start_dir to an absolute_path
+    try:
+        directory = Path(search_dir).expanduser().resolve(strict = True).as_posix()
+    except FileNotFoundError:
+        return RET(2, '', f'{search_dir} not found')
+    except RuntimeError:
+        return RET(2, '', f'Loop encountered along the resolution of {search_dir}')
 
+    filter_args_list = None
+    if find_args: filter_args_list = find_args.split()  # for local files listing we have only filtering options
 
-def fileIsValid(filename: str, size: Union[str, int], reported_md5: str, shallow_check: bool = False) -> RET:
-    """Check if the file path is consistent with the size and md5 argument. N.B.! the local file will be deleted with size,md5 not match"""
-    global AlienSessionInfo
-    if os.path.isfile(filename):  # first check
-        if int(os.stat(filename).st_size) != int(size):
-            os.remove(filename)
-            return RET(9, '', f'{filename} : Removed (invalid size)')
-        if shallow_check:
-            return RET(0, f'{filename} --> TARGET VALID (size match)')
-        if md5(filename) != reported_md5:
-            os.remove(filename)
-            return RET(9, '', f'{filename} : Removed (invalid md5)')
-        return RET(0, f'{filename} --> TARGET VALID (md5 match)')
-    return RET(2, '', f'{filename} : No such file')  # ENOENT
+    file_list = None  # make a list of filepaths (that match a regex or a glob)
+    if is_single_file:
+        file_list = [directory]
+    elif is_regex:
+        file_list = [os.path.join(root, f) for (root, dirs, files) in os.walk(directory) for f in files if regex.match(os.path.join(root, f))]
+    else:
+        file_list = [p.expanduser().resolve(strict = True).as_posix() for p in list(Path(directory).glob(f'**/{pattern}')) if p.is_file()]
 
+    if not file_list:
+        return RET(2, '', f"No files found in :: {directory} /pattern: {pattern} /find_args: {find_args}")
+
+    # convert the file_list to a list of file properties dictionaries
+    results_list = [file2file_dict(filepath) for filepath in file_list]
+
+    results_list_filtered = []
+    # items that pass the conditions are the actual/final results
+    for found_lfn_dict in results_list:  # parse results to apply filters
+        if not filter_file_prop(found_lfn_dict, directory, filter_args_list, regex): continue
+        # at this point all filters were passed
+        results_list_filtered.append(found_lfn_dict)
+
+    if not results_list_filtered:
+        return RET(2, '', f'No files passed the filters :: {directory} /pattern: {pattern} /find_args: {find_args}')
+
+    ansdict = {"results": results_list_filtered}
+    lfn_list = [get_lfn_key(lfn_obj) for lfn_obj in results_list_filtered]
+    stdout = '\n'.join(lfn_list)
+    return RET(exitcode, stdout, '', ansdict)
 
 
 def file_set_atime(path: str):
     """Set atime of file to now"""
     if not os.path.isfile(path): return
     file_stat = os.stat(path)
     os.utime(path, (datetime.datetime.now().timestamp(), file_stat.st_mtime))
 
 
-
 def file2file_dict(fn: str) -> dict:
     """Take a string as path and retur a dict with file propreties"""
     try:
         file_path = Path(fn)
     except Exception:
         return {}
     try:
@@ -136,19 +314,19 @@
     file_dict["mtime"] = str(int(file_name.stat().st_mtime * 1000))
     file_dict["md5"] = md5(file_name.as_posix())
     file_dict["owner"] = pwd.getpwuid(file_name.stat().st_uid).pw_name
     file_dict["gowner"] = gid2name(file_name.stat().st_gid)
     return file_dict
 
 
-
-
 def filter_file_prop(f_obj: dict, base_dir: str, find_opts: Union[str, list, None], compiled_regex = None) -> bool:
     """Return True if an file dict object pass the conditions in find_opts"""
     if not f_obj or not base_dir: return False
+    if f_obj['lfn'].endswith('.'): return False
+
     if not find_opts: return True
     opts = find_opts.split() if isinstance(find_opts, str) else find_opts.copy()
     lfn = get_lfn_key(f_obj)
     if not base_dir.endswith('/'): base_dir = f'{base_dir}/'
     relative_lfn = lfn.replace(base_dir, '')  # it will have N directories depth + 1 file components
 
     # string/pattern exclusion
@@ -237,90 +415,29 @@
             return False
         max_depth = abs(int(max_depth)) + 1  # add +1 for the always present file component of relative_lfn
         if len(relative_lfn.split('/')) > max_depth: return False
 
     return True
 
 
-def list_files_local(search_dir: str, pattern: Union[None, REGEX_PATTERN_TYPE, str] = None, is_regex: bool = False, find_args: str = '') -> RET:
-    """Return a list of files(local)(N.B! ONLY FILES) that match pattern found in dir"""
-    if not search_dir: return RET(2, "", "No search directory specified")
-
-    # let's process the pattern: extract it from src if is in the path globbing form
-    regex = None
-    is_single_file = False  # dir actually point to a file
-    if '*' in search_dir:  # we have globbing in src path
-        is_regex = False
-        src_arr = search_dir.split("/")
-        base_path_arr = []  # let's establish the base path
-        for el in src_arr:
-            if '*' not in el:
-                base_path_arr.append(el)
-            else:
-                break
-        for el in base_path_arr: src_arr.remove(el)  # remove the base path
-        search_dir = '/'.join(base_path_arr) + '/'  # rewrite the source path without the globbing part
-        pattern = '/'.join(src_arr)  # the globbing part is the rest of element that contain *
-    else:  # pattern is specified by argument or not specified
-        if pattern is None:
-            if not search_dir.endswith('/'):  # this is a single file
-                is_single_file = True
-            else:
-                pattern = '*'  # prefer globbing as default
-        elif type(pattern) is REGEX_PATTERN_TYPE:  # unlikely but supported to match signatures
-            regex = pattern
-            is_regex = True
-        elif is_regex and isinstance(pattern, str):  # it was explictly requested that pattern is regex
-            regex = valid_regex(pattern)
-            if regex is None:
-                msg = f'list_files_grid:: {pattern} failed to re.compile'
-                logging.error(msg)
-                return RET(-1, '', msg)
-
-    directory = None  # resolve start_dir to an absolute_path
-    try:
-        directory = Path(search_dir).expanduser().resolve(strict = True).as_posix()
-    except FileNotFoundError:
-        return RET(2, '', f'{search_dir} not found')
-    except RuntimeError:
-        return RET(2, '', f'Loop encountered along the resolution of {search_dir}')
-
-    filter_args_list = None
-    if find_args: filter_args_list = find_args.split()  # for local files listing we have only filtering options
-
-    file_list = None  # make a list of filepaths (that match a regex or a glob)
-    if is_single_file:
-        file_list = [directory]
-    elif is_regex:
-        file_list = [os.path.join(root, f) for (root, dirs, files) in os.walk(directory) for f in files if regex.match(os.path.join(root, f))]
-    else:
-        file_list = [p.expanduser().resolve(strict = True).as_posix() for p in list(Path(directory).glob(f'**/{pattern}')) if p.is_file()]
-
-    if not file_list:
-        return RET(2, '', f"No files found in :: {directory} /pattern: {pattern} /find_args: {find_args}")
-
-    # convert the file_list to a list of file properties dictionaries
-    results_list = [file2file_dict(filepath) for filepath in file_list]
-
-    results_list_filtered = []
-    # items that pass the conditions are the actual/final results
-    for found_lfn_dict in results_list:  # parse results to apply filters
-        if not filter_file_prop(found_lfn_dict, directory, filter_args_list, regex): continue
-        # at this point all filters were passed
-        results_list_filtered.append(found_lfn_dict)
-
-    if not results_list_filtered:
-        return RET(2, '', f'No files passed the filters :: {directory} /pattern: {pattern} /find_args: {find_args}')
-
-    ansdict = {"results": results_list_filtered}
-    lfn_list = [get_lfn_key(lfn_obj) for lfn_obj in results_list_filtered]
-    stdout = '\n'.join(lfn_list)
-    return RET(exitcode, stdout, '', ansdict)
-
+def lfn2tmp_fn(lfn: str = '', uuid5: bool = False) -> str:
+    """make temporary file name that can be reconstructed back to the lfn"""
+    if not lfn: return str(uuid.uuid4())
+    if uuid5:
+        return str(uuid.uuid5(uuid.NAMESPACE_URL, lfn))
+    return lfn.replace("/", '%%')
+
+
+def make_tmp_fn(lfn: str = '', ext: str = '', uuid5: bool = False) -> str:
+    """make temporary file path string either random or based on grid lfn string"""
+    if not ext: ext = f'_{str(os.getuid())}.alienpy_tmp'
+    return f'{TMPDIR}/{lfn2tmp_fn(lfn, uuid5)}{ext}'
+
+
+def get_lfn_name(tmp_name: str = '', ext: str = '') -> str:
+    lfn = tmp_name.replace(ext, '') if ext else tmp_name.replace(f'_{str(os.getuid())}.alienpy_tmp', '')
+    return lfn.replace(f'{TMPDIR}/', '').replace("%%", "/")
 
 
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
-    
-    
-
```

### Comparing `alienpy-1.4.6/alienpy/ssl_tools.py` & `alienpy-1.5.0/alienpy/connect_ssl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,64 @@
+'''alienpy:: SSL and certificate tooling'''
+
+import sys
+import os
 import logging
-import ssl
+import uuid
+from pathlib import Path
+import traceback
+
+try:
+    import ssl
+except Exception:
+    print("Python ssl module could not be imported! Make sure you can do:\npython3 -c 'import ssl'", file = sys.stderr, flush = True)
+    sys.exit(1)
 
+try:
+    import cryptography
+except Exception:
+    print("cryptography module could not be imported! Make sure you can do:\npython3 -c 'import cryptography'", file = sys.stderr, flush = True)
+    sys.exit(1)
 
 try:
     import OpenSSL
 except Exception:
     print("OpenSSL module could not be loaded", file = sys.stderr, flush = True)
     sys.exit(1)
 
+##   GLOBALS
+from .global_vars import *  # nosec PYL-W0614
+from .data_structs import *  # nosec PYL-W0614
+from .tools_misc import *  # nosec PYL-W0614
+from .tools_files import *  # nosec PYL-W0614
+
+# Have global variables for certificate file names, defaults being over-ridden by env vars
+USERCERT_NAME = os.getenv('X509_USER_CERT', f'{Path.home().as_posix()}/.globus/usercert.pem')
+USERKEY_NAME  = os.getenv('X509_USER_KEY',  f'{Path.home().as_posix()}/.globus/userkey.pem')
 
-
-def get_files_cert() -> tuple:
-    return os.getenv('X509_USER_CERT', f'{Path.home().as_posix()}/.globus/usercert.pem'), os.getenv('X509_USER_KEY', f'{Path.home().as_posix()}/.globus/userkey.pem')
-
-
-def get_token_names(files: bool = False) -> tuple:
-    if files:
-        return  __TOKENCERT_NAME, __TOKENKEY_NAME
-    return os.getenv('JALIEN_TOKEN_CERT', __TOKENCERT_NAME), os.getenv('JALIEN_TOKEN_KEY', __TOKENKEY_NAME)
+TOKENCERT_NAME = os.getenv('JALIEN_TOKEN_CERT', f'{TMPDIR}/tokencert_{str(os.getuid())}.pem')
+TOKENKEY_NAME  = os.getenv('JALIEN_TOKEN_KEY',  f'{TMPDIR}/tokenkey_{str(os.getuid())}.pem')
 
 
 def get_ca_path() -> str:
     """Return either the CA path or file; bailout application if not found"""
+    DEBUG = os.getenv('ALIENPY_DEBUG', '')
+
     system_ca_path = '/etc/grid-security/certificates'
     alice_cvmfs_ca_path_lx = '/cvmfs/alice.cern.ch/etc/grid-security/certificates'
     alice_cvmfs_ca_path_macos = f'/Users/Shared{alice_cvmfs_ca_path_lx}'
 
     x509file = os.getenv('X509_CERT_FILE') if os.path.isfile(str(os.getenv('X509_CERT_FILE'))) else ''
     if x509file:
-        if _DEBUG: logging.debug('X509_CERT_FILE = %s', x509file)
+        if DEBUG: logging.debug('X509_CERT_FILE = %s', x509file)
         return x509file
 
     x509dir = os.getenv('X509_CERT_DIR') if os.path.isdir(str(os.getenv('X509_CERT_DIR'))) else ''
     if x509dir:
-        if _DEBUG: logging.debug('X509_CERT_DIR = %s', x509dir)
+        if DEBUG: logging.debug('X509_CERT_DIR = %s', x509dir)
         return x509dir
 
     capath_default = None
     if os.path.exists(alice_cvmfs_ca_path_lx):
         capath_default = alice_cvmfs_ca_path_lx
     elif os.path.exists(alice_cvmfs_ca_path_macos):
         capath_default = alice_cvmfs_ca_path_macos
@@ -45,105 +66,120 @@
         if os.path.exists(system_ca_path): capath_default = system_ca_path
 
     if not capath_default:
         msg = "No CA location or files specified or found!!! Connection will not be possible!!"
         print_err(msg)
         logging.error(msg)
         sys.exit(2)
-    if _DEBUG: logging.debug('CApath = %s', capath_default)
+    if DEBUG: logging.debug('CApath = %s', capath_default)
     return capath_default
 
 
 def IsValidCert(fname: str) -> bool:
     """Check if the certificate file (argument) is present and valid. It will return false also for less than 5min of validity"""
     try:
         with open(fname, encoding="ascii", errors="replace") as f:
             cert_bytes = f.read()
     except Exception:
         logging.error('IsValidCert:: Unable to open certificate file %s', fname)
         return False
 
     try:
-        x509 = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, cert_bytes)
+        x509 = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, cert_bytes)  # type: ignore[attr-defined]
     except Exception:
         logging.error('IsValidCert:: Unable to load certificate %s', fname)
         return False
 
     x509_notafter = x509.get_notAfter()
     utc_time = datetime.datetime.strptime(x509_notafter.decode("utf-8"), "%Y%m%d%H%M%SZ")
     time_notafter = int((utc_time - datetime.datetime(1970, 1, 1)).total_seconds())
     time_current = int(datetime.datetime.now().timestamp())
     time_remaining = time_notafter - time_current
     if time_remaining < 1:
         logging.error('IsValidCert:: Expired certificate %s', fname)
     return time_remaining > 300
 
 
+def get_valid_certs() -> tuple:
+    """Return valid names for user certificate or None"""
+    if AlienSessionInfo['verified_cert']: return USERCERT_NAME, USERKEY_NAME
+    FOUND = path_readable(USERCERT_NAME) and path_readable(USERKEY_NAME)
+    if not FOUND:
+        msg = f'User certificate files NOT FOUND or NOT accessible!!! Connection will not be possible!!\nCheck content of {os.path.expanduser("~")}/.globus'
+        logging.error(msg)
+        return None, None
+
+    INVALID = not IsValidCert(USERCERT_NAME)
+    if INVALID:
+        msg = f'Invalid/expired user certificate!! Check the content of {USERCERT_NAME}'
+        logging.error(msg)
+        return None, None
+
+    AlienSessionInfo['verified_cert'] = True  # This means that we already checked
+    return USERCERT_NAME, USERKEY_NAME
+
+
+# Have global variables for checked at the load time of user certificates
+USERCERT_VALID, USERKEY_VALID = get_valid_certs()
+
+
 def get_valid_tokens() -> tuple:
     """Get the token filenames, including the temporary ones used as env variables"""
-    global AlienSessionInfo
-    tokencert, tokenkey = get_token_names()
+    global TOKENCERT_NAME, TOKENKEY_NAME
     random_str = None
     cert_suffix = None
-    if not path_readable(tokencert) and tokencert.startswith('-----BEGIN CERTIFICATE-----'):  # and is not a file
+    if not path_readable(TOKENCERT_NAME) and TOKENCERT_NAME.startswith('-----BEGIN CERTIFICATE-----'):  # and is not a file
         random_str = str(uuid.uuid4())
         cert_suffix = f'_{str(os.getuid())}_{random_str}.pem'
-        temp_cert = tempfile.NamedTemporaryFile(prefix = 'tokencert_', suffix = cert_suffix, delete = False)  # noqa: PLR1732
-        temp_cert.write(tokencert.encode(encoding = "ascii", errors = "replace"))
+        temp_cert = tempfile.NamedTemporaryFile(prefix = 'tokencert_', suffix = cert_suffix, delete = False)
+        temp_cert.write(TOKENCERT_NAME.encode(encoding = "ascii", errors = "replace"))
         temp_cert.seek(0)
-        tokencert = temp_cert.name  # temp file was created, let's give the filename to tokencert
-        AlienSessionInfo['templist'].append(tokencert)
-    if not path_readable(tokenkey) and tokenkey.startswith('-----BEGIN RSA PRIVATE KEY-----'):  # and is not a file
+        TOKENCERT_NAME = temp_cert.name  # temp file was created, let's give the filename to tokencert
+        AlienSessionInfo['templist'].append(TOKENCERT_NAME)  # type: ignore[attr-defined]
+    if not path_readable(TOKENKEY_NAME) and TOKENKEY_NAME.startswith('-----BEGIN RSA PRIVATE KEY-----'):  # and is not a file
         if random_str is None: random_str = str(uuid.uuid4())
-        temp_key = tempfile.NamedTemporaryFile(prefix = 'tokenkey_', suffix = cert_suffix, delete = False)  # noqa: PLR1732
-        temp_key.write(tokenkey.encode(encoding = "ascii", errors = "replace"))
+        temp_key = tempfile.NamedTemporaryFile(prefix = 'tokenkey_', suffix = cert_suffix, delete = False)
+        temp_key.write(TOKENKEY_NAME.encode(encoding = "ascii", errors = "replace"))
         temp_key.seek(0)
-        tokenkey = temp_key.name  # temp file was created, let's give the filename to tokenkey
-        AlienSessionInfo['templist'].append(tokenkey)
+        TOKENKEY_NAME = temp_key.name  # temp file was created, let's give the filename to tokenkey
+        AlienSessionInfo['templist'].append(TOKENKEY_NAME)  # type: ignore[attr-defined]
 
-    if (IsValidCert(tokencert) and path_readable(tokenkey)):
+    if (IsValidCert(TOKENCERT_NAME) and path_readable(TOKENKEY_NAME)):
         AlienSessionInfo['verified_token'] = True
-        return (tokencert, tokenkey)
+        return (TOKENCERT_NAME, TOKENKEY_NAME)
     return (None, None)
 
 
-def get_valid_certs() -> tuple:
-    """Return valid names for user certificate or None"""
-    global AlienSessionInfo
-    usercert, userkey = get_files_cert()
-    if AlienSessionInfo['verified_cert']: return usercert, userkey
-
-    INVALID = False
-    if not (path_readable(usercert) and path_readable(userkey)):
-        msg = f'User certificate files NOT FOUND or NOT accessible!!! Connection will not be possible!!\nCheck content of {os.path.expanduser("~")}/.globus'
-        logging.info(msg)
-        INVALID = True
-    if not IsValidCert(usercert):
-        msg = f'Invalid/expired user certificate!! Check the content of {usercert}'
-        logging.info(msg)
-        INVALID = True
-    AlienSessionInfo['verified_cert'] = True  # This means that we already checked
-    if INVALID: return None, None
-    return usercert, userkey
+# Check the presence of user certs and bailout before anything else
+TOKENCERT_VALID, TOKENKEY_VALID = get_valid_tokens()
+if not USERCERT_VALID and not TOKENCERT_VALID:
+    print_err(f'No valid user certificate or token found!! check {DEBUG_FILE} for further information and contact the developer if the information is not clear.')
+    sys.exit(126)
 
 
 def create_ssl_context(use_usercert: bool = False) -> ssl.SSLContext:
     """Create SSL context using either the default names for user certificate and token certificate or X509_USER_{CERT,KEY} JALIEN_TOKEN_{CERT,KEY} environment variables"""
-    cert, key = get_valid_auth_cred(use_usercert)
+    if use_usercert or not TOKENCERT_VALID:
+        AlienSessionInfo['use_usercert'] = True
+        cert, key = USERCERT_VALID, USERKEY_VALID
+    else:
+        cert, key = TOKENCERT_VALID, TOKENKEY_VALID
+
     if not cert:
         print_err('create_ssl_context:: no certificate to be used for SSL context. This message should not be printed, contact the developer if you see this!!!')
         os._exit(126)
 
-    if _DEBUG: logging.debug('\nCert = %s\nKey = %s\nCreating SSL context .. ', cert, key)
+    DEBUG = os.getenv('ALIENPY_DEBUG', '')
+    if DEBUG: logging.debug('\nCert = %s\nKey = %s\nCreating SSL context .. ', cert, key)
     ssl_protocol = ssl.PROTOCOL_TLS if sys.version_info[1] < 10 else ssl.PROTOCOL_TLS_CLIENT
     ctx = ssl.SSLContext(ssl_protocol)
     ctx.options |= ssl.OP_NO_SSLv3
     ctx.verify_mode = ssl.CERT_REQUIRED  # CERT_NONE, CERT_OPTIONAL, CERT_REQUIRED
     ctx.check_hostname = False
-    if _DEBUG: logging.debug("SSL context:: Load verify locations")
+    if DEBUG: logging.debug("SSL context:: Load verify locations")
 
     ca_verify_location = get_ca_path()
     cafile = capath = None
     if os.path.isfile(ca_verify_location):
         cafile = ca_verify_location
     else:
         capath = ca_verify_location
@@ -151,27 +187,26 @@
     try:
         ctx.load_verify_locations(cafile = cafile, capath = capath)
     except Exception:
         logging.exception('Could not load verify location >>> %s <<<\n', ca_verify_location)  # EIO /* I/O error */
         print_err(f'Verify location could not be loaded!!! check content of >>> {ca_verify_location} <<< and the log')
         os._exit(126)
 
-    if _DEBUG: logging.debug('SSL context:: Loading cert,key pair\n%s\n%s', cert, key)
+    if DEBUG: logging.debug('SSL context:: Loading cert,key pair\n%s\n%s', cert, key)
     try:
         ctx.load_cert_chain(certfile = cert, keyfile = key)
     except Exception:
         logging.exception('Could not load certificates!!!\n')  # EIO /* I/O error */
-        print_err('Error loading certificate pair!! Check the content of {_DEBUG_FILE}')
+        print_err('Error loading certificate pair!! Check the content of {DEBUG_FILE}')
         os._exit(126)
 
-    if _DEBUG: logging.debug('... SSL context done.')
+    if DEBUG: logging.debug('... SSL context done.')
     return ctx
 
 
-
 def CertInfo(fname: str) -> RET:
     """Print certificate information (subject, issuer, notbefore, notafter)"""
     try:
         with open(fname, encoding = "ascii", errors = "replace") as f:
             cert_bytes = f.read()
     except Exception:
         return RET(2, '', f'File >>>{fname}<<< not found')  # ENOENT /* No such file or directory */
@@ -185,15 +220,14 @@
     utc_time_notbefore = datetime.datetime.strptime(x509.get_notBefore().decode("utf-8"), "%Y%m%d%H%M%SZ")
     issuer = '/'.join([f'{k.decode("utf-8")}={v.decode("utf-8")}' for k, v in x509.get_issuer().get_components()])
     subject = '/'.join([f'{k.decode("utf-8")}={v.decode("utf-8")}' for k, v in x509.get_subject().get_components()])
     info = f'DN >>> {subject}\nISSUER >>> {issuer}\nBEGIN >>> {utc_time_notbefore}\nEXPIRE >>> {utc_time_notafter}'
     return RET(0, info)
 
 
-
 def CertVerify(fname: str) -> RET:
     """Print certificate information (subject, issuer, notbefore, notafter)"""
     try:
         with open(fname, encoding="ascii", errors="replace") as f:
             cert_bytes = f.read()
     except Exception:
         return RET(2, "", f"File >>>{fname}<<< not found")  # ENOENT /* No such file or directory */
@@ -266,11 +300,12 @@
     try:
         ctx.check_privatekey()
         return RET(0, f'Cert/key {PrintColor(COLORS.BIGreen)}match{PrintColor(COLORS.ColorReset)}')
     except OpenSSL.SSL.Error:
         return RET(0, '', f'Cert/key {PrintColor(COLORS.BIRed)}DO NOT match{PrintColor(COLORS.ColorReset)}')
 
 
-
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
+    
+
```

### Comparing `alienpy-1.4.6/alienpy/tools.py` & `alienpy-1.5.0/alienpy/tools_misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,123 +1,38 @@
-import re
+'''alienpy:: Misc tooling functions'''
+
+import ast
+import sys
+import datetime
 import json
-import time
-import logging
+import re
 from typing import Union
-
-from data import *
-from re_patt import *
-
-ignore_comments_re = re.compile('^\\s*(#|;|//)+', re.MULTILINE)  # identifiy a range of comments
-emptyline_re = re.compile('^\\s*$', re.MULTILINE)  # whitespace line
-
-def print_out(msg: str, toLog: bool = False):
-    if toLog:
-        logging.log(90, msg)
-    else:
-        print(msg, flush = True)
-
-
-def print_err(msg: str, toLog: bool = False):
-    if toLog:
-        logging.log(95, msg)
-    else:
-        print(msg, file = sys.stderr, flush = True)
-
-
-def PrintDict(in_arg: Union[str, dict, list], compact: bool = False):
-    """Print a dictionary in a nice format"""
-    if isinstance(in_arg, str):
-        try:
-            in_arg = json.loads(in_arg)
-        except Exception as e:
-            print_err(f'PrintDict:: Could not load argument as json!\n{e!r}')
-    if compact:
-        print_out(json.dumps(in_arg, sort_keys = False, indent = None, separators = (',', ':')))
-    else:
-        print_out(json.dumps(in_arg, sort_keys = False, indent = 2))
-
-
-def CreateJsonCommand(cmdline: Union[str, dict], args: Union[None, list] = None, opts: str = '', get_dict: bool = False) -> Union[str, dict]:
-    """Return a json with command and argument list"""
-    if args is None: args = []
-    if isinstance(cmdline, dict):
-        out_dict = cmdline.copy()
-        if 'showmsg' in opts: opts = opts.replace('nomsg', '')
-        if 'showkeys' in opts: opts = opts.replace('nokeys', '')
-        if 'nomsg' in opts: out_dict["options"].insert(0, '-nomsg')
-        if 'nokeys' in opts: out_dict["options"].insert(0, '-nokeys')
-        return out_dict if get_dict else json.dumps(out_dict)
-
-    if not args:
-        args = shlex.split(cmdline)
-        cmd = args.pop(0) if args else ''
-    else:
-        cmd = cmdline
-    if 'nomsg' in opts: args.insert(0, '-nomsg')
-    if 'nokeys' in opts: args.insert(0, '-nokeys')
-    jsoncmd = {"command": cmd, "options": args}
-    return jsoncmd if get_dict else json.dumps(jsoncmd)
-
-
-def GetMeta(result: dict, meta: str = '') -> list:
-    """Extract from input and return a list of 2nd arg selectable of cwd user error exitcode"""
-    output = []
-    if not result: return output
-    if isinstance(result, dict) and 'metadata' in result:  # these works only for AliEn responses
-        meta_opts_list = meta.split() if meta else []
-        if 'cwd' in meta_opts_list or 'all' in meta_opts_list: output.append(result["metadata"]["currentdir"])
-        if 'user' in meta_opts_list or 'all' in meta_opts_list: output.append(result["metadata"]["user"])
-        if 'error' in meta_opts_list or 'all' in meta_opts_list: output.append(result["metadata"]["error"])
-        if 'exitcode' in meta_opts_list or 'all' in meta_opts_list: output.append(result["metadata"]["exitcode"])
-    return output
+import socket
+import time
+import grp
+import pwd
+from .global_vars import *  # nosec PYL-W0614
+from .setup_logging import print_out, print_err
 
 
 def PrintColor(color: str) -> str:
     """Disable color if the terminal does not have capability"""
-    return color if _HAS_COLOR else ''
-
-
-def cursor_vertical(lines: int = 0):
-    """Move the cursor up/down N lines"""
-    if lines == 0: return
-    out_char = '\x1b[1A'  # UP
-    if lines < 0:
-        out_char = '\x1b[1B'  # DOWN
-        lines = abs(lines)
-    sys.stdout.write(out_char * lines)
-    sys.stdout.flush()
-
-
-def cursor_horizontal(lines: int = 0):
-    """Move the cursor left/right N lines"""
-    if lines == 0: return
-    out_char = '\x1b[1C'  # RIGHT
-    if lines < 0:
-        out_char = '\x1b[1D'  # LEFT
-        lines = abs(lines)
-    sys.stdout.write(out_char * lines)
-    sys.stdout.flush()
-
+    return color if HAS_COLOR else ''
 
 
 def exit_message(code: int = 0, msg = ''):
     """Exit with msg and with specied code"""
     print_out(msg if msg else 'Exit')
     sys.exit(code)
 
 
-def is_guid(guid: str) -> bool:
-    """Recognize a GUID format"""
-    return bool(guid_regex.fullmatch(guid))  # identify if argument in an AliEn GUID
-
-
-def run_function(function_name: str, *args, **kwargs):
-    """Python code:: run some arbitrary function name (found in globals) with arbitrary arguments"""
-    return globals()[function_name](*args, *kwargs)  # run arbitrary function
+def signal_handler(sig, frame):  # pylint: disable=unused-argument
+    """Generig signal handler: just print the signal and exit"""
+    print_out(f"\nCought signal {sig}, let\'s exit")
+    exit_message(int(AlienSessionInfo['exitcode']))
 
 
 def is_float(arg: Union[str, float, None]) -> bool:
     if not arg: return False
     s = str(arg).replace('.', '', 1)
     if s[0] in ('-', '+'): return s[1:].isdigit()
     return s.isdigit()
@@ -128,18 +43,18 @@
     s = str(arg)
     if s[0] in ('-', '+'): return s[1:].isdigit()
     return s.isdigit()
 
 
 def time_unix2simple(time_arg: Union[str, int, None]) -> str:
     if not time_arg: return ''
-    return datetime.datetime.fromtimestamp(time_arg).replace(microsecond=0).isoformat().replace('T', ' ')
+    return datetime.datetime.fromtimestamp(float(time_arg)).replace(microsecond=0).isoformat().replace('T', ' ')
 
 
-def time_str2unixmili(time_arg: Union[str, int, None]) -> int:  # noqa: FQ004
+def time_str2unixmili(time_arg: Union[str, int, None]) -> int:
     if not time_arg:
         return int((datetime.datetime.utcnow() - datetime.datetime(1970, 1, 1)).total_seconds() * 1000)
     time_arg = str(time_arg)
 
     if time_arg.isdigit() or is_float(time_arg):
         if is_float(time_arg) and len(time_arg) == 10:
             return int(float(time_arg) * 1000)
@@ -149,14 +64,101 @@
 
     # asume that this is a strptime arguments in the form of: time_str, format_str
     try:
         time_obj = ast.literal_eval(f'datetime.datetime.strptime({time_arg})')
         return int((time_obj - datetime.datetime(1970, 1, 1)).total_seconds() * 1000)
     except Exception:
         return int(-1)
+
+
+def unixtime2local(timestamp: Union[str, int], decimals: bool = True) -> str:
+    """Convert unix time to a nice custom format"""
+    timestr = str(timestamp)
+    if len(timestr) < 10: return ''
+    micros = None
+    millis = None
+    time_decimals = ''
+    if len(timestr) > 10:
+        time_decimals = timestr[10:]
+        if len(time_decimals) <= 3:
+            time_decimals = time_decimals.ljust(3, '0')
+            millis = datetime.timedelta(milliseconds=int(time_decimals))
+        else:
+            time_decimals = time_decimals.ljust(6, '0')
+            micros = datetime.timedelta(microseconds=int(time_decimals))
+
+    unixtime = timestr[:10]
+    utc_time = datetime.datetime.fromtimestamp(int(unixtime), datetime.timezone.utc)
+    local_time = utc_time.astimezone()
+    if decimals and millis:
+        return f'{(local_time + millis).strftime("%Y-%m-%d %H:%M:%S")}.{time_decimals}{local_time.strftime("%z")}'
+    if decimals and micros:
+        return (local_time + micros).strftime("%Y-%m-%d %H:%M:%S.%f%z")  # (%Z)"))
+    return local_time.strftime("%Y-%m-%d %H:%M:%S%z")  # (%Z)"))
+
+
+def convert_time(str_line: str) -> str:
+    """Convert the first 10 digit unix time like string from str argument to a nice time"""
+    timestamp = re.findall(r"^(\d{10}) \[.*", str_line)
+    if timestamp:
+        nice_timestamp = f"{PrintColor(COLORS.BIGreen)}{unixtime2local(timestamp[0])}{PrintColor(COLORS.ColorReset)}"
+        return str_line.replace(str(timestamp[0]), nice_timestamp)
+    return ''
+
+
+def unquote_str(arg):
+    if type(arg) is str: return ast.literal_eval(arg)
+    return arg
+
+
+def is_guid(guid: str) -> bool:
+    """Recognize a GUID format"""
+    return bool(guid_regex.fullmatch(guid))  # identify if argument in an AliEn GUID
+
+
+def run_function(function_name: str, *args, **kwargs):
+    """Python code:: run some arbitrary function name (found in globals) with arbitrary arguments"""
+    return globals()[function_name](*args, *kwargs)  # run arbitrary function
+
+
+def PrintDict(in_arg: Union[str, dict], compact: bool = False):
+    """Print a dictionary in a nice format"""
+    if isinstance(in_arg, str):
+        try:
+            in_arg = json.loads(in_arg)
+        except Exception as e:
+            print_err(f'PrintDict:: Could not load argument as json!\n{e!r}')
+    if isinstance(in_arg, dict):
+        indent = None if compact else 2
+        separators = (',', ':') if compact else None
+        print_out(json.dumps(in_arg, sort_keys = False, indent = indent, separators = separators))
+
+
+def cursor_vertical(lines: int = 0):
+    """Move the cursor up/down N lines"""
+    if lines == 0: return
+    out_char = '\x1b[1A'  # UP
+    if lines < 0:
+        out_char = '\x1b[1B'  # DOWN
+        lines = abs(lines)
+    sys.stdout.write(out_char * lines)
+    sys.stdout.flush()
+
+
+def cursor_horizontal(lines: int = 0):
+    """Move the cursor left/right N lines"""
+    if lines == 0: return
+    out_char = '\x1b[1C'  # RIGHT
+    if lines < 0:
+        out_char = '\x1b[1D'  # LEFT
+        lines = abs(lines)
+    sys.stdout.write(out_char * lines)
+    sys.stdout.flush()
+
+
 def now_str() -> str: return str(datetime.datetime.now().strftime("%Y%m%d_%H%M%S"))
 
 
 def deltat_ms(t0: Union[str, float, None] = None) -> str:
     """Return delta t in ms from a time start; if no argment it return a timestamp in ms"""
     now = datetime.datetime.now().timestamp()
     return f"{(now - float(t0)) * 1000:.3f}" if t0 else f"{now * 1000:.3f}"
@@ -183,33 +185,28 @@
 def is_help(args: Union[str, list]) -> bool:
     if not args: return False
     if isinstance(args, str): args = args.split()
     help_opts = ('-h', '--h', '-help', '--help')
     return any(opt in args for opt in help_opts)
 
 
-def unquote_str(arg):
-    if type(arg) is str: return ast.literal_eval(arg)
-    return arg
-
-
 def read_conf_file(conf_file: str) -> dict:
     """Convert a configuration file with key = value format to a dict"""
     if not conf_file or not os.path.isfile(conf_file): return {}
     DICT_INFO = {}
     try:
         with open(conf_file, encoding="ascii", errors="replace") as rel_file:
             for line in rel_file:
                 line = line.partition('#')[0].rstrip()
                 name, var = line.partition("=")[::2]
                 var = re.sub(r"^\"", '', str(var.strip()))
                 var = re.sub(r"\"$", '', var)
                 DICT_INFO[name.strip()] = var
     except Exception:
-        pass
+        logging.error('Error reading the configuration file: %s', conf_file)
     return DICT_INFO
 
 
 def file2list(input_file: str) -> list:
     """Parse a file and return a list of elements"""
     if not input_file or not os.path.isfile(input_file): return []
     file_list = []
@@ -239,77 +236,40 @@
     """get either lfn key or file key from a file description"""
     if not lfn_obj or not isinstance(lfn_obj, dict): return ''
     if "lfn" in lfn_obj: return lfn_obj["lfn"]
     if "file" in lfn_obj: return lfn_obj["file"]
     return ''
 
 
-
 def pid_uid(pid: int) -> int:
     """Return username of UID of process pid"""
     uid = int(-1)
     try:
         with open(f'/proc/{pid}/status', encoding="ascii", errors="replace") as proc_status:
             for line in proc_status:
                 # Uid, Gid: Real, effective, saved set, and filesystem UIDs(GIDs)
                 if line.startswith('Uid:'): uid = int((line.split()[1]))
     except Exception:
-        pass
+        logging.error('Error getting uid of pid: %d', pid)
     return uid  # noqa: R504
 
 
 def is_my_pid(pid: int) -> bool: return bool(pid_uid(int(pid)) == os.getuid())
 
 
 def writePidFile(filename: str):
     try:
         with open(filename, 'w', encoding="ascii", errors="replace") as f: f.write(str(os.getpid()))
     except Exception:
         logging.exception('Error writing the pid file: %s', filename)
 
 
-def GetSessionFilename() -> str: return os.path.join(os.path.expanduser("~"), ".alienpy_session")
-
-
-def unixtime2local(timestamp: Union[str, int], decimals: bool = True) -> str:
-    """Convert unix time to a nice custom format"""
-    timestr = str(timestamp)
-    if len(timestr) < 10: return ''
-    micros = None
-    millis = None
-    time_decimals = ''
-    if len(timestr) > 10:
-        time_decimals = timestr[10:]
-        if len(time_decimals) <= 3:
-            time_decimals = time_decimals.ljust(3, '0')
-            millis = datetime.timedelta(milliseconds=int(time_decimals))
-        else:
-            time_decimals = time_decimals.ljust(6, '0')
-            micros = datetime.timedelta(microseconds=int(time_decimals))
-
-    unixtime = timestr[:10]
-    utc_time = datetime.datetime.fromtimestamp(int(unixtime), datetime.timezone.utc)
-    local_time = utc_time.astimezone()
-    if decimals and millis:
-        return f'{(local_time + millis).strftime("%Y-%m-%d %H:%M:%S")}.{time_decimals}{local_time.strftime("%z")}'
-    if decimals and micros:
-        return (local_time + micros).strftime("%Y-%m-%d %H:%M:%S.%f%z")  # (%Z)"))
-    return local_time.strftime("%Y-%m-%d %H:%M:%S%z")  # (%Z)"))
-
-
-def convert_time(str_line: str) -> str:
-    """Convert the first 10 digit unix time like string from str argument to a nice time"""
-    timestamp = re.findall(r"^(\d{10}) \[.*", str_line)
-    if timestamp:
-        nice_timestamp = f"{PrintColor(COLORS.BIGreen)}{unixtime2local(timestamp[0])}{PrintColor(COLORS.ColorReset)}"
-        return str_line.replace(str(timestamp[0]), nice_timestamp)
-    return ''
-
-
 def list_remove_item(target_list: list, item_list):
+    """Remove all instances of item from list"""
+    if not target_list: return
     target_list[:] = [el for el in target_list if el != item_list]
 
 
 def get_arg(target: list, item) -> bool:
     """Remove inplace all instances of item from list and return True if found"""
     len_begin = len(target)
     list_remove_item(target, item)
@@ -348,112 +308,186 @@
     try:
         group_info = grp.getgrgid(int(gid))
         return group_info.gr_name
     except Exception:
         return str(gid)
 
 
-def GetHumanReadable(size, precision = 2):
+def GetHumanReadableSize(size, precision = 2):
     """Convert bytes to higher units"""
     suffixes = ['B', 'KiB', 'MiB', 'GiB']
     suffixIndex = 0
     while size > 1024 and suffixIndex < 5:
         suffixIndex += 1  # increment the index of the suffix
         size = size / 1024.0  # apply the division
     return f'{size:.{precision}f} {suffixes[suffixIndex]}'
 
 
-def valid_regex(regex_str: str) -> Union[None, REGEX_PATTERN_TYPE]:
-    """Validate a regex string and return a re.Pattern if valid"""
-    regex = None
-    try:
-        regex = re.compile(regex_str.encode('unicode-escape').decode())  # try to no hit https://docs.python.org/3.6/howto/regex.html#the-backslash-plague
-    except re.error:
-        logging.error('regex validation failed:: %s', regex_str)
-    return regex  # noqa: R504
-
-
-def file2xml_el(filepath: str) -> ALIEN_COLLECTION_EL:
-    """Get a file and return an XML element structure"""
-    if not filepath or not os.path.isfile(filepath): return ALIEN_COLLECTION_EL()
-    p = Path(filepath).expanduser().resolve(strict = True)
-    if p.is_dir(): return ALIEN_COLLECTION_EL()
-    p_stat = p.stat()
-    turl = f'file://{p.as_posix()}'
-    return ALIEN_COLLECTION_EL(
-        name = p.name, aclId = "", broken = "0", ctime = time_unix2simple(p_stat.st_ctime),
-        dir = '', entryId = '', expiretime = '', gowner = p.group(), guid = '', guidtime = '', jobid = '', lfn = turl,
-        md5 = md5(p.as_posix()), owner = p.owner(), perm = str(oct(p_stat.st_mode))[5:], replicated = "0",
-        size = str(p_stat.st_size), turl = turl, type = 'f')
-
-
-def mk_xml_local(filepath_list: list):
-    xml_root = ET.Element('alien')
-    collection = ET.SubElement(xml_root, 'collection', attrib={'name': 'tempCollection'})
-    for idx, item in enumerate(filepath_list, start = 1):
-        e = ET.SubElement(collection, 'event', attrib={'name': str(idx)})
-        f = ET.SubElement(e, 'file', attrib = file2xml_el(lfn_prefix_re.sub('', item))._asdict())  # noqa:F841
-    oxml = ET.tostring(xml_root, encoding = 'ascii')
-    dom = MD.parseString(oxml)
-    return dom.toprettyxml()
-
-
-def runShellCMD(INPUT: str = '', captureout: bool = True, do_shell: bool = False, timeout: Union[str, int, None] = None) -> RET:
-    """Run shell command in subprocess; if exists, print stdout and stderr"""
-    if not INPUT: return RET(1, '', 'No command to be run provided')
-    sh_cmd = re.sub(r'^!', '', INPUT)
-    args = sh_cmd if do_shell else shlex.split(sh_cmd)
-    capture_args = {'stdout': subprocess.PIPE, 'stderr': subprocess.PIPE} if captureout else {}
-    status = exitcode = except_msg = None
-    msg_out = msg_err = ''
-    try:
-        status = subprocess.run(args, encoding = 'utf-8', errors = 'replace', shell = do_shell, **capture_args)  # pylint: disable=subprocess-run-check
-    except subprocess.TimeoutExpired:
-        print_err(f"Expired timeout: {timeout} for: {sh_cmd}")
-        exitcode = int(62)
-    except FileNotFoundError:
-        print_err(f"Command not found: {sh_cmd}")
-        exitcode = int(2)
-    except Exception:
-        ex_type, ex_value, ex_traceback = sys.exc_info()
-        except_msg = f'Exception:: {ex_type} -> {ex_value}\n{ex_traceback}\n'
-        exitcode = int(1)
-
-    if status:
-        if status.stdout: msg_out = status.stdout.strip()
-        if status.stderr: msg_err = status.stderr.strip()
-        exitcode = status.returncode
-    if except_msg: msg_err = f'{except_msg}\n{msg_err}'
-    return RET(exitcode, msg_out, msg_err)
-
-
-
 def check_ip_port(socket_object: tuple) -> bool:
     """Check connectivity to an address, port; adress should be the tuple given by getaddrinfo"""
     if not socket_object: return False
+    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     is_open = False
     # socket_object = (family, type, proto, canonname, sockaddr)
     with socket.socket(socket_object[0], socket_object[1], socket_object[2]) as s:  # Create a TCP socket
         s.settimeout(2)  # timeout 2s
         try:
             s.connect(socket_object[4])
             is_open = True
-        except Exception:
-            pass
+        except Exception as e:
+            logging.error('check_ip_port:: error connecting to %s', str(socket_object[4]))
+            if DEBUG: logging.exception(e)
     return is_open  # noqa: R504
 
 
 def check_port(address: str, port: Union[str, int]) -> list:
     """Check TCP connection to fqdn:port"""
-    ip_list = socket.getaddrinfo(address, int(port), proto = socket.IPPROTO_TCP)
+    try:
+        ip_list = socket.getaddrinfo(address, int(port), proto = socket.IPPROTO_TCP)
+    except:
+        print_out(f'check_port:: error getting address info for host: {address} ; port: {port}')
+        return []
     return [(*sock_obj[-1], check_ip_port(sock_obj)) for sock_obj in ip_list]
 
 
 def isReachable(address: str = 'alice-jcentral.cern.ch', port: Union[str, int] = 8097) -> bool:
     result_list = check_port(address, port)
     return any(ip[-1] for ip in result_list)
 
 
+def exitcode(args: Union[list, None] = None):  # pylint: disable=unused-argument
+    """Return the latest global recorded exitcode"""
+    return RET(0, f"{AlienSessionInfo['exitcode']}", '')  # type: ignore [call-arg]
+
+
+def valid_regex(regex_str: str) -> Union[None, REGEX_PATTERN_TYPE]:
+    """Validate a regex string and return a re.Pattern if valid"""
+    regex = None
+    try:
+        regex = re.compile(regex_str.encode('unicode-escape').decode())  # try to no hit https://docs.python.org/3.6/howto/regex.html#the-backslash-plague
+    except re.error:
+        logging.error('regex validation failed:: %s', regex_str)
+    return regex  # noqa: R504
+
+
+def name2regex(pattern_regex: str = '') -> str:
+    """Convert -name/-select argument of cp/find2 to regex form"""
+    if not pattern_regex: return ''
+    translated_pattern_regex = ''
+    re_all = '.*'
+    re_all_end = '[^/]*'
+    verbs = ('begin', 'contain', 'ends', 'ext')
+    pattern_list = pattern_regex.split('_')
+    if any(verb in pattern_regex for verb in verbs):
+        if pattern_list.count('begin') > 1 or pattern_list.count('end') > 1 or pattern_list.count('ext') > 1:
+            print_out('<begin>, <end>, <ext> verbs cannot appear more than once in the name selection')
+            return ''
+
+        list_begin = []
+        list_contain = []
+        list_ends = []
+        list_ext = []
+        for idx, tokenstr in enumerate(pattern_list):
+            if tokenstr == 'begin': list_begin.append(KV(tokenstr, pattern_list[idx + 1]))
+            if tokenstr == 'contain': list_contain.append(KV(tokenstr, pattern_list[idx + 1]))
+            if tokenstr == 'ends': list_ends.append(KV(tokenstr, pattern_list[idx + 1]))
+            if tokenstr == 'ext': list_ext.append(KV(tokenstr, pattern_list[idx + 1]))
+
+        if list_begin:
+            translated_pattern_regex = re_all + '/' + f'{list_begin[0].val}{re_all_end}'  # first string after the last slash (last match exclude /)
+        for patt in list_contain:
+            if not list_begin: translated_pattern_regex = f'{re_all}'
+            translated_pattern_regex = f'{translated_pattern_regex}{patt.val}{re_all_end}'
+        if list_ends:
+            translated_pattern_regex = f'{translated_pattern_regex}{list_ends[0].val}{re_all_end}'
+        if list_ext:
+            translated_pattern_regex = translated_pattern_regex + "\\." + list_ext[0].val
+        if translated_pattern_regex:
+            if list_ext:
+                translated_pattern_regex = f'{translated_pattern_regex}' + '$'
+            else:
+                translated_pattern_regex = f'{translated_pattern_regex}{re_all_end}' + '$'
+    return translated_pattern_regex  # noqa: R504
+
+
+def cleanup_temp(item: str = ''):
+    """Remove from disk all recorded temporary files"""
+    try:
+        AlienSessionInfo
+    except NameError:
+        return
+    if not AlienSessionInfo['templist']: return
+
+    def rm_item(i: str = ''):
+        if not i: return
+        if os.path.isfile(i):
+            AlienSessionInfo['templist'].remove(i)
+            os.remove(i)
+    if item:
+        rm_item(item)
+    else:
+        for f in AlienSessionInfo['templist']: rm_item(f)
+
+
+def import_aliases():
+    """Import defined aliases in the global session variable"""
+    try:
+        AlienSessionInfo
+    except NameError:
+        return
+    alias_file = os.path.join(os.path.expanduser("~"), ".alienpy_aliases")
+    if os.path.exists(alias_file): AlienSessionInfo['alias_cache'] = read_conf_file(alias_file)
+
+
+def convert_trace2dict(trace:str = '') -> dict:
+    """Convert an JAliEn trace output to a somewhat usable dictionary"""
+    trace_dict = { 'state': [], 'trace': [], 'proc': [], 'workdir': '', 'wn': '', 'queue': []}
+    procfmt = []
+    for line in trace.split('\n'):
+        nice_line = convert_time(str(line))
+
+        rez = nice_line.split('[state     ]: ')
+        if len(rez) > 1:
+            trace_dict['state'].append(' '.join(rez))
+            continue
+        rez = nice_line.split('[trace     ]: ')
+        if len(rez) > 1:
+            trace_dict['trace'].append(' '.join(rez))
+            if 'Created workdir' in rez[1]:
+                trace_dict['workdir'] = rez[1].split(': ')[1]
+            if re.match('Running.*on.*', rez[1], re.IGNORECASE):
+                trace_dict['wn'] = rez[1].split()[-1]
+            if 'BatchId' in rez[1]:
+                q_info = rez[1].replace('BatchId', '').strip()
+                trace_dict['queue'].append(q_info)
+            continue
+        rez = nice_line.split('[proc      ]: ')
+        if len(rez) > 1:
+            trace_dict['proc'].append(' '.join(rez))
+            continue
+        rez = nice_line.split('[procfmt   ]: ')
+        if len(rez) > 1:
+            procfmt.append(' '.join(rez))
+            continue
+    trace_dict['proc'][0:0] = procfmt
+    return trace_dict
+
+
+def convert_jdl2dict(jdl:str = '') -> dict:
+    """Convert an JAliEn jdl to a dictionary"""
+    jdl_dict = dict()
+    for line in re.split(r';\s+', jdl):
+        line = re.sub(r'\s+', ' ', line).strip()
+        k, _, v = line.partition('=')
+        v = v.replace('"', '').strip()
+        if v.startswith('{') and v.endswith('}'):
+            v = v.replace('{', '').replace('}', '').strip()
+            v = v.split(', ')
+            list(map(str.strip, v))
+        jdl_dict[k.strip()] = v
+    return jdl_dict
+
+
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
```

### Comparing `alienpy-1.4.6/alienpy.egg-info/PKG-INFO` & `alienpy-1.5.0/alienpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alienpy
-Version: 1.4.6
+Version: 1.5.0
 Summary: Websocket based cli interface for ALICE experiment GRID infrastructure
 Home-page: https://gitlab.cern.ch/jalien/xjalienfs
 Author: Adrian Sevcenco
 Author-email: adrian.sevcenco@cern.ch
 Project-URL: Dev git, https://github.com/adriansev/jalien_py
 Project-URL: Issues, https://github.com/adriansev/jalien_py/issues
 Project-URL: Changelog, https://github.com/adriansev/jalien_py/commits/master
```

### Comparing `alienpy-1.4.6/alienpy.egg-info/SOURCES.txt` & `alienpy-1.5.0/alienpy.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 LICENSE
 README.md
 setup.py
-alienpy/VERSION
 alienpy/__init__.py
 alienpy/alien.py
-alienpy/cmds_client_local.py
-alienpy/cmds_client_wb.py
-alienpy/data.py
-alienpy/fs_grid.py
-alienpy/fs_local.py
-alienpy/http_tools.py
-alienpy/jalien_talk.py
-alienpy/re_patt.py
-alienpy/ssl_tools.py
-alienpy/tools.py
+alienpy/async_tools.py
+alienpy/connect_ssl.py
+alienpy/data_structs.py
+alienpy/global_vars.py
+alienpy/setup_cwd.py
+alienpy/setup_logging.py
+alienpy/tools_files.py
+alienpy/tools_misc.py
+alienpy/tools_shell.py
+alienpy/tools_stackcmd.py
+alienpy/version.py
 alienpy/wb_api.py
-alienpy/wb_base.py
+alienpy/wb_async.py
+alienpy/xrd_core.py
+alienpy/xrd_tools.py
 alienpy.egg-info/PKG-INFO
 alienpy.egg-info/SOURCES.txt
 alienpy.egg-info/dependency_links.txt
 alienpy.egg-info/entry_points.txt
 alienpy.egg-info/requires.txt
 alienpy.egg-info/top_level.txt
 examples/alien_wbtime
```

### Comparing `alienpy-1.4.6/alienpy.egg-info/entry_points.txt` & `alienpy-1.5.0/alienpy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `alienpy-1.4.6/examples/alien_wbtime` & `alienpy-1.5.0/examples/alien_wbtime`

 * *Files identical despite different names*

### Comparing `alienpy-1.4.6/setup.py` & `alienpy-1.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import os
 import sys
 import setuptools
 import traceback
 
 
-def get_version_from_file():
+try:
+    from alienpy.version import *  # nosec PYL-W0614
+except Exception:
     try:
-        f = open('alienpy/VERSION', encoding="ascii")
-        version = f.read().strip()
-        f.close()
-        return version
+        from xjalienfs.version import *  # nosec PYL-W0614
     except Exception:
         traceback.print_exc()
-        print('Failed to get version from file. Using unknown')
-        return 'unknown'
-
+        print('Failed to get version from file. Using 0.0.0')
+        ALIENPY_VERSION_STR = '0.0.0'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 base_requirements = [ 'async-stagger', 'pyOpenSSL', 'rich', 'requests', ]
 alibuild_requirements = [ 'gnureadline' ]
 local_requirements = [ 'xrootd' ]
@@ -32,37 +30,37 @@
 # also the xrootd is built in a separate recipe
 if "ALIBUILD" in os.environ:
     selected_requirements = base_requirements + alibuild_requirements
 else:
     selected_requirements = base_requirements + local_requirements
 
 setuptools.setup(
-    name="alienpy",
-    version=get_version_from_file(),
-    author="Adrian Sevcenco",
-    author_email="adrian.sevcenco@cern.ch",
-    description="Websocket based cli interface for ALICE experiment GRID infrastructure",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://gitlab.cern.ch/jalien/xjalienfs",
-    packages=setuptools.find_packages(),
-    install_requires=selected_requirements,
-    python_requires='>=3.6',
-    classifiers=[
+    name = "alienpy",
+    version = ALIENPY_VERSION_STR,
+    packages = setuptools.find_packages(),
+    author = "Adrian Sevcenco",
+    author_email = "adrian.sevcenco@cern.ch",
+    description = "Websocket based cli interface for ALICE experiment GRID infrastructure",
+    long_description = long_description,
+    long_description_content_type = "text/markdown",
+    url = "https://gitlab.cern.ch/jalien/xjalienfs",
+    install_requires = selected_requirements,
+    python_requires = '>=3.6',
+    classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
-    ],
-    project_urls={
+        ],
+    project_urls = {
         "Dev git": "https://github.com/adriansev/jalien_py",
         "Issues": "https://github.com/adriansev/jalien_py/issues",
         "Changelog": "https://github.com/adriansev/jalien_py/commits/master",
         "Documentation": "https://jalien.docs.cern.ch",
         "CERN Mattermost/JAliEn": "https://mattermost.web.cern.ch/alice/channels/jalien",
-    },
+        },
     entry_points = {
         'console_scripts': [
             'alien.py = alienpy.alien:main',
             'alien_cmd = alienpy.alien:main',
             'alien_cp = alienpy.alien:main',
             'alien_find = alienpy.alien:main',
             'alien_guid2lfn = alienpy.alien:main',
@@ -78,17 +76,15 @@
             'alien_stat = alienpy.alien:main',
             'alien_submit = alienpy.alien:main',
             'alien_whereis = alienpy.alien:main',
             'alien-cert-info = alienpy.alien:cmd_cert_info',
             'alien-token-info = alienpy.alien:cmd_token_info',
             'alien-token-init = alienpy.alien:cmd_token_init',
             'alien-token-destroy = alienpy.alien:cmd_token_destroy',
-        ]
-    },
+            ]
+        },
     scripts = [
         'examples/alien_wbtime',
         ],
-    data_files = [('alienpy', ['alienpy/VERSION'])],
     keywords = 'CERN ALICE JAliEn GRID',
-
 )
```

