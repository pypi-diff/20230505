# Comparing `tmp/gpt4all-0.1.4.tar.gz` & `tmp/gpt4all-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-0.1.4.tar", last modified: Fri May  5 14:29:33 2023, max compression
+gzip compressed data, was "gpt4all-0.1.5.tar", last modified: Fri May  5 16:44:32 2023, max compression
```

## Comparing `gpt4all-0.1.4.tar` & `gpt4all-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.771147 gpt4all-0.1.4/
--rw-r--r--   0 richardguo   (501) staff       (20)     1054 2023-05-04 16:02:39.000000 gpt4all-0.1.4/LICENSE.txt
--rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-05 14:29:33.770988 gpt4all-0.1.4/PKG-INFO
--rw-r--r--   0 richardguo   (501) staff       (20)      987 2023-05-04 16:00:37.000000 gpt4all-0.1.4/README.md
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.769194 gpt4all-0.1.4/gpt4all/
--rw-r--r--   0 richardguo   (501) staff       (20)       65 2023-05-03 19:06:54.000000 gpt4all-0.1.4/gpt4all/__init__.py
--rw-r--r--   0 richardguo   (501) staff       (20)     2418 2023-05-03 19:13:41.000000 gpt4all-0.1.4/gpt4all/gpt4all.py
--rw-r--r--   0 richardguo   (501) staff       (20)   285210 2023-05-04 20:22:29.000000 gpt4all-0.1.4/gpt4all/pyllmodel.c
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.769928 gpt4all-0.1.4/gpt4all.egg-info/
--rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/PKG-INFO
--rw-r--r--   0 richardguo   (501) staff       (20)      384 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/SOURCES.txt
--rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/dependency_links.txt
--rw-r--r--   0 richardguo   (501) staff       (20)       30 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/requires.txt
--rw-r--r--   0 richardguo   (501) staff       (20)       14 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/top_level.txt
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.770027 gpt4all-0.1.4/llmodel_DO_NOT_MODIFY/
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.770130 gpt4all-0.1.4/llmodel_DO_NOT_MODIFY/build/
--rwxr-xr-x   0 richardguo   (501) staff       (20)   202605 2023-05-01 13:57:50.000000 gpt4all-0.1.4/llmodel_DO_NOT_MODIFY/build/libllmodel.dylib
--rw-r--r--   0 richardguo   (501) staff       (20)     1553 2023-05-01 03:53:22.000000 gpt4all-0.1.4/llmodel_DO_NOT_MODIFY/llmodel.h
--rw-r--r--   0 richardguo   (501) staff       (20)       38 2023-05-05 14:29:33.771201 gpt4all-0.1.4/setup.cfg
--rw-r--r--   0 richardguo   (501) staff       (20)     3161 2023-05-05 14:29:21.000000 gpt4all-0.1.4/setup.py
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.770690 gpt4all-0.1.4/tests/
--rw-r--r--   0 richardguo   (501) staff       (20)        0 2023-05-03 19:03:47.000000 gpt4all-0.1.4/tests/__init__.py
--rw-r--r--   0 richardguo   (501) staff       (20)      687 2023-05-03 19:05:28.000000 gpt4all-0.1.4/tests/test_gpt4all.py
--rw-r--r--   0 richardguo   (501) staff       (20)     1129 2023-05-03 19:05:34.000000 gpt4all-0.1.4/tests/test_pyllmodel.py
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 16:44:32.664003 gpt4all-0.1.5/
+-rw-r--r--   0 richardguo   (501) staff       (20)     1054 2023-05-04 16:02:39.000000 gpt4all-0.1.5/LICENSE.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-05 16:44:32.663713 gpt4all-0.1.5/PKG-INFO
+-rw-r--r--   0 richardguo   (501) staff       (20)      987 2023-05-04 16:00:37.000000 gpt4all-0.1.5/README.md
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 16:44:32.662274 gpt4all-0.1.5/gpt4all/
+-rw-r--r--   0 richardguo   (501) staff       (20)       65 2023-05-03 19:06:54.000000 gpt4all-0.1.5/gpt4all/__init__.py
+-rw-r--r--   0 richardguo   (501) staff       (20)     2418 2023-05-03 19:13:41.000000 gpt4all-0.1.5/gpt4all/gpt4all.py
+-rw-r--r--   0 richardguo   (501) staff       (20)   285280 2023-05-05 15:06:13.000000 gpt4all-0.1.5/gpt4all/pyllmodel.c
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 16:44:32.662948 gpt4all-0.1.5/gpt4all.egg-info/
+-rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-05 16:44:32.000000 gpt4all-0.1.5/gpt4all.egg-info/PKG-INFO
+-rw-r--r--   0 richardguo   (501) staff       (20)      307 2023-05-05 16:44:32.000000 gpt4all-0.1.5/gpt4all.egg-info/SOURCES.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-05 16:44:32.000000 gpt4all-0.1.5/gpt4all.egg-info/dependency_links.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       30 2023-05-05 16:44:32.000000 gpt4all-0.1.5/gpt4all.egg-info/requires.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       14 2023-05-05 16:44:32.000000 gpt4all-0.1.5/gpt4all.egg-info/top_level.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       38 2023-05-05 16:44:32.664073 gpt4all-0.1.5/setup.cfg
+-rw-r--r--   0 richardguo   (501) staff       (20)     3597 2023-05-05 16:44:14.000000 gpt4all-0.1.5/setup.py
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 16:44:32.663363 gpt4all-0.1.5/tests/
+-rw-r--r--   0 richardguo   (501) staff       (20)        0 2023-05-03 19:03:47.000000 gpt4all-0.1.5/tests/__init__.py
+-rw-r--r--   0 richardguo   (501) staff       (20)      687 2023-05-03 19:05:28.000000 gpt4all-0.1.5/tests/test_gpt4all.py
+-rw-r--r--   0 richardguo   (501) staff       (20)     1129 2023-05-03 19:05:34.000000 gpt4all-0.1.5/tests/test_pyllmodel.py
```

### Comparing `gpt4all-0.1.4/LICENSE.txt` & `gpt4all-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.4/README.md` & `gpt4all-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.4/gpt4all/gpt4all.py` & `gpt4all-0.1.5/gpt4all/gpt4all.py`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.4/gpt4all/pyllmodel.c` & `gpt4all-0.1.5/gpt4all/pyllmodel.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "../../llmodel/llmodel_c.h"
+            "gpt4all/llmodel_DO_NOT_MODIFY/llmodel_c.h"
         ],
         "extra_link_args": [
-            "-Wl,-rpath,../../llmodel/build/"
+            "-Wl,-rpath=$ORIGIN/gpt4all/llmodel_DO_NOT_MODIFY/build"
         ],
         "include_dirs": [
-            "../../llmodel/"
+            "gpt4all/llmodel_DO_NOT_MODIFY/"
         ],
         "libraries": [
             "llmodel"
         ],
         "library_dirs": [
-            "../../llmodel/build/"
+            "gpt4all/llmodel_DO_NOT_MODIFY/build"
         ],
         "name": "gpt4all.pyllmodel",
         "sources": [
             "gpt4all/pyllmodel.pyx"
         ]
     },
     "module_name": "gpt4all.pyllmodel"
```

### Comparing `gpt4all-0.1.4/setup.py` & `gpt4all-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,20 +8,26 @@
 package_name = "gpt4all"
 
 # Define the location of your prebuilt C library files
 SRC_CLIB_DIRECtORY = "../../llmodel/"
 SRC_CLIB_BUILD_DIRECTORY = "../../llmodel/build"
 
 LIB_NAME = "llmodel"
-DEST_CLIB_DIRECTORY = f"{LIB_NAME}_DO_NOT_MODIFY/"
-DEST_CLIB_BUILD_DIRECTORY = os.path.join(DEST_CLIB_DIRECTORY, "build")
 
 
+DEST_CLIB_DIRECTORY = os.path.abspath(f"{package_name}/{LIB_NAME}_DO_NOT_MODIFY")
+DEST_CLIB_BUILD_DIRECTORY = os.path.abspath(os.path.join(DEST_CLIB_DIRECTORY, "build"))
+# LIB_BUILD_DIR is where Cython extension will look for library via rpath
+LIB_BUILD_DIR = os.path.abspath(f"{LIB_NAME}_DO_NOT_MODIFY/build")
+HOME_DIR = os.path.abspath(".")
+
+system = platform.system()
+
 def get_c_shared_lib_extension():
-    system = platform.system()
+    
     if system == "Darwin":
         return "dylib"
     elif system == "Linux":
         return "so"
     elif system == "Windows":
         return "dll"
     else:
@@ -46,48 +52,56 @@
 
     if not os.path.exists(dest_build_dir):
         os.mkdir(dest_build_dir)
     for item in os.listdir(src_build_dir):
         # copy over shared library to dest build dir
         if item.endswith(lib_ext):
             s = os.path.join(src_build_dir, item)
-            d = os.path.join(dest_build_dir, item)
+
+            # Need to copy .dll right next to Cython extension for Windows
+            if system == "Windows":
+                d = os.path.join(HOME_DIR, item)
+                shutil.copy2(s, d)
+            else:
+                d = os.path.join(dest_build_dir, item)
+            
             shutil.copy2(s, d)
             files_copied += 1
     
     return files_copied
 
 
 # NOTE: To build Cython extension correctly, you must provide correct path to
 # the prebuilt llmodel C library. Specifically, the llmodel.h and C shared library are needed.
-copy_prebuilt_C_lib(SRC_CLIB_DIRECtORY, 
-                    SRC_CLIB_BUILD_DIRECTORY, 
-                    DEST_CLIB_DIRECTORY, 
+copy_prebuilt_C_lib(SRC_CLIB_DIRECtORY,
+                    SRC_CLIB_BUILD_DIRECTORY,
+                    DEST_CLIB_DIRECTORY,
                     DEST_CLIB_BUILD_DIRECTORY)
 
+def get_extra_link_args():
+    if system != "Windows":
+        return [f'-Wl,-rpath,{DEST_CLIB_BUILD_DIRECTORY}', f'-Wl,-rpath,{LIB_BUILD_DIR}']
+    else:
+        # no rpath option for Windows
+        return []
+
 llmodel_extension = Extension(
     name="gpt4all.pyllmodel",
     sources=["gpt4all/pyllmodel.pyx"],
     libraries=["llmodel"],
-    library_dirs=[DEST_CLIB_BUILD_DIRECTORY],
+    library_dirs=[DEST_CLIB_BUILD_DIRECTORY, LIB_BUILD_DIR, HOME_DIR],
     include_dirs=[DEST_CLIB_DIRECTORY],
-    extra_link_args=[f'-Wl,-rpath,{DEST_CLIB_BUILD_DIRECTORY}']
+    extra_link_args=get_extra_link_args()
 )
 
-# Create a data_files list to include the prebuilt C library files
-data_files = [
-    (os.path.join('share', package_name, 'lib'), [os.path.join(DEST_CLIB_BUILD_DIRECTORY, f'lib{LIB_NAME}.{lib_ext}')]),
-    (os.path.join('share', package_name, 'include'), [os.path.join(DEST_CLIB_DIRECTORY, f'{LIB_NAME}.h')]),
-]
-
 ext_modules = cythonize([llmodel_extension])
 
 setup(
     name=package_name,
-    version="0.1.4",
+    version="0.1.5",
     description="Python bindings for GPT4All",
     author="Richard Guo",
     author_email="richard@nomic.ai",
     url="https://pypi.org/project/gpt4all/",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
@@ -95,9 +109,10 @@
     ],
     python_requires='>=3.8',
     packages=find_packages(),
     install_requires=[
         "Cython==0.29.34",
         "pytest==7.3.1"],
     ext_modules=ext_modules,
-    data_files = data_files
+    package_data={'llmodel': [f"{DEST_CLIB_DIRECTORY}/*", f"{HOME_DIR}/*.dll"]},
+    include_package_data=True
 )
```

### Comparing `gpt4all-0.1.4/tests/test_gpt4all.py` & `gpt4all-0.1.5/tests/test_gpt4all.py`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.4/tests/test_pyllmodel.py` & `gpt4all-0.1.5/tests/test_pyllmodel.py`

 * *Files identical despite different names*

