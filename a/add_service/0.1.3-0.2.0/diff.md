# Comparing `tmp/add_service-0.1.3.tar.gz` & `tmp/add_service-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/add_service-0.1.3.tar", last modified: Fri May  5 05:49:24 2023, max compression
+gzip compressed data, was "dist/add_service-0.2.0.tar", last modified: Fri May  5 06:26:57 2023, max compression
```

## Comparing `add_service-0.1.3.tar` & `add_service-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 05:49:24.000000 add_service-0.1.3/
--rw-rw-r--   0 dl        (1000) dl        (1000)       18 2022-01-21 10:58:17.000000 add_service-0.1.3/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      575 2023-05-05 05:49:24.000000 add_service-0.1.3/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     1953 2023-05-05 05:45:42.000000 add_service-0.1.3/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service/
--rw-rw-r--   0 dl        (1000) dl        (1000)        0 2022-01-21 11:03:02.000000 add_service-0.1.3/add_service/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     5730 2023-05-05 05:49:07.000000 add_service-0.1.3/add_service/__main__.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      575 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      218 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-05-05 05:49:24.000000 add_service-0.1.3/add_service.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-05-05 05:49:24.000000 add_service-0.1.3/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      959 2022-01-21 10:59:47.000000 add_service-0.1.3/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 06:26:57.000000 add_service-0.2.0/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       18 2022-01-21 10:58:17.000000 add_service-0.2.0/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      569 2023-05-05 06:26:57.000000 add_service-0.2.0/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1919 2023-05-05 06:24:46.000000 add_service-0.2.0/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 06:26:57.000000 add_service-0.2.0/add_service/
+-rw-rw-r--   0 dl        (1000) dl        (1000)        0 2022-01-21 11:03:02.000000 add_service-0.2.0/add_service/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5784 2023-05-05 06:24:04.000000 add_service-0.2.0/add_service/__main__.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-05-05 06:26:57.000000 add_service-0.2.0/add_service.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      569 2023-05-05 06:26:57.000000 add_service-0.2.0/add_service.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      256 2023-05-05 06:26:57.000000 add_service-0.2.0/add_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-05-05 06:26:57.000000 add_service-0.2.0/add_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       59 2023-05-05 06:26:57.000000 add_service-0.2.0/add_service.egg-info/entry_points.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-05-05 06:26:57.000000 add_service-0.2.0/add_service.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-05-05 06:26:57.000000 add_service-0.2.0/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1078 2023-05-05 06:11:57.000000 add_service-0.2.0/setup.py
```

### Comparing `add_service-0.1.3/README.md` & `add_service-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# add_service: python tool for simply adding startup item by systemd.
+# `add_service`: CLI tool for simply adding startup item by systemd.
 
 ```bash
-Python tool for simply adding startup item by systemd.
+CLI tool for simply adding startup item by systemd.
 
 Install:
     pip install add_service
 
 Usage:
-    python -m add_service shell_file/cmd [--user root(default `whoami`)] [--name service_name] [--start]
+    add_service shell_file/cmd [--user root(default `whoami`)] [--name service_name] [--start]
 
     positional arguments:
         script       Executable file or cmd
 
     optional arguments:
     -h, --help   show this help message and exit
     -l, --ls     List all services created by add_service
     --rm NAME    Remove the service created by add_service
     --user USER  User to exec script, default is `whoami`
     --name NAME  Service name, default add_service0.service
     --start      Start service immediately
 
 Examples:
+    add_service "`which python3` -m http.server 80" --user root --name http_server
     python -m add_service ssh_nat.sh   # defaut service name is ssh_nat.service
-    python -m add_service "`which python3` -m http.server 80" --user root --name http_server
 ```
 **For example:** share directory "~/share" by python http.server when system startup.
 ```bash
 user@host:~$ cd ~/share/
-user@host:~/share$ python -m add_service "`which python3` -m http.server 80" --user root --name http_server
+user@host:~/share$ add_service "`which python3` -m http.server 80" --user root --name http_server
 ```
 ```
 Below will write to "http_server.service"
 --------------------
 
 [Unit]
 Description="http_server.service added by add_service: Namespace(name='http_server', script='/home/dl/miniconda3/bin/python3 -m http.server 80', user='root')"
```

### Comparing `add_service-0.1.3/add_service/__main__.py` & `add_service-0.2.0/add_service/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
-__version__ = "0.1.3"
-__description__ = "Python tool for simply adding startup item by systemd."
+__version__ = "0.2.0"
+__description__ = "CLI tool for simply adding startup item by systemd."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
 __url__ = "https://github.com/DIYer22/add_service"
@@ -24,19 +24,19 @@
 doc = f"""
 {__description__}
 
 Install:
     pip install add_service
 
 Usage:
-    python -m add_service shell_file/cmd [--user root(default `whoami`)] [--name service_name] [--start]
+    add_service shell_file/cmd [--user root(default `whoami`)] [--name service_name] [--start]
 
 Examples:
+    add_service "`which python3` -m http.server 80" --user root --name http_server
     python -m add_service ssh_nat.sh   # defaut service name is ssh_nat.service
-    python -m add_service "`which python3` -m http.server 80" --user root --name http_server
 
 See: 
     https://github.com/DIYer22/add_service
 """
 
 
 def execmd(cmd):
@@ -72,15 +72,15 @@
                 str += f"\n\t{os.path.basename(service_path)}\t{service_path}"
         except:
             pass
     str = "Services created by add_service:" + (str if str else " null")
     return str
 
 
-if __name__ == "__main__":
+def main():
     if (
         "-l" in sys.argv
         or "--ls" in sys.argv
         or ("ls" in sys.argv and len(sys.argv) == 2)
     ):
         print(list_all_services())
         exit(0)
@@ -93,18 +93,20 @@
             assert os.path.isfile(service_path), service_path
             cmd = f'sudo systemctl stop "{service_name}"; sudo systemctl disable "{service_name}"; sudo rm "{service_path}"'
             print(f"Remove {service_name} by cmd:\n\t{cmd}")
             os.system(cmd)
         exit(0)
 
     if "-h" in sys.argv or "--help" in sys.argv:
-        doc = doc + "\n" + list_all_services()
+        description = doc + "\n" + list_all_services()
+    else:
+        description = doc
 
     parser = argparse.ArgumentParser(
-        description=doc, formatter_class=argparse.RawTextHelpFormatter
+        description=description, formatter_class=argparse.RawTextHelpFormatter
     )
     parser.add_argument("script", type=str, help="Executable file or cmd")
     parser.add_argument(
         "-l",
         "--ls",
         action="store_true",
         help="List all services created by add_service",
@@ -187,7 +189,11 @@
     print("Execute cmd:")
     print("\t" + cmd)
     assert not os.system(cmd)
 
     if not args.start:
         print("Start service right now by manual:")
         print(f"\t{start_cmd}")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `add_service-0.1.3/add_service.egg-info/PKG-INFO` & `add_service-0.2.0/add_service.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: add-service
-Version: 0.1.3
-Summary: Python tool for simply adding startup item by systemd.
+Version: 0.2.0
+Summary: CLI tool for simply adding startup item by systemd.
 Home-page: https://github.com/DIYer22/add_service
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
-Description: Python tool for simply adding startup item by systemd.
+Description: CLI tool for simply adding startup item by systemd.
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `add_service-0.1.3/setup.py` & `add_service-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,8 +29,13 @@
     long_description=info["__description__"],
     long_description_content_type="text/markdown",
     url=info["__url__"],
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=info["__classifiers__"],
     include_package_data=True,
+    entry_points={
+        "console_scripts": [
+            "add_service=add_service.__main__:main",
+        ],
+    },
 )
```

