# Comparing `tmp/safer-4.6.1.tar.gz` & `tmp/safer-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safer-4.6.1.tar", max compression
+gzip compressed data, was "safer-4.7.0.tar", max compression
```

## Comparing `safer-4.6.1.tar` & `safer-4.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-05-02 09:24:25.348741 safer-4.6.1/LICENSE
--rw-r--r--   0        0        0     4713 2023-05-02 09:24:25.349032 safer-4.6.1/README.md
--rw-r--r--   0        0        0      604 2023-05-02 11:02:19.297041 safer-4.6.1/pyproject.toml
--rw-r--r--   0        0        0    21471 2023-05-02 11:00:05.016093 safer-4.6.1/safer.py
--rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 safer-4.6.1/setup.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 safer-4.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-02 09:24:25.348741 safer-4.7.0/LICENSE
+-rw-r--r--   0        0        0     4713 2023-05-02 09:24:25.349032 safer-4.7.0/README.md
+-rw-r--r--   0        0        0      604 2023-05-05 08:41:09.854840 safer-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0    21475 2023-05-04 14:26:28.993404 safer-4.7.0/safer.py
+-rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 safer-4.7.0/setup.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 safer-4.7.0/PKG-INFO
```

### Comparing `safer-4.6.1/LICENSE` & `safer-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safer-4.6.1/README.md` & `safer-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `safer-4.6.1/pyproject.toml` & `safer-4.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 target-version = ['py37']
 
 [tool.doks]
 auto = true
 
 [tool.poetry]
 name = "safer"
-version = "4.6.1"
+version = "4.7.0"
 description = "🧿 A safer writer for files and streams 🧿"
 authors = ["Tom Ritchford <tom@swirly.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `safer-4.6.1/safer.py` & `safer-4.7.0/safer.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
   a function that prints to the stream.
 
 By default, `safer` buffers the written data in memory in a `io.StringIO`
 or `io.BytesIO`.
 
 For very large files, `safer.open()` has a `temp_file` argument which
 writes the data to a temporary file on disk, which is moved over using
-`os.rename` if the operation completes successfully.  This functionality
+`os.replace` if the operation completes successfully.  This functionality
 does not work on Windows.  (In fact, it's unclear if any of this works on
 Windows, but that certainly won't.  Windows developer solicted!)
 
 
 ### Example: `safer.writer()`
 
 `safer.writer()` wraps an existing stream - a writer, socket, or callback -
@@ -197,15 +197,15 @@
           If `is_binary` is ``None``, deduce whether it's a binary file from
           the stream, or assume it's text otherwise.
 
       close_on_exit: If True, the underlying stream is closed when the writer
         closes
 
       temp_file: If `temp_file` is truthy, write to a disk file and use
-          os.rename() at the end, otherwise cache the writes in memory.
+          os.replace() at the end, otherwise cache the writes in memory.
 
           If `temp_file` is a string, use it as the name of the temporary
           file, otherwise select one in the same directory as the target
           file, or in the system tempfile for streams that aren't files.
 
       chunk_size: Chunk size, in bytes for transfer data from the temporary
           file to the underlying stream.
@@ -319,15 +319,15 @@
     Args:
       make_parents: If true, create the parent directory of the file if needed
 
       delete_failures: If false, any temporary files created are not deleted
         if there is an exception.
 
       temp_file: If `temp_file` is truthy, write to a disk file and use
-          os.rename() at the end, otherwise cache the writes in memory.
+          os.replace() at the end, otherwise cache the writes in memory.
 
           If `temp_file` is a string, use it as the name of the temporary
           file, otherwise select one in the same directory as the target
           file, or in the system tempfile for streams that aren't files.
 
       dry_run:
          If dry_run is True, the file is not written to at all
@@ -639,15 +639,15 @@
 
     def _success(self):
         if not self.dry_run:
             if os.path.exists(self.target_file):
                 shutil.copymode(self.target_file, self.temp_file)
             else:
                 os.chmod(self.temp_file, 0o100644)
-            os.rename(self.temp_file, self.target_file)
+            os.replace(self.temp_file, self.target_file)
 
 
 class _StreamCloser(_Closer):
     def __init__(self, write, close_on_exit):
         self.write = write
         self.close_on_exit = close_on_exit
```

### Comparing `safer-4.6.1/setup.py` & `safer-4.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['safer']
 setup_kwargs = {
     'name': 'safer',
-    'version': '4.6.1',
+    'version': '4.7.0',
     'description': '🧿 A safer writer for files and streams 🧿',
     'long_description': "# 🧿 `safer`: A safer writer 🧿\n\nAvoid partial writes or corruption!\n\n`safer` wraps file streams, sockets, or a callable, and offers a drop-in\nreplacement for regular old `open()`.\n\n## Quick summary\n\n### A tiny example\n\n    import safer\n\n    with safer.open(filename, 'w') as fp:\n        fp.write('one')\n        print('two', file=fp)\n        raise ValueError\n        # filename was not written.\n\n\n### How to use\n\nUse [pip](https://pypi.org/project/pip) to install `safer` from the command\nline: `pip install safer`.\n\nTested on Python 3.4 - 3.11.  An old Python 2.7 version\nis [here](https://github.com/rec/safer/tree/v2.0.5).\n\nSee the Medium article [here](https://medium.com/@TomSwirly/%EF%B8%8F-safer-a-safer-file-writer-%EF%B8%8F-5fe267dbe3f5)\n\n### The details\n\n`safer` helps prevent programmer error from corrupting files, socket\nconnections, or generalized streams by writing a whole file or nothing.\n\nIt does not prevent concurrent modification of files from other threads or\nprocesses: if you need atomic file writing, see\nhttps://pypi.org/project/atomicwrites/\n\nIt also has a useful `dry_run` setting to let you test your code without\nactually overwriting the target file.\n\n* `safer.writer()` wraps an existing writer, socket or stream and writes a\n  whole response or nothing\n\n* `safer.open()` is a drop-in replacement for built-in `open` that\n  writes a whole file or nothing\n\n* `safer.closer()` returns a stream like from `safer.write()` that also\n  closes the underlying stream or callable when it closes.\n\n* `safer.dump()` is like a safer `json.dump()` which can be used for any\n  serialization protocol, including Yaml and Toml, and also allows you to\n  write to file streams or any other callable.\n\n* `safer.printer()` is `safer.open()` except that it yields a\n  a function that prints to the stream.\n\nBy default, `safer` buffers the written data in memory in a `io.StringIO`\nor `io.BytesIO`.\n\nFor very large files, `safer.open()` has a `temp_file` argument which\nwrites the data to a temporary file on disk, which is moved over using\n`os.rename` if the operation completes successfully.  This functionality\ndoes not work on Windows.  (In fact, it's unclear if any of this works on\nWindows, but that certainly won't.  Windows developer solicted!)\n\n\n### Example: `safer.writer()`\n\n`safer.writer()` wraps an existing stream - a writer, socket, or callback -\nin a temporary stream which is only copied to the target stream at close(), and\nonly if no exception was raised.\n\nSuppose `sock = socket.socket(*args)`.\n\nThe old, dangerous way goes like this.\n\n    try:\n        write_header(sock)\n        write_body(sock)   # Exception is thrown here\n        write_footer(sock)\n     except Exception:\n        write_error(sock)  # Oops, the header was already written\n\nWith `safer` you write all or nothing:\n\n    try:\n        with safer.writer(sock) as s:\n            write_header(s)\n            write_body(s)  # Exception is thrown here\n            write_footer(s)\n     except Exception:\n        write_error(sock)  # Nothing has been written\n\n### Example: `safer.open()` and json\n\n`safer.open()` is a a drop-in replacement for built-in `open()` except that\nwhen used as a context, it leaves the original file unchanged on failure.\n\nIt's easy to write broken JSON if something within it doesn't serialize.\n\n    with open(filename, 'w') as fp:\n        json.dump(data, fp)\n        # If an exception is raised, the file is empty or partly written\n\n`safer` prevents this:\n\n    with safer.open(filename, 'w') as fp:\n        json.dump(data, fp)\n        # If an exception is raised, the file is unchanged.\n\n`safer.open(filename)` returns a file stream `fp` like `open(filename)`\nwould, except that `fp` writes to memory stream or a temporary file in the\nsame directory.\n\nIf `fp` is used as a context manager and an exception is raised, then the\nproperty `fp.safer_failed` on the stream is automatically set to `True`.\n\nAnd when `fp.close()` is called, the cached data is stored in `filename` -\n*unless* `fp.safer_failed` is true.\n\n### Example: `safer.printer()`\n\n`safer.printer()` is similar to `safer.open()` except it yields a function\nthat prints to the open file - it's very convenient for printing text.\n\nLike `safer.open()`, if an exception is raised within its context manager,\nthe original file is left unchanged.\n\nBefore.\n\n    with open(file, 'w') as fp:\n        for item in items:\n            print(item, file=fp)\n        # Prints lines until the first exception\n\nWith `safer`\n\n    with safer.printer(file) as print:\n        for item in items:\n            print(item)\n        # Either the whole file is written, or nothing\n\n\n### [API Documentation](https://rec.github.io/safer#safer--api-documentation)\n",
     'author': 'Tom Ritchford',
     'author_email': 'tom@swirly.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `safer-4.6.1/PKG-INFO` & `safer-4.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safer
-Version: 4.6.1
+Version: 4.7.0
 Summary: 🧿 A safer writer for files and streams 🧿
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

