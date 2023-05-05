# Comparing `tmp/add_service-0.1.2.tar.gz` & `tmp/add_service-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/add_service-0.1.2.tar", last modified: Thu Mar  2 09:50:47 2023, max compression
+gzip compressed data, was "dist/add_service-0.1.3.tar", last modified: Fri May  5 05:49:24 2023, max compression
```

## Comparing `add_service-0.1.2.tar` & `add_service-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-03-02 09:50:47.000000 add_service-0.1.2/
--rw-rw-r--   0 dl        (1000) dl        (1000)       18 2022-01-21 10:58:17.000000 add_service-0.1.2/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      575 2023-03-02 09:50:47.000000 add_service-0.1.2/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     1864 2023-03-02 09:44:20.000000 add_service-0.1.2/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-03-02 09:50:47.000000 add_service-0.1.2/add_service/
--rw-rw-r--   0 dl        (1000) dl        (1000)        0 2022-01-21 11:03:02.000000 add_service-0.1.2/add_service/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4970 2023-03-02 09:48:22.000000 add_service-0.1.2/add_service/__main__.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-03-02 09:50:47.000000 add_service-0.1.2/add_service.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      575 2023-03-02 09:50:47.000000 add_service-0.1.2/add_service.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      218 2023-03-02 09:50:47.000000 add_service-0.1.2/add_service.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-03-02 09:50:47.000000 add_service-0.1.2/add_service.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-03-02 09:50:47.000000 add_service-0.1.2/add_service.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-03-02 09:50:47.000000 add_service-0.1.2/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      959 2022-01-21 10:59:47.000000 add_service-0.1.2/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 05:49:24.000000 add_service-0.1.3/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       18 2022-01-21 10:58:17.000000 add_service-0.1.3/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      575 2023-05-05 05:49:24.000000 add_service-0.1.3/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1953 2023-05-05 05:45:42.000000 add_service-0.1.3/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service/
+-rw-rw-r--   0 dl        (1000) dl        (1000)        0 2022-01-21 11:03:02.000000 add_service-0.1.3/add_service/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5730 2023-05-05 05:49:07.000000 add_service-0.1.3/add_service/__main__.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      575 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      218 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-05-05 05:49:24.000000 add_service-0.1.3/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)      959 2022-01-21 10:59:47.000000 add_service-0.1.3/setup.py
```

### Comparing `add_service-0.1.2/PKG-INFO` & `add_service-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: add_service
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python tool for simply adding startup item by systemd.
 Home-page: https://github.com/DIYer22/add_service
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Python tool for simply adding startup item by systemd.
 Platform: UNKNOWN
```

### Comparing `add_service-0.1.2/README.md` & `add_service-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 
     positional arguments:
         script       Executable file or cmd
 
     optional arguments:
     -h, --help   show this help message and exit
     -l, --ls     List all services created by add_service
+    --rm NAME    Remove the service created by add_service
     --user USER  User to exec script, default is `whoami`
-    --name NAME  Service name
+    --name NAME  Service name, default add_service0.service
     --start      Start service immediately
 
 Examples:
     python -m add_service ssh_nat.sh   # defaut service name is ssh_nat.service
     python -m add_service "`which python3` -m http.server 80" --user root --name http_server
 ```
 **For example:** share directory "~/share" by python http.server when system startup.
```

### Comparing `add_service-0.1.2/add_service/__main__.py` & `add_service-0.1.3/add_service/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __description__ = "Python tool for simply adding startup item by systemd."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
@@ -68,45 +68,65 @@
     service_paths = sorted(glob.glob("/etc/systemd/system/*.service"))
     for service_path in service_paths:
         try:
             if added_by_add_service in open(service_path).read():
                 str += f"\n\t{os.path.basename(service_path)}\t{service_path}"
         except:
             pass
-    str = "Services created by add_service:\n" + (str if str else "\tnull")
+    str = "Services created by add_service:" + (str if str else " null")
     return str
 
 
 if __name__ == "__main__":
     if (
         "-l" in sys.argv
         or "--ls" in sys.argv
         or ("ls" in sys.argv and len(sys.argv) == 2)
     ):
         print(list_all_services())
         exit(0)
+
+    if "--rm" in sys.argv:
+        service_names = sys.argv[sys.argv.index("--rm") + 1 :]
+        for service_name in service_names:
+            service_name = service_name.replace(".service", "") + ".service"
+            service_path = f"/etc/systemd/system/{service_name}"
+            assert os.path.isfile(service_path), service_path
+            cmd = f'sudo systemctl stop "{service_name}"; sudo systemctl disable "{service_name}"; sudo rm "{service_path}"'
+            print(f"Remove {service_name} by cmd:\n\t{cmd}")
+            os.system(cmd)
+        exit(0)
+
     if "-h" in sys.argv or "--help" in sys.argv:
         doc = doc + "\n" + list_all_services()
 
     parser = argparse.ArgumentParser(
         description=doc, formatter_class=argparse.RawTextHelpFormatter
     )
     parser.add_argument("script", type=str, help="Executable file or cmd")
     parser.add_argument(
         "-l",
         "--ls",
         action="store_true",
         help="List all services created by add_service",
     )
     parser.add_argument(
+        "--rm",
+        metavar="NAME",
+        default=None,
+        help="Remove the service created by add_service",
+    )
+    parser.add_argument(
         "--user",
         default=execmd("whoami"),
         help="User to exec script, default is `whoami`",
     )
-    parser.add_argument("--name", default=None, help="Service name")
+    parser.add_argument(
+        "--name", default=None, help="Service name, default add_service0.service"
+    )
     parser.add_argument(
         "--start", action="store_true", help="Start service immediately"
     )
 
     args = parser.parse_args()
 
     if os.path.isfile(args.script):
```

### Comparing `add_service-0.1.2/add_service.egg-info/PKG-INFO` & `add_service-0.1.3/add_service.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: add-service
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python tool for simply adding startup item by systemd.
 Home-page: https://github.com/DIYer22/add_service
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Python tool for simply adding startup item by systemd.
 Platform: UNKNOWN
```

### Comparing `add_service-0.1.2/setup.py` & `add_service-0.1.3/setup.py`

 * *Files identical despite different names*

