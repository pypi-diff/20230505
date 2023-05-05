# Comparing `tmp/trex_imager_readfile-1.1.1.tar.gz` & `tmp/trex_imager_readfile-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex_imager_readfile-1.1.1.tar", max compression
+gzip compressed data, was "trex_imager_readfile-1.2.0.tar", max compression
```

## Comparing `trex_imager_readfile-1.1.1.tar` & `trex_imager_readfile-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.1.1/README.md
--rw-r--r--   0        0        0      677 2023-04-26 18:45:57.197926 trex_imager_readfile-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      431 2023-04-26 18:45:57.231927 trex_imager_readfile-1.1.1/trex_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8171 2023-03-07 15:42:19.050937 trex_imager_readfile-1.1.1/trex_imager_readfile/blueline.py
--rw-r--r--   0        0        0     8121 2023-03-07 15:42:32.213166 trex_imager_readfile-1.1.1/trex_imager_readfile/nir.py
--rw-r--r--   0        0        0    15985 2023-04-26 18:43:07.594848 trex_imager_readfile-1.1.1/trex_imager_readfile/rgb.py
--rw-r--r--   0        0        0     8215 2023-03-07 15:41:52.731479 trex_imager_readfile-1.1.1/trex_imager_readfile/spectrograph.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 trex_imager_readfile-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.2.0/README.md
+-rw-r--r--   0        0        0      693 2023-05-02 21:24:27.831819 trex_imager_readfile-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      397 2023-05-02 20:56:40.056544 trex_imager_readfile-1.2.0/trex_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8497 2023-05-03 20:42:44.563933 trex_imager_readfile-1.2.0/trex_imager_readfile/blueline.py
+-rw-r--r--   0        0        0     8447 2023-05-03 20:42:40.512856 trex_imager_readfile-1.2.0/trex_imager_readfile/nir.py
+-rw-r--r--   0        0        0    19860 2023-05-03 21:02:38.314477 trex_imager_readfile-1.2.0/trex_imager_readfile/rgb.py
+-rw-r--r--   0        0        0     8541 2023-05-03 20:42:47.366986 trex_imager_readfile-1.2.0/trex_imager_readfile/spectrograph.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 trex_imager_readfile-1.2.0/PKG-INFO
```

### Comparing `trex_imager_readfile-1.1.1/pyproject.toml` & `trex_imager_readfile-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "trex-imager-readfile"
-version = "1.1.1"
+version = "1.2.0"
 description = "Read functions for TREx ASI raw image files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "trex_imager_readfile" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 numpy = "^1.24.0"
 opencv-python = "^4.7.0"
+h5py = "^3.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 flake8 = "^6.0.0"
 pylint = "^2.16.0"
 
 [build-system]
```

### Comparing `trex_imager_readfile-1.1.1/trex_imager_readfile/blueline.py` & `trex_imager_readfile-1.2.0/trex_imager_readfile/blueline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-# Author: Lukas Vollmerhaus
-# Date: 2020-10-16
-
-import gzip as _gzip
-import numpy as _np
-import signal as _signal
-from multiprocessing import Pool as _Pool
-from functools import partial as _partial
+import gzip
+import numpy as np
+import signal
+import os
+from multiprocessing import Pool
+from functools import partial
 
 # globals
 __BLUELINE_IMAGE_SIZE_BYTES = 270 * 320 * 2
-__BLUELINE_DT = _np.dtype("uint16")
+__BLUELINE_DT = np.dtype("uint16")
 __BLUELINE_DT = __BLUELINE_DT.newbyteorder('>')  # force big endian byte ordering
 
 
 def __blueline_readfile_worker(file, quiet=False):
     # init
-    images = _np.array([])
+    images = np.array([])
     metadata_dict_list = []
     first_frame = True
     metadata_dict = {}
     site_uid = ""
     device_uid = ""
     problematic = False
     error_message = ""
 
+    # set site UID and device UID in case we need it (ie. dark frames, or unstacked files)
+    file_split = os.path.basename(file).split('_')
+    if (len(file_split) == 5):
+        # is a regular file
+        site_uid = file_split[2]
+        device_uid = file_split[3]
+    elif (len(file_split) > 5):
+        # is likely a dark frame or a unstacked frame
+        site_uid = file_split[3]
+        device_uid = file_split[4]
+
     # check file extension to see if it's gzipped or not
     try:
         if file.endswith("pgm.gz"):
-            unzipped = _gzip.open(file, mode='rb')
+            unzipped = gzip.open(file, mode='rb')
         elif file.endswith("pgm"):
             unzipped = open(file, mode='rb')
         else:
             if (quiet is False):
                 print("Unrecognized file type: %s" % (file))
             return images, metadata_dict_list, problematic, file, error_message
     except Exception as e:
@@ -47,15 +56,15 @@
         try:
             line = unzipped.readline()
         except Exception as e:
             if (quiet is False):
                 print("Error reading before image data in file '%s'" % (file))
             problematic = True
             metadata_dict_list = []
-            images = _np.array([])
+            images = np.array([])
             error_message = "error reading before image data: %s" % (str(e))
             return images, metadata_dict_list, problematic, file, error_message
 
         # break loop at end of file
         if (line == b''):
             break
 
@@ -106,32 +115,32 @@
             # read image
             try:
                 # read the image size in bytes from the file
                 image_bytes = unzipped.read(__BLUELINE_IMAGE_SIZE_BYTES)
 
                 # format bytes into numpy array of unsigned shorts (2byte numbers, 0-65536),
                 # effectively an array of pixel values
-                image_np = _np.frombuffer(image_bytes, dtype=__BLUELINE_DT)
+                image_np = np.frombuffer(image_bytes, dtype=__BLUELINE_DT)
 
                 # change 1d numpy array into 270x320 matrix with correctly located pixels
-                image_matrix = _np.reshape(image_np, (270, 320, 1))
+                image_matrix = np.reshape(image_np, (270, 320, 1))
             except Exception as e:
                 if (quiet is False):
                     print("Failed reading image data frame: %s" % (str(e)))
                 metadata_dict_list.pop()  # remove corresponding metadata entry
                 problematic = True
                 error_message = "image data read failure: %s" % (str(e))
                 continue  # skip to next frame
 
             # initialize image stack
             if first_frame:
                 images = image_matrix
                 first_frame = False
             else:
-                images = _np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
+                images = np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
 
     # close gzip file
     unzipped.close()
 
     # return
     return images, metadata_dict_list, problematic, file, error_message
 
@@ -148,35 +157,35 @@
     :type quiet: bool, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 20
-    images = _np.empty([270, 320, predicted_num_frames], dtype=__BLUELINE_DT)
+    images = np.empty([270, 320, predicted_num_frames], dtype=__BLUELINE_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
     # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = _signal.signal(_signal.SIGINT, _signal.SIG_IGN)
-    pool = _Pool(processes=workers)
-    _signal.signal(_signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+    pool = Pool(processes=workers)
+    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
 
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
     # call readfile function, run each iteration with a single input file from file_list
     # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
     data = []
     try:
-        data = pool.map(_partial(__blueline_readfile_worker, quiet=quiet), file_list)
+        data = pool.map(partial(__blueline_readfile_worker, quiet=quiet), file_list)
     except KeyboardInterrupt:
         pool.terminate()  # gracefully kill children
-        return _np.empty((0, 0, 0), dtype=__BLUELINE_DT), [], []
+        return np.empty((0, 0, 0), dtype=__BLUELINE_DT), [], []
     else:
         pool.close()
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
@@ -197,15 +206,15 @@
         # metadata dictionary list at data[][1]
         metadata_dict_list[list_position:list_position + real_num_frames] = data[i][1]
         images[:, :, list_position:list_position + real_num_frames] = data[i][0]  # image arrays at data[][0]
         list_position = list_position + real_num_frames  # advance list position
 
     # trim unused elements from predicted array sizes
     metadata_dict_list = metadata_dict_list[0:list_position]
-    images = _np.delete(images, range(list_position, predicted_num_frames), axis=2)
+    images = np.delete(images, range(list_position, predicted_num_frames), axis=2)
 
     # ensure entire array views as uint16
-    images = images.astype(_np.uint16)
+    images = images.astype(np.uint16)
 
     # return
     data = None
     return images, metadata_dict_list, problematic_file_list
```

### Comparing `trex_imager_readfile-1.1.1/trex_imager_readfile/nir.py` & `trex_imager_readfile-1.2.0/trex_imager_readfile/nir.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-# Author: Lukas Vollmerhaus
-# Date: 2020-10-16
-
-import gzip as _gzip
-import numpy as _np
-import signal as _signal
-from multiprocessing import Pool as _Pool
-from functools import partial as _partial
+import gzip
+import numpy as np
+import signal
+import os
+from multiprocessing import Pool
+from functools import partial
 
 # globals
 __NIR_IMAGE_SIZE_BYTES = 256 * 256 * 2
-__NIR_DT = _np.dtype("uint16")
+__NIR_DT = np.dtype("uint16")
 __NIR_DT = __NIR_DT.newbyteorder('>')  # force big endian byte ordering
 
 
 def __nir_readfile_worker(file, quiet=False):
     # init
-    images = _np.array([])
+    images = np.array([])
     metadata_dict_list = []
     first_frame = True
     metadata_dict = {}
     site_uid = ""
     device_uid = ""
     problematic = False
     error_message = ""
 
+    # set site UID and device UID in case we need it (ie. dark frames, or unstacked files)
+    file_split = os.path.basename(file).split('_')
+    if (len(file_split) == 5):
+        # is a regular file
+        site_uid = file_split[2]
+        device_uid = file_split[3]
+    elif (len(file_split) > 5):
+        # is likely a dark frame or a unstacked frame
+        site_uid = file_split[3]
+        device_uid = file_split[4]
+
     # check file extension to see if it's gzipped or not
     try:
         if file.endswith("pgm.gz"):
-            unzipped = _gzip.open(file, mode='rb')
+            unzipped = gzip.open(file, mode='rb')
         elif file.endswith("pgm"):
             unzipped = open(file, mode='rb')
         else:
             if (quiet is False):
                 print("Unrecognized file type: %s" % (file))
             return images, metadata_dict_list, problematic, file, error_message
     except Exception as e:
@@ -47,15 +56,15 @@
         try:
             line = unzipped.readline()
         except Exception as e:
             if (quiet is False):
                 print("Error reading before image data in file '%s'" % (file))
             problematic = True
             metadata_dict_list = []
-            images = _np.array([])
+            images = np.array([])
             error_message = "error reading before image data: %s" % (str(e))
             return images, metadata_dict_list, problematic, file, error_message
 
         # break loop at end of file
         if (line == b''):
             break
 
@@ -106,32 +115,32 @@
             # read image
             try:
                 # read the image size in bytes from the file
                 image_bytes = unzipped.read(__NIR_IMAGE_SIZE_BYTES)
 
                 # format bytes into numpy array of unsigned shorts (2byte numbers, 0-65536),
                 # effectively an array of pixel values
-                image_np = _np.frombuffer(image_bytes, dtype=__NIR_DT)
+                image_np = np.frombuffer(image_bytes, dtype=__NIR_DT)
 
                 # change 1d numpy array into 256x256 matrix with correctly located pixels
-                image_matrix = _np.reshape(image_np, (256, 256, 1))
+                image_matrix = np.reshape(image_np, (256, 256, 1))
             except Exception as e:
                 if (quiet is False):
                     print("Failed reading image data frame: %s" % (str(e)))
                 metadata_dict_list.pop()  # remove corresponding metadata entry
                 problematic = True
                 error_message = "image data read failure: %s" % (str(e))
                 continue  # skip to next frame
 
             # initialize image stack
             if first_frame:
                 images = image_matrix
                 first_frame = False
             else:
-                images = _np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
+                images = np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
 
     # close gzip file
     unzipped.close()
 
     # return
     return images, metadata_dict_list, problematic, file, error_message
 
@@ -148,35 +157,35 @@
     :type quiet: bool, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 10
-    images = _np.empty([256, 256, predicted_num_frames], dtype=__NIR_DT)
+    images = np.empty([256, 256, predicted_num_frames], dtype=__NIR_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
     # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = _signal.signal(_signal.SIGINT, _signal.SIG_IGN)
-    pool = _Pool(processes=workers)
-    _signal.signal(_signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+    pool = Pool(processes=workers)
+    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
 
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
     # call readfile function, run each iteration with a single input file from file_list
     # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
     data = []
     try:
-        data = pool.map(_partial(__nir_readfile_worker, quiet=quiet), file_list)
+        data = pool.map(partial(__nir_readfile_worker, quiet=quiet), file_list)
     except KeyboardInterrupt:
         pool.terminate()  # gracefully kill children
-        return _np.empty((0, 0, 0), dtype=__NIR_DT), [], []
+        return np.empty((0, 0, 0), dtype=__NIR_DT), [], []
     else:
         pool.close()
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
@@ -197,15 +206,15 @@
         # metadata dictionary list at data[][1]
         metadata_dict_list[list_position:list_position + real_num_frames] = data[i][1]
         images[:, :, list_position:list_position + real_num_frames] = data[i][0]  # image arrays at data[][0]
         list_position = list_position + real_num_frames  # advance list position
 
     # trim unused elements from predicted array sizes
     metadata_dict_list = metadata_dict_list[0:list_position]
-    images = _np.delete(images, range(list_position, predicted_num_frames), axis=2)
+    images = np.delete(images, range(list_position, predicted_num_frames), axis=2)
 
     # ensure entire array views as uint16
-    images = images.astype(_np.uint16)
+    images = images.astype(np.uint16)
 
     # return
     data = None
     return images, metadata_dict_list, problematic_file_list
```

### Comparing `trex_imager_readfile-1.1.1/trex_imager_readfile/rgb.py` & `trex_imager_readfile-1.2.0/trex_imager_readfile/rgb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-# Author: Lukas Vollmerhaus
-# Date: 2020-10-16
-
-import gzip as _gzip
-import numpy as _np
-import signal as _signal
-import cv2 as _cv2
-import tarfile as _tarfile
-import os as _os
-import datetime as _datetime
-from multiprocessing import Pool as _Pool
+import gzip
+import numpy as np
+import signal
+import cv2
+import tarfile
+import os
+import datetime
+import h5py
+from pathlib import Path
+from multiprocessing import Pool
 
 # static globals
 __RGB_PGM_IMAGE_SIZE_BYTES = 480 * 553 * 2
-__RGB_PGM_DT = _np.dtype("uint16")
+__RGB_PGM_DT = np.dtype("uint16")
 __RGB_PGM_DT = __RGB_PGM_DT.newbyteorder('>')  # force big endian byte ordering
-__RGB_PNG_DT = _np.dtype("uint8")
+__RGB_PNG_DT = np.dtype("uint8")
+__RGB_H5_DT = np.dtype("uint8")
 __PNG_METADATA_PROJECT_UID = "trex"
-__FLEX_FRAME_COUNT = 2
-__EXPECTED_FRAME_COUNT = 20 + __FLEX_FRAME_COUNT
+__FLEX_NOMINAL_FRAME_COUNT = 2
+__FLEX_BURST_FRAME_COUNT = 50
+__EXPECTED_NOMINAL_FRAME_COUNT = 20 + __FLEX_NOMINAL_FRAME_COUNT
+__EXPECTED_BURST_FRAME_COUNT = 150 + __FLEX_BURST_FRAME_COUNT
 
 
 def __trex_readfile_worker(file_obj):
     # init
-    images = _np.array([])
+    images = np.array([])
     metadata_dict_list = []
     problematic = False
     error_message = ""
     image_width = 0
     image_height = 0
     image_channels = 0
-    image_dtype = _np.dtype("uint16")
-    image_dtype = image_dtype.newbyteorder('>')
+    image_dtype = np.dtype("uint8")
 
     # check file extension to know how to process
     try:
         if (file_obj["filename"].endswith("pgm") or file_obj["filename"].endswith("pgm.gz")):
             return __rgb_readfile_worker_pgm(file_obj)
         elif (file_obj["filename"].endswith("png") or file_obj["filename"].endswith("png.tar")):
             return __rgb_readfile_worker_png(file_obj)
+        elif (file_obj["filename"].endswith("h5")):
+            return __rgb_readfile_worker_h5(file_obj)
         else:
             if (file_obj["quiet"] is False):
                 print("Unrecognized file type: %s" % (file_obj["filename"]))
             raise Exception("Unrecognized file type: %s" % ((file_obj["filename"])))
     except Exception as e:
         if (file_obj["quiet"] is False):
             import traceback
@@ -49,38 +52,255 @@
             print("Failed to process file '%s' " % (file_obj["filename"]))
         problematic = True
         error_message = "failed to process file: %s" % (str(e))
     return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
         image_width, image_height, image_channels, image_dtype
 
 
+def __parse_frame_metadata(frame_list):
+    # init
+    metadata = {}
+
+    # process frame metadata
+    for frame_item in frame_list:
+        separator_idx = frame_item.find(':')
+        key = frame_item[0:separator_idx]
+        value = frame_item[(separator_idx + 1):]
+        key = key.strip()
+        value = value.strip()
+        metadata[key] = value
+
+    # return
+    return metadata
+
+
+def __rgb_readfile_worker_h5(file_obj):
+    # init
+    images = np.array([])
+    metadata_dict_list = []
+    problematic = False
+    error_message = ""
+    image_width = 0
+    image_height = 0
+    image_channels = 0
+    image_dtype = __RGB_H5_DT
+    nframes = 0
+
+    # open H5 file
+    f = h5py.File(file_obj["filename"], 'r')
+
+    # get dataset
+    dataset = f["data"]
+
+    # read file metadata
+    file_metadata = {}
+    frame_keys = []
+    for key in dataset.attrs.keys():
+        value = dataset.attrs[key]
+        if (isinstance(value, np.ndarray) is False):
+            file_metadata[key] = value.strip()
+        else:
+            frame_keys.append(key)
+
+    # check that there's frame metadata
+    if (len(frame_keys) == 0):
+        problematic = True
+        error_message = "No frame metadata exists"
+        return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
+            image_width, image_height, image_channels, image_dtype
+
+    # set first frame
+    frame_keys = sorted(frame_keys)
+    frame_metadata = __parse_frame_metadata(dataset.attrs[frame_keys[0]])
+    file_metadata.update(frame_metadata)
+    metadata_dict_list.append(file_metadata)
+
+    # set remaining frame metadata
+    if (len(frame_keys) >= 2):
+        for key in frame_keys[1:]:
+            frame_metadata = __parse_frame_metadata(dataset.attrs[key])
+            metadata_dict_list.append(frame_metadata)
+
+    # read data
+    images = dataset[()]
+
+    # close H5 file
+    f.close()
+
+    # set image vars and reshape if multiple images
+    if (len(images.shape) == 3):
+        # single frame
+        nframes = 1
+        image_height = images.shape[0]
+        image_width = images.shape[1]
+        image_channels = images.shape[2]
+        images = images.reshape((image_height, image_width, image_channels, 1))
+    else:
+        # multiple frames
+        nframes = images.shape[0]
+        image_height = images.shape[1]
+        image_width = images.shape[2]
+        image_channels = images.shape[3]
+        images = images.reshape((image_height, image_width, image_channels, nframes))
+
+    # verify that metadata list size matches number of images
+    if (len(metadata_dict_list) != nframes):
+        problematic = True
+        error_message = "Found different number of images and metadata records" \
+            "(images=%d, metadata=%d)" % (nframes, len(metadata_dict_list))
+        return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
+            image_width, image_height, image_channels, image_dtype
+
+    # return
+    return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
+        image_width, image_height, image_channels, image_dtype
+
+
+def __rgb_readfile_worker_png(file_obj):
+    # init
+    images = np.array([])
+    metadata_dict_list = []
+    problematic = False
+    first_frame = True
+    error_message = ""
+    image_width = 0
+    image_height = 0
+    image_channels = 0
+    image_dtype = __RGB_PNG_DT
+    is_tar_file = False
+
+    # check if it's a tar file
+    file_list = []
+    if (file_obj["filename"].endswith(".png.tar")):
+        # tar file, extract all frames and add to list
+        try:
+            tf = tarfile.open(file_obj["filename"])
+            file_list = sorted(tf.getnames())
+            tf.extractall(path=file_obj["tar_tempdir"])
+            for i in range(0, len(file_list)):
+                file_list[i] = "%s/%s" % (file_obj["tar_tempdir"], file_list[i])
+            tf.close()
+            is_tar_file = True
+        except Exception as e:
+            if ("file_list" in locals()):
+                # cleanup
+                for f in file_list:
+                    try:
+                        os.remove(f)
+                    except Exception:
+                        pass
+            if (file_obj["quiet"] is False):
+                print("Failed to open file '%s' " % (file_obj["filename"]))
+            problematic = True
+            error_message = "failed to open file: %s" % (str(e))
+            return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
+                image_width, image_height, image_channels, image_dtype
+    else:
+        # regular png
+        file_list = [file_obj["filename"]]
+
+    # read each png file
+    for f in file_list:
+        # process metadata
+        try:
+            # set metadata values
+            file_split = os.path.basename(f).split('_')
+            site_uid = file_split[3]
+            device_uid = file_split[4]
+            exposure = "%.03f ms" % (float(file_split[5][:-2]))
+            mode_uid = file_split[6][:-4]
+
+            # set timestamp
+            if ("burst" in f):
+                timestamp = datetime.datetime.strptime("%sT%s.%s" % (file_split[0], file_split[1], file_split[2]),
+                                                       "%Y%m%dT%H%M%S.%f")
+            else:
+                timestamp = datetime.datetime.strptime("%sT%s" % (file_split[0], file_split[1]),
+                                                       "%Y%m%dT%H%M%S")
+
+            # set the metadata dict
+            metadata_dict = {
+                "Project unique ID": __PNG_METADATA_PROJECT_UID,
+                "Site unique ID": site_uid,
+                "Imager unique ID": device_uid,
+                "Mode unique ID": mode_uid,
+                "Image request start": timestamp,
+                "Subframe requested exposure": exposure,
+            }
+            metadata_dict_list.append(metadata_dict)
+        except Exception as e:
+            if (file_obj["quiet"] is False):
+                print("Failed to read metadata from file '%s' " % (f))
+            problematic = True
+            error_message = "failed to read metadata: %s" % (str(e))
+            break
+
+        # read png file
+        try:
+            # read file
+            image_np = cv2.imread(f)
+            image_height = image_np.shape[0]
+            image_width = image_np.shape[1]
+            image_channels = image_np.shape[2] if len(image_np.shape) > 2 else 1
+            if (image_channels > 1):
+                image_matrix = np.reshape(image_np, (image_height, image_width, image_channels, 1))
+            else:
+                image_matrix = np.reshape(image_np, (image_height, image_width, 1))
+
+            # initialize image stack
+            if (first_frame is True):
+                images = image_matrix
+                first_frame = False
+            else:
+                if (image_channels > 1):
+                    images = np.concatenate([images, image_matrix], axis=3)  # concatenate (on last axis)
+                else:
+                    images = np.dstack([images, image_matrix])  # depth stack images (on last axis)
+        except Exception as e:
+            if (file_obj["quiet"] is False):
+                print("Failed reading image data frame: %s" % (str(e)))
+            metadata_dict_list.pop()  # remove corresponding metadata entry
+            problematic = True
+            error_message = "image data read failure: %s" % (str(e))
+            continue  # skip to next frame
+
+    # remove untarred files
+    if (is_tar_file is True):
+        for f in file_list:
+            os.remove(f)
+
+    # return
+    return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
+        image_width, image_height, image_channels, image_dtype
+
+
 def __rgb_readfile_worker_pgm(file_obj):
     # init
-    images = _np.array([])
+    images = np.array([])
     metadata_dict_list = []
     first_frame = True
     metadata_dict = {}
     site_uid = ""
     device_uid = ""
     problematic = False
     error_message = ""
-    image_width = 480
-    image_height = 553
+    image_width = 553
+    image_height = 480
     image_channels = 1
     image_dtype = __RGB_PGM_DT
 
     # Set metadata values
-    file_split = _os.path.basename(file_obj["filename"]).split('_')
+    file_split = os.path.basename(file_obj["filename"]).split('_')
     site_uid = file_split[3]
     device_uid = file_split[4]
 
     # check file extension to see if it's gzipped or not
     try:
         if file_obj["filename"].endswith("pgm.gz"):
-            unzipped = _gzip.open(file_obj["filename"], mode='rb')
+            unzipped = gzip.open(file_obj["filename"], mode='rb')
         elif file_obj["filename"].endswith("pgm"):
             unzipped = open(file_obj["filename"], mode='rb')
         else:
             if (file_obj["quiet"] is False):
                 print("Unrecognized file type: %s" % (file_obj["filename"]))
             return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
                 image_width, image_height, image_channels, image_dtype
@@ -98,15 +318,15 @@
         try:
             line = unzipped.readline()
         except Exception as e:
             if (file_obj["quiet"] is False):
                 print("Error reading before image data in file '%s'" % (file_obj["filename"]))
             problematic = True
             metadata_dict_list = []
-            images = _np.array([])
+            images = np.array([])
             error_message = "error reading before image data: %s" % (str(e))
             return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
                 image_width, image_height, image_channels, image_dtype
 
         # break loop at end of file
         if (line == b''):
             break
@@ -157,32 +377,32 @@
             # read image
             try:
                 # read the image size in bytes from the file
                 image_bytes = unzipped.read(__RGB_PGM_IMAGE_SIZE_BYTES)
 
                 # format bytes into numpy array of unsigned shorts (2byte numbers, 0-65536),
                 # effectively an array of pixel values
-                image_np = _np.frombuffer(image_bytes, dtype=__RGB_PGM_DT)
+                image_np = np.frombuffer(image_bytes, dtype=__RGB_PGM_DT)
 
                 # change 1d numpy array into 480x553 matrix with correctly located pixels
-                image_matrix = _np.reshape(image_np, (480, 553, 1))
+                image_matrix = np.reshape(image_np, (480, 553, 1))
             except Exception as e:
                 if (file_obj["quiet"] is False):
                     print("Failed reading image data frame: %s" % (str(e)))
                 metadata_dict_list.pop()  # remove corresponding metadata entry
                 problematic = True
                 error_message = "image data read failure: %s" % (str(e))
                 continue  # skip to next frame
 
             # initialize image stack
             if first_frame:
                 images = image_matrix
                 first_frame = False
             else:
-                images = _np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
+                images = np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
 
     # close gzip file
     unzipped.close()
 
     # set the site/device uids, or inject the site and device UIDs if they are missing
     if ("Site unique ID" not in metadata_dict):
         metadata_dict["Site unique ID"] = site_uid
@@ -191,146 +411,40 @@
         metadata_dict["Imager unique ID"] = device_uid
 
     # return
     return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
         image_width, image_height, image_channels, image_dtype
 
 
-def __rgb_readfile_worker_png(file_obj):
-    # init
-    images = _np.array([])
-    metadata_dict_list = []
-    problematic = False
-    first_frame = True
-    error_message = ""
-    image_width = 0
-    image_height = 0
-    image_channels = 0
-    image_dtype = __RGB_PNG_DT
-    is_tar_file = False
-
-    # check if it's a tar file
-    file_list = []
-    if (file_obj["filename"].endswith(".png.tar")):
-        # tar file, extract all frames and add to list
-        try:
-            tf = _tarfile.open(file_obj["filename"])
-            file_list = sorted(tf.getnames())
-            tf.extractall(path=file_obj["tar_tempdir"])
-            for i in range(0, len(file_list)):
-                file_list[i] = "%s/%s" % (file_obj["tar_tempdir"], file_list[i])
-            tf.close()
-            is_tar_file = True
-        except Exception as e:
-            if ("file_list" in locals()):
-                # cleanup
-                for f in file_list:
-                    try:
-                        _os.remove(f)
-                    except Exception:
-                        pass
-            if (file_obj["quiet"] is False):
-                print("Failed to open file '%s' " % (file_obj["filename"]))
-            problematic = True
-            error_message = "failed to open file: %s" % (str(e))
-            return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
-                image_width, image_height, image_channels, image_dtype
-    else:
-        # regular png
-        file_list = [file_obj["filename"]]
-
-    # read each png file
-    for f in file_list:
-        # process metadata
-        try:
-            # set metadata values
-            file_split = _os.path.basename(f).split('_')
-            site_uid = file_split[3]
-            device_uid = file_split[4]
-            exposure = "%.03f ms" % (float(file_split[5][:-2]))
-            mode_uid = file_split[6][:-4]
-            timestamp = _datetime.datetime.strptime("%sT%s" % (file_split[0], file_split[1]), "%Y%m%dT%H%M%S")
-
-            # set the metadata dict
-            metadata_dict = {
-                "Project unique ID": __PNG_METADATA_PROJECT_UID,
-                "Site unique ID": site_uid,
-                "Imager unique ID": device_uid,
-                "Mode unique ID": mode_uid,
-                "Image request start": timestamp,
-                "Subframe requested exposure": exposure,
-            }
-            metadata_dict_list.append(metadata_dict)
-        except Exception as e:
-            if (file_obj["quiet"] is False):
-                print("Failed to read metadata from file '%s' " % (f))
-            problematic = True
-            error_message = "failed to read metadata: %s" % (str(e))
-            break
-
-        # read png file
-        try:
-            # read file
-            image_np = _cv2.imread(f)
-            image_width = image_np.shape[0]
-            image_height = image_np.shape[1]
-            image_channels = image_np.shape[2] if len(image_np.shape) > 2 else 1
-            if (image_channels > 1):
-                image_matrix = _np.reshape(image_np, (image_width, image_height, image_channels, 1))
-            else:
-                image_matrix = _np.reshape(image_np, (image_width, image_height, 1))
-
-            # initialize image stack
-            if (first_frame is True):
-                images = image_matrix
-                first_frame = False
-            else:
-                if (image_channels > 1):
-                    images = _np.concatenate([images, image_matrix], axis=3)  # concatenate (on last axis)
-                else:
-                    images = _np.dstack([images, image_matrix])  # depth stack images (on last axis)
-        except Exception as e:
-            if (file_obj["quiet"] is False):
-                print("Failed reading image data frame: %s" % (str(e)))
-            metadata_dict_list.pop()  # remove corresponding metadata entry
-            problematic = True
-            error_message = "image data read failure: %s" % (str(e))
-            continue  # skip to next frame
-
-    # remove untarred files
-    if (is_tar_file is True):
-        for f in file_list:
-            _os.remove(f)
-
-    # return
-    return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
-        image_width, image_height, image_channels, image_dtype
-
-
-def read(file_list, workers=1, tar_tempdir=_os.getcwd(), quiet=False):
+def read(file_list, workers=1, tar_tempdir=None, quiet=False):
     """
-    Read in a single PGM or PNG.TAR file, or an array of them. All files
-    must be the same type.
+    Read in a single H5 or PNG.tar file, or an array of them. All files
+    must be the same type. This also works for reading in PGM or untarred PNG
+    files.
 
     :param file_list: filename or list of filenames
     :type file_list: str
     :param workers: number of worker processes to spawn, defaults to 1
     :type workers: int, optional
     :param tar_tempdir: path to untar to, defaults to '.'
     :type tar_tempdir: str, optional
     :param quiet: reduce output while reading data
     :type quiet: bool, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
+    # set tar path
+    if (tar_tempdir is None):
+        tar_tempdir = Path("%s/.trex_imager_readfile" % (str(Path.home())))
+
     # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = _signal.signal(_signal.SIGINT, _signal.SIG_IGN)
-    pool = _Pool(processes=workers)
-    _signal.signal(_signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+    pool = Pool(processes=workers)
+    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
 
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
     # convert to object, injecting other data we need for processing
     processing_list = []
@@ -343,30 +457,35 @@
 
     # call readfile function, run each iteration with a single input file from file_list
     pool_data = []
     try:
         pool_data = pool.map(__trex_readfile_worker, processing_list)
     except KeyboardInterrupt:
         pool.terminate()  # gracefully kill children
-        return _np.empty((0, 0, 0)), [], []
+        return np.empty((0, 0, 0)), [], []
     else:
         pool.close()
 
     # set sizes
     image_width = pool_data[0][5]
     image_height = pool_data[0][6]
     image_channels = pool_data[0][7]
     image_dtype = pool_data[0][8]
 
+    # set max predicted frame count
+    if ("burst" in f):
+        predicted_num_frames = len(processing_list) * __EXPECTED_BURST_FRAME_COUNT
+    else:
+        predicted_num_frames = len(processing_list) * __EXPECTED_NOMINAL_FRAME_COUNT
+
     # pre-allocate array sizes (optimization)
-    predicted_num_frames = len(processing_list) * __EXPECTED_FRAME_COUNT
     if (image_channels > 1):
-        images = _np.empty([image_width, image_height, image_channels, predicted_num_frames], dtype=image_dtype)
+        images = np.empty([image_height, image_width, image_channels, predicted_num_frames], dtype=image_dtype)
     else:
-        images = _np.empty([image_width, image_height, predicted_num_frames], dtype=image_dtype)
+        images = np.empty([image_height, image_width, predicted_num_frames], dtype=image_dtype)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
     # reorganize data
     list_position = 0
     for i in range(0, len(pool_data)):
         # check if file was problematic
@@ -391,17 +510,17 @@
         else:
             images[:, :, list_position:list_position + real_num_frames] = pool_data[i][0]
         list_position = list_position + real_num_frames  # advance list position
 
     # trim unused elements from predicted array sizes
     metadata_dict_list = metadata_dict_list[0:list_position]
     if (image_channels > 1):
-        images = _np.delete(images, range(list_position, predicted_num_frames), axis=3)
+        images = np.delete(images, range(list_position, predicted_num_frames), axis=3)
     else:
-        images = _np.delete(images, range(list_position, predicted_num_frames), axis=2)
+        images = np.delete(images, range(list_position, predicted_num_frames), axis=2)
 
     # ensure entire array views as the dtype
     images = images.astype(image_dtype)
 
     # return
     pool_data = None
     return images, metadata_dict_list, problematic_file_list
```

### Comparing `trex_imager_readfile-1.1.1/trex_imager_readfile/spectrograph.py` & `trex_imager_readfile-1.2.0/trex_imager_readfile/spectrograph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-# Author: Lukas Vollmerhaus
-# Date: 2020-10-16
-
-import gzip as _gzip
-import numpy as _np
-import signal as _signal
-from multiprocessing import Pool as _Pool
-from functools import partial as _partial
+import gzip
+import numpy as np
+import signal
+import os
+from multiprocessing import Pool
+from functools import partial
 
 # globals
 __SPECTROGRAPH_IMAGE_SIZE_BYTES = 1024 * 256 * 2
-__SPECTROGRAPH_DT = _np.dtype("uint16")
+__SPECTROGRAPH_DT = np.dtype("uint16")
 __SPECTROGRAPH_DT = __SPECTROGRAPH_DT.newbyteorder('>')  # force big endian byte ordering
 
 
 def __spectrograph_readfile_worker(file, quiet=False):
     # init
-    images = _np.array([])
+    images = np.array([])
     metadata_dict_list = []
     first_frame = True
     metadata_dict = {}
     site_uid = ""
     device_uid = ""
     problematic = False
     error_message = ""
 
+    # set site UID and device UID in case we need it (ie. dark frames, or unstacked files)
+    file_split = os.path.basename(file).split('_')
+    if (len(file_split) == 5):
+        # is a regular file
+        site_uid = file_split[2]
+        device_uid = file_split[3]
+    elif (len(file_split) > 5):
+        # is likely a dark frame or a unstacked frame
+        site_uid = file_split[3]
+        device_uid = file_split[4]
+
     # check file extension to see if it's gzipped or not
     try:
         if file.endswith("pgm.gz"):
-            unzipped = _gzip.open(file, mode='rb')
+            unzipped = gzip.open(file, mode='rb')
         elif file.endswith("pgm"):
             unzipped = open(file, mode='rb')
         else:
             if (quiet is False):
                 print("Unrecognized file type: %s" % (file))
             return images, metadata_dict_list, problematic, file, error_message
     except Exception as e:
@@ -47,15 +56,15 @@
         try:
             line = unzipped.readline()
         except Exception as e:
             if (quiet is False):
                 print("Error reading before image data in file '%s'" % (file))
             problematic = True
             metadata_dict_list = []
-            images = _np.array([])
+            images = np.array([])
             error_message = "error reading before image data: %s" % (str(e))
             return images, metadata_dict_list, problematic, file, error_message
 
         # break loop at end of file
         if (line == b''):
             break
 
@@ -106,32 +115,32 @@
             # read image
             try:
                 # read the image size in bytes from the file
                 image_bytes = unzipped.read(__SPECTROGRAPH_IMAGE_SIZE_BYTES)
 
                 # format bytes into numpy array of unsigned shorts (2byte numbers, 0-65536),
                 # effectively an array of pixel values
-                image_np = _np.frombuffer(image_bytes, dtype=__SPECTROGRAPH_DT)
+                image_np = np.frombuffer(image_bytes, dtype=__SPECTROGRAPH_DT)
 
                 # change 1d numpy array into 1024x256 matrix with correctly located pixels
-                image_matrix = _np.reshape(image_np, (1024, 256, 1))
+                image_matrix = np.reshape(image_np, (1024, 256, 1))
             except Exception as e:
                 if (quiet is False):
                     print("Failed reading image data frame: %s" % (str(e)))
                 metadata_dict_list.pop()  # remove corresponding metadata entry
                 problematic = True
                 error_message = "image data read failure: %s" % (str(e))
                 continue  # skip to next frame
 
             # initialize image stack
             if first_frame:
                 images = image_matrix
                 first_frame = False
             else:
-                images = _np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
+                images = np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
 
     # close gzip file
     unzipped.close()
 
     # return
     return images, metadata_dict_list, problematic, file, error_message
 
@@ -148,35 +157,35 @@
     :type quiet: bool, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 4
-    images = _np.empty([1024, 256, predicted_num_frames], dtype=__SPECTROGRAPH_DT)
+    images = np.empty([1024, 256, predicted_num_frames], dtype=__SPECTROGRAPH_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
     # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = _signal.signal(_signal.SIGINT, _signal.SIG_IGN)
-    pool = _Pool(processes=workers)
-    _signal.signal(_signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+    pool = Pool(processes=workers)
+    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
 
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
     # call readfile function, run each iteration with a single input file from file_list
     # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
     data = []
     try:
-        data = pool.map(_partial(__spectrograph_readfile_worker, quiet=quiet), file_list)
+        data = pool.map(partial(__spectrograph_readfile_worker, quiet=quiet), file_list)
     except KeyboardInterrupt:
         pool.terminate()  # gracefully kill children
-        return _np.empty((0, 0, 0), dtype=__SPECTROGRAPH_DT), [], []
+        return np.empty((0, 0, 0), dtype=__SPECTROGRAPH_DT), [], []
     else:
         pool.close()
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
@@ -197,15 +206,15 @@
         # metadata dictionary list at data[][1]
         metadata_dict_list[list_position:list_position + real_num_frames] = data[i][1]
         images[:, :, list_position:list_position + real_num_frames] = data[i][0]  # image arrays at data[][0]
         list_position = list_position + real_num_frames  # advance list position
 
     # trim unused elements from predicted array sizes
     metadata_dict_list = metadata_dict_list[0:list_position]
-    images = _np.delete(images, range(list_position, predicted_num_frames), axis=2)
+    images = np.delete(images, range(list_position, predicted_num_frames), axis=2)
 
     # ensure entire array views as uint16
-    images = images.astype(_np.uint16)
+    images = images.astype(np.uint16)
 
     # return
     data = None
     return images, metadata_dict_list, problematic_file_list
```

