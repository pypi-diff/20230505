# Comparing `tmp/openxes_cli_py-0.1.8.tar.gz` & `tmp/openxes_cli_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxes_cli_py-0.1.8.tar", max compression
+gzip compressed data, was "openxes_cli_py-0.1.9.tar", max compression
```

## Comparing `openxes_cli_py-0.1.8.tar` & `openxes_cli_py-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      744 2023-05-04 15:36:43.323321 openxes_cli_py-0.1.8/README.md
--rw-r--r--   0        0        0  3717531 2023-05-04 15:36:43.339321 openxes_cli_py-0.1.8/lib/openxes-cli.jar
--rw-r--r--   0        0        0      481 2023-05-04 15:36:43.339321 openxes_cli_py-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 15:36:43.339321 openxes_cli_py-0.1.8/src/openxes_cli/__init__.py
--rw-r--r--   0        0        0     1216 2023-05-04 15:36:43.339321 openxes_cli_py-0.1.8/src/openxes_cli/lib.py
--rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      744 2023-05-04 16:40:32.450478 openxes_cli_py-0.1.9/README.md
+-rw-r--r--   0        0        0  3718105 2023-05-04 16:40:32.478478 openxes_cli_py-0.1.9/lib/openxes-cli.jar
+-rw-r--r--   0        0        0      481 2023-05-04 16:40:32.478478 openxes_cli_py-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 16:40:32.478478 openxes_cli_py-0.1.9/src/openxes_cli/__init__.py
+-rw-r--r--   0        0        0     1216 2023-05-04 16:40:32.478478 openxes_cli_py-0.1.9/src/openxes_cli/lib.py
+-rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 openxes_cli_py-0.1.9/PKG-INFO
```

### Comparing `openxes_cli_py-0.1.8/README.md` & `openxes_cli_py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.8/lib/openxes-cli.jar` & `openxes_cli_py-0.1.9/lib/openxes-cli.jar`

 * *Files 0% similar despite different names*

#### zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 3717531 bytes, number of entries: 3013
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 18:33 META-INF/
+Zip file size: 3718105 bytes, number of entries: 3013
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 19:39 META-INF/
 -rw-r--r--  2.0 unx       67 b- defN 23-May-04 13:51 META-INF/MANIFEST.MF
 drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:19 ee/
 drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:19 ee/ut/
 drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:19 ee/ut/cs/
 drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 14:19 ee/ut/cs/sep/
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 18:33 ee/ut/cs/sep/openxescli/
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-04 19:35 ee/ut/cs/sep/openxescli/
 -rw-r--r--  2.0 unx     7140 b- defN 23-May-04 14:19 ee/ut/cs/sep/openxescli/Event.class
--rw-r--r--  2.0 unx     5199 b- defN 23-May-04 18:33 ee/ut/cs/sep/openxescli/CsvSerializer.class
+-rw-r--r--  2.0 unx     7439 b- defN 23-May-04 19:35 ee/ut/cs/sep/openxescli/CsvSerializer.class
 -rw-r--r--  2.0 unx     3164 b- defN 23-May-04 14:41 ee/ut/cs/sep/openxescli/Main.class
 -rw-r--r--  2.0 unx     6693 b- defN 23-May-04 14:19 ee/ut/cs/sep/openxescli/EventLog.class
--rw-r--r--  2.0 unx     4911 b- defN 23-May-04 18:33 ee/ut/cs/sep/openxescli/Converter.class
+-rw-r--r--  2.0 unx     4911 b- defN 23-May-04 19:35 ee/ut/cs/sep/openxescli/Converter.class
 -rw-r--r--  2.0 unx     2220 b- defN 23-May-04 14:19 ee/ut/cs/sep/openxescli/Trace.class
 drwxr-xr-x  2.0 unx        0 b- defN 15-May-27 16:27 org/
 drwxr-xr-x  2.0 unx        0 b- defN 15-May-27 16:27 org/deckfour/
 drwxr-xr-x  2.0 unx        0 b- defN 15-May-27 16:27 org/deckfour/xes/
 drwxr-xr-x  2.0 unx        0 b- defN 15-May-27 16:27 org/deckfour/xes/classification/
 -rw-r--r--  2.0 unx     1667 b- defN 17-Dec-08 11:48 org/deckfour/xes/classification/XEventAndClassifier.class
 -rw-r--r--  2.0 unx     4206 b- defN 17-Dec-12 15:41 org/deckfour/xes/classification/XEventAttributeClassifier.class
@@ -3008,8 +3008,8 @@
 -rw-r--r--  2.0 unx      907 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport$2.class
 -rw-r--r--  2.0 unx     1510 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport$3.class
 -rw-r--r--  2.0 unx     1408 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport$4.class
 -rw-r--r--  2.0 unx      775 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport$5.class
 -rw-r--r--  2.0 unx     2116 b- defN 17-Sep-06 14:23 javax/activation/SecuritySupport.class
 -rw-r--r--  2.0 unx     1420 b- defN 17-Sep-06 14:23 javax/activation/URLDataSource.class
 -rw-r--r--  2.0 unx      485 b- defN 17-Sep-06 14:23 javax/activation/UnsupportedDataTypeException.class
-3013 files, 7969640 bytes uncompressed, 3164213 bytes compressed:  60.3%
+3013 files, 7971880 bytes uncompressed, 3164787 bytes compressed:  60.3%
```

#### ee/ut/cs/sep/openxescli/CsvSerializer.class

##### procyon -ec {}

```diff
@@ -1,18 +1,19 @@
 
 package ee.ut.cs.sep.openxescli;
 
 import org.deckfour.xes.model.XTrace;
 import org.deckfour.xes.model.XAttributeMap;
 import java.io.IOException;
-import org.deckfour.xes.model.impl.XAttributeLiteralImpl;
 import org.deckfour.xes.model.XEvent;
-import org.deckfour.xes.model.XAttribute;
 import org.apache.commons.csv.CSVPrinter;
 import org.apache.commons.csv.CSVFormat;
+import org.deckfour.xes.model.XAttribute;
+import com.google.common.collect.ComparisonChain;
+import org.deckfour.xes.model.impl.XAttributeLiteralImpl;
 import java.io.OutputStream;
 import org.deckfour.xes.model.XLog;
 import org.deckfour.xes.out.XSerializer;
 
 public class CsvSerializer implements XSerializer
 {
     static final /* synthetic */ boolean $assertionsDisabled;
@@ -30,27 +31,33 @@
     }
     
     public String[] getSuffices() {
         return new String[] { "csv" };
     }
     
     public void serialize(final XLog xLog, final OutputStream outputStream) throws IOException {
+        final XAttributeLiteralImpl defaultConceptName = new XAttributeLiteralImpl("concept:name", "");
+        final XAttributeLiteralImpl defaultResource = new XAttributeLiteralImpl("org:resource", "");
+        final XAttributeLiteralImpl defaultTimestamp = new XAttributeLiteralImpl("time:timestamp", "");
+        final XAttributeLiteralImpl defaultTransition = new XAttributeLiteralImpl("lifecycle:transition", "complete");
+        xLog.sort((xTrace1, xTrace2) -> ComparisonChain.start().compare((Comparable)((XAttribute)xTrace1.getAttributes().getOrDefault((Object)"concept:name", (Object)defaultConceptName)).toString(), (Comparable)((XAttribute)xTrace2.getAttributes().getOrDefault((Object)"concept:name", (Object)defaultConceptName)).toString()).result());
         final Appendable csvBuffer = new StringBuilder();
         try (final CSVPrinter csvPrinter = new CSVPrinter(csvBuffer, CSVFormat.DEFAULT)) {
             csvPrinter.printRecord(new Object[] { "case:concept:name", "concept:name", "org:resource", "start_timestamp", "time:timestamp" });
             xLog.forEach(xTrace -> {
+                xTrace.sort((xEvent1, xEvent2) -> ComparisonChain.start().compare((Comparable)((XAttribute)xEvent1.getAttributes().getOrDefault((Object)"org:resource", (Object)defaultResource)).toString(), (Comparable)((XAttribute)xEvent2.getAttributes().getOrDefault((Object)"org:resource", (Object)defaultResource)).toString()).compare((Comparable)((XAttribute)xEvent1.getAttributes().getOrDefault((Object)"concept:name", (Object)defaultConceptName)).toString(), (Comparable)((XAttribute)xEvent2.getAttributes().getOrDefault((Object)"concept:name", (Object)defaultConceptName)).toString()).result());
                 Event csvEvent = new Event();
                 for (int i = 0; i < xTrace.size(); ++i) {
                     csvEvent.setCaseId(((XAttribute)xTrace.getAttributes().get((Object)"concept:name")).toString());
                     final XEvent event = (XEvent)xTrace.get(i);
                     final XAttributeMap attributes = event.getAttributes();
-                    final String timestamp = ((XAttribute)attributes.getOrDefault((Object)"time:timestamp", (Object)new XAttributeLiteralImpl("time:timestamp", ""))).toString();
-                    final String activity = ((XAttribute)attributes.getOrDefault((Object)"concept:name", (Object)new XAttributeLiteralImpl("concept:name", ""))).toString();
-                    final String resource = ((XAttribute)attributes.getOrDefault((Object)"org:resource", (Object)new XAttributeLiteralImpl("org:resource", ""))).toString();
-                    final String transition = ((XAttribute)attributes.getOrDefault((Object)"lifecycle:transition", (Object)new XAttributeLiteralImpl("lifecycle:transition", "complete"))).toString().toLowerCase();
+                    final String timestamp = ((XAttribute)attributes.getOrDefault((Object)"time:timestamp", (Object)defaultTimestamp)).toString();
+                    final String activity = ((XAttribute)attributes.getOrDefault((Object)"concept:name", (Object)defaultConceptName)).toString();
+                    final String resource = ((XAttribute)attributes.getOrDefault((Object)"org:resource", (Object)defaultResource)).toString();
+                    final String transition = ((XAttribute)attributes.getOrDefault((Object)"lifecycle:transition", (Object)defaultTransition)).toString().toLowerCase();
                     if (transition.equals("start")) {
                         csvEvent.setStartTimestamp(timestamp);
                         csvEvent.setActivity(activity);
                         csvEvent.setResource(resource);
                     }
                     else if (transition.equals("complete")) {
                         if (!CsvSerializer.$assertionsDisabled && csvEvent.getActivity() != null && !csvEvent.getActivity().equals(activity)) {
```

### Comparing `openxes_cli_py-0.1.8/src/openxes_cli/lib.py` & `openxes_cli_py-0.1.9/src/openxes_cli/lib.py`

 * *Files identical despite different names*

### Comparing `openxes_cli_py-0.1.8/PKG-INFO` & `openxes_cli_py-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxes-cli-py
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Ihar Suvorau
 Author-email: ihar.suvorau@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

