# Comparing `tmp/audioviz-0.1.4.tar.gz` & `tmp/audioviz-0.1.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.1.4.tar", last modified: Sat Apr 29 03:34:31 2023, max compression
+gzip compressed data, was "audioviz-0.1.5.dev0.tar", last modified: Fri May  5 03:26:26 2023, max compression
```

## Comparing `audioviz-0.1.4.tar` & `audioviz-0.1.5.dev0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-29 03:34:31.307517 audioviz-0.1.4/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      684 2023-04-29 03:34:31.307517 audioviz-0.1.4/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1258 2023-04-25 05:51:15.000000 audioviz-0.1.4/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-29 03:34:31.307517 audioviz-0.1.4/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.4/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9467 2023-04-23 03:57:05.000000 audioviz-0.1.4/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     3211 2023-04-23 03:57:05.000000 audioviz-0.1.4/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.4/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.4/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.4/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      264 2023-04-29 03:28:24.000000 audioviz-0.1.4/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.4/audioviz/colabInterface.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      708 2023-04-29 03:30:14.000000 audioviz-0.1.4/audioviz/utils.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-04-29 03:34:31.307517 audioviz-0.1.4/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      684 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      446 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.4/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       51 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-04-29 03:34:31.000000 audioviz-0.1.4/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-04-29 03:34:31.307517 audioviz-0.1.4/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1122 2023-04-29 03:33:20.000000 audioviz-0.1.4/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-05 03:26:26.001868 audioviz-0.1.5.dev0/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      689 2023-05-05 03:26:26.001868 audioviz-0.1.5.dev0/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1258 2023-04-25 05:51:15.000000 audioviz-0.1.5.dev0/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-05 03:26:25.997868 audioviz-0.1.5.dev0/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.5.dev0/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.5.dev0/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.5.dev0/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2653 2023-05-05 03:17:01.000000 audioviz-0.1.5.dev0/audioviz/Panel.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.5.dev0/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.5.dev0/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.5.dev0/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      284 2023-05-05 03:18:02.000000 audioviz-0.1.5.dev0/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.5.dev0/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1077 2023-04-30 07:26:37.000000 audioviz-0.1.5.dev0/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-05 03:26:26.001868 audioviz-0.1.5.dev0/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      689 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.5.dev0/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       69 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-05 03:26:26.001868 audioviz-0.1.5.dev0/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1197 2023-05-05 03:25:30.000000 audioviz-0.1.5.dev0/setup.py
```

### Comparing `audioviz-0.1.4/PKG-INFO` & `audioviz-0.1.5.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.4
+Version: 0.1.5.dev0
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.1.4/README.md` & `audioviz-0.1.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.4/audioviz/BeatAnalysis.py` & `audioviz-0.1.5.dev0/audioviz/BeatAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.4/audioviz/ChordAnalysis.py` & `audioviz-0.1.5.dev0/audioviz/ChordAnalysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,39 @@
 import librosa
 import libfmp.b
 import libfmp.c3
 import libfmp.c4
 
 from .colabInterface import *
 
+def simple_chord(filename: str) -> None:
+    
+    dcp = DeepChromaProcessor()
+    decode = DeepChromaChordRecognitionProcessor()
+    chroma = dcp(filename)
+    chrod_rec_res = decode(chroma)
+    
+    chord_seq = [c[2] for c in chrod_rec_res]
+    time_slice = [np.round(c[0], 1) for c in chrod_rec_res]
+    end_time = np.round(chrod_rec_res[-1][1], 1)
+    duration = np.arange(0, end_time, 0.1)
+    color_encode_list = list(set(chord_seq))
+    
+    chord_hm = np.ones((len(color_encode_list), len(duration)))
+    for i in range(1, len(time_slice)):
+        chord_hm[color_encode_list.index(chord_seq[i-1])][int(time_slice[i-1]*10):int(time_slice[i]*10)] = 0
+        
+    plt.figure(figsize=(30, 12))
+    plt.imshow(chord_hm, interpolation='none', cmap='spring', aspect='auto')
+    plt.xticks(np.arange(0, len(duration), 300), duration[::300])
+    plt.xlabel('Time (seconds)')
+    plt.yticks(np.arange(0, len(color_encode_list)), color_encode_list)
+    plt.ylabel('Chord')
+    plt.title('Chord recognition')
+
 def compute_chromagram_from_filename(fn_wav, Fs=22050, N=4096, H=2048, gamma=None, version='STFT', norm='2'):
     """Compute chromagram for WAV file specified by filename
 
     Notebook: C5/C5S2_ChordRec_Templates.ipynb
 
     Args:
         fn_wav (str): Filenname of WAV
```

### Comparing `audioviz-0.1.4/audioviz/GeneralAnalysis.py` & `audioviz-0.1.5.dev0/audioviz/GeneralAnalysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,46 +4,33 @@
 import plotly.graph_objects as go
 
 from numpy import typing as npt
 
 from .colabInterface import *
 
 
-def plot_waveform(y: npt.ArrayLike, sr: int, start_time: float = 0.0, end_time: float = None) -> None :
+def plot_waveform(y: npt.ArrayLike, sr: int) -> None :
     
     '''
     To show the waveform in time domain of a sound file
 
     y: input signal
     sr: sampling rate (22050 Hz by default)
     '''
 
-    startIdx = int(start_time * sr)
     fig = go.Figure()
     config = {'scrollZoom': True}
     
-    if not end_time :
-        times = 1 / sr * np.arange(startIdx, len(y))
-        fig.add_trace(go.Scatter(x = times, y = y[startIdx:],
-                        mode = 'lines'))
-        fig.update_layout(title='Waveform',
+    times = 1 / sr * np.arange(len(y))
+    fig.add_trace(go.Scatter(x = times, y = y,
+                    mode = 'lines'))
+    fig.update_layout(title='Waveform',
                     xaxis_title='Time (sec)',
                     yaxis_title='Amplitude')
-        fig.show(config=config)
-    
-    else :
-        endIdx = int(end_time * sr)
-        times = 1 / sr * np.arange(startIdx, endIdx)
-        fig.add_trace(go.Scatter(x = times, y = y[startIdx:endIdx-1],
-                        mode = 'lines'))
-        fig.update_layout(title='Waveform',
-                    xaxis_title='Time (sec)',
-                    yaxis_title='Amplitude')
-        fig.show(config=config)
-
+    fig.show(config=config)
 
 def signal_RMS_analysis(y: npt.ArrayLike) :
 
     '''
     To show the RMS amplitude in time domain of a sound file
 
     y: input signal
```

### Comparing `audioviz-0.1.4/audioviz/PitchAnalysis.py` & `audioviz-0.1.5.dev0/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.4/audioviz/StructureAnalysis.py` & `audioviz-0.1.5.dev0/audioviz/StructureAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.4/audioviz/TimbreAnalysis.py` & `audioviz-0.1.5.dev0/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.4/audioviz/colabInterface.py` & `audioviz-0.1.5.dev0/audioviz/colabInterface.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.4/audioviz.egg-info/PKG-INFO` & `audioviz-0.1.5.dev0/audioviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.4
+Version: 0.1.5.dev0
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.1.4/setup.py` & `audioviz-0.1.5.dev0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.1.4',
+    version='0.1.5dev',
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
 
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
     author_email='andrew.chuang@gapp.nthu.edu.tw',
     license='MIT',
     zip_safe=False,
     keywords=['Music Information Retrieval', "Academia Sinica", "NTHU"],
 
     install_requires = ["numpy", 
+                        "matplotlib",
+                        "pandas",
                         "scipy", 
                         "librosa", 
                         "madmom", 
                         "libfmp", 
                         "plotly",
                         "soundfile",
                         ],
```

