# Comparing `tmp/ndtiff-1.9.1.tar.gz` & `tmp/ndtiff-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtiff-1.9.1.tar", last modified: Mon Feb  6 21:29:19 2023, max compression
+gzip compressed data, was "ndtiff-2.0.0.tar", last modified: Fri May  5 18:40:50 2023, max compression
```

## Comparing `ndtiff-1.9.1.tar` & `ndtiff-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:19.118307 ndtiff-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-06 21:29:19.118307 ndtiff-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-06 21:29:08.000000 ndtiff-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:19.114307 ndtiff-1.9.1/ndtiff/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/_superclass.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    45349 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/nd_tiff_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    28496 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/nd_tiff_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45349 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/ndtiff_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:19.118307 ndtiff-1.9.1/ndtiff/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/test/data_loading_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:19.118307 ndtiff-1.9.1/ndtiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-06 21:29:08.000000 ndtiff-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 21:29:19.118307 ndtiff-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-06 21:29:08.000000 ndtiff-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:50.313797 ndtiff-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 18:40:50.313797 ndtiff-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-05 18:40:39.000000 ndtiff-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:50.313797 ndtiff-2.0.0/ndtiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/_superclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/nd_tiff_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28211 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/nd_tiff_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/ndtiff_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:50.313797 ndtiff-2.0.0/ndtiff/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/test/data_loading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-05 18:40:39.000000 ndtiff-2.0.0/ndtiff/test/test_custom_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:40:50.313797 ndtiff-2.0.0/ndtiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 18:40:50.000000 ndtiff-2.0.0/ndtiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 18:40:39.000000 ndtiff-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:40:50.313797 ndtiff-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-05 18:40:39.000000 ndtiff-2.0.0/setup.py
```

### Comparing `ndtiff-1.9.1/PKG-INFO` & `ndtiff-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 1.9.1
+Version: 2.0.0
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-1.9.1/ndtiff/nd_tiff_current.py` & `ndtiff-2.0.0/ndtiff/nd_tiff_current.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Library for reading NDTiff datasets
 """
 import os
-import mmap
 import numpy as np
 import sys
 import json
-import platform
 import dask.array as da
 import warnings
 import struct
 import threading
-import inspect
+from functools import partial
+from ndtiff.file_io import NDTiffFileIO, BUILTIN_FILE_IO
 
 _POSITION_AXIS = "position"
 _ROW_AXIS = "row"
 _COLUMN_AXIS = "column"
 _Z_AXIS = "z"
 _TIME_AXIS = "time"
 _CHANNEL_AXIS = "channel"
@@ -34,36 +33,41 @@
     else:
         return 3  # stack next to channel axes
 
 class _SingleNDTiffReader:
     """
     Class corresponsing to a single multipage tiff file
     Pass the full path of the TIFF to instantiate and call close() when finished
+
+
     """
 
     # file format constants
     SUMMARY_MD_HEADER = 2355492
     EIGHT_BIT_MONOCHROME = 0
     SIXTEEN_BIT_MONOCHROME = 1
     EIGHT_BIT_RGB = 2
     TEN_BIT_MONOCHROME = 3
     TWELVE_BIT_MONOCHROME = 4
     FOURTEEN_BIT_MONOCHROME = 5
+    ELEVEN_BIT_MONOCHROME = 6
 
     UNCOMPRESSED = 0
 
-    def __init__(self, tiff_path):
+    def __init__(self, tiff_path, file_io: NDTiffFileIO = BUILTIN_FILE_IO):
+        """
+        tiff_path: str
+            The path to a .tiff file to load
+        file_io: ndtiff.file_io.NDTiffFileIO
+            A container containing various methods for interacting with files.
+        """
+        self.file_io = file_io
         self.tiff_path = tiff_path
-        self.file = open(tiff_path, "rb")
-        if platform.system() == "Windows":
-            self.mmap_file = mmap.mmap(self.file.fileno(), 0, access=mmap.ACCESS_READ)
-        else:
-            self.mmap_file = mmap.mmap(self.file.fileno(), 0, prot=mmap.PROT_READ)
+        self.file = self.file_io.open(tiff_path, "rb")
         self.summary_md, self.first_ifd_offset = self._read_header()
-        self.mmap_file.close()
 
     def close(self):
         """ """
         self.file.close()
 
     def _read_header(self):
         """
@@ -87,15 +91,14 @@
         else:
             raise Exception("Endian type not specified correctly")
         if np.frombuffer(self._read(2,4), dtype=np.uint16)[0] != 42:
             raise Exception("Tiff magic 42 missing")
         first_ifd_offset = np.frombuffer(self._read(4,8), dtype=np.uint32)[0]
 
         # read custom stuff: header, summary md
-        # int.from_bytes(self.mmap_file[24:28], sys.byteorder) # should be equal to 483729 starting in version 1
         self.major_version = int.from_bytes(self._read(12, 16), sys.byteorder)
         self.minor_version = int.from_bytes(self._read(16, 20), sys.byteorder)
 
         summary_md_header, summary_md_length = np.frombuffer(self._read(20, 28), dtype=np.uint32)
         if summary_md_header != self.SUMMARY_MD_HEADER:
             raise Exception("Summary metadata header wrong")
         summary_md = json.loads(self._read(28, 28 + summary_md_length))
@@ -103,117 +106,105 @@
 
     def _read(self, start, end):
         """
         convert to python ints
         """
         self.file.seek(int(start), 0)
         return self.file.read(end - start)
-        # return self.np_memmap[int(start) : int(end)].tobytes()
 
     def read_metadata(self, index):
         return json.loads(
             self._read(
                 index["metadata_offset"], index["metadata_offset"] + index["metadata_length"]
             )
         )
 
-    def read_image(self, index, memmapped=False):
+    def read_image(self, index):
         if index["pixel_type"] == self.EIGHT_BIT_RGB:
             bytes_per_pixel = 3
             dtype = np.uint8
         elif index["pixel_type"] == self.EIGHT_BIT_MONOCHROME:
             bytes_per_pixel = 1
             dtype = np.uint8
         elif index["pixel_type"] == self.SIXTEEN_BIT_MONOCHROME or \
                 index["pixel_type"] == self.TEN_BIT_MONOCHROME or \
                 index["pixel_type"] == self.TWELVE_BIT_MONOCHROME or \
-                index["pixel_type"] == self.FOURTEEN_BIT_MONOCHROME:
+                index["pixel_type"] == self.FOURTEEN_BIT_MONOCHROME or \
+                index["pixel_type"] == self.ELEVEN_BIT_MONOCHROME:
             bytes_per_pixel = 2
             dtype = np.uint16
         else:
             raise Exception("unrecognized pixel type")
         width = index["image_width"]
         height = index["image_height"]
-
-        if memmapped:
-            np_memmap = np.memmap(self.file, dtype=np.uint8, mode="r")
-            image = np.reshape(
-                np_memmap[
-                    index["pixel_offset"] : index["pixel_offset"] + width * height * bytes_per_pixel
-                ].view(dtype),
-                [height, width, 3] if bytes_per_pixel == 3 else [height, width],
-            )
-        else:
-            image = np.reshape(
-                np.frombuffer(self._read(
-                index["pixel_offset"], index["pixel_offset"] + width * height * bytes_per_pixel)
-                    , dtype=dtype),
-                [height, width, 3] if bytes_per_pixel == 3 else [height, width],
-            )
+        image = np.reshape(
+            np.frombuffer(self._read(
+            index["pixel_offset"], index["pixel_offset"] + width * height * bytes_per_pixel)
+                , dtype=dtype),
+            [height, width, 3] if bytes_per_pixel == 3 else [height, width],
+        )
         return image
 
 class NDTiffDataset():
     """
     Class that opens a single NDTiff dataset
     """
 
-    def __init__(self, dataset_path=None, remote_storage_monitor=None, **kwargs):
+    def __init__(self, dataset_path=None, file_io: NDTiffFileIO = BUILTIN_FILE_IO, _summary_metadata=None,  **kwargs):
         """
         Provides access to an NDTiffStorage dataset,
         either one currently being acquired or one on disk
 
         Parameters
         ----------
         dataset_path : str
             Abosolute path of top level folder of a dataset on disk
-        remote_storage_monitor : JavaObjectShadow
-            Object that allows callbacks from remote NDTiffStorage. User's need not call this directly
+        file_io: ndtiff.file_io.NDTiffFileIO
+            A container containing various methods for interacting with files.
+        _summary_metadata : dict
+            Summary metadata for a dataset that is currently being acquired. Users shouldn't call this
         """
+        self.file_io = file_io
         # if it is in fact a pyramid, the parent class will handle this. I think this implies that
         # resolution levels cannot be opened seperately and expected to stitch correctly when there
         # is tile overlap
         self._full_resolution = False
         self._lock = threading.RLock()
-        if remote_storage_monitor is not None:
+        if _summary_metadata is not None:
             # this dataset is a view of an active acquisition. Image data is being written by code on the Java side
             self._new_image_arrived = False # used by custom (e.g. napari) viewer to check for updates. Will be reset to false by them
-            self._remote_storage_monitor = remote_storage_monitor
-            self.summary_metadata = self._remote_storage_monitor.get_summary_metadata()
-            if dataset_path is None:
-                self.path = remote_storage_monitor.get_disk_location()
-            else:
-                self.path = dataset_path #Overriden by pyramid storage class creating this
-            self.path += "" if self.path[-1] == os.sep else os.sep
             self.axes = {}
             self.axes_types = {}
             self.index = {}
             self._readers_by_filename = {}
+            self._summary_metadata = _summary_metadata
+            self.path = dataset_path
+            self.path += "" if self.path[-1] == os.sep else os.sep
             return
 
-        self._remote_storage_monitor = None
         self.path = dataset_path
         self.path += "" if self.path[-1] == os.sep else os.sep
         self.index = self.read_index(self.path)
         tiff_names = [
-            os.path.join(self.path, tiff) for tiff in os.listdir(self.path) if tiff.endswith(".tif")
+            self.file_io.path_join(self.path, tiff) for tiff in self.file_io.listdir(self.path) if tiff.endswith(".tif")
         ]
         self._readers_by_filename = {}
         self.summary_metadata = {}
         self.major_version, self.minor_version = (0, 0)
         # Count how many files need to be opened
         num_tiffs = 0
         count = 0
-        for file in os.listdir(self.path):
+        for file in self.file_io.listdir(self.path):
             if file.endswith(".tif"):
                 num_tiffs += 1
         # populate list of readers and tree mapping indices to readers
         for tiff in tiff_names:
             print("\rOpening file {} of {}...".format(count + 1, num_tiffs), end="")
             count += 1
-            new_reader = _SingleNDTiffReader(tiff)
+            new_reader = _SingleNDTiffReader(tiff, file_io=self.file_io)
             self._readers_by_filename[tiff.split(os.sep)[-1]] = new_reader
             # Should be the same on every file so resetting them is fine
             self.major_version, self.minor_version = new_reader.major_version, new_reader.minor_version
 
         if len(self._readers_by_filename) > 0:
             self.summary_metadata = list(self._readers_by_filename.values())[0].summary_md
 
@@ -283,15 +274,15 @@
     def has_image(
         self,
         channel=None,
         z=None,
         time=None,
         position=None,
         row=None,
-        col=None,
+        column=None,
         **kwargs
     ):
         """Check if this image is present in the dataset
 
         Parameters
         ----------
         channel : int or str
@@ -300,37 +291,36 @@
             index of z slice, if applicable (Default value = None)
         time : int
             index of the time point, if applicable (Default value = None)
         position : int
             index of the XY position, if applicable (Default value = None)
         row : int
             index of tile row for XY tiled datasets (Default value = None)
-        col : int
-            index of tile col for XY tiled datasets (Default value = None)
+        column : int
+            index of tile column for XY tiled datasets (Default value = None)
         **kwargs :
             names and integer positions of any other axes
 
         Returns
         -------
         bool :
             indicating whether the dataset has an image matching the specifications
         """
         with self._lock:
             return self._does_have_image(self._consolidate_axes(
-                channel, z, position, time, row, col, **kwargs))
+                channel, z, position, time, row, column, **kwargs))
 
     def read_image(
         self,
         channel=None,
         z=None,
         time=None,
         position=None,
         row=None,
-        col=None,
-        memmapped=False,
+        column=None,
         **kwargs
     ):
         """
         Read image data as numpy array
 
         Parameters
         ----------
@@ -340,40 +330,38 @@
             index of z slice, if applicable (Default value = None)
         time : int
             index of the time point, if applicable (Default value = None)
         position : int
             index of the XY position, if applicable (Default value = None)
         row : int
             index of tile row for XY tiled datasets (Default value = None)
-        col : int
-            index of tile col for XY tiled datasets (Default value = None)
-        memmapped : bool
-             (Default value = False)
+        column : int
+            index of tile column for XY tiled datasets (Default value = None)
         **kwargs :
             names and integer positions of any other axes
 
         Returns
         -------
         image : numpy array or tuple
             image as a 2D numpy array, or tuple with image and image metadata as dict
 
         """
         with self._lock:
-            axes = self._consolidate_axes(channel, z, position, time, row, col, **kwargs )
+            axes = self._consolidate_axes(channel, z, position, time, row, column, **kwargs )
 
-            return self._do_read_image(axes, memmapped)
+            return self._do_read_image(axes)
 
     def read_metadata(
         self,
         channel=None,
         z=None,
         time=None,
         position=None,
         row=None,
-        col=None,
+        column=None,
         **kwargs
     ):
         """
         Read metadata only. Faster than using read_image to retrieve metadata
 
         Parameters
         ----------
@@ -383,28 +371,28 @@
             index of z slice, if applicable (Default value = None)
         time : int
             index of the time point, if applicable (Default value = None)
         position : int
             index of the XY position, if applicable (Default value = None)
         row : int
             index of tile row for XY tiled datasets (Default value = None)
-        col : int
+        column : int
             index of tile col for XY tiled datasets (Default value = None)
 
         **kwargs :
             names and integer positions of any other axes
 
         Returns
         -------
         metadata : dict
 
         """
         with self._lock:
             axes = self._consolidate_axes(
-                channel, z, position, time, row, col, **kwargs
+                channel, z, position, time, row, column, **kwargs
             )
 
             return self._do_read_metadata(axes)
 
 
 
     def get_index_keys(self):
@@ -421,15 +409,15 @@
         This is used to get access to a dataset that is currently being
         written by java side
         """
         with self._lock:
             _, axes, index_entry = self._read_single_index_entry(data, self.index)
 
             if index_entry["filename"] not in self._readers_by_filename:
-                new_reader = _SingleNDTiffReader(self.path + index_entry["filename"] )
+                new_reader = _SingleNDTiffReader(self.path + index_entry["filename"], file_io=self.file_io)
                 self._readers_by_filename[index_entry["filename"]] = new_reader
                 # Should be the same on every file so resetting them is fine
                 self.major_version, self.minor_version = new_reader.major_version, new_reader.minor_version
 
 
             # update the axes that have been seen
             for axis_name in axes.keys():
@@ -444,25 +432,25 @@
 
         if not hasattr(self, 'image_width'):
             self._parse_first_index(index_entry)
 
         return axes
 
     def _consolidate_axes(self, channel: int or str, z: int, position: int,
-                          time: int, row: int, col: int, **kwargs):
+                          time: int, row: int, column: int, **kwargs):
         """
         Pack axes into a convenient format
         """
         if ('channel_name' in kwargs):
             warnings.warn('channel_name is deprecated, use "channel" instead')
             channel = kwargs['channel_name']
             del kwargs['channel_name']
 
         axis_positions = {'channel': channel, 'z': z, 'position': position,
-                    'time': time, 'row': row, 'col': col, **kwargs}
+                    'time': time, 'row': row, 'column': column, **kwargs}
         # ignore ones that are None
         axis_positions = {n: axis_positions[n] for n in axis_positions.keys() if axis_positions[n] is not None}
         for axis_name in axis_positions.keys():
             # convert any string-valued axes passed as ints into strings
             if self.axes_types[axis_name] == str and type(axis_positions[axis_name]) == int:
                 axis_positions[axis_name] = self._string_axes_values[axis_name][axis_positions[axis_name]]
 
@@ -515,60 +503,22 @@
             self.dtype = np.uint8
         elif first_index["pixel_type"] == _SingleNDTiffReader.EIGHT_BIT_MONOCHROME:
             self.bytes_per_pixel = 1
             self.dtype = np.uint8
         elif first_index["pixel_type"] == _SingleNDTiffReader.SIXTEEN_BIT_MONOCHROME or \
                 first_index["pixel_type"] == _SingleNDTiffReader.FOURTEEN_BIT_MONOCHROME or \
                 first_index["pixel_type"] == _SingleNDTiffReader.TWELVE_BIT_MONOCHROME or \
-                first_index["pixel_type"] == _SingleNDTiffReader.TEN_BIT_MONOCHROME:
+                first_index["pixel_type"] == _SingleNDTiffReader.TEN_BIT_MONOCHROME or \
+                first_index["pixel_type"] == _SingleNDTiffReader.ELEVEN_BIT_MONOCHROME:
             self.bytes_per_pixel = 2
             self.dtype = np.uint16
 
         self.image_width = first_index["image_width"]
         self.image_height = first_index["image_height"]
 
-
-    def _add_storage_monitor_fn(self, acquisition, storage_monitor_fn, callback_fn=None, debug=False):
-        """
-        Add a callback function that gets called whenever a new image is writtern to disk (for acquisitions in
-        progress only)
-
-        Parameters
-        ----------
-        callback_fn : Callable
-            callable with that takes 1 argument, the axes dict of the image just written
-        """
-        if self._remote_storage_monitor is None:
-            raise Exception("Only valid for datasets with writing in progress")
-
-        connected_event = threading.Event()
-
-        push_port = self._remote_storage_monitor.get_port()
-        monitor_thread = threading.Thread(
-            target=storage_monitor_fn,
-            args=(
-                acquisition,
-                self,
-                push_port,
-                connected_event,
-                callback_fn,
-                debug,
-            ),
-            name="ImageSavedCallbackThread",
-        )
-
-        monitor_thread.start()
-
-        # Wait for pulling to start before you signal for pushing to start
-        connected_event.wait()  # wait for push/pull sockets to connect
-
-        # start pushing out all the image written events (including ones that have already accumulated)
-        self._remote_storage_monitor.start()
-        return monitor_thread
-
     def _does_have_image(self, axes):
         key = frozenset(axes.items())
         return key in self.index
 
     def _read_single_index_entry(self, data, entries, position=0):
         index_entry = {}
         (axes_length,) = struct.unpack("I", data[position : position + 4])
@@ -597,15 +547,15 @@
         ) = struct.unpack("IIIIIIII", data[position : position + 32])
         position += 32
         entries[frozenset(axes.items())] = index_entry
         return position, axes, index_entry
 
     def read_index(self, path):
         print("\rReading index...          ", end="")
-        with open(path + os.sep + "NDTiff.index", "rb") as index_file:
+        with self.file_io.open(path + os.sep + "NDTiff.index", "rb") as index_file:
             data = index_file.read()
         entries = {}
         position = 0
         while position < len(data):
             print(
                 "\rReading index... {:.1f}%       ".format(
                     100 * (1 - (len(data) - position) / len(data))
@@ -621,23 +571,22 @@
 
         print("\rFinshed reading index          ", end="")
         return entries
 
     def _do_read_image(
         self,
         axes,
-        memmapped=False,
     ):
         # determine which reader contains the image
         key = frozenset(axes.items())
         if key not in self.index:
             raise Exception("image with keys {} not present in data set".format(key))
         index = self.index[key]
         reader = self._readers_by_filename[index["filename"]]
-        return reader.read_image(index, memmapped)
+        return reader.read_image(index)
 
     def _do_read_metadata(self, axes):
         """
 
         Parameters
         ----------
         axes : dict
@@ -653,14 +602,57 @@
         reader = self._readers_by_filename[index["filename"]]
         return reader.read_metadata(index)
 
     def close(self):
         for reader in self._readers_by_filename.values():
             reader.close()
 
+    def _read_one_image(self, block_id, axes_to_stack=None, axes_to_slice=None, stitched=False, rgb=False):
+        # a function that reads in one chunk of data
+        axes = {key: block_id[i] for i, key in enumerate(axes_to_stack.keys())}
+        if stitched:
+            # Combine all rows and cols into one stitched image
+            # get spatial layout of position indices
+            row_values = np.array(list(self.axes["row"]))
+            column_values = np.array(list(self.axes["column"]))
+            # fill in missing values
+            row_values = np.arange(np.min(row_values), np.max(row_values) + 1)
+            column_values = np.arange(np.min(column_values), np.max(column_values) + 1)
+            # make nested list of rows and columns
+            blocks = []
+            for row in row_values:
+                blocks.append([])
+                for column in column_values:
+                    # remove overlap between tiles
+                    if not self.has_image(**axes, **axes_to_slice, row=row, column=column):
+                        blocks[-1].append(self._empty_tile)
+                    else:
+                        tile = self.read_image(**axes, **axes_to_slice, row=row, column=column)
+                        # remove half of the overlap around each tile so that that image stitches correctly
+                        # only need this for full resoution because downsampled ones already have the edges removed
+                        if np.any(self.overlap[0] > 0) and self._full_resolution:
+                            min_index = np.floor(self.overlap / 2).astype(np.int_)
+                            max_index = np.ceil(self.overlap / 2).astype(np.int_)
+                            tile = tile[min_index[0]:-max_index[0], min_index[1]:-max_index[1]]
+                        blocks[-1].append(tile)
+
+            if rgb:
+                image = np.concatenate([np.concatenate(row, axis=len(blocks[0][0].shape) - 2)
+                        for row in blocks],  axis=0)
+            else:
+                image = np.array(da.block(blocks))
+        else:
+            if not self.has_image(**axes, **axes_to_slice):
+                image = self._empty_tile
+            else:
+                image = self.read_image(**axes, **axes_to_slice)
+        for i in range(len(axes_to_stack.keys())):
+            image = image[None]
+        return image
+
     def as_array(self, axes=None, stitched=False, **kwargs):
         """
         Read all data image data as one big Dask array with last two axes as y, x and preceeding axes depending on data.
         The dask array is made up of memory-mapped numpy arrays, so the dataset does not need to be able to fit into RAM.
         If the data doesn't fully fill out the array (e.g. not every z-slice collected at every time point), zeros will
         be added automatically.
 
@@ -707,137 +699,94 @@
             if 'column' in axes_to_stack:
                 del axes_to_stack['column']
             if 'row' in axes_to_slice:
                 del axes_to_slice['row']
             if 'column' in axes_to_slice:
                 del axes_to_slice['column']
 
-        def read_one_image(block_id, axes_to_stack=axes_to_stack, axes_to_slice=axes_to_slice):
-            # a function that reads in one chunk of data
-            axes = {key: block_id[i] for i, key in enumerate(axes_to_stack.keys())}
-            if stitched:
-                # Combine all rows and cols into one stitched image
-                # get spatial layout of position indices
-                row_values = np.array(list(self.axes["row"]))
-                column_values = np.array(list(self.axes["column"]))
-                # fill in missing values
-                row_values = np.arange(np.min(row_values), np.max(row_values) + 1)
-                column_values = np.arange(np.min(column_values), np.max(column_values) + 1)
-                # make nested list of rows and columns
-                blocks = []
-                for row in row_values:
-                    blocks.append([])
-                    for column in column_values:
-                        # remove overlap between tiles
-                        if not self.has_image(**axes, **axes_to_slice, row=row, column=column):
-                            blocks[-1].append(self._empty_tile)
-                        else:
-                            tile = self.read_image(**axes, **axes_to_slice, row=row, column=column, memmapped=True)
-                            # remove half of the overlap around each tile so that that image stitches correctly
-                            # only need this for full resoution because downsampled ones already have the edges removed
-                            if np.any(self.overlap[0] > 0) and self._full_resolution:
-                                min_index = np.floor(self.overlap / 2).astype(np.int_)
-                                max_index = np.ceil(self.overlap / 2).astype(np.int_)
-                                tile = tile[min_index[0]:-max_index[0], min_index[1]:-max_index[1]]
-                            blocks[-1].append(tile)
-
-                if rgb:
-                    image = np.concatenate([np.concatenate(row, axis=len(blocks[0][0].shape) - 2)
-                            for row in blocks],  axis=0)
-                else:
-                    image = np.array(da.block(blocks))
-            else:
-                if not self.has_image(**axes, **axes_to_slice):
-                    image = self._empty_tile
-                else:
-                    image = self.read_image(**axes, **axes_to_slice)
-            for i in range(len(axes_to_stack.keys())):
-                image = image[None]
-            return image
-
-
         chunks = tuple([(1,) * len(axes_to_stack[axis]) for axis in axes_to_stack.keys()])
         if stitched:
             row_values = np.array(list(self.axes["row"]))
             column_values = np.array(list(self.axes["column"]))
             chunks += (h * (np.max(row_values) - np.min(row_values) + 1),
                        w * (np.max(column_values) - np.min(column_values) + 1))
         else:
-            chunks += (w, h)
+            chunks += (h, w)
         if rgb:
             chunks += (3,)
 
         array = da.map_blocks(
-            read_one_image,
+            partial(self._read_one_image, axes_to_stack=axes_to_stack, axes_to_slice=axes_to_slice, stitched=stitched, rgb=rgb),
             dtype=self.dtype,
             chunks=chunks,
             meta=self._empty_tile
         )
 
         return array
 
 
 class NDTiffPyramidDataset():
     """Class that opens a single NDTiffStorage multi-resolution pyramid dataset"""
 
-    def __init__(self, dataset_path=None, remote_storage_monitor=None):
+    def __init__(self, dataset_path=None, file_io: NDTiffFileIO = BUILTIN_FILE_IO, _summary_metadata=None):
         """
         Provides access to a NDTiffStorage pyramid dataset,
         either one currently being acquired or one on disk
 
         Parameters
         ----------
         dataset_path : str
             Abosolute path of top level folder of a dataset on disk
-        remote_storage_monitor : JavaObjectShadow
-            Object that allows callbacks from remote NDTiffStorage. Users need not call this directly
+        file_io: ndtiff.file_io.NDTiffFileIO
+            A container containing various methods for interacting with files.
+        _summary_metadata : dict
+            Summary metadata, only not None for in progress datasets. Users need not call directly
         """
+        self.file_io = file_io
         self._lock = threading.RLock()
-        if remote_storage_monitor is not None:
-            self._remote_storage_monitor = None # It belongs to the full resolution subclass
+        if _summary_metadata is not None:
             # this dataset is a view of an active acquisition. The storage exists on the java side
-            self.path = remote_storage_monitor.get_disk_location()
+            self.path = dataset_path
             self.path += "" if self.path[-1] == os.sep else os.sep
+            self.summary_metadata = _summary_metadata
 
             with self._lock:
-                full_res = NDTiffDataset(remote_storage_monitor=remote_storage_monitor,
-                                     dataset_path=self.path + "Full resolution" + os.sep)
+                full_res = NDTiffDataset(dataset_path=self.path + "Full resolution" + os.sep,
+                                         _summary_metadata=_summary_metadata, file_io=file_io)
                 self.res_levels = {0: full_res}
                 full_res._full_resolution = True
             # No information related higher res levels when remote storage monitoring right now
 
             #Copy stuff from the full res class for convenience
-            self.summary_metadata = self.res_levels[0].summary_metadata
             self.axes = self.res_levels[0].axes
 
             self.overlap = (np.array([self.summary_metadata["GridPixelOverlapY"],
                                         self.summary_metadata["GridPixelOverlapX"] ]))
             self.res_levels[0].overlap = self.overlap
             # TODO maybe open other resoutions here too
             return
 
         # Loading from disk
-        self._remote_storage_monitor = None
         self.path = dataset_path
         self.path += "" if self.path[-1] == os.sep else os.sep
         res_dirs = [
-            dI for dI in os.listdir(dataset_path) if os.path.isdir(os.path.join(dataset_path, dI))
+            dI for dI in self.file_io.listdir(dataset_path) if self.file_io.isdir(self.file_io.path_join(dataset_path, dI))
         ]
         # map from downsample factor to dataset
         with self._lock:
             self.res_levels = {}
         if "Full resolution" not in res_dirs:
             #Probably won't happen because this was already checked for
             raise Exception(
                 "Couldn't find full resolution directory. Is this the correct path to a dataset?"
             )
 
         for res_dir in res_dirs:
-            res_dir_path = os.path.join(dataset_path, res_dir)
-            res_level = NDTiffDataset(dataset_path=res_dir_path)
+            res_dir_path = self.file_io.path_join(dataset_path, res_dir)
+            res_level = NDTiffDataset(dataset_path=res_dir_path, file_io=self.file_io)
             if res_dir == "Full resolution":
                 with self._lock:
                     self.res_levels[0] = res_level
                 res_level._full_resolution = True
                 # get summary metadata and index tree from full resolution image
                 self.summary_metadata = res_level.summary_metadata
 
@@ -955,38 +904,35 @@
 
     def has_image(
         self,
         channel=None,
         z=None,
         time=None,
         position=None,
-        channel_name=None,
         resolution_level=0,
         row=None,
-        col=None,
+        column=None,
         **kwargs
     ):
         """Check if this image is present in the dataset
 
         Parameters
         ----------
         channel : int
             index of the channel, if applicable (Default value = None)
         z : int
             index of z slice, if applicable (Default value = None)
         time : int
             index of the time point, if applicable (Default value = None)
         position : int
             index of the XY position, if applicable (Default value = None)
-        channel_name : str
-            Name of the channel. Overrides channel index if supplied (Default value = None)
         row : int
             index of tile row for XY tiled datasets (Default value = None)
-        col : int
-            index of tile col for XY tiled datasets (Default value = None)
+        column : int
+            index of tile column for XY tiled datasets (Default value = None)
         resolution_level :
             0 is full resolution, otherwise represents downampling of pixels
             at 2 ** (resolution_level) (Default value = 0)
         **kwargs :
             names and integer positions of any other axes
 
         Returns
@@ -996,31 +942,28 @@
         """
         with self._lock:
             return self.res_levels[resolution_level].has_image(
                 channel=channel,
                 z=z,
                 time=time,
                 position=position,
-                channel_name=channel_name,
                 row=row,
-                col=col,
+                column=column,
                 **kwargs
             )
 
     def read_image(
         self,
         channel=None,
         z=None,
         time=None,
         position=None,
         row=None,
-        col=None,
-        channel_name=None,
+        column=None,
         resolution_level=0,
-        memmapped=False,
         **kwargs
     ):
         """
         Read image data as numpy array
 
         Parameters
         ----------
@@ -1028,25 +971,21 @@
             index of the channel, if applicable (Default value = None)
         z : int
             index of z slice, if applicable (Default value = None)
         time : int
             index of the time point, if applicable (Default value = None)
         position : int
             index of the XY position, if applicable (Default value = None)
-        channel_name :
-            Name of the channel. Overrides channel index if supplied (Default value = None)
         row : int
             index of tile row for XY tiled datasets (Default value = None)
-        col : int
+        column : int
             index of tile col for XY tiled datasets (Default value = None)
         resolution_level :
             0 is full resolution, otherwise represents downampling of pixels
             at 2 ** (resolution_level) (Default value = 0)
-        memmapped : bool
-             (Default value = False)
         **kwargs :
             names and integer positions of any other axes
 
         Returns
         -------
         image : numpy array or tuple
             image as a 2D numpy array, or tuple with image and image metadata as dict
@@ -1054,28 +993,25 @@
         """
         with self._lock:
             return self.res_levels[resolution_level].read_image(channel=channel,
                     z=z,
                     time=time,
                     position=position,
                     row=row,
-                    col=col,
-                    channel_name=channel_name,
-                    memmapped=memmapped,
+                    column=column,
                     **kwargs)
 
     def read_metadata(
         self,
         channel=None,
         z=None,
         time=None,
         position=None,
-        channel_name=None,
         row=None,
-        col=None,
+        column=None,
         resolution_level=0,
         **kwargs
     ):
         """
         Read metadata only. Faster than using read_image to retrieve metadata
 
         Parameters
@@ -1084,19 +1020,17 @@
             index of the channel, if applicable (Default value = None)
         z : int
             index of z slice, if applicable (Default value = None)
         time : int
             index of the time point, if applicable (Default value = None)
         position : int
             index of the XY position, if applicable (Default value = None)
-        channel_name :
-            Name of the channel. Overrides channel index if supplied (Default value = None)
         row : int
             index of tile row for XY tiled datasets (Default value = None)
-        col : int
+        column : int
             index of tile col for XY tiled datasets (Default value = None)
         resolution_level :
             0 is full resolution, otherwise represents downampling of pixels
             at 2 ** (resolution_level) (Default value = 0)
         **kwargs :
             names and integer positions of any other axes
 
@@ -1107,24 +1041,18 @@
         """
         with self._lock:
             return self.res_levels[resolution_level].read_metadata(
                     channel=channel,
                     z=z,
                     time=time,
                     position=position,
-                    channel_name=channel_name,
                     row=row,
-                    col=col,
+                    column=column,
                     **kwargs)
 
-    # TODO: this needs to be cleaned up probably--seems like this functionality belongs in pycromanager
-    def _add_storage_monitor_fn(self, acquisition, storage_monitor_fn, callback_fn=None, debug=False):
-        # Only valid for the full res data
-        return self.res_levels[0]._add_storage_monitor_fn(acquisition, storage_monitor_fn, callback_fn, debug)
-
     def _add_index_entry(self, index_entry):
         # Pass through to full res data
         return self.res_levels[0]._add_index_entry(index_entry)
 
     def close(self):
         with self._lock:
             for res_level in self.res_levels:
```

### Comparing `ndtiff-1.9.1/ndtiff/nd_tiff_v2.py` & `ndtiff-2.0.0/ndtiff/nd_tiff_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """ 
 Library for reading multiresolution micro-magellan
 """
 import os
-import mmap
 import numpy as np
 import sys
 import json
-import platform
 import dask.array as da
 import warnings
 import struct
 import threading
-
+from ndtiff.file_io import NDTiffFileIO, BUILTIN_FILE_IO
 
 class _MultipageTiffReader:
     """
     Class corresponsing to a single multipage tiff file in a Micro-Magellan dataset.
     Pass the full path of the TIFF to instantiate and call close() when finished
     """
 
     # file format constants
     SUMMARY_MD_HEADER = 2355492
     EIGHT_BIT = 0
     SIXTEEN_BIT = 1
     EIGHT_BIT_RGB = 2
     UNCOMPRESSED = 0
 
-    def __init__(self, tiff_path):
+    def __init__(self, tiff_path, file_io: NDTiffFileIO = BUILTIN_FILE_IO):
+        """
+        tiff_path: str
+            The path to a .tiff file to load
+        file_io: ndtiff.file_io.NDTiffFileIO
+            A container containing various methods for interacting with files.
+        """
+        self.file_io = file_io
         self.tiff_path = tiff_path
-        self.file = open(tiff_path, "rb")
-        if platform.system() == "Windows":
-            self.mmap_file = mmap.mmap(self.file.fileno(), 0, access=mmap.ACCESS_READ)
-        else:
-            self.mmap_file = mmap.mmap(self.file.fileno(), 0, prot=mmap.PROT_READ)
+        self.file = self.file_io.open(tiff_path, "rb")
         self.summary_md, self.first_ifd_offset = self._read_header()
-        self.mmap_file.close()
 
     def close(self):
         """ """
         self.file.close()
 
     def _read_header(self):
         """
@@ -62,15 +62,14 @@
         else:
             raise Exception("Endian type not specified correctly")
         if np.frombuffer(self._read(2,4), dtype=np.uint16)[0] != 42:
             raise Exception("Tiff magic 42 missing")
         first_ifd_offset = np.frombuffer(self._read(4,8), dtype=np.uint32)[0]
 
         # read custom stuff: header, summary md
-        # int.from_bytes(self.mmap_file[24:28], sys.byteorder) # should be equal to 483729 starting in version 1
         self._major_version = int.from_bytes(self._read(12,16), sys.byteorder)
 
         summary_md_header, summary_md_length = np.frombuffer(self._read(16,24), dtype=np.uint32)
         if summary_md_header != self.SUMMARY_MD_HEADER:
             raise Exception("Summary metadata header wrong")
         summary_md = json.loads(self._read(24, 24 + summary_md_length))
         return summary_md, first_ifd_offset
@@ -83,84 +82,75 @@
     
     def _read(self, start, end):
         """
         convert to python ints
         """
         self.file.seek(int(start), 0)
         return self.file.read(end - start)
-        # return self.np_memmap[int(start) : int(end)].tobytes()
 
     def read_metadata(self, index):
         return json.loads(
             self._read(
                 index["metadata_offset"], index["metadata_offset"] + index["metadata_length"]
             )
         )
 
-    def read_image(self, index, memmapped=False):
+    def read_image(self, index):
         if index["pixel_type"] == self.EIGHT_BIT_RGB:
             bytes_per_pixel = 3
             dtype = np.uint8
         elif index["pixel_type"] == self.EIGHT_BIT:
             bytes_per_pixel = 1
             dtype = np.uint8
         elif index["pixel_type"] == self.SIXTEEN_BIT:
             bytes_per_pixel = 2
             dtype = np.uint16
         else:
             raise Exception("unrecognized pixel type")
         width = index["image_width"]
         height = index["image_height"]
 
-        if memmapped:
-            np_memmap = np.memmap(self.file, dtype=np.uint8, mode="r")
-            image = np.reshape(
-                np_memmap[
-                    index["pixel_offset"] : index["pixel_offset"] + width * height * bytes_per_pixel
-                ].view(dtype),
-                [height, width, 3] if bytes_per_pixel == 3 else [height, width],
-            )
-        else:
-            image = np.reshape(
-                np.frombuffer(self._read(
-                index["pixel_offset"], index["pixel_offset"] + width * height * bytes_per_pixel)
-                    , dtype=dtype),
-                [height, width, 3] if bytes_per_pixel == 3 else [height, width],
-            )
+        image = np.reshape(
+            np.frombuffer(self._read(
+            index["pixel_offset"], index["pixel_offset"] + width * height * bytes_per_pixel)
+                , dtype=dtype),
+            [height, width, 3] if bytes_per_pixel == 3 else [height, width],
+        )
         return image
 
 
 class _ResolutionLevel:
-    def __init__(self, path=None, count=None, max_count=None, remote=False, summary_metadata=False):
+    def __init__(self, path=None, count=None, max_count=None, remote=False, summary_metadata=False, file_io: NDTiffFileIO = BUILTIN_FILE_IO):
         """
         Open all tiff files in directory, keep them in a list, and a tree based on image indices
 
         Parameters
         ----------
         path : str
         count : int
         max_count : int
 
         """
+        self.file_io = file_io
         self.path_root = path + ("" if path[-1] == os.sep else os.sep)
         if remote:
             self.summary_metadata = summary_metadata
             self.index = {}
             self._readers_by_filename = {}
         else:
             self.index = self.read_index(path)
             tiff_names = [
-                os.path.join(path, tiff) for tiff in os.listdir(path) if tiff.endswith(".tif")
+                self.file_io.path_join(path, tiff) for tiff in self.file_io.listdir(path) if tiff.endswith(".tif")
             ]
             self._readers_by_filename = {}
             # populate list of readers and tree mapping indices to readers
             for tiff in tiff_names:
                 print("\rOpening file {} of {}...".format(count + 1, max_count), end="")
                 count += 1
-                self._readers_by_filename[tiff.split(os.sep)[-1]] = _MultipageTiffReader(tiff)
+                self._readers_by_filename[tiff.split(os.sep)[-1]] = _MultipageTiffReader(tiff, file_io=self.file_io)
             self.summary_metadata = list(self._readers_by_filename.values())[0].summary_md
 
     def has_image(self, axes):
         key = frozenset(axes.items())
         return key in self.index
 
     def add_index_entry(self, data):
@@ -168,15 +158,15 @@
         Manually add a single index entry
         :param data: bytes object of a single index entry
         """
         _, axes, index_entry = self.read_single_index_entry(data, self.index)
 
         if index_entry["filename"] not in self._readers_by_filename:
             self._readers_by_filename[index_entry["filename"]] = _MultipageTiffReader(
-                self.path_root + index_entry["filename"]
+                self.path_root + index_entry["filename"], file_io=self.file_io
             )
         return axes, index_entry
 
     def read_single_index_entry(self, data, entries, position=0):
         index_entry = {}
         (axes_length,) = struct.unpack("I", data[position : position + 4])
         if axes_length == 0:
@@ -204,15 +194,15 @@
         ) = struct.unpack("IIIIIIII", data[position : position + 32])
         position += 32
         entries[frozenset(axes.items())] = index_entry
         return position, axes, index_entry
 
     def read_index(self, path):
         print("\rReading index...          ", end="")
-        with open(path + os.sep + "NDTiff.index", "rb") as index_file:
+        with self.file_io.open(path + os.sep + "NDTiff.index", "rb") as index_file:
             data = index_file.read()
         entries = {}
         position = 0
         while position < len(data):
             print(
                 "\rReading index... {:.1f}%       ".format(
                     100 * (1 - (len(data) - position) / len(data))
@@ -228,35 +218,32 @@
 
         print("\rFinshed reading index          ", end="")
         return entries
 
     def read_image(
         self,
         axes,
-        memmapped=False,
     ):
         """
 
         Parameters
         ----------
         axes : dict
-        memmapped : bool
-             (Default value = False)
 
         Returns
         -------
         image :
         """
         # determine which reader contains the image
         key = frozenset(axes.items())
         if key not in self.index:
             raise Exception("image with keys {} not present in data set".format(key))
         index = self.index[key]
         reader = self._readers_by_filename[index["filename"]]
-        return reader.read_image(index, memmapped)
+        return reader.read_image(index)
 
     def read_metadata(self, axes):
         """
 
         Parameters
         ----------
         axes : dict
@@ -286,27 +273,30 @@
     _POSITION_AXIS = "position"
     _ROW_AXIS = "row"
     _COLUMN_AXIS = "column"
     _Z_AXIS = "z"
     _TIME_AXIS = "time"
     _CHANNEL_AXIS = "channel"
 
-    def __init__(self, dataset_path=None, full_res_only=True, remote_storage_monitor=None):
+    def __init__(self, dataset_path=None, full_res_only=True, remote_storage_monitor=None, file_io: NDTiffFileIO = BUILTIN_FILE_IO):
         """
         Creat a Object providing access to and NDTiffStorage dataset, either one currently being acquired or one on disk
 
         Parameters
         ----------
         dataset_path : str
             Abosolute path of top level folder of a dataset on disk
         full_res_only : bool
             One open the full resolution data, if it is multi-res
         remote_storage_monitor : JavaObjectShadow
             Object that allows callbacks from remote NDTiffStorage
+        file_io: ndtiff.file_io.NDTiffFileIO
+            A container containing various methods for interacting with files.
         """
+        self.file_io = file_io
         self._tile_width = None
         self._tile_height = None
         self._lock = threading.Lock()
         if remote_storage_monitor is not None:
             # this dataset is a view of an active acquisiiton. The storage exists on the java side
             self.new_image_arrived = False # used by napari viewer to check for updates. Will be reset to false by them
             self._remote_storage_monitor = remote_storage_monitor
@@ -321,44 +311,45 @@
 
             dataset_path = remote_storage_monitor.get_disk_location()
             dataset_path += "" if dataset_path[-1] == os.sep else os.sep
             full_res_path = dataset_path + "Full resolution"
             with self._lock:
                 self.res_levels = {
                     0: _ResolutionLevel(
-                        remote=True, summary_metadata=self.summary_metadata, path=full_res_path
+                        remote=True, summary_metadata=self.summary_metadata, path=full_res_path,
+                        file_io=self.file_io
                     )
                 }
             self.axes = {}
             return
         else:
             self._remote_storage_monitor = None
 
         self.path = dataset_path
         res_dirs = [
-            dI for dI in os.listdir(dataset_path) if os.path.isdir(os.path.join(dataset_path, dI))
+            dI for dI in self.file_io.listdir(dataset_path) if self.file_io.isdir(self.file_io.path_join(dataset_path, dI))
         ]
         # map from downsample factor to datset
         with self._lock:
             self.res_levels = {}
         if "Full resolution" not in res_dirs:
             raise Exception(
                 "Couldn't find full resolution directory. Is this the correct path to a dataset?"
             )
         num_tiffs = 0
         count = 0
         for res_dir in res_dirs:
-            for file in os.listdir(os.path.join(dataset_path, res_dir)):
+            for file in self.file_io.listdir(self.file_io.path_join(dataset_path, res_dir)):
                 if file.endswith(".tif"):
                     num_tiffs += 1
         for res_dir in res_dirs:
             if full_res_only and res_dir != "Full resolution":
                 continue
-            res_dir_path = os.path.join(dataset_path, res_dir)
-            res_level = _ResolutionLevel(res_dir_path, count, num_tiffs)
+            res_dir_path = self.file_io.path_join(dataset_path, res_dir)
+            res_level = _ResolutionLevel(res_dir_path, count, num_tiffs, file_io=self.file_io)
             if res_dir == "Full resolution":
                 with self._lock:
                     self.res_levels[0] = res_level
                 # get summary metadata and index tree from full resolution image
                 self.summary_metadata = res_level.summary_metadata
 
                 self.overlap = (
@@ -527,15 +518,15 @@
                 for row in row_values:
                     blocks.append([])
                     for column in column_values:
                         #remove overlap between tiles
                         if not self.has_image(**axes, **axes_to_slice, row=row, column=column):
                             blocks[-1].append(self._empty_tile)
                         else:
-                            tile = self.read_image(**axes, **axes_to_slice, row=row, column=column, memmapped=True)
+                            tile = self.read_image(**axes, **axes_to_slice, row=row, column=column)
                             if self.half_overlap[0] != 0:
                                 tile = tile[
                                     self.half_overlap[0] : -self.half_overlap[0],
                                     self.half_overlap[1] : -self.half_overlap[1],
                                 ]
                             blocks[-1].append(tile)
 
@@ -624,15 +615,14 @@
         z=None,
         time=None,
         position=None,
         row=None,
         col=None,
         channel_name=None,
         resolution_level=0,
-        memmapped=False,
         **kwargs
     ):
         """
         Read image data as numpy array
 
         Parameters
         ----------
@@ -649,16 +639,14 @@
         row : int
             index of tile row for XY tiled datasets (Default value = None)
         col : int
             index of tile col for XY tiled datasets (Default value = None)
         resolution_level :
             0 is full resolution, otherwise represents downampling of pixels
             at 2 ** (resolution_level) (Default value = 0)
-        memmapped : bool
-             (Default value = False)
         **kwargs :
             names and integer positions of any other axes
 
         Returns
         -------
         image : numpy array or tuple
             image as a 2D numpy array, or tuple with image and image metadata as dict
@@ -666,15 +654,15 @@
         """
         with self._lock:
             axes = self._consolidate_axes(
                 channel, channel_name, z, position, time, row, col, kwargs
             )
 
             res_level = self.res_levels[resolution_level]
-            return res_level.read_image(axes, memmapped)
+            return res_level.read_image(axes)
 
     def read_metadata(
         self,
         channel=0,
         z=None,
         time=None,
         position=None,
```

### Comparing `ndtiff-1.9.1/ndtiff/ndtiff_v1.py` & `ndtiff-2.0.0/ndtiff/ndtiff_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 Library for reading multiresolution micro-magellan
 """
 import os
-import mmap
 import numpy as np
 import sys
 import json
-import platform
 import dask.array as da
 import warnings
 import struct
-
+from ndtiff.file_io import NDTiffFileIO, BUILTIN_FILE_IO
 
 class _MultipageTiffReader:
     # Class corresponsing to a single multipage tiff file in a Micro-Magellan dataset. Pass the full path of the TIFF to
     # instantiate and call close() when finished
     # TIFF constants
     WIDTH = 256
     HEIGHT = 257
@@ -32,24 +30,25 @@
     MM_METADATA = 51123
 
     # file format constants
     INDEX_MAP_OFFSET_HEADER = 54773648
     INDEX_MAP_HEADER = 3453623
     SUMMARY_MD_HEADER = 2355492
 
-    def __init__(self, tiff_path):
+    def __init__(self, tiff_path, file_io: NDTiffFileIO = BUILTIN_FILE_IO):
+        """
+        tiff_path: str
+            The path to a .tiff file to load
+        file_io: ndtiff.file_io.NDTiffFileIO
+            A container containing various methods for interacting with files.
+        """
+        self.file_io = file_io
         self.tiff_path = tiff_path
         self.file = open(tiff_path, "rb")
-        if platform.system() == "Windows":
-            self.mmap_file = mmap.mmap(self.file.fileno(), 0, access=mmap.ACCESS_READ)
-        else:
-            self.mmap_file = mmap.mmap(self.file.fileno(), 0, prot=mmap.PROT_READ)
         self.summary_md, self.index_tree, self.first_ifd_offset = self._read_header()
-        self.mmap_file.close()
-        self.np_memmap = np.memmap(self.file, dtype=np.uint8, mode="r")
 
         # get important metadata fields
         self.rgb = "RGB" in self.summary_md["PixelType"]
         self.width = self.summary_md["Width"]
         self.height = self.summary_md["Height"]
         self.dtype = (
             np.uint8
@@ -68,52 +67,52 @@
         summary metadata : dict
         byte offsets : nested dict
             The byte offsets of TIFF Image File Directories with keys [channel_index][z_index][frame_index][position_index]
         first_image_byte_offset : int
             int byte offset of first image IFD
         """
         # read standard tiff header
-        if self.mmap_file[:2] == b"\x4d\x4d":
+        if self._read(0,2) == b"\x4d\x4d":
             # Big endian
             if sys.byteorder != "big":
                 raise Exception("Potential issue with mismatched endian-ness")
-        elif self.mmap_file[:2] == b"\x49\x49":
+        elif self._read(0,2)== b"\x49\x49":
             # little endian
             if sys.byteorder != "little":
                 raise Exception("Potential issue with mismatched endian-ness")
         else:
             raise Exception("Endian type not specified correctly")
-        if np.frombuffer(self.mmap_file[2:4], dtype=np.uint16)[0] != 42:
+        if np.frombuffer(self._read(2,4), dtype=np.uint16)[0] != 42:
             raise Exception("Tiff magic 42 missing")
-        first_ifd_offset = np.frombuffer(self.mmap_file[4:8], dtype=np.uint32)[0]
+        first_ifd_offset = np.frombuffer(self._read(4,8), dtype=np.uint32)[0]
 
         # read custom stuff: summary md, index map
         index_map_offset_header, index_map_offset = np.frombuffer(
-            self.mmap_file[8:16], dtype=np.uint32
+            self._read(8, 16), dtype=np.uint32
         )
         if index_map_offset_header != self.INDEX_MAP_OFFSET_HEADER:
             raise Exception("Index map offset header wrong")
-        # int.from_bytes(self.mmap_file[24:28], sys.byteorder) # should be equal to 483729 starting in version 1
-        self._major_version = int.from_bytes(self.mmap_file[28:32], sys.byteorder)
+        # int.from_bytes(self._read[24:28], sys.byteorder) # should be equal to 483729 starting in version 1
+        self._major_version = int.from_bytes(self._read(28,32), sys.byteorder)
 
-        summary_md_header, summary_md_length = np.frombuffer(self.mmap_file[32:40], dtype=np.uint32)
+        summary_md_header, summary_md_length = np.frombuffer(self._read(32,40), dtype=np.uint32)
         if summary_md_header != self.SUMMARY_MD_HEADER:
             raise Exception("Index map offset header wrong")
-        summary_md = json.loads(self.mmap_file[40 : 40 + summary_md_length])
+        summary_md = json.loads(self._read(40 , 40 + summary_md_length))
         index_map_header, index_map_length = np.frombuffer(
-            self.mmap_file[40 + summary_md_length : 48 + summary_md_length], dtype=np.uint32
+            self._read(40 + summary_md_length, 48 + summary_md_length), dtype=np.uint32
         )
         if index_map_header != self.INDEX_MAP_HEADER:
             raise Exception("Index map header incorrect")
         # get index map as nested list of ints
         index_map_raw = np.reshape(
             np.frombuffer(
-                self.mmap_file[
-                    48 + summary_md_length : 48 + summary_md_length + index_map_length * 20
-                ],
+                self._read(
+                    48 + summary_md_length , 48 + summary_md_length + index_map_length * 20
+            ),
                 dtype=np.int32,
             ),
             [-1, 5],
         )
         index_map_keys = index_map_raw[:, :4].view(np.int32)
         index_map_byte_offsets = index_map_raw[:, 4].view(np.uint32)
         # If index map contains an offset value of 0, something has gone wrong
@@ -156,15 +155,16 @@
                             )
         return summary_md, index_tree, first_ifd_offset
 
     def _read(self, start, end):
         """
         convert to python ints
         """
-        return self.np_memmap[int(start) : int(end)].tobytes()
+        self.file.seek(int(start), 0)
+        return self.file.read(end - start)
 
     def _read_ifd(self, byte_offset):
         """
         Read image file directory. First two bytes are number of entries (n), next n*12 bytes are individual IFDs, final 4
         bytes are next IFD offset location
 
         Parameters
@@ -209,53 +209,45 @@
             self._read(byte_offset + num_entries * 12 + 2, byte_offset + num_entries * 12 + 6),
             dtype=np.uint32,
         )[0]
         if "bytes_per_image" not in info or "pixel_offset" not in info:
             raise Exception("Missing tags in IFD entry, file may be corrupted")
         return info
 
-    # def _read_pixels(self, offset, length, memmapped):
+    # def _read_pixels(self, offset, length):
     #     if self.width * self.height * 2 == length:
     #         pixel_type = np.uint16
     #     elif self.width * self.height == length:
     #         pixel_type = np.uint8
     #     else:
     #         raise Exception('Unknown pixel type')
     #
-    #     if memmapped:
-    #         return np.reshape(self.np_memmap[offset:offset + self.height * self.width * (2 if \
-    #                             pixel_type == np.uint16 else 1)].view(pixel_type), (self.height, self.width))
-    #     else:
-    #         pixels = np.frombuffer(self._read(offset, offset + length), dtype=pixel_type)
-    #         return np.reshape(pixels, [self.height, self.width])
+        # pixels = np.frombuffer(self._read(offset, offset + length), dtype=pixel_type)
+        # return np.reshape(pixels, [self.height, self.width])
 
     def read_metadata(self, channel_index, z_index, t_index, pos_index):
         ifd_offset, pixels_offset = self.index_tree[channel_index][z_index][t_index][pos_index]
         ifd_data = self._read_ifd(ifd_offset)
         metadata = json.loads(
             self._read(ifd_data["md_offset"], ifd_data["md_offset"] + ifd_data["md_length"])
         )
         return metadata
 
     def read_image(
-        self, channel_index, z_index, t_index, pos_index, read_metadata=False, memmapped=False
+        self, channel_index, z_index, t_index, pos_index, read_metadata=False
     ):
         ifd_offset, pixels_offset = self.index_tree[channel_index][z_index][t_index][pos_index]
+        bytes_per_pixel = (3 if self.rgb else 1) * (2 if self.dtype == np.uint16 else 1)
         image = np.reshape(
-            self.np_memmap[
-                pixels_offset : pixels_offset
-                + self.width
-                * self.height
-                * (3 if self.rgb else 1)
-                * (2 if self.dtype == np.uint16 else 1)
-            ].view(self.dtype),
-            [self.height, self.width, 3] if self.rgb else [self.height, self.width],
+            np.frombuffer(self._read(
+            pixels_offset, pixels_offset + self.width * self.height * bytes_per_pixel)
+                , dtype=self.dtype),
+            [self.height, self.width, 3] if bytes_per_pixel == 3 else [self.height, self.width],
         )
-        if not memmapped:
-            image = np.copy(image)
+        image = np.copy(image)
         # image = self._read_pixels(ifd_data['pixel_offset'], ifd_data['bytes_per_image'], memmapped)
         if read_metadata:
             ifd_data = self._read_ifd(ifd_offset)
             metadata = json.loads(
                 self._read(ifd_data["md_offset"], ifd_data["md_offset"] + ifd_data["md_length"])
             )
             return image, metadata
@@ -267,35 +259,36 @@
             ifd_data = self._read_ifd(ifd_offset)
             return True
         except:
             return False
 
 
 class _ResolutionLevel:
-    def __init__(self, path, count, max_count):
+    def __init__(self, path, count, max_count, file_io: NDTiffFileIO = BUILTIN_FILE_IO):
         """
         Open all tiff files in directory, keep them in a list, and a tree based on image indices
 
         Parameters
         ----------
         path : str
         count : int
         max_count : int
 
         """
+        self.file_io = file_io
         tiff_names = [
-            os.path.join(path, tiff) for tiff in os.listdir(path) if tiff.endswith(".tif")
+            self.file_io.path_join(path, tiff) for tiff in self.file_io.listdir(path) if tiff.endswith(".tif")
         ]
         self.reader_list = []
         self.reader_tree = {}
         # populate list of readers and tree mapping indices to readers
         for tiff in tiff_names:
             print("\rOpening file {} of {}".format(count + 1, max_count), end="")
             count += 1
-            reader = _MultipageTiffReader(tiff)
+            reader = _MultipageTiffReader(tiff, file_io=self.file_io)
             self.reader_list.append(reader)
             it = reader.index_tree
             for c in it.keys():
                 if c not in self.reader_tree.keys():
                     self.reader_tree[c] = {}
                 for z in it[c].keys():
                     if z not in self.reader_tree[c].keys():
@@ -309,15 +302,14 @@
     def read_image(
         self,
         channel_index=0,
         z_index=0,
         t_index=0,
         pos_index=0,
         read_metadata=False,
-        memmapped=False,
     ):
         """
 
         Parameters
         ----------
         channel_index : int
              (Default value = 0)
@@ -325,25 +317,23 @@
              (Default value = 0)
         t_index : int
              (Default value = 0)
         pos_index : int
              (Default value = 0)
         read_metadata : bool
              (Default value = False)
-        memmapped : bool
-             (Default value = False)
 
         Returns
         -------
         image :
         """
         # determine which reader contains the image
         reader = self.reader_tree[channel_index][z_index][t_index][pos_index]
         return reader.read_image(
-            channel_index, z_index, t_index, pos_index, read_metadata, memmapped
+            channel_index, z_index, t_index, pos_index, read_metadata
         )
 
     def read_metadata(self, channel_index=0, z_index=0, t_index=0, pos_index=0):
         """
 
         Parameters
         ----------
@@ -394,15 +384,16 @@
     """Class that opens a single NDTiffStorage dataset (major versions 0 and 1)"""
 
     _POSITION_AXIS = "position"
     _Z_AXIS = "z"
     _TIME_AXIS = "time"
     _CHANNEL_AXIS = "channel"
 
-    def __init__(self, dataset_path=None, full_res_only=True, remote_storage=None):
+    def __init__(self, dataset_path=None, full_res_only=True, remote_storage=None, file_io: NDTiffFileIO = BUILTIN_FILE_IO):
+        self.file_io = file_io
         self._tile_width = None
         self._tile_height = None
         # if remote_storage is not None:
         #     # this dataset is a view of an active acquisiiton. The storage exists on the java side
         #     self._remote_storage = remote_storage
         #     self._bridge = Bridge()
         #     smd = self._remote_storage.get_summary_metadata()
@@ -411,33 +402,33 @@
         #         self._tile_height = smd["Height"] - smd["GridPixelOverlapY"]
         #     return
         # else:
         self._remote_storage = None
 
         self.path = dataset_path
         res_dirs = [
-            dI for dI in os.listdir(dataset_path) if os.path.isdir(os.path.join(dataset_path, dI))
+            dI for dI in self.file_io.listdir(dataset_path) if self.file_io.listdir(self.file_io.path_join(dataset_path, dI))
         ]
         # map from downsample factor to datset
         self.res_levels = {}
         if "Full resolution" not in res_dirs:
             raise Exception(
                 "Couldn't find full resolution directory. Is this the correct path to a dataset?"
             )
         num_tiffs = 0
         count = 0
         for res_dir in res_dirs:
-            for file in os.listdir(os.path.join(dataset_path, res_dir)):
+            for file in self.file_io.listdir(self.file_io.path_join(dataset_path, res_dir)):
                 if file.endswith(".tif"):
                     num_tiffs += 1
         for res_dir in res_dirs:
             if full_res_only and res_dir != "Full resolution":
                 continue
-            res_dir_path = os.path.join(dataset_path, res_dir)
-            res_level = _ResolutionLevel(res_dir_path, count, num_tiffs)
+            res_dir_path = self.file_io.path_join(dataset_path, res_dir)
+            res_level = _ResolutionLevel(res_dir_path, count, num_tiffs, file_io=self.file_io)
             if res_dir == "Full resolution":
                 # TODO: might want to move this within the resolution level class to facilitate loading pyramids
                 self.res_levels[0] = res_level
                 # get summary metadata and index tree from full resolution image
                 self.summary_metadata = res_level.reader_list[0].summary_md
                 self.rgb = res_level.reader_list[0].rgb
                 self._channel_names = {}  # read them from image metadata
@@ -492,15 +483,15 @@
 
                     self._extra_axes_to_storage_channel[
                         frozenset(non_zpt_axes.items())
                     ] = channel_index
                     return non_zpt_axes
 
                 print("Parsing metadata\r", end="")
-                if "Axes_metedata" in os.listdir(dataset_path):
+                if "Axes_metedata" in self.file_io.listdir(dataset_path):
                     # newer version with a metadata file where this is written explicitly
                     with open(
                         dataset_path
                         + (os.sep if dataset_path[-1] != os.sep else "")
                         + "Axes_metedata",
                         "rb",
                     ) as axes_metadata_file:
@@ -664,23 +655,23 @@
         def recurse_axes(loop_axes, point_axes):
             if len(loop_axes.values()) == 0:
                 if verbose:
                     print("\rAdding data chunk {} of {}".format(self._count, total), end="")
                 self._count += 1
                 if None not in point_axes.values() and self.has_image(**point_axes):
                     if stitched:
-                        img = self.read_image(**point_axes, memmapped=True)
+                        img = self.read_image(**point_axes)
                         if self.half_overlap[0] != 0:
                             img = img[
                                 self.half_overlap[0] : -self.half_overlap[0],
                                 self.half_overlap[1] : -self.half_overlap[1],
                             ]
                         return img
                     else:
-                        return self.read_image(**point_axes, memmapped=True)
+                        return self.read_image(**point_axes)
                 else:
                     # return np.zeros((self.image_height, self.image_width), self.dtype)
                     return self._empty_tile
             else:
                 # do position first because it makes stitching faster
                 axis = (
                     "position"
@@ -869,15 +860,14 @@
         time=None,
         position=None,
         channel_name=None,
         read_metadata=False,
         resolution_level=0,
         row=None,
         col=None,
-        memmapped=False,
         **kwargs
     ):
         """
         Read image data as numpy array
 
         Parameters
         ----------
@@ -896,16 +886,14 @@
         col : int
             index of tile col for XY tiled datasets (Default value = None)
         resolution_level :
             0 is full resolution, otherwise represents downampling of pixels
             at 2 ** (resolution_level) (Default value = 0)
         read_metadata : bool
              (Default value = False)
-        memmapped : bool
-             (Default value = False)
         **kwargs :
             names and integer positions of any other axes
 
         Returns
         -------
         image : numpy array or tuple
             image as a 2D numpy array, or tuple with image and image metadata as dict
@@ -917,16 +905,14 @@
             kwargs["z"] = z
         if time is not None:
             kwargs["time"] = time
         if position is not None:
             kwargs["position"] = position
 
         # if self._remote_storage is not None:
-        #     if memmapped:
-        #         raise Exception("Memory mapping not available for in progress acquisitions")
         #     axes = self._bridge._construct_java_object("java.util.HashMap")
         #     for key in kwargs.keys():
         #         axes.put(key, kwargs[key])
         #     if not self._remote_storage.has_image(axes, resolution_level):
         #         return None
         #     if row is not None and col is not None:
         #         tagged_image = self._remote_storage.get_tile_by_row_col(
@@ -962,15 +948,15 @@
             # self.row_col_array #TODO: find position index in here
 
         storage_c_index, t_index, p_index, z_index = self._convert_to_storage_axes(
             kwargs, channel_name=channel_name
         )
         res_level = self.res_levels[resolution_level]
         return res_level.read_image(
-            storage_c_index, z_index, t_index, p_index, read_metadata, memmapped
+            storage_c_index, z_index, t_index, p_index, read_metadata
         )
 
     def read_first_image_metadata(self):
         """
         Get the first image metadata in the dataset (according to position along axes).
         This is useful if you want to access the image metadata in a dataset sparse, nonzero azes
```

### Comparing `ndtiff-1.9.1/ndtiff/test/data_loading_test.py` & `ndtiff-2.0.0/ndtiff/test/data_loading_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,104 @@
 import numpy as np
 from ndtiff import Dataset
 import os
 
-test_data_path = os.path.join(os.getcwd(), 'test_data')
 
-def test_v2_data():
+def test_v2_data(test_data_path):
     data_path = os.path.join(test_data_path, "v2", "ndtiffv2.0_test")
     dataset = Dataset(data_path)
     assert(np.mean(dataset.as_array()) > 0)
 
-def test_v3_data():
+def test_v3_data(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'ndtiffv3.0_test')
     dataset = Dataset(data_path)
     assert(np.mean(dataset.as_array()) > 0)
     for channel_name, correct_channel_name in zip(dataset.get_channel_names(), ['DAPI', 'FITC']):
         assert(channel_name == correct_channel_name)
 
-def test_v2_stitched_data():
+def test_v2_stitched_data(test_data_path):
     data_path = os.path.join(test_data_path, "v2", "ndtiffv2.0_stitched_test")
     dataset = Dataset(data_path)
     stitched = np.array(dataset.as_array(stitched=True))
     assert(stitched[..., 0, 0] > 0)
     assert(stitched[..., -1, -1] > 0)
     assert(stitched[..., 0, -1] == 0)
     assert(stitched[..., -1, 0] == 0)
 
-def test_v3_stitched_data():
+def test_v3_stitched_data(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'ndtiffv3.0_stitched_test')
     dataset = Dataset(data_path)
     stitched = np.array(dataset.as_array(stitched=True, res_level=0))
     assert(stitched[..., 0, 0] > 0)
     assert(stitched[..., -1, -1] > 0)
     assert(stitched[..., 0, -1] == 0)
     assert(stitched[..., -1, 0] == 0)
 
-def test_v3_magellan_explore():
+def test_v3_magellan_explore(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'Magellan_expolore_multi_channel')
     dataset = Dataset(data_path)
     stitched = np.array(dataset.as_array(stitched=True, res_level=0))
     
-def test_v3_magellan_explore_negative_and_overwritten():
+def test_v3_magellan_explore_negative_and_overwritten(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'Magellan_expolore_negative_indices_and_overwritten')
     dataset = Dataset(data_path)
     stitched = np.array(dataset.as_array(stitched=True, res_level=0))
 
-def test_v3_non_ctzp_axes():
+def test_v3_non_ctzp_axes(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'Nonstandard_axis_names')
     dataset = Dataset(data_path)
     stitched = np.array(dataset.as_array())
 
-def test_v3_mm_mda():
+def test_v3_mm_mda(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'mm_mda_tcz_15')
     dataset = Dataset(data_path)
     stitched = np.array(dataset.as_array())
 
-def test_v3_2_multichannel():
+def test_v3_2_multichannel(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'ndtiff3.2_multichannel')
     dataset = Dataset(data_path)
     assert(np.mean(dataset.read_image(channel='DAPI', time=0, z=1)) > 0)
     for channel_name, correct_channel_name in zip(dataset.get_channel_names(), ['DAPI', 'FITC']):
         assert(channel_name == correct_channel_name)
 
-def test_v3_2_multichannel_axis_sorting():
+def test_v3_2_multichannel_axis_sorting(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'ndtiff3.2_multichannel')
     dataset = Dataset(data_path)
     num_timepoints = len(dataset.axes['time'])
     num_channels = len(dataset.axes['channel'])
     num_slices = len(dataset.axes['z'])
     data = dataset.as_array(axes=None)
     assert data.shape[:-2] == (num_timepoints, num_channels, num_slices)
 
-def test_v3_2_monochrome():
+def test_v3_2_monochrome(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'ndtiff3.2_monochrome')
     dataset = Dataset(data_path)
     assert (np.mean(dataset.read_image(time=0, z=1)) > 0)
 
-def test_v3_2_magellan_rgb_explore():
+def test_v3_2_magellan_rgb_explore(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'ndtiff3.2_magellan_explore_rgb')
     dataset = Dataset(data_path)
     assert(np.sum(np.array(dataset.as_array(stitched=True)[0])) > 0)
 
-def test_v3_2_12bit_pycromanager_data():
+def test_v3_2_11bit_data(test_data_path):
+    data_path = os.path.join(test_data_path, 'v3', 'ndtiff3.2_11bit_1')
+    dataset = Dataset(data_path)
+    assert(dataset.read_metadata(time=0)['BitDepth'] == 11)
+    assert(dataset.read_image(time=0).dtype == np.uint16)
+
+def test_v3_2_12bit_pycromanager_data(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', '12_bit_pycromanager_mda')
     dataset = Dataset(data_path)
     assert(dataset.read_image(time=0, channel='DAPI').dtype == np.uint16)
+
+def test_v3_2_no_magellan_explore_channels(test_data_path):
+    data_path = os.path.join(test_data_path, 'v3', 'no_magellan_explore_multi_channel')
+    dataset = Dataset(data_path)
+    assert(np.sum(np.array(dataset.as_array(stitched=True)[0])) > 0)
+
+def test_v3_2_no_magellan_explore_no_channels(test_data_path):
+    data_path = os.path.join(test_data_path, 'v3', 'no_magellan_explore_no_channel')
+    dataset = Dataset(data_path)
+    assert(np.sum(np.array(dataset.as_array(stitched=True)[0])) > 0)
+
+
+
```

### Comparing `ndtiff-1.9.1/ndtiff.egg-info/PKG-INFO` & `ndtiff-2.0.0/ndtiff.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 1.9.1
+Version: 2.0.0
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-1.9.1/setup.py` & `ndtiff-2.0.0/setup.py`

 * *Files identical despite different names*

