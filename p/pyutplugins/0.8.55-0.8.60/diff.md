# Comparing `tmp/pyutplugins-0.8.55.tar.gz` & `tmp/pyutplugins-0.8.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutplugins-0.8.55.tar", last modified: Tue Apr 18 14:00:20 2023, max compression
+gzip compressed data, was "pyutplugins-0.8.60.tar", last modified: Fri May  5 01:33:48 2023, max compression
```

## Comparing `pyutplugins-0.8.55.tar` & `pyutplugins-0.8.60.tar`

### file list

```diff
@@ -1,149 +1,147 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.319635 pyutplugins-0.8.55/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-04-18 14:00:20.319508 pyutplugins-0.8.55/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1956 2023-04-14 20:22:33.000000 pyutplugins-0.8.55/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.304290 pyutplugins-0.8.55/pyutplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6400 2023-01-04 04:59:38.000000 pyutplugins-0.8.55/pyutplugins/ExternalTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-01-20 18:33:44.000000 pyutplugins-0.8.55/pyutplugins/IPluginAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8054 2023-03-31 00:30:02.000000 pyutplugins-0.8.55/pyutplugins/PluginManager.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.305427 pyutplugins-0.8.55/pyutplugins/common/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1130 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/common/ElementTreeData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2353 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/common/LinkMakerMixin.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-01-19 02:57:18.000000 pyutplugins-0.8.55/pyutplugins/common/PluginTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/common/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/common/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.306096 pyutplugins-0.8.55/pyutplugins/common/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-01-20 15:07:17.000000 pyutplugins-0.8.55/pyutplugins/common/ui/BaseEditDialog.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      705 2023-01-19 02:57:28.000000 pyutplugins-0.8.55/pyutplugins/common/ui/Dimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2505 2023-01-20 15:07:17.000000 pyutplugins-0.8.55/pyutplugins/common/ui/DimensionsControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4602 2023-02-01 03:01:55.000000 pyutplugins-0.8.55/pyutplugins/common/ui/DualSpinnerControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/common/ui/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.306304 pyutplugins-0.8.55/pyutplugins/common/ui/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5181 2023-02-05 15:39:41.000000 pyutplugins-0.8.55/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-01 02:55:47.000000 pyutplugins-0.8.55/pyutplugins/common/ui/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/common/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.306830 pyutplugins-0.8.55/pyutplugins/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/exceptions/InvalidPluginExtensionException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/exceptions/InvalidPluginNameException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/exceptions/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/exceptions/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.308146 pyutplugins-0.8.55/pyutplugins/ioplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1924 2023-01-20 18:45:21.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IOAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IODTD.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IOGML.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IOJava.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-01-30 01:49:48.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IOMermaid.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3864 2023-02-03 02:52:30.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IOPdf.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7373 2023-01-20 18:45:21.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IOPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IOWxImage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8266 2023-01-30 01:49:48.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/IOXml.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.308772 pyutplugins-0.8.55/pyutplugins/ioplugins/dtd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/dtd/DTDAttribute.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/dtd/DTDElementTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10397 2023-01-20 18:33:44.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/dtd/DTDParser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/dtd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/dtd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.309195 pyutplugins-0.8.55/pyutplugins/ioplugins/gml/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8647 2023-02-01 01:59:25.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/gml/GMLExporter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/gml/UnsupportedOperation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/gml/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/gml/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.309751 pyutplugins-0.8.55/pyutplugins/ioplugins/java/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    27944 2023-01-20 18:45:21.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/java/JavaReader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11156 2023-02-01 01:52:43.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/java/JavaWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/java/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/java/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.310326 pyutplugins-0.8.55/pyutplugins/ioplugins/mermaid/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-02-01 20:38:32.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/mermaid/MermaidDirection.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12464 2023-04-17 23:17:22.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/mermaid/MermaidWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-30 01:49:48.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/mermaid/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/mermaid/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.310974 pyutplugins-0.8.55/pyutplugins/ioplugins/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/pdf/ImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/pdf/ImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9553 2023-01-20 18:33:44.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/pdf/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/pdf/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.312132 pyutplugins-0.8.55/pyutplugins/ioplugins/python/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3579 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/Python3LexerBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      192 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/Python3ParserBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/PythonParseException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12836 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/PyutPythonVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12487 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/PyutToPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    17467 2023-01-20 18:33:44.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/ReverseEngineerPython2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.313105 pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    47673 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   399206 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    37475 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    22412 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      804 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/python/transformGrammar.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.313632 pyutplugins-0.8.55/pyutplugins/ioplugins/wximage/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4854 2023-01-20 15:07:17.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/wximage/WxImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/wximage/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/ioplugins/wximage/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.314273 pyutplugins-0.8.55/pyutplugins/plugininterfaces/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11799 2023-01-30 01:49:48.000000 pyutplugins-0.8.55/pyutplugins/plugininterfaces/BasePluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-01-20 21:59:06.000000 pyutplugins-0.8.55/pyutplugins/plugininterfaces/IOPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-01-20 15:37:30.000000 pyutplugins-0.8.55/pyutplugins/plugininterfaces/ToolPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/plugininterfaces/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/plugininterfaces/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.315691 pyutplugins-0.8.55/pyutplugins/plugintypes/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-02-03 02:56:53.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/BaseFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/BaseRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/ExportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/ImportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/InputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-01-20 18:45:21.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/MultipleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/OutputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/PluginDataTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-01-20 18:45:21.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/SingleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/plugintypes/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.316045 pyutplugins-0.8.55/pyutplugins/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7651 2023-03-31 00:30:24.000000 pyutplugins-0.8.55/pyutplugins/preferences/PluginPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-18 02:02:54.000000 pyutplugins-0.8.55/pyutplugins/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutplugins-0.8.55/pyutplugins/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.316933 pyutplugins-0.8.55/pyutplugins/toolplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1730 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/ToolArrangeLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3592 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/ToolAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2023-01-20 18:45:21.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/ToolSugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-01-20 18:45:20.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/ToolTransforms.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.317697 pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1994 2023-01-20 15:07:17.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-01-19 03:33:52.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-01-20 18:33:44.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.319339 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3545 2023-02-22 02:39:48.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28462 2023-02-01 01:51:21.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/Sugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-01-20 15:25:55.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-18 14:00:20.304869 pyutplugins-0.8.55/pyutplugins.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-04-18 14:00:20.000000 pyutplugins-0.8.55/pyutplugins.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5226 2023-04-18 14:00:20.000000 pyutplugins-0.8.55/pyutplugins.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-18 14:00:20.000000 pyutplugins-0.8.55/pyutplugins.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      203 2023-04-18 14:00:20.000000 pyutplugins-0.8.55/pyutplugins.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-18 14:00:20.000000 pyutplugins-0.8.55/pyutplugins.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-18 14:00:20.319671 pyutplugins-0.8.55/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     3207 2023-04-18 13:35:51.000000 pyutplugins-0.8.55/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.783559 pyutplugins-0.8.60/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-05-05 01:33:48.783406 pyutplugins-0.8.60/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1956 2023-04-14 20:22:33.000000 pyutplugins-0.8.60/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.768492 pyutplugins-0.8.60/pyutplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6400 2023-01-04 04:59:38.000000 pyutplugins-0.8.60/pyutplugins/ExternalTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-01-20 18:33:44.000000 pyutplugins-0.8.60/pyutplugins/IPluginAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8054 2023-03-31 00:30:02.000000 pyutplugins-0.8.60/pyutplugins/PluginManager.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.769621 pyutplugins-0.8.60/pyutplugins/common/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1130 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/ElementTreeData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2353 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/LinkMakerMixin.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-01-19 02:57:18.000000 pyutplugins-0.8.60/pyutplugins/common/PluginTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.769919 pyutplugins-0.8.60/pyutplugins/common/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-01-20 15:07:17.000000 pyutplugins-0.8.60/pyutplugins/common/ui/BaseEditDialog.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/ui/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.770163 pyutplugins-0.8.60/pyutplugins/common/ui/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5175 2023-05-03 19:43:51.000000 pyutplugins-0.8.60/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-01 02:55:47.000000 pyutplugins-0.8.60/pyutplugins/common/ui/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/common/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.770756 pyutplugins-0.8.60/pyutplugins/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/InvalidPluginExtensionException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/InvalidPluginNameException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/exceptions/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.771988 pyutplugins-0.8.60/pyutplugins/ioplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1924 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IODTD.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOGML.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOJava.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-01-30 01:49:48.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOMermaid.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3864 2023-02-03 02:52:30.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOPdf.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7942 2023-05-05 01:14:03.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOWxImage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8266 2023-01-30 01:49:48.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/IOXml.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.772533 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/DTDAttribute.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/DTDElementTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10397 2023-01-20 18:33:44.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/DTDParser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.772995 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8647 2023-02-01 01:59:25.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/GMLExporter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/UnsupportedOperation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/gml/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.773468 pyutplugins-0.8.60/pyutplugins/ioplugins/java/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    27944 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/java/JavaReader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11156 2023-02-01 01:52:43.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/java/JavaWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/java/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/java/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.773929 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-02-01 20:38:32.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/MermaidDirection.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12464 2023-04-17 23:17:22.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/MermaidWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-30 01:49:48.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.774492 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/ImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/ImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9553 2023-01-20 18:33:44.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.775671 pyutplugins-0.8.60/pyutplugins/ioplugins/python/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-05-05 01:14:03.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3579 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/Python3LexerBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      192 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/Python3ParserBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/PythonParseException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12836 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/PyutPythonVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12487 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/PyutToPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    18319 2023-05-05 01:14:03.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/ReverseEngineerPython2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.776577 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    47673 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   399206 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    37475 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    22412 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      804 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/python/transformGrammar.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.777006 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4853 2023-05-05 01:14:03.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/WxImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.777521 pyutplugins-0.8.60/pyutplugins/plugininterfaces/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11797 2023-05-03 19:43:51.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/BasePluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-01-20 21:59:06.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/IOPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-01-20 15:37:30.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/ToolPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugininterfaces/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.778739 pyutplugins-0.8.60/pyutplugins/plugintypes/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-02-03 02:56:53.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/BaseFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/BaseRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/ExportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/ImportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/InputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/MultipleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/OutputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/PluginDataTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/SingleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/plugintypes/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.779050 pyutplugins-0.8.60/pyutplugins/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7651 2023-03-31 00:30:24.000000 pyutplugins-0.8.60/pyutplugins/preferences/PluginPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-18 02:02:54.000000 pyutplugins-0.8.60/pyutplugins/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutplugins-0.8.60/pyutplugins/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.780276 pyutplugins-0.8.60/pyutplugins/toolplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1730 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolArrangeLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3592 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2023-01-20 18:45:21.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolSugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-01-20 18:45:20.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/ToolTransforms.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.781273 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1996 2023-05-03 19:43:51.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-01-19 03:33:52.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-01-20 18:33:44.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.783219 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3545 2023-02-22 02:39:48.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28462 2023-02-01 01:51:21.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/Sugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-01-20 15:25:55.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-05 01:33:48.769069 pyutplugins-0.8.60/pyutplugins.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5161 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      203 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-05-05 01:33:48.000000 pyutplugins-0.8.60/pyutplugins.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-05 01:33:48.783600 pyutplugins-0.8.60/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3207 2023-05-03 19:43:51.000000 pyutplugins-0.8.60/setup.py
```

### Comparing `pyutplugins-0.8.55/LICENSE` & `pyutplugins-0.8.60/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/PKG-INFO` & `pyutplugins-0.8.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 0.8.55
+Version: 0.8.60
 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 0.8.55 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 0.8.60 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins Author: Humberto A. Sanchez
 II Author-email: humberto.a.sanchez.ii@gmail.com Maintainer: Humberto A.
 Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com Description-
 Content-Type: text/markdown License-File: LICENSE [./developer/agpl-license-
 web-badge-version-2-256x48.png] [![Maintenance](https://img.shields.io/badge/
 Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
 commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
```

### Comparing `pyutplugins-0.8.55/README.md` & `pyutplugins-0.8.60/README.md`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ExternalTypes.py` & `pyutplugins-0.8.60/pyutplugins/ExternalTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/IPluginAdapter.py` & `pyutplugins-0.8.60/pyutplugins/IPluginAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/PluginManager.py` & `pyutplugins-0.8.60/pyutplugins/PluginManager.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/common/ElementTreeData.py` & `pyutplugins-0.8.60/pyutplugins/common/ElementTreeData.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/common/LinkMakerMixin.py` & `pyutplugins-0.8.60/pyutplugins/common/LinkMakerMixin.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/common/ui/BaseEditDialog.py` & `pyutplugins-0.8.60/pyutplugins/common/ui/BaseEditDialog.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/common/ui/preferences/PluginPreferencesPage.py` & `pyutplugins-0.8.60/pyutplugins/common/ui/preferences/PluginPreferencesPage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List
 from typing import cast
 
 from logging import Logger
 from logging import getLogger
 
-
 from wx import EVT_CHECKBOX
 from wx import EVT_CHOICE
 from wx import EVT_TEXT
 from wx import ID_ANY
 
 from wx import CommandEvent
 from wx import StaticText
@@ -18,18 +17,22 @@
 from wx import Choice
 
 from wx import NewIdRef as wxNewIdRef
 
 from wx.lib.sized_controls import SizedPanel
 from wx.lib.sized_controls import SizedStaticBox
 
-from pyutplugins.common.ui.Dimensions import Dimensions
-from pyutplugins.common.ui.DimensionsControl import DimensionsControl
+from hasiihelper.Dimensions import Dimensions
+
+from hasiicommon.ui.widgets.DimensionsControl import DimensionsControl
+
 from pyutplugins.ioplugins.mermaid.MermaidDirection import MermaidDirection
+
 from pyutplugins.preferences.PluginPreferences import PluginPreferences
+
 from pyutplugins.toolplugins.orthogonal.LayoutAreaSize import LayoutAreaSize
 
 
 class PluginPreferencesPage(SizedPanel):
 
     def __init__(self, parent: Window):
         self.logger: Logger = getLogger(__name__)
```

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IOAscii.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IOAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IODTD.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IODTD.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IOGML.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IOGML.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IOJava.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IOJava.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IOMermaid.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IOMermaid.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IOPdf.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IOPdf.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IOPython.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IOPython.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,30 +24,34 @@
 
 from wx import Yield as wxYield
 
 from pyutplugins.IPluginAdapter import IPluginAdapter
 from pyutplugins.plugininterfaces.IOPluginInterface import IOPluginInterface
 
 from pyutplugins.ExternalTypes import OglClasses
-from pyutplugins.ExternalTypes import OglLinks
 from pyutplugins.ExternalTypes import OglObjects
 
 from pyutplugins.plugintypes.PluginDataTypes import PluginExtension
 from pyutplugins.plugintypes.PluginDataTypes import PluginName
 from pyutplugins.plugintypes.PluginDataTypes import FormatName
 from pyutplugins.plugintypes.PluginDataTypes import PluginDescription
 
 from pyutplugins.plugintypes.ExportDirectoryResponse import ExportDirectoryResponse
-from pyutplugins.plugintypes.MultipleFileRequestResponse import MultipleFileRequestResponse
 from pyutplugins.plugintypes.InputFormat import InputFormat
 from pyutplugins.plugintypes.OutputFormat import OutputFormat
 
 from pyutplugins.ioplugins.python.PyutToPython import MethodsCodeType
 from pyutplugins.ioplugins.python.PyutToPython import PyutToPython
+
 from pyutplugins.ioplugins.python.ReverseEngineerPython2 import ReverseEngineerPython2
+from pyutplugins.ioplugins.python.ReverseEngineerPython2 import OglClassesDict
+from pyutplugins.ioplugins.python.DlgSelectMultiplePackages import DlgSelectMultiplePackages
+from pyutplugins.ioplugins.python.DlgSelectMultiplePackages import ImportPackages
+from pyutplugins.ioplugins.python.DlgSelectMultiplePackages import Package
+
 
 FORMAT_NAME:        FormatName        = FormatName("Python File(s)")
 PLUGIN_EXTENSION:   PluginExtension   = PluginExtension('py')
 PLUGIN_DESCRIPTION: PluginDescription = PluginDescription('Python code generation and reverse engineering')
 
 
 class IOPython(IOPluginInterface):
@@ -61,34 +65,38 @@
         # from super class
         self._name    = PluginName('IOPython')
         self._author  = 'Humberto A. Sanchez II'
         self._version = '1.0'
         self._inputFormat  = InputFormat(formatName=FORMAT_NAME, extension=PLUGIN_EXTENSION, description=PLUGIN_DESCRIPTION)
         self._outputFormat = OutputFormat(formatName=FORMAT_NAME, extension=PLUGIN_EXTENSION, description=PLUGIN_DESCRIPTION)
 
-        self._exportDirectoryName: str         = ''
-        self._importDirectoryName: str         = ''
-        self._filesToImport:       List['str'] = []
+        self._exportDirectoryName: str            = ''
+
+        self._importPackages: ImportPackages = ImportPackages([])
+        self._packageCount:   int = 0
+        self._moduleCount:    int = 0
 
-        self._readProgressDlg: ProgressDialog = cast(ProgressDialog, None)
+        self._readProgressDlg:     ProgressDialog = cast(ProgressDialog, None)
 
     def setImportOptions(self) -> bool:
         """
         We do need to ask for the input file names
 
         Returns:  'True', we support import
         """
-        response: MultipleFileRequestResponse = self.askToImportMultipleFiles(startDirectory=None)
-        if response.cancelled is True:
-            return False
-        else:
-            self._importDirectoryName = response.directoryName
-            self._filesToImport   = response.fileList
 
-        return True
+        with DlgSelectMultiplePackages(startDirectory='/Users/humberto.a.sanchez.ii/pyut-diagrams', inputFormat=self.inputFormat) as dlg:
+            if dlg.ShowModal() == OK:
+                self._packageCount   = dlg.packageCount
+                self._moduleCount    = dlg.moduleCount
+                self._importPackages = dlg.importPackages
+
+                return True
+            else:
+                return False
 
     def setExportOptions(self) -> bool:
         response: ExportDirectoryResponse = self.askForExportDirectoryName(preferredDefaultPath=None)
         if response.cancelled is True:
             return False
         else:
             self._exportDirectoryName = response.directoryName
@@ -99,36 +107,39 @@
 
         Returns:
         """
         BeginBusyCursor()
         wxYield()
         status: bool = True
         try:
+            self._readProgressDlg = ProgressDialog('Parsing Files', 'Starting', parent=None, style=PD_APP_MODAL | PD_ELAPSED_TIME)
+            oglClassesDict:  OglClassesDict         = OglClassesDict({})
             reverseEngineer: ReverseEngineerPython2 = ReverseEngineerPython2()
 
-            fileCount: int        = len(self._filesToImport)
-            self._readProgressDlg = ProgressDialog('Parsing Files', 'Starting',  parent=None, style=PD_APP_MODAL | PD_ELAPSED_TIME)
-            self._readProgressDlg.SetRange(fileCount)
-
-            reverseEngineer.reversePython(directoryName=self._importDirectoryName, files=self._filesToImport, progressCallback=self._readProgressCallback)
-            oglClasses: OglClasses = reverseEngineer.oglClasses
-            oglLinks:   OglLinks   = reverseEngineer.oglLinks()
+            self._readProgressDlg.SetRange(self._moduleCount)
 
-            self.logger.warning(f'Classes: {oglClasses}')
-            self.logger.warning(f'Links:   {oglLinks}')
+            for directory in self._importPackages:
+                importPackage: Package = cast(Package, directory)
 
-            self._layoutUmlClasses(oglClasses=oglClasses)
-            self._layoutLinks(oglLinks=oglLinks)
+                reverseEngineer.reversePython(directoryName=importPackage.packageName, files=importPackage.moduleToImport, progressCallback=self._readProgressCallback)
+                oglClassesDict.update(reverseEngineer.oglClasses)
+                self.logger.warning(f'Classes: {oglClassesDict}')
+
+            reverseEngineer.generateInheritanceLinks(oglClassesDict)
+            self._layoutUmlClasses(oglClasses=OglClasses(list(oglClassesDict.values())))
+            self._layoutLinks(oglLinks=reverseEngineer.oglLinks)
         except (ValueError, Exception) as e:
             self._readProgressDlg.Destroy()
             MessageBox(f'{e}', 'Error', OK | ICON_ERROR)
             status = False
         else:
             self._readProgressDlg.Destroy()
             EndBusyCursor()
+            self._pluginAdapter.refreshFrame()
+            wxYield()
             self._pluginAdapter.indicatePluginModifiedProject()
         return status
 
     def write(self, oglObjects: OglObjects):
 
         directoryName: str = self._exportDirectoryName
```

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IOWxImage.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IOWxImage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/IOXml.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/IOXml.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/dtd/DTDParser.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/dtd/DTDParser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/gml/GMLExporter.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/gml/GMLExporter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/java/JavaReader.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/java/JavaReader.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/java/JavaWriter.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/java/JavaWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/mermaid/MermaidDirection.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/MermaidDirection.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/mermaid/MermaidWriter.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/mermaid/MermaidWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/pdf/ImageOptions.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/ImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/Python3LexerBase.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/Python3LexerBase.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/PyutPythonVisitor.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/PyutPythonVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/PyutToPython.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/PyutToPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/ReverseEngineerPython2.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/ReverseEngineerPython2.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,86 +51,119 @@
 
 PyutClassName  = NewType('PyutClassName', str)
 PyutClasses    = NewType('PyutClasses', Dict[PyutClassName, PyutClass])
 OglClassesDict = NewType('OglClassesDict', Dict[Union[PyutClassName, ParentName, ChildName, ClassName], OglClass])
 
 
 class ReverseEngineerPython2(LinkMakerMixin):
+    """
+    How to use this code
+
+    After instance initialization call the .reversePython method with the necessary parameters.  That method populates a dictionary
+    of class names to OglClasses;  After it returns the caller captures the parsed Ogl classes vi the .oglClasses property.  Through
+    each call with a different package and module names the class is updating a dictionary of classes that are parents.
+    The dictionary is keyed by the name of the class that is a parent class.  The value is a list of class names that
+    are subclasses (aka children)
+
+    TODO:
+
+    This interaction is weird;  I think this class should keep track of all internal state
+    """
 
     PYTHON_ASSIGNMENT:     str = '='
     PYTHON_TYPE_DELIMITER: str = ':'
     PYTHON_EOL_COMMENT:    str = '#'
 
     def __init__(self):
 
         super().__init__()
         self.logger: Logger = getLogger(__name__)
 
         self._pyutClasses:    PyutClasses     = PyutClasses({})
         self._oglClassesDict: OglClassesDict  = OglClassesDict({})
         self._oglClasses:     OglClasses      = cast(OglClasses, None)
         self._oglLinks:       OglLinks        = OglLinks([])
+        self._onGoingParents: Parents = Parents({})
 
         self.visitor: PyutPythonVisitor = cast(PyutPythonVisitor, None)
 
     def reversePython(self,  directoryName: str, files: List[str], progressCallback: Callable):
         """
         Reverse engineering Python files to OglClass's
 
         Args:
             directoryName:  The directory name where the selected files reside
             files:          A list of files to parse
             progressCallback: The method to call to report progress
         """
         currentFileCount: int = 0
 
-        onGoingParents: Parents = Parents({})
+        self._pyutClasses    = PyutClasses({})
+        self._oglClassesDict = OglClassesDict({})
+        self._oglClasses     = cast(OglClasses, None)
+        self._oglLinks       = OglLinks([])
+
         for fileName in files:
 
             try:
                 fqFileName: str = f'{directoryName}{osSep}{fileName}'
                 self.logger.info(f'Processing file: {fqFileName}')
 
-                progressCallback(currentFileCount, f'Processing: {fileName}')
+                progressCallback(currentFileCount, f'Processing: {directoryName}\n {fileName}')
 
                 fileStream: FileStream   = FileStream(fqFileName)
                 lexer:      Python3Lexer = Python3Lexer(fileStream)
 
                 stream: CommonTokenStream = CommonTokenStream(lexer)
                 parser: Python3Parser     = Python3Parser(stream)
 
                 tree: Python3Parser.File_inputContext = parser.file_input()
                 if parser.getNumberOfSyntaxErrors() != 0:
                     eMsg: str = f"File {fileName} contains {parser.getNumberOfSyntaxErrors()} syntax errors"
                     self.logger.error(eMsg)
                     raise PythonParseException(eMsg)
 
                 self.visitor = PyutPythonVisitor()
-                self.visitor.parents = onGoingParents
+                self.visitor.parents = self._onGoingParents
                 self.visitor.visit(tree)
                 self._generatePyutClasses()
 
-                onGoingParents = self.visitor.parents
+                self._onGoingParents = self.visitor.parents
                 currentFileCount += 1
             except (ValueError, Exception) as e:
                 self.logger.error(e)
                 raise PythonParseException(e)
         self._generateOglClasses()
-        self._generateInheritanceLinks()
+        # self._generateInheritanceLinks()
 
     @property
-    def oglClasses(self) -> OglClasses:
-        if self._oglClasses is None:
-            self._oglClasses = list(self._oglClassesDict.values())
-
-        return self._oglClasses
+    def oglClasses(self) -> OglClassesDict:
+        return self._oglClassesDict
 
+    @property
     def oglLinks(self) -> OglLinks:
         return self._oglLinks
 
+    def generateInheritanceLinks(self, oglClassesDict: OglClassesDict):
+
+        parents: Parents = self._onGoingParents
+
+        for parentName in parents.keys():
+            children: Children = parents[parentName]
+            for childName in children:
+
+                try:
+                    parentOglClass: OglClass = oglClassesDict[parentName]
+                    childOglClass:  OglClass = oglClassesDict[childName]
+                    oglLink: OglLink = self.createLink(src=childOglClass, dst=parentOglClass, linkType=PyutLinkType.INHERITANCE)
+                    self._oglLinks.append(oglLink)
+                except KeyError as ke:        # Probably there is no parent we are tracking
+                    self.logger.warning(f'Apparently we are not tracking this parent:  {ke}')
+                    continue
+
     def _generateOglClasses(self):
 
         for pyutClassName in self._pyutClasses:
             try:
                 pyutClass: PyutClass = self._pyutClasses[pyutClassName]
                 oglClass:  OglClass  = OglClass(pyutClass)
 
@@ -258,31 +291,14 @@
         for fieldData in self.visitor.fields:
             self.logger.debug(f'fieldData: {fieldData}')
             pyutField: PyutField = self._parseFieldToPyut(fieldData)
             pyutClass.addField(pyutField)
 
         return pyutClass
 
-    def _generateInheritanceLinks(self):
-
-        parents: Parents = self.visitor.parents
-
-        for parentName in parents.keys():
-            children: Children = parents[parentName]
-            for childName in children:
-
-                try:
-                    parentOglClass: OglClass = self._oglClassesDict[parentName]
-                    childOglClass:  OglClass = self._oglClassesDict[childName]
-                    oglLink: OglLink = self.createLink(src=childOglClass, dst=parentOglClass, linkType=PyutLinkType.INHERITANCE)
-                    self._oglLinks.append(oglLink)
-                except KeyError as ke:        # Probably there is no parent we are tracking
-                    self.logger.warning(f'Apparently we are not tracking this parent:  {ke}')
-                    continue
-
     def _methodNames(self, className: ClassName) -> MethodNames:
 
         methodNames: MethodNames = MethodNames([])
         try:
             methodNames = self.visitor.classMethods[className]
         except KeyError:
             self.logger.warning(f'{className} has no methods')
```

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/python/transformGrammar.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/python/transformGrammar.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,20 +50,16 @@
         self._outputFileName: str           = PluginPreferences().wxImageFileName
         self._imageFormat:    WxImageFormat = WxImageFormat.PNG
 
         self._layoutFileSelection(parent=self.GetContentsPane())
         self._layoutImageFormatChoice(parent=self.GetContentsPane())
 
         self._layoutStandardOkCancelButtonSizer()
-
         self._bindEventHandlers()
 
-        self.Bind(EVT_BUTTON, self._onOk, id=ID_OK)
-        self.Bind(EVT_CLOSE, self._onClose, id=ID_CANCEL)
-
     @property
     def imageFormat(self) -> WxImageFormat:
         return self._imageFormat
 
     @imageFormat.setter
     def imageFormat(self, newFormat: WxImageFormat):
         self._imageFormat = newFormat
@@ -78,14 +74,17 @@
 
     def _bindEventHandlers(self):
 
         self.Bind(EVT_BUTTON, self._onFileSelectClick,   self._fileSelectBtn)
         self.Bind(EVT_CHOICE, self._onImageFormatChoice, self._imageFormatChoice)
         #
         self._selectedFile.Bind(EVT_MOTION, self._fileSelectionMotion, self._selectedFile)
+        self.Bind(EVT_BUTTON, self._onOk, id=ID_OK)
+        self.Bind(EVT_CLOSE, self._onClose, id=ID_CANCEL)
+
 
     def _fileSelectionMotion(self, event: MouseEvent):
 
         ctrl: TextCtrl = event.GetEventObject()
 
         tip = ctrl.GetToolTip()
         tip.SetTip(self._outputFileName)
```

### Comparing `pyutplugins-0.8.55/pyutplugins/ioplugins/wximage/WxImageFormat.py` & `pyutplugins-0.8.60/pyutplugins/ioplugins/wximage/WxImageFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/plugininterfaces/BasePluginInterface.py` & `pyutplugins-0.8.60/pyutplugins/plugininterfaces/BasePluginInterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         Menu handlers may instantiate a plugin merely to get plugin information.  In that case,
         the input parameter will be None
 
         Args:
             pluginAdapter:   A class that implements ICommunicator
 
         """
-        self._pluginAdapter:     IPluginAdapter      = pluginAdapter
+        self._pluginAdapter:     IPluginAdapter    = pluginAdapter
         self._pluginPreferences: PluginPreferences = PluginPreferences()
 
         #
         # To be set by implementor constructor and read by property
         self._name:         PluginName = PluginName('Implementor must provide the plugin name')
         self._author:       str = 'Implementor must provide the plugin author'
         self._version:      str = 'Implementor must provide the version'
```

### Comparing `pyutplugins-0.8.55/pyutplugins/plugininterfaces/IOPluginInterface.py` & `pyutplugins-0.8.60/pyutplugins/plugininterfaces/IOPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/plugininterfaces/ToolPluginInterface.py` & `pyutplugins-0.8.60/pyutplugins/plugininterfaces/ToolPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/plugintypes/BaseFormat.py` & `pyutplugins-0.8.60/pyutplugins/plugintypes/BaseFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/plugintypes/InputFormat.py` & `pyutplugins-0.8.60/pyutplugins/plugintypes/InputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/plugintypes/OutputFormat.py` & `pyutplugins-0.8.60/pyutplugins/plugintypes/OutputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/plugintypes/PluginDataTypes.py` & `pyutplugins-0.8.60/pyutplugins/plugintypes/PluginDataTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/preferences/PluginPreferences.py` & `pyutplugins-0.8.60/pyutplugins/preferences/PluginPreferences.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/ToolArrangeLinks.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolArrangeLinks.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/ToolAscii.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/ToolSugiyama.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolSugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/ToolTransforms.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/ToolTransforms.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from typing import cast
 
 from logging import Logger
 from logging import getLogger
 
 from wx.lib.sized_controls import SizedPanel
 
-from pyutplugins.common.ui.DimensionsControl import DimensionsControl
+from hasiicommon.ui.widgets.DimensionsControl import DimensionsControl
+
 from pyutplugins.common.ui.BaseEditDialog import BaseEditDialog
 
 from pyutplugins.preferences.PluginPreferences import PluginPreferences
 
 from pyutplugins.toolplugins.orthogonal.LayoutAreaSize import LayoutAreaSize
```

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/ALayoutLink.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/ALayoutLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/ALayoutNode.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/ALayoutNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/Sugiyama.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/Sugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py` & `pyutplugins-0.8.60/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.55/pyutplugins.egg-info/PKG-INFO` & `pyutplugins-0.8.60/pyutplugins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 0.8.55
+Version: 0.8.60
 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 0.8.55 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 0.8.60 Summary: Pyut Plugins
 Home-page: https://github.com/hasii2011/pyutplugins Author: Humberto A. Sanchez
 II Author-email: humberto.a.sanchez.ii@gmail.com Maintainer: Humberto A.
 Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com Description-
 Content-Type: text/markdown License-File: LICENSE [./developer/agpl-license-
 web-badge-version-2-256x48.png] [![Maintenance](https://img.shields.io/badge/
 Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
 commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
```

### Comparing `pyutplugins-0.8.55/pyutplugins.egg-info/SOURCES.txt` & `pyutplugins-0.8.60/pyutplugins.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 pyutplugins.egg-info/top_level.txt
 pyutplugins/common/ElementTreeData.py
 pyutplugins/common/LinkMakerMixin.py
 pyutplugins/common/PluginTypes.py
 pyutplugins/common/__init__.py
 pyutplugins/common/py.typed
 pyutplugins/common/ui/BaseEditDialog.py
-pyutplugins/common/ui/Dimensions.py
-pyutplugins/common/ui/DimensionsControl.py
-pyutplugins/common/ui/DualSpinnerControl.py
 pyutplugins/common/ui/__init__.py
 pyutplugins/common/ui/py.typed
 pyutplugins/common/ui/preferences/PluginPreferencesPage.py
 pyutplugins/common/ui/preferences/__init__.py
 pyutplugins/exceptions/AbstractMethodNotImplementedException.py
 pyutplugins/exceptions/InvalidPluginExtensionException.py
 pyutplugins/exceptions/InvalidPluginNameException.py
@@ -58,14 +55,15 @@
 pyutplugins/ioplugins/mermaid/__init__.py
 pyutplugins/ioplugins/mermaid/py.typed
 pyutplugins/ioplugins/pdf/ImageFormat.py
 pyutplugins/ioplugins/pdf/ImageOptions.py
 pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
 pyutplugins/ioplugins/pdf/__init__.py
 pyutplugins/ioplugins/pdf/py.typed
+pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
 pyutplugins/ioplugins/python/Python3LexerBase.py
 pyutplugins/ioplugins/python/Python3ParserBase.py
 pyutplugins/ioplugins/python/PythonParseException.py
 pyutplugins/ioplugins/python/PyutPythonVisitor.py
 pyutplugins/ioplugins/python/PyutToPython.py
 pyutplugins/ioplugins/python/ReverseEngineerPython2.py
 pyutplugins/ioplugins/python/__init__.py
```

### Comparing `pyutplugins-0.8.55/setup.py` & `pyutplugins-0.8.60/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="pyutplugins",
-    version="0.8.55",
+    version="0.8.60",
     author='Humberto A. Sanchez II',
     author_email='humberto.a.sanchez.ii@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Pyut Plugins',
     long_description=README,
     long_description_content_type="text/markdown",
```

